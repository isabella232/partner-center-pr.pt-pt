---
title: Restabelecer privilégios de administração para a Azure CSP
ms.topic: how-to
ms.date: 07/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como ajudar os clientes a restabelecer os privilégios de administração de um parceiro para que o parceiro possa ajudar a gerir as subscrições Azure CSP de um cliente.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 13fdeb01ecd73dc1a63d174a4ad5cb8e1bdc813a
ms.sourcegitcommit: 455894365fa488368f7572ac72312e84a267ef5e
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/10/2020
ms.locfileid: "97011507"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a>Repor privilégios de administração para subscrições Azure CSP de um cliente  

**Funções aplicáveis**

- Administrador global
- Agente administrativo

Como parceiro da CSP, os seus clientes esperam muitas vezes que gere o seu uso Azure e os seus sistemas para eles. Fazê-lo requer que tenha privilégios administrativos. Alguns privilégios são concedidos quando a sua relação de revendedor com o cliente é estabelecida. Outros são-lhe concedidos pelo seu cliente.

## <a name="admin-privileges-for-azure-in-csp"></a>Privilégios de administração para a Azure na CSP

Há dois níveis de privilégios administrativos para o Azure na CSP.

**Privilégios de administração de nível** de inquilino **(privilégios de administração delegados**) - os parceiros da CSP obtêm esses privilégios ao mesmo tempo que estabelecem a relação de revendedor CSP com os clientes. Isto dá aos parceiros da CSP acesso aos inquilinos dos seus clientes, o que lhes permite desempenhar funções administrativas como adicionar/gerir utilizadores, redefinir palavras-passe e gerir licenças de utilizador.

**Privilégios de administração de nível de subscrição** - os parceiros da CSP obtêm estes privilégios ao mesmo tempo que criam subscrições Azure CSP para os seus clientes. Ter estes privilégios dá aos parceiros da CSP acesso completo a estas subscrições, o que lhes permite provisão e gestão dos recursos da Azure.

## <a name="reinstate-csp-partners-admin-privileges"></a>Restabelecer os privilégios de administração dos parceiros da CSP

Para recuperar privilégios de administração delegados, precisa de trabalhar com o seu cliente.

1. Inscreva-se no painel partner center e no menu Partner Center, selecione **Clientes**.

2. Selecione o cliente com quem está a trabalhar e **solicite uma relação de revendedor.** Isto gera uma ligação com o cliente que tem direitos de administração de inquilinos.

3. Esse utilizador precisa de selecionar o link e aprovar o pedido de relacionamento do revendedor.

   :::image type="content" source="images/azure/revoke4.png" alt-text="relação de revendedor":::

## <a name="adding-the-admin-agents-group-as-an-owner-for-the-azure-csp-subscription"></a>Adicionar o grupo de agentes administrativos como proprietário para a assinatura Azure CSP

O seu cliente terá de adicionar o seu grupo de agente administrativo como proprietário de uma subscrição Azure CSP, um grupo de Recursos ou um recurso. 

1. Utilize a consola PowerShell ou o Ambiente integrado de Scripts PowerShell (ISE). Certifique-se de que os módulos AzureAD estão instalados.

2. Ligue-se ao seu Inquilino AD Azure.

   ```powershell
   Connect-AzureAD
   ```

3. Obtenha objectid dos grupos de agentes administrativos.

   ```powershell
   Get-AzureADGroup
   ```
   Os seguintes passos são realizados pelo utilizador na empresa do seu cliente que tem acesso ao proprietário à subscrição Azure CSP.

4. O utilizador com acesso do proprietário à assinatura Azure CSP, assina em Azure usando as suas credenciais.

   ```powershell
   Connect-AzureRmAccount
   ```

5. Em seguida, pode adicionar o seu grupo de agente administrativo como proprietário à subscrição CSP Azure, grupo de recursos ou recurso, aplicando um parâmetro de Recursos Uri no Âmbito. 

    ```powershell
    # Grant owner role at subscription level
    New-AzureRmRoleAssignment -ObjectId <Object Id that you got from step 3> -RoleDefinitionName Owner -Scope "/subscriptions/<SubscriptionId of CSP subscription>"

    # Grant owner role at resource group level
    New-AzureRmRoleAssignment -ObjectId <Object Id that you got from step 3> -RoleDefinitionName Owner -Scope "/subscriptions/<SubscriptionId of CSP subscription>/resourceGroups/<Resource group name>"

    # Grant owner role at resource level
    New-AzureRmRoleAssignment -ObjectId <Object Id that you got from step 3> -RoleDefinitionName Owner -Scope "<Resource Uri>"
    ```

## <a name="next-steps"></a>Passos seguintes

[Manage subscriptions and resources under the Azure plan](azure-plan-manage.md) (Gerir subscrições e recursos ao abrigo do plano do Azure)
