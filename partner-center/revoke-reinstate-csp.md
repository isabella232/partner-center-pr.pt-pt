---
title: Restabelecer privilégios de administração para a Azure CSP
ms.topic: how-to
ms.date: 04/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como ajudar os clientes a restabelecer os privilégios de administração de um parceiro para que o parceiro possa ajudar a gerir as subscrições Azure CSP de um cliente.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 26768bdf33c03145a893fa445eab6ebf92ca9b1c
ms.sourcegitcommit: efd711b0e65c55f24ce5b9636abd7b5a8cc719fe
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/27/2021
ms.locfileid: "108018192"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a>Repor privilégios de administração para subscrições Azure CSP de um cliente  

**Funções adequadas**

- Administrador global
- Agente administrativo

Como parceiro da CSP, os seus clientes esperam muitas vezes que gere o seu uso Azure e os seus sistemas para eles. Fazê-lo requer que tenha privilégios administrativos. Alguns privilégios são concedidos quando a sua relação de revendedor com o cliente é estabelecida. Outros são-lhe concedidos pelo seu cliente.

## <a name="admin-privileges-for-azure-in-csp"></a>Privilégios de administração para a Azure na CSP

Há dois níveis de privilégios administrativos para o Azure na CSP.

**Privilégios de administração de nível** de inquilino **(privilégios de administração delegados**) - os parceiros da CSP obtêm esses privilégios ao mesmo tempo que estabelecem a relação de revendedor CSP com os clientes. Os privilégios de administração delegados dão aos parceiros da CSP acesso aos inquilinos dos seus clientes, o que lhes permite desempenhar funções administrativas como adicionar/gerir utilizadores, redefinir palavras-passe e gerir licenças de utilizador.

**Privilégios de administração de nível de subscrição** - os parceiros da CSP obtêm estes privilégios ao mesmo tempo que criam subscrições Azure CSP para os seus clientes. Ter estes privilégios dá aos parceiros da CSP acesso completo a estas subscrições, o que lhes permite provisão e gestão dos recursos da Azure.

## <a name="reinstate-csp-partners-admin-privileges"></a>Restabelecer os privilégios de administração dos parceiros da CSP

O seu cliente pode recriar a atribuição de funções CSP desde que forneça ao seu cliente o ID do objeto do grupo AdminAgents. Para recuperar privilégios de administração delegados, precisa de trabalhar com o seu cliente.

1. Inscreva-se no painel partner Center e no menu Partner Center, selecione **Clientes**.

2. Selecione o cliente com quem está a trabalhar e **solicite uma relação de revendedor.** Esta ação gera uma ligação com o cliente que tem direitos de administração de inquilinos.

3. Esse cliente precisa de selecionar o link e aprovar o pedido de relacionamento do revendedor.

   :::image type="content" source="images/azure/revoke4.png" alt-text="Exemplo de e-mail de criar relacionamento revendedor":::

4. Você, o parceiro, precisa de se conectar com o inquilino parceiro para obter o Objeto ID do grupo AdminAgents.

  
    ```powershell

    PS C:\WINDOWS\system32> Connect-AzAccount -Tenant "Partner tenant"
      Get Object ID of AdminAgents group
   
    

   S C:\WINDOWS\system32> Get-AzADGroup -DisplayName AdminAgents
    ```


5. O seu cliente que tem o papel de **proprietário ou administrador** de acesso ao utilizador e tem permissão para criar uma atribuição de funções ao nível da subscrição faz o seguinte:


    1. Liga-se ao arrendatário onde existe a assinatura CSP.
      ```powershell
        PS C:\WINDOWS\system32> Connect-AzAccount -TenantID "Customer tenant"
      ```

    2. Conecta-se à subscrição (só aplicável se o utilizador tiver permissões de atribuição de funções sobre várias subscrições no arrendatário).
   
         PS C:\WINDOWS\system32> Set-AzContext -SubscriçãoID "CSP Subscription ID"'


    3. Cria a atribuição de funções
    
    ```powershell
      PS C:\WINDOWS\system32> New-AzRoleAssignment -ObjectID "Object ID of the Admin Agents group- needs to be provided by partner" -RoleDefinitionName "Owner" -Scope "/subscriptions/CSP subscription ID"
    ```


Se pretender conceder permissão de função do proprietário a nível de grupo de recursos ou ao nível de recursos em vez de âmbito de subscrição, os seguintes comandos podem funcionar:


```powershell
Grant owner role at resource group level

   New-AzRoleAssignment -ObjectID "Object ID that you got from step 3" -RoleDefinitionName Owner -Scope "/subscriptions/"SubscriptionID of CSP subscription"/resourceGroups/"Resource group name"

Grant owner role at resource level

   New-AzRoleAssignment -ObjectID <Object ID that you got from step 3> -RoleDefinitionName Owner -Scope "Resource URI"
```


## <a name="next-steps"></a>Passos seguintes

- [Manage subscriptions and resources under the Azure plan](azure-plan-manage.md) (Gerir subscrições e recursos ao abrigo do plano do Azure)
