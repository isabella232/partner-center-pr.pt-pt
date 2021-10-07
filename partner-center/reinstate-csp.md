---
title: Restabelecer privilégios de administrador para o Azure CSP
ms.topic: how-to
ms.date: 05/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: Saiba como ajudar os clientes a restabelecer os privilégios de administração de um parceiro para que o parceiro possa ajudar a gerir as subscrições Azure Fornecedor de Soluções em Nuvem (CSP) de um cliente.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 6b0390e47b1dedfd1e6438b783d8a502a6267954
ms.sourcegitcommit: 76a7dac540d129ae15cd4c251a4ff43d768370da
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/06/2021
ms.locfileid: "129598556"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a>Repor privilégios de administração para as assinaturas Azure CSP de um cliente  

**Funções adequadas**: Administração global | Agente administrativo

Como parceiro de programa Fornecedor de Soluções em Nuvem (CSP), os seus clientes dependem frequentemente de si para gerir o seu uso Azure e os seus sistemas. Vai precisar de privilégios administrativos para ajudá-los. Se ainda não tiver privilégios de administração, pode trabalhar com o seu cliente para os reintegrar.

## <a name="admin-privileges-for-azure-in-the-csp-program"></a>Privilégios de administração para a Azure no programa CSP

Alguns privilégios administrativos são concedidos automaticamente quando estabelece uma relação de revendedor com o cliente. Outros devem ser-lhe concedidos pelo cliente. Há dois níveis de privilégios administrativos para o Azure na CSP.

- **Privilégios administrativos ao nível do inquilino (isto é, privilégios administrativos delegados)** dão-lhe acesso aos inquilinos dos seus clientes. Este acesso permite-lhe fazer funções administrativas como adicionar e gerir utilizadores, redefinir palavras-passe e gerir licenças de utilizador. Obtém-se estes privilégios ao estabelecer relações de revendedor CSP com os clientes.
- **Os privilégios de administração ao nível de subscrição dão-lhe** acesso completo às subscrições Azure CSP dos seus clientes. Este acesso permite-lhe provisões e gerir os seus recursos Azure. Obtém estes privilégios ao criar subscrições Azure CSP para os seus clientes.

## <a name="how-to-reinstate-your-csp-admin-privileges"></a>Como restabelecer os seus privilégios de administração CSP

Pode trabalhar com o seu cliente para recuperar privilégios de administração delegados.

> [!NOTE]
> Para saber mais sobre a interface de espaços de trabalho, consulte [o Centro de Parceiros.](get-around-partner-center.md#turn-workspaces-on-and-off)

#### <a name="workspaces-view"></a>[Vista de espaços de trabalho](#tab/workspaces-view)

1. Inicie sessão no [dashboard do Centro de Parceiros](https://partner.microsoft.com/dashboard).

2. Selecione **o** azulejo cliente.

3. Escolha o cliente com quem está a trabalhar e **solicite uma relação de revendedor.** Esta ação envia um link para o seu cliente.

   :::image type="content" source="images/azure/revoke4.png" alt-text="Exemplo de e-mail de criar relacionamento de revendedor.":::

4. Assim que o seu cliente aprovar o pedido de relacionamento do revendedor através do link fornecido, conecte-se ao inquilino parceiro para obter `object ID` o do grupo AdminAgents.
  
   ```powershell
   Connect-AzAccount -Tenant "Partner tenant"
   # Get Object ID of AdminAgents group
   Get-AzADGroup -DisplayName AdminAgents
   ```

5. Certifique-se de que o seu cliente tem:

   * O papel do **proprietário** ou administrador de **acesso ao utilizador** 
   * Permissões para criar atribuições de funções ao nível da subscrição

6. Para concluir o processo, o seu cliente deve então fazer o seguinte, utilizando o PowerShell ou o Azure CLI. 

   1. Se utilizar o PowerShell, o cliente deve atualizar o `Az.Resources` módulo.

       ```powershell
       Update-Module Az.Resources
       ```

   2. O cliente deve ligar-se ao arrendatário em que existe a assinatura CSP.

      ```powershell
      Connect-AzAccount -TenantID "<Customer tenant>"
      ```

      ```azurecli
      az login --tenant <Customer tenant>
      ```

   3. O cliente deve ligar-se ao subscrição. Isto *só* é aplicável se o utilizador tiver permissões de atribuição de funções sobre várias subscrições no arrendatário.

      ```powershell
      Set-AzContext -SubscriptionID <"CSP Subscription ID">
      ```

      ```azurecli
      az account set --subscription <CSP Subscription ID>
      ```

   4. O cliente pode então criar a atribuição de funções.

      ```powershell
      New-AzRoleAssignment -ObjectID "<Object ID of the AdminAgents group from step 4>" -RoleDefinitionName "Owner" -Scope "/subscriptions/'<CSP subscription ID>'"
      ```

      ```azurecli
      az role assignment create --role "Owner" --assignee-object-id <Object ID of the AdminAgents group from step 4> --scope "/subscriptions/<CSP Subscription Id>"
      ```

Em vez de conceder permissões ao proprietário ao nível da subscrição, pode concedê-las ao nível do grupo de recursos ou recursos: 

- Ao nível do grupo de recursos

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID of the AdminAgents group from step 4>" -RoleDefinitionName Owner -Scope "/subscriptions/'SubscriptionID of CSP subscription'/resourceGroups/'Resource group name'"
   ```

   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object ID of the AdminAgents group from step 4> --scope "/subscriptions/<CSP Subscription Id>//resourceGroups/<Resource group name>"
   ```

- Ao nível dos recursos

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID of the AdminAgents group from step 4>" -RoleDefinitionName Owner -Scope "<Resource URI>"
   ```

   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object ID of the AdminAgents group from step 4> --scope "<Resource URI>"
   ```

Se os passos acima não funcionarem ou se tiver erros ao tentar, experimente o seguinte procedimento "catch-all" para restabelecer os direitos de administração do seu cliente:

```powershell
Install-Module -Name Az.Resources -Force -Verbose
Import-Module -Name Az.Resources -Verbose -MinimumVersion 4.1.1
Connect-AzAccount -Tenant <customer tenant>
Set-AzContext -SubscriptionId <customer subscriptions>
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<customer subscription>" -ObjectType "ForeignGroup"
```

#### <a name="current-view"></a>[Vista atual](#tab/current-view)

1. Inicie sessão no [dashboard do Centro de Parceiros](https://partner.microsoft.com/dashboard).

2. No menu Partner Center, selecione **Clientes.**

3. Escolha o cliente com quem está a trabalhar e **solicite uma relação de revendedor.** Esta ação envia um link para o seu cliente.

   :::image type="content" source="images/azure/revoke4.png" alt-text="Exemplo de e-mail de criar relacionamento de revendedor.":::

4. Assim que o seu cliente aprovar o pedido de relacionamento do revendedor através do link fornecido, conecte-se ao inquilino parceiro para obter `object ID` o do grupo AdminAgents.
  
   ```powershell
   Connect-AzAccount -Tenant "Partner tenant"
   # Get Object ID of AdminAgents group
   Get-AzADGroup -DisplayName AdminAgents
   ```

5. Certifique-se de que o seu cliente tem:

   1. O papel do **proprietário** ou administrador de **acesso ao utilizador** 
   2. Permissões para criar atribuições de funções ao nível da subscrição

6. Para concluir o processo, o seu cliente deve então fazer o seguinte, utilizando o PowerShell ou o Azure CLI. 

   1. Se utilizar o PowerShell, o cliente deve atualizar o `Az.Resources` módulo.

       ```powershell
       Update-Module Az.Resources
       ```

   2. O cliente deve ligar-se ao arrendatário em que existe a assinatura CSP.

      ```powershell
      Connect-AzAccount -TenantID "<Customer tenant>"
      ```

      ```azurecli
      az login --tenant <Customer tenant>
      ```

   3. O cliente deve ligar-se ao subscrição. Isto *só* é aplicável se o utilizador tiver permissões de atribuição de funções sobre várias subscrições no arrendatário.

      ```powershell
      Set-AzContext -SubscriptionID <"CSP Subscription ID">
      ```

      ```azurecli
      az account set --subscription <CSP Subscription ID>
      ```

   4. O cliente pode então criar a atribuição de funções.

      ```powershell
      New-AzRoleAssignment -ObjectID "<Object ID of the AdminAgents group from step 4>" -RoleDefinitionName "Owner" -Scope "/subscriptions/'<CSP subscription ID>'"
      ```

      ```azurecli
      az role assignment create --role "Owner" --assignee-object-id <Object ID of the AdminAgents group from step 4> --scope "/subscriptions/<CSP Subscription Id>"
      ```

Em vez de conceder permissões ao proprietário ao nível da subscrição, pode concedê-las ao nível do grupo de recursos ou recursos: 

- Ao nível do grupo de recursos

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID of the AdminAgents group from step 4>" -RoleDefinitionName Owner -Scope "/subscriptions/'SubscriptionID of CSP subscription'/resourceGroups/'Resource group name'"
   ```

   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object ID of the AdminAgents group from step 4> --scope "/subscriptions/<CSP Subscription Id>//resourceGroups/<Resource group name>"
   ```

- Ao nível dos recursos

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID of the AdminAgents group from step 4>" -RoleDefinitionName Owner -Scope "<Resource URI>"
   ```

   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object ID of the AdminAgents group from step 4> --scope "<Resource URI>"
   ```

Se os passos acima não funcionarem ou se tiver erros ao tentar, experimente o seguinte procedimento "catch-all" para restabelecer os direitos de administração do seu cliente:

```powershell
Install-Module -Name Az.Resources -Force -Verbose
Import-Module -Name Az.Resources -Verbose -MinimumVersion 4.1.1
Connect-AzAccount -Tenant <customer tenant>
Set-AzContext -SubscriptionId <customer subscriptions>
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<customer subscription>" -ObjectType "ForeignGroup"
```

* * *

### <a name="troubleshooting"></a>Resolução de problemas
Se o cliente não conseguir completar o passo 6, sugira o seguinte comando e forneça o ficheiro resultante `newRoleAssignment.log` à Microsoft para posterior análise:

```powershell
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<customer subscription>" -ObjectType "ForeignGroup" -Debug > newRoleAssignment.log
```

Se o procedimento "catch-all" falhar durante o `Import-Module` procedimento , experimente os seguintes passos:
- Se a importação falhar porque o módulo está a ser utilizado, reinicie a sessão PowerShell fechando e reabrindo todas as janelas.
- Verifique a versão de `Az.Resources` `Get-Module Az.Resources -ListAvailable` com .
- Se a versão 4.1.1 não estiver na lista disponível, deve utilizar `Update-Module Az.Resources -Force` .
- Se o erro indicar que `Az.Accounts` precisa de ser uma versão específica, atualize também esse módulo, substituindo por `Az.Resources` `Az.Accounts` . Em seguida, deve reiniciar a sessão PowerShell.


## <a name="next-steps"></a>Passos seguintes

- [Manage subscriptions and resources under the Azure plan](azure-plan-manage.md) (Gerir subscrições e recursos ao abrigo do plano do Azure)
