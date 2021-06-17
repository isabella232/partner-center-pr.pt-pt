---
title: Restabelecer privilégios de administração para a Azure CSP
ms.topic: how-to
ms.date: 05/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como ajudar os clientes a restabelecer os privilégios de administração de um parceiro para que o parceiro possa ajudar a gerir as subscrições Azure CSP de um cliente.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 81df7578f7f15def64a3c20b15f95f3b89a28d1c
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/17/2021
ms.locfileid: "112277781"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a><span data-ttu-id="dc2c9-103">Repor privilégios de administração para subscrições Azure CSP de um cliente</span><span class="sxs-lookup"><span data-stu-id="dc2c9-103">Reinstate admin privileges for a customer's Azure CSP subscriptions</span></span>  

<span data-ttu-id="dc2c9-104">**Funções adequadas**: Administração global | Agente administrativo</span><span class="sxs-lookup"><span data-stu-id="dc2c9-104">**Appropriate roles**: Global admin | Admin agent</span></span>

<span data-ttu-id="dc2c9-105">Como parceiro da CSP, os seus clientes esperam muitas vezes que gere o seu uso Azure e os seus sistemas para eles.</span><span class="sxs-lookup"><span data-stu-id="dc2c9-105">As a CSP partner, your customers often expect that you'll manage their Azure usage and their systems for them.</span></span> <span data-ttu-id="dc2c9-106">Deve ter privilégios administrativos para o fazer.</span><span class="sxs-lookup"><span data-stu-id="dc2c9-106">You must have admin privileges to do so.</span></span> <span data-ttu-id="dc2c9-107">Alguns privilégios são concedidos quando a sua relação de revendedor com o cliente é estabelecida.</span><span class="sxs-lookup"><span data-stu-id="dc2c9-107">Some privileges are granted when your reseller relationship with the customer is established.</span></span> <span data-ttu-id="dc2c9-108">Outros são-lhe concedidos pelo seu cliente.</span><span class="sxs-lookup"><span data-stu-id="dc2c9-108">Others are granted to you by your customer.</span></span>

## <a name="admin-privileges-for-azure-in-csp"></a><span data-ttu-id="dc2c9-109">Privilégios de administração para a Azure na CSP</span><span class="sxs-lookup"><span data-stu-id="dc2c9-109">Admin privileges for Azure in CSP</span></span>

<span data-ttu-id="dc2c9-110">Há dois níveis de privilégios administrativos para o Azure na CSP.</span><span class="sxs-lookup"><span data-stu-id="dc2c9-110">There are two levels of admin privileges for Azure in CSP.</span></span>

- <span data-ttu-id="dc2c9-111">**Privilégios de administração de nível de inquilino (privilégios de administração delegados)**: Os parceiros da CSP obtêm esses privilégios ao mesmo tempo que estabelecem a relação de revendedor CSP com os clientes.</span><span class="sxs-lookup"><span data-stu-id="dc2c9-111">**Tenant level admin privileges (Delegated admin privileges)**:  CSP partners get these privileges while establishing CSP reseller relationship with customers.</span></span> <span data-ttu-id="dc2c9-112">Os privilégios de administração delegados dão aos parceiros da CSP acesso aos inquilinos dos seus clientes.</span><span class="sxs-lookup"><span data-stu-id="dc2c9-112">Delegated admin privileges give CSP partners access to their customers' tenants.</span></span> <span data-ttu-id="dc2c9-113">Este acesso permite-lhes fazer funções administrativas como adicionar/gerir utilizadores, redefinir palavras-passe e gerir licenças de utilizador.</span><span class="sxs-lookup"><span data-stu-id="dc2c9-113">This access allows them to do administrative functions such as add/manage users, reset passwords and manage user licenses.</span></span>
- <span data-ttu-id="dc2c9-114">**Privilégios de administração de nível de subscrição**: os parceiros CSP obtêm estes privilégios ao mesmo tempo que criam subscrições Azure CSP para os seus clientes.</span><span class="sxs-lookup"><span data-stu-id="dc2c9-114">**Subscription level admin privileges**: CSP partners get these privileges while creating Azure CSP subscriptions for their customers.</span></span> <span data-ttu-id="dc2c9-115">Ter estes privilégios dá aos parceiros da CSP acesso completo a estas subscrições, o que lhes permite provisão e gestão dos recursos da Azure.</span><span class="sxs-lookup"><span data-stu-id="dc2c9-115">Having these privileges gives CSP partners complete access to these subscriptions, which allows them to provision and manage Azure resources.</span></span>

## <a name="reinstate-csp-a-partners-admin-privileges"></a><span data-ttu-id="dc2c9-116">Repor os privilégios de administração de um parceiro</span><span class="sxs-lookup"><span data-stu-id="dc2c9-116">Reinstate CSP a partner's admin privileges</span></span>

<span data-ttu-id="dc2c9-117">O seu cliente pode recriar a atribuição de funções CSP se fornecer `object ID` o grupo AdminAgents ao seu cliente.</span><span class="sxs-lookup"><span data-stu-id="dc2c9-117">Your customer can re-create the CSP role assignment if you provide the `object ID` of the AdminAgents group to your customer.</span></span> <span data-ttu-id="dc2c9-118">Para recuperar privilégios de administração delegados, precisa de trabalhar com o seu cliente através dos seguintes passos.</span><span class="sxs-lookup"><span data-stu-id="dc2c9-118">To regain delegated admin privileges, you need to work with your customer through the following steps.</span></span>

1. <span data-ttu-id="dc2c9-119">Inscreva-se no painel do Centro de Parceiros.</span><span class="sxs-lookup"><span data-stu-id="dc2c9-119">Sign into the Partner Center dashboard.</span></span>

2. <span data-ttu-id="dc2c9-120">No menu Partner Center, selecione **Clientes.**</span><span class="sxs-lookup"><span data-stu-id="dc2c9-120">On the Partner Center menu, select **Customers**.</span></span>

3. <span data-ttu-id="dc2c9-121">Selecione o cliente com quem está a trabalhar e **solicite uma relação de revendedor**.</span><span class="sxs-lookup"><span data-stu-id="dc2c9-121">Select the customer you are working with and **request a reseller relationship**.</span></span> <span data-ttu-id="dc2c9-122">Esta ação gera uma ligação com o cliente que tem direitos de administração de inquilinos.</span><span class="sxs-lookup"><span data-stu-id="dc2c9-122">This action generates a link to the customer who has tenant admin rights.</span></span>

4. <span data-ttu-id="dc2c9-123">O seu cliente precisa de selecionar o link e aprovar o pedido de relacionamento do revendedor.</span><span class="sxs-lookup"><span data-stu-id="dc2c9-123">Your customer needs to select the link and approve the reseller relationship request.</span></span>

   :::image type="content" source="images/azure/revoke4.png" alt-text="Exemplo de e-mail de criar relacionamento revendedor.":::

5. <span data-ttu-id="dc2c9-125">Você, o parceiro, precisa de se conectar com o inquilino parceiro para obter o Objeto ID do grupo AdminAgents.</span><span class="sxs-lookup"><span data-stu-id="dc2c9-125">You, the partner, need to connect to partner tenant to get the Object ID of the AdminAgents group.</span></span>
  
   ```powershell
   Connect-AzAccount -Tenant "Partner tenant"
   # Get Object ID of AdminAgents group
   Get-AzADGroup -DisplayName AdminAgents
   ```

6. <span data-ttu-id="dc2c9-126">Em seguida, o seu cliente deve fazer os seguintes passos utilizando o PowerShell ou o Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="dc2c9-126">Your customer must then do the following steps using either PowerShell or Azure CLI.</span></span> <span data-ttu-id="dc2c9-127">O seu cliente deve ter:</span><span class="sxs-lookup"><span data-stu-id="dc2c9-127">Your customer must have:</span></span>

- <span data-ttu-id="dc2c9-128">O papel do **proprietário** ou administrador de **acesso ao utilizador**</span><span class="sxs-lookup"><span data-stu-id="dc2c9-128">The role of **owner** or **user access administrator**</span></span> 
- <span data-ttu-id="dc2c9-129">Permissões para criar atribuições de funções ao nível da subscrição</span><span class="sxs-lookup"><span data-stu-id="dc2c9-129">Permissions to create role assignments at the subscription level</span></span>

   <span data-ttu-id="dc2c9-130">a.</span><span class="sxs-lookup"><span data-stu-id="dc2c9-130">a.</span></span> <span data-ttu-id="dc2c9-131">Apenas para o PowerShell, o cliente deve atualizar o `Az.Resources` módulo.</span><span class="sxs-lookup"><span data-stu-id="dc2c9-131">For PowerShell only, the customer must update the `Az.Resources` module.</span></span>
   ```powershell
   Update-Module Az.Resources
   ```

   <span data-ttu-id="dc2c9-132">b.</span><span class="sxs-lookup"><span data-stu-id="dc2c9-132">b.</span></span> <span data-ttu-id="dc2c9-133">O cliente conecta-se ao inquilino onde existe a assinatura CSP.</span><span class="sxs-lookup"><span data-stu-id="dc2c9-133">The customer connects to the tenant where the CSP subscription exists.</span></span>
   ```powershell
   Connect-AzAccount -TenantID "<Customer tenant>"
   ```
   ```azurecli
   az login --tenant <Customer tenant>
   ```

   <span data-ttu-id="dc2c9-134">c.</span><span class="sxs-lookup"><span data-stu-id="dc2c9-134">c.</span></span> <span data-ttu-id="dc2c9-135">O cliente conecta-se à subscrição.</span><span class="sxs-lookup"><span data-stu-id="dc2c9-135">The customer connects to the subscription.</span></span> <span data-ttu-id="dc2c9-136">Isto *só* é aplicável se o utilizador tiver permissões de atribuição de funções sobre várias subscrições no arrendatário.</span><span class="sxs-lookup"><span data-stu-id="dc2c9-136">This is *only* applicable if the user has role assignment permissions over multiple subscriptions in the tenant.</span></span>

   ```powershell
   Set-AzContext -SubscriptionID <"CSP Subscription ID">
   ```
   ```azurecli
   az account set --subscription <CSP Subscription ID>
   ```

   <span data-ttu-id="dc2c9-137">d.</span><span class="sxs-lookup"><span data-stu-id="dc2c9-137">d.</span></span> <span data-ttu-id="dc2c9-138">Em seguida, o cliente cria a atribuição de funções.</span><span class="sxs-lookup"><span data-stu-id="dc2c9-138">The customer then creates the role assignment.</span></span>
    
   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID of the Admin Agents group provided by partner>" -RoleDefinitionName "Owner" -Scope "/subscriptions/'<CSP subscription ID>'"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>"
   ```

<span data-ttu-id="dc2c9-139">Em vez de conceder permissões ao proprietário no âmbito de subscrição, pode conceder ao nível do grupo de recursos ou recursos.</span><span class="sxs-lookup"><span data-stu-id="dc2c9-139">Instead of granting owner permissions at the subscription scope, you can grant at the resource group or resource level.</span></span> 

- <span data-ttu-id="dc2c9-140">Ao nível do grupo de recursos</span><span class="sxs-lookup"><span data-stu-id="dc2c9-140">At the resource group level</span></span>

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "/subscriptions/'SubscriptionID of CSP subscription'/resourceGroups/'Resource group name'"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>//resourceGroups/<Resource group name>"
   ```

- <span data-ttu-id="dc2c9-141">Ao nível dos recursos</span><span class="sxs-lookup"><span data-stu-id="dc2c9-141">At the resource level</span></span>

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "<Resource URI>"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "<Resource URI>"
   ```

<span data-ttu-id="dc2c9-142">Se os passos acima não funcionarem ou se tiver erros ao tentar, experimente o seguinte procedimento "catch-all" para restabelecer os direitos de administração do seu cliente.</span><span class="sxs-lookup"><span data-stu-id="dc2c9-142">If the above steps don't work or you get errors when attempting them, try the following "catch-all" procedure to reinstate admin rights for your customer.</span></span>

```powershell
Install-Module -Name Az.Resources -Force -Verbose
Import-Module -Name Az.Resources -Verbose -MinimumVersion 4.1.1
Connect-AzAccount -Tenant <customer tenant>
Set-AzContext -SubscriptionId <customer subscriptions>
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<customer subscription>" -ObjectType "ForeignGroup"
```

### <a name="troubleshooting"></a><span data-ttu-id="dc2c9-143">Resolução de problemas</span><span class="sxs-lookup"><span data-stu-id="dc2c9-143">Troubleshooting</span></span>

<span data-ttu-id="dc2c9-144">Se o cliente não conseguir completar o passo 6 acima, faça com que o cliente experimente o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="dc2c9-144">If the customer is unable to complete step 6 above, have the customer try the following command:</span></span>

```powershell
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<costumer subscription>" -ObjectType "ForeignGroup" -Debug > newRoleAssignment.log
```

<span data-ttu-id="dc2c9-145">Forneça o ficheiro resultante `newRoleAssignment.log` à Microsoft para uma análise mais aprofundada.</span><span class="sxs-lookup"><span data-stu-id="dc2c9-145">Provide the resulting `newRoleAssignment.log` file to Microsoft for further analysis.</span></span>

<span data-ttu-id="dc2c9-146">Se o procedimento "catch-all" falhar durante o `Import-Module` procedimento , experimente os seguintes passos:</span><span class="sxs-lookup"><span data-stu-id="dc2c9-146">If the "catch-all" procedure fails during the `Import-Module`, try the following steps:</span></span>
- <span data-ttu-id="dc2c9-147">Se a importação falhar porque o módulo está a ser utilizado, reinicie a sessão PowerShell fechando e reabrindo todas as janelas.</span><span class="sxs-lookup"><span data-stu-id="dc2c9-147">If the import fails because the module is in use, restart the PowerShell session by closing and reopening all windows.</span></span>
- <span data-ttu-id="dc2c9-148">Ver versão de `Az.Resources` com `Get-Module Az.Resources -ListAvailable` .</span><span class="sxs-lookup"><span data-stu-id="dc2c9-148">Check version of `Az.Resources` with `Get-Module Az.Resources -ListAvailable`.</span></span>
- <span data-ttu-id="dc2c9-149">Se a versão 4.1.1 não estiver na lista disponível, deve utilizar `Update-Module Az.Resources -Force` .</span><span class="sxs-lookup"><span data-stu-id="dc2c9-149">If version 4.1.1 is not within the available list, you must use `Update-Module Az.Resources -Force`.</span></span>
- <span data-ttu-id="dc2c9-150">Se o erro indicar que `Az.Accounts` tem de ser uma versão específica, atualize também esse módulo, substituindo por `Az.Resources` `Az.Accounts` .</span><span class="sxs-lookup"><span data-stu-id="dc2c9-150">If the error states that `Az.Accounts` needs to be a specific version, update that module as well, replacing `Az.Resources` with `Az.Accounts`.</span></span> <span data-ttu-id="dc2c9-151">Em seguida, deve reiniciar a sessão PowerShell.</span><span class="sxs-lookup"><span data-stu-id="dc2c9-151">You must then restart the PowerShell session.</span></span>


## <a name="next-steps"></a><span data-ttu-id="dc2c9-152">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="dc2c9-152">Next steps</span></span>

- <span data-ttu-id="dc2c9-153">[Manage subscriptions and resources under the Azure plan](azure-plan-manage.md) (Gerir subscrições e recursos ao abrigo do plano do Azure)</span><span class="sxs-lookup"><span data-stu-id="dc2c9-153">[Manage subscriptions and resources under the Azure plan](azure-plan-manage.md)</span></span>
