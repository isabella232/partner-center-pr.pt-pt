---
title: Restabelecer privilégios de administração para a Azure CSP
ms.topic: how-to
ms.date: 05/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como ajudar os clientes a restabelecer os privilégios de administração de um parceiro para que o parceiro possa ajudar a gerir as subscrições do Azure Cloud Solution Provider (CSP) de um cliente.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 5d784aef33cce2a722583a77e73c35d5fc8136b1
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551593"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a>Repor privilégios de administração para subscrições Azure CSP de um cliente  

**Funções adequadas**: Administração global | Agente administrativo

Como parceiro cloud solution provider (CSP), os seus clientes esperam muitas vezes que gere o seu uso Azure e os seus sistemas para eles. Deve ter privilégios administrativos para o fazer. Alguns privilégios são concedidos quando a sua relação de revendedor com o cliente é estabelecida. Outros são-lhe concedidos pelo seu cliente.

## <a name="admin-privileges-for-azure-in-csp"></a>Privilégios de administração para a Azure na CSP

Há dois níveis de privilégios administrativos para o Azure na CSP.

- **Privilégios de administração de nível de inquilino (privilégios de administração delegados)**: Os parceiros da CSP obtêm esses privilégios ao mesmo tempo que estabelecem a relação de revendedor CSP com os clientes. Os privilégios de administração delegados dão aos parceiros da CSP acesso aos inquilinos dos seus clientes. Este acesso permite-lhes fazer funções administrativas como adicionar/gerir utilizadores, redefinir palavras-passe e gerir licenças de utilizador.
- **Privilégios de administração de nível de subscrição**: os parceiros CSP obtêm estes privilégios ao mesmo tempo que criam subscrições Azure CSP para os seus clientes. Ter estes privilégios dá aos parceiros da CSP acesso completo a estas subscrições, o que lhes permite provisão e gestão dos recursos da Azure.

## <a name="reinstate-csp-a-partners-admin-privileges"></a>Repor os privilégios de administração de um parceiro

O seu cliente pode recriar a atribuição de funções CSP se fornecer `object ID` o grupo AdminAgents ao seu cliente. Para recuperar privilégios de administração delegados, precisa de trabalhar com o seu cliente através dos seguintes passos.

1. Inscreva-se no painel do Centro de Parceiros.

2. No menu Partner Center, selecione **Clientes.**

3. Selecione o cliente com quem está a trabalhar e **solicite uma relação de revendedor**. Esta ação gera uma ligação com o cliente que tem direitos de administração de inquilinos.

4. O seu cliente precisa de selecionar o link e aprovar o pedido de relacionamento do revendedor.

   :::image type="content" source="images/azure/revoke4.png" alt-text="Exemplo de e-mail de criar relacionamento revendedor.":::

5. Você, o parceiro, precisa de se conectar com o inquilino parceiro para obter o Objeto ID do grupo AdminAgents.
  
   ```powershell
   Connect-AzAccount -Tenant "Partner tenant"
   # Get Object ID of AdminAgents group
   Get-AzADGroup -DisplayName AdminAgents
   ```

6. Em seguida, o seu cliente deve fazer os seguintes passos utilizando o PowerShell ou o Azure CLI. O seu cliente deve ter:

- O papel do **proprietário** ou administrador de **acesso ao utilizador** 
- Permissões para criar atribuições de funções ao nível da subscrição

   a. Apenas para o PowerShell, o cliente deve atualizar o `Az.Resources` módulo.
   ```powershell
   Update-Module Az.Resources
   ```

   b. O cliente conecta-se ao inquilino onde existe a assinatura CSP.
   ```powershell
   Connect-AzAccount -TenantID "<Customer tenant>"
   ```
   ```azurecli
   az login --tenant <Customer tenant>
   ```

   c. O cliente conecta-se à subscrição. Isto *só* é aplicável se o utilizador tiver permissões de atribuição de funções sobre várias subscrições no arrendatário.

   ```powershell
   Set-AzContext -SubscriptionID <"CSP Subscription ID">
   ```
   ```azurecli
   az account set --subscription <CSP Subscription ID>
   ```

   d. Em seguida, o cliente cria a atribuição de funções.
    
   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID of the Admin Agents group provided by partner>" -RoleDefinitionName "Owner" -Scope "/subscriptions/'<CSP subscription ID>'"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>"
   ```

Em vez de conceder permissões ao proprietário no âmbito de subscrição, pode conceder ao nível do grupo de recursos ou recursos. 

- Ao nível do grupo de recursos

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "/subscriptions/'SubscriptionID of CSP subscription'/resourceGroups/'Resource group name'"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>//resourceGroups/<Resource group name>"
   ```

- Ao nível dos recursos

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "<Resource URI>"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "<Resource URI>"
   ```

Se os passos acima não funcionarem ou se tiver erros ao tentar, experimente o seguinte procedimento "catch-all" para restabelecer os direitos de administração do seu cliente.

```powershell
Install-Module -Name Az.Resources -Force -Verbose
Import-Module -Name Az.Resources -Verbose -MinimumVersion 4.1.1
Connect-AzAccount -Tenant <customer tenant>
Set-AzContext -SubscriptionId <customer subscriptions>
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<customer subscription>" -ObjectType "ForeignGroup"
```

### <a name="troubleshooting"></a>Resolução de problemas

Se o cliente não conseguir completar o passo 6 acima, faça com que o cliente experimente o seguinte comando:

```powershell
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<costumer subscription>" -ObjectType "ForeignGroup" -Debug > newRoleAssignment.log
```

Forneça o ficheiro resultante `newRoleAssignment.log` à Microsoft para uma análise mais aprofundada.

Se o procedimento "catch-all" falhar durante o `Import-Module` procedimento , experimente os seguintes passos:
- Se a importação falhar porque o módulo está a ser utilizado, reinicie a sessão PowerShell fechando e reabrindo todas as janelas.
- Ver versão de `Az.Resources` com `Get-Module Az.Resources -ListAvailable` .
- Se a versão 4.1.1 não estiver na lista disponível, deve utilizar `Update-Module Az.Resources -Force` .
- Se o erro indicar que `Az.Accounts` tem de ser uma versão específica, atualize também esse módulo, substituindo por `Az.Resources` `Az.Accounts` . Em seguida, deve reiniciar a sessão PowerShell.


## <a name="next-steps"></a>Passos seguintes

- [Manage subscriptions and resources under the Azure plan](azure-plan-manage.md) (Gerir subscrições e recursos ao abrigo do plano do Azure)
