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
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a><span data-ttu-id="aa36d-103">Repor privilégios de administração para subscrições Azure CSP de um cliente</span><span class="sxs-lookup"><span data-stu-id="aa36d-103">Reinstate admin privileges for a customer's Azure CSP subscriptions</span></span>  

<span data-ttu-id="aa36d-104">**Funções adequadas**</span><span class="sxs-lookup"><span data-stu-id="aa36d-104">**Appropriate roles**</span></span>

- <span data-ttu-id="aa36d-105">Administrador global</span><span class="sxs-lookup"><span data-stu-id="aa36d-105">Global admin</span></span>
- <span data-ttu-id="aa36d-106">Agente administrativo</span><span class="sxs-lookup"><span data-stu-id="aa36d-106">Admin agent</span></span>

<span data-ttu-id="aa36d-107">Como parceiro da CSP, os seus clientes esperam muitas vezes que gere o seu uso Azure e os seus sistemas para eles.</span><span class="sxs-lookup"><span data-stu-id="aa36d-107">As a CSP partner your customers often expect that you will manage their Azure usage and their systems for them.</span></span> <span data-ttu-id="aa36d-108">Fazê-lo requer que tenha privilégios administrativos.</span><span class="sxs-lookup"><span data-stu-id="aa36d-108">Doing so requires you to have admin privileges.</span></span> <span data-ttu-id="aa36d-109">Alguns privilégios são concedidos quando a sua relação de revendedor com o cliente é estabelecida.</span><span class="sxs-lookup"><span data-stu-id="aa36d-109">Some privileges are granted when your reseller relationship with the customer is established.</span></span> <span data-ttu-id="aa36d-110">Outros são-lhe concedidos pelo seu cliente.</span><span class="sxs-lookup"><span data-stu-id="aa36d-110">Others are granted to you by your customer.</span></span>

## <a name="admin-privileges-for-azure-in-csp"></a><span data-ttu-id="aa36d-111">Privilégios de administração para a Azure na CSP</span><span class="sxs-lookup"><span data-stu-id="aa36d-111">Admin privileges for Azure in CSP</span></span>

<span data-ttu-id="aa36d-112">Há dois níveis de privilégios administrativos para o Azure na CSP.</span><span class="sxs-lookup"><span data-stu-id="aa36d-112">There are two levels of admin privileges for Azure in CSP.</span></span>

<span data-ttu-id="aa36d-113">**Privilégios de administração de nível** de inquilino **(privilégios de administração delegados**) - os parceiros da CSP obtêm esses privilégios ao mesmo tempo que estabelecem a relação de revendedor CSP com os clientes.</span><span class="sxs-lookup"><span data-stu-id="aa36d-113">**Tenant level admin privileges** (**Delegated admin privileges**) -  CSP partners get these privileges while establishing CSP reseller relationship with customers.</span></span> <span data-ttu-id="aa36d-114">Os privilégios de administração delegados dão aos parceiros da CSP acesso aos inquilinos dos seus clientes, o que lhes permite desempenhar funções administrativas como adicionar/gerir utilizadores, redefinir palavras-passe e gerir licenças de utilizador.</span><span class="sxs-lookup"><span data-stu-id="aa36d-114">Delegated admin privileges give CSP partners access to their customers' tenants, which allows them to perform administrative functions such as add/manage users, reset passwords and manage user licenses.</span></span>

<span data-ttu-id="aa36d-115">**Privilégios de administração de nível de subscrição** - os parceiros da CSP obtêm estes privilégios ao mesmo tempo que criam subscrições Azure CSP para os seus clientes.</span><span class="sxs-lookup"><span data-stu-id="aa36d-115">**Subscription level admin privileges** - CSP partners get these privileges while creating Azure CSP subscriptions for their customers.</span></span> <span data-ttu-id="aa36d-116">Ter estes privilégios dá aos parceiros da CSP acesso completo a estas subscrições, o que lhes permite provisão e gestão dos recursos da Azure.</span><span class="sxs-lookup"><span data-stu-id="aa36d-116">Having these privileges gives CSP partners complete access to these subscriptions, which allows them to provision and manage Azure resources.</span></span>

## <a name="reinstate-csp-partners-admin-privileges"></a><span data-ttu-id="aa36d-117">Restabelecer os privilégios de administração dos parceiros da CSP</span><span class="sxs-lookup"><span data-stu-id="aa36d-117">Reinstate CSP partners' admin privileges</span></span>

<span data-ttu-id="aa36d-118">O seu cliente pode recriar a atribuição de funções CSP desde que forneça ao seu cliente o ID do objeto do grupo AdminAgents.</span><span class="sxs-lookup"><span data-stu-id="aa36d-118">Your customer can re-create the CSP role assignment as long as you provide the object ID of the AdminAgents group to your customer.</span></span> <span data-ttu-id="aa36d-119">Para recuperar privilégios de administração delegados, precisa de trabalhar com o seu cliente.</span><span class="sxs-lookup"><span data-stu-id="aa36d-119">To regain delegated admin privileges, you need to work with your customer.</span></span>

1. <span data-ttu-id="aa36d-120">Inscreva-se no painel partner Center e no menu Partner Center, selecione **Clientes**.</span><span class="sxs-lookup"><span data-stu-id="aa36d-120">Sign into the Partner Center dashboard and from the Partner Center menu, select **Customers**.</span></span>

2. <span data-ttu-id="aa36d-121">Selecione o cliente com quem está a trabalhar e **solicite uma relação de revendedor.**</span><span class="sxs-lookup"><span data-stu-id="aa36d-121">Select the customer you are working with and **request a reseller relationship.**</span></span> <span data-ttu-id="aa36d-122">Esta ação gera uma ligação com o cliente que tem direitos de administração de inquilinos.</span><span class="sxs-lookup"><span data-stu-id="aa36d-122">This action generates a link to the customer who has tenant admin rights.</span></span>

3. <span data-ttu-id="aa36d-123">Esse cliente precisa de selecionar o link e aprovar o pedido de relacionamento do revendedor.</span><span class="sxs-lookup"><span data-stu-id="aa36d-123">That customer needs to select the link and approve the reseller relationship request.</span></span>

   :::image type="content" source="images/azure/revoke4.png" alt-text="Exemplo de e-mail de criar relacionamento revendedor":::

4. <span data-ttu-id="aa36d-125">Você, o parceiro, precisa de se conectar com o inquilino parceiro para obter o Objeto ID do grupo AdminAgents.</span><span class="sxs-lookup"><span data-stu-id="aa36d-125">You, the partner, need to connect to partner tenant to get the Object ID of the AdminAgents group.</span></span>

  
    ```powershell

    PS C:\WINDOWS\system32> Connect-AzAccount -Tenant "Partner tenant"
      Get Object ID of AdminAgents group
   
    

   S C:\WINDOWS\system32> Get-AzADGroup -DisplayName AdminAgents
    ```


5. <span data-ttu-id="aa36d-126">O seu cliente que tem o papel de **proprietário ou administrador** de acesso ao utilizador e tem permissão para criar uma atribuição de funções ao nível da subscrição faz o seguinte:</span><span class="sxs-lookup"><span data-stu-id="aa36d-126">Your customer who has the role of **owner or user access administrator** and has permission to create role assignment at the subscription level does the following:</span></span>


    1. <span data-ttu-id="aa36d-127">Liga-se ao arrendatário onde existe a assinatura CSP.</span><span class="sxs-lookup"><span data-stu-id="aa36d-127">Connects to the tenant where the CSP subscription exists.</span></span>
      ```powershell
        PS C:\WINDOWS\system32> Connect-AzAccount -TenantID "Customer tenant"
      ```

    2. <span data-ttu-id="aa36d-128">Conecta-se à subscrição (só aplicável se o utilizador tiver permissões de atribuição de funções sobre várias subscrições no arrendatário).</span><span class="sxs-lookup"><span data-stu-id="aa36d-128">Connects to the subscription (only applicable if the user has role assignment permissions over multiple subscriptions in the tenant).</span></span>
   
         <span data-ttu-id="aa36d-129">PS C:\WINDOWS\system32> Set-AzContext -SubscriçãoID "CSP Subscription ID"'</span><span class="sxs-lookup"><span data-stu-id="aa36d-129">PS C:\WINDOWS\system32> Set-AzContext -SubscriptionID "CSP Subscription ID"\`</span></span>


    3. <span data-ttu-id="aa36d-130">Cria a atribuição de funções</span><span class="sxs-lookup"><span data-stu-id="aa36d-130">Creates the role assignment</span></span>
    
    ```powershell
      PS C:\WINDOWS\system32> New-AzRoleAssignment -ObjectID "Object ID of the Admin Agents group- needs to be provided by partner" -RoleDefinitionName "Owner" -Scope "/subscriptions/CSP subscription ID"
    ```


<span data-ttu-id="aa36d-131">Se pretender conceder permissão de função do proprietário a nível de grupo de recursos ou ao nível de recursos em vez de âmbito de subscrição, os seguintes comandos podem funcionar:</span><span class="sxs-lookup"><span data-stu-id="aa36d-131">If you want to grant owner role permission at resource group level or resource level instead of subscription scope, the following commands can work:</span></span>


```powershell
Grant owner role at resource group level

   New-AzRoleAssignment -ObjectID "Object ID that you got from step 3" -RoleDefinitionName Owner -Scope "/subscriptions/"SubscriptionID of CSP subscription"/resourceGroups/"Resource group name"

Grant owner role at resource level

   New-AzRoleAssignment -ObjectID <Object ID that you got from step 3> -RoleDefinitionName Owner -Scope "Resource URI"
```


## <a name="next-steps"></a><span data-ttu-id="aa36d-132">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="aa36d-132">Next steps</span></span>

- <span data-ttu-id="aa36d-133">[Manage subscriptions and resources under the Azure plan](azure-plan-manage.md) (Gerir subscrições e recursos ao abrigo do plano do Azure)</span><span class="sxs-lookup"><span data-stu-id="aa36d-133">[Manage subscriptions and resources under the Azure plan](azure-plan-manage.md)</span></span>
