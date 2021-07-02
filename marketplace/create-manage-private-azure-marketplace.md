---
title: Criar e gerir o Private Azure Marketplace no portal Azure
description: Saiba como criar e gerir o Private Azure Marketplace (pré-visualização) no portal Azure. O Private Azure Marketplace (pré-visualização) permite aos administradores governar quais as soluções de terceiros que os seus utilizadores podem utilizar.
ms.service: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 02/24/2021
ms.openlocfilehash: 8a3ffbe5b57c49004518341d27c785dcd1b9ce87
ms.sourcegitcommit: c4601069340445135b551fa96bee6d9923d8aa97
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/01/2021
ms.locfileid: "113173699"
---
# <a name="create-and-manage-private-azure-marketplace-in-the-azure-portal"></a><span data-ttu-id="053c0-104">Criar e gerir o Private Azure Marketplace no portal Azure</span><span class="sxs-lookup"><span data-stu-id="053c0-104">Create and manage Private Azure Marketplace in the Azure portal</span></span>

<span data-ttu-id="053c0-105">O Private Azure Marketplace permite aos administradores governar quais as soluções de terceiros que os seus utilizadores podem utilizar.</span><span class="sxs-lookup"><span data-stu-id="053c0-105">Private Azure Marketplace lets administrators govern which third-party solutions their users can use.</span></span> <span data-ttu-id="053c0-106">Fá-lo permitindo que o utilizador implemente apenas ofertas que sejam aprovadas pelo administrador e cumpram as políticas da sua empresa.</span><span class="sxs-lookup"><span data-stu-id="053c0-106">It does this by allowing the user to deploy only offers that are approved by the administrator and comply with your enterprise's policies.</span></span> <span data-ttu-id="053c0-107">Com o Private Azure Marketplace, os utilizadores podem pesquisar na loja online ofertas compatíveis para comprar e implementar.</span><span class="sxs-lookup"><span data-stu-id="053c0-107">With Private Azure Marketplace, users can search the online store for compliant offers to purchase and deploy.</span></span>

<span data-ttu-id="053c0-108">Como administrador do Marketplace (papel atribuído), começará com uma Loja Privada desativada e vazia, onde poderá adicionar as suas ofertas e planos aprovados.</span><span class="sxs-lookup"><span data-stu-id="053c0-108">As a Marketplace admin (assigned role), you will start with a disabled and empty Private Store where you can add your approved offers and plans.</span></span> <span data-ttu-id="053c0-109">Este artigo explica como atribuir a função necessária, criar uma loja privada, gerir itens, aprovar pedidos de utilizador e ativar o Private Azure Marketplace para os seus utilizadores.</span><span class="sxs-lookup"><span data-stu-id="053c0-109">This article explains how to assign the needed role, create a private store, manage items, approve user requests, and enable Private Azure Marketplace for your users.</span></span>

> [!NOTE]
> - <span data-ttu-id="053c0-110">O Private Azure Marketplace está ao nível dos inquilinos, pelo que todos os utilizadores sob o inquilino verão a mesma lista com curadoria.</span><span class="sxs-lookup"><span data-stu-id="053c0-110">Private Azure Marketplace is at a tenant level, so all users under the tenant will see the same curated list.</span></span>
> - <span data-ttu-id="053c0-111">Todas as soluções microsoft (incluindo [as distribuições de Linux endossadas)](/azure/virtual-machines/linux/endorsed-distros)são automaticamente adicionadas ao Private Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="053c0-111">All Microsoft solutions (including [Endorsed Linux Distributions](/azure/virtual-machines/linux/endorsed-distros)) are automatically added to Private Azure Marketplace.</span></span>

## <a name="assign-the-marketplace-admin-role"></a><span data-ttu-id="053c0-112">Atribuir o papel de administrador do Marketplace</span><span class="sxs-lookup"><span data-stu-id="053c0-112">Assign the Marketplace admin role</span></span>

<span data-ttu-id="053c0-113">O administrador global inquilino deve atribuir o papel **de administrador do Marketplace** ao administrador privado Azure Marketplace que irá gerir a loja privada.</span><span class="sxs-lookup"><span data-stu-id="053c0-113">The tenant Global administrator must assign the **Marketplace admin** role to the Private Azure Marketplace admin who will manage the private store.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="053c0-114">O acesso à gestão private Azure Marketplace só está disponível para administradores de TI com a função de administração do Marketplace atribuída.</span><span class="sxs-lookup"><span data-stu-id="053c0-114">Access to Private Azure Marketplace management is only available to IT admins with the Marketplace admin role assigned.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="053c0-115">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="053c0-115">Prerequisites</span></span>

<span data-ttu-id="053c0-116">Estes pré-requisitos são necessários antes de poder atribuir a função de Administrador do Mercado a um utilizador no âmbito do arrendatário:</span><span class="sxs-lookup"><span data-stu-id="053c0-116">These prerequisites are required before you can assign the Marketplace Admin role to a user on the tenant scope:</span></span>

- <span data-ttu-id="053c0-117">Tem acesso a um utilizador **administrador global.**</span><span class="sxs-lookup"><span data-stu-id="053c0-117">You have access to a **Global administrator** user.</span></span>
- <span data-ttu-id="053c0-118">O arrendatário tem pelo menos uma subscrição (pode ser qualquer tipo).</span><span class="sxs-lookup"><span data-stu-id="053c0-118">The tenant has at least one subscription (can be any type).</span></span>
- <span data-ttu-id="053c0-119">O utilizador administrador Global é atribuído à função **Contribuinte** ou superior para a subscrição escolhida.</span><span class="sxs-lookup"><span data-stu-id="053c0-119">The Global administrator user is assigned the **Contributor** role or higher for the chosen subscription.</span></span>

### <a name="assign-the-marketplace-admin-role-with-access-control-iam"></a><span data-ttu-id="053c0-120">Atribuir a função de administrador do Marketplace com controlo de acesso (IAM)</span><span class="sxs-lookup"><span data-stu-id="053c0-120">Assign the Marketplace admin role with access control (IAM)</span></span>

1. <span data-ttu-id="053c0-121">Inicie sessão no [portal do Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="053c0-121">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

1. <span data-ttu-id="053c0-122">Selecione **Todos os serviços** e, em seguida, **Marketplace**.</span><span class="sxs-lookup"><span data-stu-id="053c0-122">Select **All services** and then **Marketplace**.</span></span>

1. <span data-ttu-id="053c0-123">Selecione **Private Marketplace** a partir do menu à esquerda.</span><span class="sxs-lookup"><span data-stu-id="053c0-123">Select **Private Marketplace** from the menu on the left.</span></span>

   :::image type="content" source="media/private-azure/private-marketplace.png" lightbox="media/private-azure/private-marketplace-zoom.png" alt-text="Mostra a opção de menu de mercado privado no lado esquerdo do Mercado.":::

1. <span data-ttu-id="053c0-125">Selecione **o controlo de acesso (IAM)** para atribuir a função de administração do Marketplace.</span><span class="sxs-lookup"><span data-stu-id="053c0-125">Select **Access control (IAM)** to assign the Marketplace admin role.</span></span>

   :::image type="content" source="media/private-azure/access-control-iam.png" alt-text="Mostra o ecrã de controlo de acesso I A M.":::

1. <span data-ttu-id="053c0-127">Selecione **+ Adicionar** > **Adicionar atribuição de função**.</span><span class="sxs-lookup"><span data-stu-id="053c0-127">Select **+ Add** > **Add role assignment**.</span></span>

1. <span data-ttu-id="053c0-128">Under **Role**, escolha **Marketplace Admin**.</span><span class="sxs-lookup"><span data-stu-id="053c0-128">Under **Role**, choose **Marketplace Admin**.</span></span>

    :::image type="content" source="media/private-azure/iam-role-assignment.png" alt-text="Mostra o menu de atribuição de funções.":::

1. <span data-ttu-id="053c0-130">Selecione o utilizador desejado da lista de retirada e, em seguida, selecione **'Fazer'.**</span><span class="sxs-lookup"><span data-stu-id="053c0-130">Select the desired user from the dropdown list, then select **Done**.</span></span>

### <a name="assign-the-marketplace-admin-role-with-powershell"></a><span data-ttu-id="053c0-131">Atribuir o papel de administrador do Marketplace com o PowerShell</span><span class="sxs-lookup"><span data-stu-id="053c0-131">Assign the Marketplace admin role with PowerShell</span></span>

<span data-ttu-id="053c0-132">Utilize o seguinte script PowerShell para atribuir a função de Administrador marketplace; requer os seguintes parâmetros:</span><span class="sxs-lookup"><span data-stu-id="053c0-132">Use the following PowerShell script to assign the Marketplace Admin role; it requires the following parameters:</span></span>

- <span data-ttu-id="053c0-133">**TenantId:** A ID do inquilino em âmbito (a função de administrador do Marketplace é atribuível no âmbito do arrendatário).</span><span class="sxs-lookup"><span data-stu-id="053c0-133">**TenantId:** The ID of the tenant in scope (Marketplace admin role is assignable on the tenant scope).</span></span>
- <span data-ttu-id="053c0-134">**SubscriçãoId:** Uma subscrição da qual o administrador global tem **papel contributivo** ou superior atribuído.</span><span class="sxs-lookup"><span data-stu-id="053c0-134">**SubscriptionId:** A subscription of which the global admin has **Contributor** role or higher assigned.</span></span>
- <span data-ttu-id="053c0-135">**GlobalAdminUsername:** O nome de utilizador da administração global.</span><span class="sxs-lookup"><span data-stu-id="053c0-135">**GlobalAdminUsername:** The username of the global admin.</span></span>
- <span data-ttu-id="053c0-136">**Nome de utilizadorToAssignRoleFor:** O nome de utilizador ao qual será atribuída a função de administrador do Marketplace.</span><span class="sxs-lookup"><span data-stu-id="053c0-136">**UsernameToAssignRoleFor:** The user name to which the Marketplace admin role will be assigned.</span></span>

> [!NOTE]
> <span data-ttu-id="053c0-137">Para os utilizadores convidados convidados ao arrendatário, pode demorar até 48 horas até que a sua conta esteja disponível para atribuir o papel de Administrador do Mercado.</span><span class="sxs-lookup"><span data-stu-id="053c0-137">For guest users invited to the tenant, it may take up to 48 hours until their account is available for assigning the Marketplace Admin role.</span></span> <span data-ttu-id="053c0-138">Para mais informações, consulte [as propriedades de um utilizador de colaboração B2B Azure Ative Directory.](/azure/active-directory/b2b/user-properties)</span><span class="sxs-lookup"><span data-stu-id="053c0-138">For more information, see [Properties of an Azure Active Directory B2B collaboration user](/azure/active-directory/b2b/user-properties).</span></span>

```PowerShell
function Assign-MarketplaceAdminRole { 
[CmdletBinding()] 
param( 
[Parameter(Mandatory)] 
[string]$TenantId, 
 
[Parameter(Mandatory)] 
[string]$SubscriptionId, 

 

[Parameter(Mandatory)] 
[string]$GlobalAdminUsername, 

 

[Parameter(Mandatory)] 
[string]$UsernameToAssignRoleFor 
) 

$MarketplaceAdminRoleDefinitionName = "Marketplace Admin" 

 

Write-Output "TenantId = $TenantId" 
Write-Output "SubscriptionId = $SubscriptionId" 
Write-Output "GlobalAdminUsername = $GlobalAdminUsername" 
Write-Output "UsernameToAssignRoleFor = $UsernameToAssignRoleFor" 

 

Write-Output "$($GlobalAdminUsername) is about to assign '$($MarketplaceAdminRoleDefinitionName)' role for $($UsernameToAssignRoleFor)" 

 

$profile = Connect-AzAccount -Tenant $TenantId -SubscriptionId $SubscriptionId

 

 
if($profile -eq $null) 
{ 
Write-Error -Message "Failed to connect to tenant and/or subscription" -ErrorAction Stop 
} 
elseif($profile.Context.Account.Id -ne $GlobalAdminUsername) 
{ 
Write-Error "Connected with $($profile.Context.Account.Id) instead of with the global admin that was specified in the script parameters, which is $($GlobalAdminUsername)" 
} 
else 
{ 
Write-Output "$($GlobalAdminUsername) was connected successfully to Tenant=$($profile.Context.Tenant), Subscription=$($profile.Context.Subscription), AccountId=$($profile.Context.Account.Id), Environment=$($profile.Context.Environment)" 
} 

 

$MarketPlaceAdminRole = Get-AzRoleDefinition $MarketplaceAdminRoleDefinitionName -Scope "/providers/Microsoft.Marketplace"

 

if($MarketPlaceAdminRole -eq $null) 
{ 
Write-Error -Message "'$($MarketplaceAdminRoleDefinitionName)' role is not available" -ErrorAction Stop 
} 
else 
{ 
Write-Output -Message "'$($MarketplaceAdminRoleDefinitionName)' role is available" 
} 

 

Write-Output -Message "About to assign '$($MarketplaceAdminRoleDefinitionName)' role for $($UsernameToAssignRoleFor)..." 

New-AzRoleAssignment -SignInName $UsernameToAssignRoleFor -RoleDefinitionName $MarketplaceAdminRoleDefinitionName -Scope "/providers/Microsoft.Marketplace" 

} 

Assign-MarketplaceAdminRole 
```

<span data-ttu-id="053c0-139">Para obter mais informações sobre os cmdlets contidos no módulo Az.Portal PowerShell, consulte [Microsoft Azure PowerShell: Cmdlets portal Dashboard](/powershell/module/az.portal/).</span><span class="sxs-lookup"><span data-stu-id="053c0-139">For more information about the cmdlets contained in the Az.Portal PowerShell module, see [Microsoft Azure PowerShell: Portal Dashboard cmdlets](/powershell/module/az.portal/).</span></span>

## <a name="create-private-azure-marketplace"></a><span data-ttu-id="053c0-140">Criar Mercado Privado Azure</span><span class="sxs-lookup"><span data-stu-id="053c0-140">Create Private Azure Marketplace</span></span>

1. <span data-ttu-id="053c0-141">Inicie sessão no [portal do Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="053c0-141">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="053c0-142">Selecione **Todos os serviços** e, em seguida, **Marketplace**.</span><span class="sxs-lookup"><span data-stu-id="053c0-142">Select **All services** and then **Marketplace**.</span></span>

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Mostra a janela principal do portal Azure.":::

3. <span data-ttu-id="053c0-144">Selecione **Private Marketplace** a partir do menu à esquerda.</span><span class="sxs-lookup"><span data-stu-id="053c0-144">Select **Private Marketplace** from the menu on the left.</span></span>

4. <span data-ttu-id="053c0-145">Selecione **Introdução** para criar o Private Azure Marketplace (só tem de o fazer uma vez).</span><span class="sxs-lookup"><span data-stu-id="053c0-145">Select **Get Started** to create Private Azure Marketplace (you only have to do this once).</span></span>

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Mostra como selecionar a 'Introdução na janela principal do portal Azure'.":::

    <span data-ttu-id="053c0-147">Se o Private Azure Marketplace já existir para este inquilino, **o Manage Marketplace** será selecionado por padrão.</span><span class="sxs-lookup"><span data-stu-id="053c0-147">If Private Azure Marketplace already exists for this tenant, **Manage Marketplace** will be selected by default.</span></span>

5. <span data-ttu-id="053c0-148">Uma vez concluído, terá um Mercado Privado Azure vazio e desativado.</span><span class="sxs-lookup"><span data-stu-id="053c0-148">Once completed you will have an empty and disabled Private Azure Marketplace.</span></span>

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="Mostra o ecrã vazio do Mercado Privado Azure.":::

## <a name="add-items-from-gallery"></a><span data-ttu-id="053c0-150">Adicione artigos da galeria</span><span class="sxs-lookup"><span data-stu-id="053c0-150">Add items from gallery</span></span>

<span data-ttu-id="053c0-151">Um item é uma combinação de uma oferta e um plano.</span><span class="sxs-lookup"><span data-stu-id="053c0-151">An item is a combination of an offer and a plan.</span></span> <span data-ttu-id="053c0-152">Pode pesquisar e adicionar itens na página 'Gerir Mercado'.</span><span class="sxs-lookup"><span data-stu-id="053c0-152">You can search for and add items on the Manage Marketplace page.</span></span>

1. <span data-ttu-id="053c0-153">**Selecione Adicionar itens**.</span><span class="sxs-lookup"><span data-stu-id="053c0-153">Select **Add items**.</span></span>

2. <span data-ttu-id="053c0-154">Navegue na **Galeria** ou utilize o campo de pesquisa para encontrar o item que deseja.</span><span class="sxs-lookup"><span data-stu-id="053c0-154">Browse the **Gallery** or use the search field to find the item you want.</span></span>

   :::image type="content" source="media/private-azure/marketplace-gallery.png" lightbox="media/private-azure/marketplace-gallery-zoom.png" alt-text="Mostra como navegar na galeria ou utilizar o campo de pesquisa.":::

3. <span data-ttu-id="053c0-156">Como padrão, ao adicionar uma nova oferta, todos os planos atuais serão adicionados à lista aprovada.</span><span class="sxs-lookup"><span data-stu-id="053c0-156">As default, when adding a new offer, all current plans will be added to the approved list.</span></span> <span data-ttu-id="053c0-157">Para modificar a seleção do plano antes de adicionar os itens selecionados, selecione o menu suspenso no azulejo da oferta e atualize os planos necessários.</span><span class="sxs-lookup"><span data-stu-id="053c0-157">To modify the plan selection before adding the selected items, select the drop-down menu in the offer's tile and update the required plans.</span></span>

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Mostra como atualizar os planos necessários.":::

4. <span data-ttu-id="053c0-159">Selecione **Feito** na parte inferior esquerda depois de ter feito as suas seleções.</span><span class="sxs-lookup"><span data-stu-id="053c0-159">Select **Done** at the bottom-left after you've made your selections.</span></span>

>[!Note]
> <span data-ttu-id="053c0-160">**Adicionar itens** ao Mercado estará disponível apenas para ofertas não microsoft.</span><span class="sxs-lookup"><span data-stu-id="053c0-160">**Add Items** to the Marketplace will be available for non-Microsoft offers only.</span></span> <span data-ttu-id="053c0-161">As soluções da Microsoft (incluindo [as Distribuições Linux endossadas)](/azure/virtual-machines/linux/endorsed-distros)serão marcadas como "Aprovadas por padrão" e não podem ser geridas no Private Marketplace.</span><span class="sxs-lookup"><span data-stu-id="053c0-161">Microsoft solutions (including [Endorsed Linux Distributions](/azure/virtual-machines/linux/endorsed-distros)) will be tagged as "Approved by default" and cannot be managed in Private Marketplace.</span></span>

## <a name="edit-items-plans"></a><span data-ttu-id="053c0-162">Editar os planos do item</span><span class="sxs-lookup"><span data-stu-id="053c0-162">Edit item's plans</span></span>

<span data-ttu-id="053c0-163">Pode editar os planos de um item na página Manage Marketplace.</span><span class="sxs-lookup"><span data-stu-id="053c0-163">You can edit an item's plans on the Manage Marketplace page.</span></span>

1. <span data-ttu-id="053c0-164">Na coluna **Planos,** reveja os planos disponíveis do menu suspenso para esse item.</span><span class="sxs-lookup"><span data-stu-id="053c0-164">In the **Plans** column, review the available plans from the dropdown menu for that item.</span></span>

2. <span data-ttu-id="053c0-165">Selecione ou limpe as caixas de verificação para escolher quais os planos para disponibilizar aos seus utilizadores.</span><span class="sxs-lookup"><span data-stu-id="053c0-165">Select or clear the checkboxes to choose which plans to make available to your users.</span></span>

   :::image type="content" source="media/private-azure/edit-items.png" alt-text="Mostra como selecionar ou limpar a caixa de verificação para o item necessário.":::

   > [!NOTE]
   > <span data-ttu-id="053c0-167">Cada oferta precisa de pelo menos um plano selecionado para que a atualização ocorra.</span><span class="sxs-lookup"><span data-stu-id="053c0-167">Each offer needs at least one plan selected for the update to occur.</span></span> <span data-ttu-id="053c0-168">Para remover todos os planos relacionados com uma oferta, elimine toda a oferta (ver secção seguinte).</span><span class="sxs-lookup"><span data-stu-id="053c0-168">To remove all plans related to an offer, delete the entire offer (see next section).</span></span>

## <a name="delete-offers"></a><span data-ttu-id="053c0-169">Excluir ofertas</span><span class="sxs-lookup"><span data-stu-id="053c0-169">Delete offers</span></span>

<span data-ttu-id="053c0-170">Na página Manage Marketplace, selecione a caixa de verificação ao lado do nome da oferta (ver ecrã acima) e selecione **Eliminar itens**.</span><span class="sxs-lookup"><span data-stu-id="053c0-170">In the Manage Marketplace page, select the check box next to the offer name (see screen above) and select **Delete items**.</span></span>

## <a name="enabledisable-private-azure-marketplace"></a><span data-ttu-id="053c0-171">Ativar/desativar o Mercado Privado de Azure</span><span class="sxs-lookup"><span data-stu-id="053c0-171">Enable/disable Private Azure Marketplace</span></span>

<span data-ttu-id="053c0-172">Na página Manage Marketplace você verá um destes banners, que mostram o estado atual do Mercado Privado Azure:</span><span class="sxs-lookup"><span data-stu-id="053c0-172">In the Manage Marketplace page you will see one of these banners, which show the current state of Private Azure Marketplace:</span></span>

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Mostra o banner &quot;Desativar o estado&quot;.":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Mostra o banner &quot;Enable state&quot;.":::

<span data-ttu-id="053c0-175">Pode ativar ou desativar o Private Azure Marketplace conforme necessário.</span><span class="sxs-lookup"><span data-stu-id="053c0-175">You can enable or disable Private Azure Marketplace as needed.</span></span>

- <span data-ttu-id="053c0-176">Se estiver desativado, selecione **Enable Private Marketplace** para ativar.</span><span class="sxs-lookup"><span data-stu-id="053c0-176">If disabled, select **Enable Private Marketplace** to enable.</span></span>
- <span data-ttu-id="053c0-177">Se estiver ativado, **selecione Desativar o Mercado Privado** para desativar.</span><span class="sxs-lookup"><span data-stu-id="053c0-177">If enabled, select **Disable Private Marketplace** to disable.</span></span>

## <a name="private-azure-marketplace-notification-center"></a><span data-ttu-id="053c0-178">Centro de notificação private Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="053c0-178">Private Azure Marketplace notification center</span></span>

<span data-ttu-id="053c0-179">O Centro de Notificação é composto por três tipos de notificações e permite ao administrador do Marketplace tomar medidas com base na notificação:</span><span class="sxs-lookup"><span data-stu-id="053c0-179">Notification Center consists of three types of notifications and allows the Marketplace admin to take actions based on the notification:</span></span>

- <span data-ttu-id="053c0-180">Pedidos de aprovação dos utilizadores para itens que não constam da lista aprovada (ver [Pedido de adicionar ofertas ou planos](#request-to-add-offers-or-plans) abaixo).</span><span class="sxs-lookup"><span data-stu-id="053c0-180">Approval requests from users for items that are not in the approved list (see [Request to add offers or plans](#request-to-add-offers-or-plans) below).</span></span>
- <span data-ttu-id="053c0-181">Novas notificações de plano para ofertas que já tenham um ou mais planos na lista aprovada.</span><span class="sxs-lookup"><span data-stu-id="053c0-181">New plan notifications for offers that already have one or more plans in the approved list.</span></span>
- <span data-ttu-id="053c0-182">Removidos notificações do plano para itens que estão na lista aprovada, mas foram removidos do mercado global de Azure.</span><span class="sxs-lookup"><span data-stu-id="053c0-182">Removed plan notifications for items that are in the approved list but were removed from the global Azure Marketplace.</span></span>

<span data-ttu-id="053c0-183">Para aceder ao centro de notificação:</span><span class="sxs-lookup"><span data-stu-id="053c0-183">To access the notification center:</span></span>

1. <span data-ttu-id="053c0-184">Selecione **Notificações** do menu do lado esquerdo.</span><span class="sxs-lookup"><span data-stu-id="053c0-184">Select **Notifications** from the left-side menu.</span></span>

   :::image type="content" source="media/private-azure/marketplace-notifications-small.png" lightbox="media/private-azure/marketplace-notifications.png" alt-text="Mostra o menu notificações.":::

1. <span data-ttu-id="053c0-186">Selecione o menu de elipses para mais ações.</span><span class="sxs-lookup"><span data-stu-id="053c0-186">Select the ellipsis menu for more actions.</span></span>

    :::image type="content" source="media/private-azure/notifications-more-options.png" alt-text="Mostra os resultados do menu Mais Opções.":::

1. <span data-ttu-id="053c0-188">Para pedidos de plano, **os pedidos do Show** abrem o formulário de pedido de aprovação onde pode rever todos os pedidos do utilizador para a oferta específica.</span><span class="sxs-lookup"><span data-stu-id="053c0-188">For plan requests, **Show requests** opens the approval request form where you can review all user requests for the specific offer.</span></span>
1. <span data-ttu-id="053c0-189">Selecione **Aprovar** ou **Rejeitar**.</span><span class="sxs-lookup"><span data-stu-id="053c0-189">Select **Approve** or **Reject**.</span></span>

   :::image type="content" source="media/private-azure/notifications-approve-reject-small.png" lightbox="media/private-azure/notifications-approve-reject.png" alt-text="Mostra as opções de aprovação e rejeição.":::

1. <span data-ttu-id="053c0-191">Selecione o plano para aprovar no menu suspenso.</span><span class="sxs-lookup"><span data-stu-id="053c0-191">Select the plan to approve from the drop-down menu.</span></span>
1. <span data-ttu-id="053c0-192">Adicione um comentário e **selecione Enviar por isso.**</span><span class="sxs-lookup"><span data-stu-id="053c0-192">Add a comment and select **Submit**.</span></span>

## <a name="browsing-private-azure-marketplace"></a><span data-ttu-id="053c0-193">Navegar no Mercado Privado Azure</span><span class="sxs-lookup"><span data-stu-id="053c0-193">Browsing Private Azure Marketplace</span></span>

<span data-ttu-id="053c0-194">Quando o Private Azure Marketplace estiver ativado, os utilizadores verão quais os planos que o administrador do Marketplace aprovou.</span><span class="sxs-lookup"><span data-stu-id="053c0-194">When Private Azure Marketplace is enabled, users will see which plans the Marketplace admin has approved.</span></span>

- <span data-ttu-id="053c0-195">Um **aviso** aprovado verde indica uma oferta de Parceiro (não Microsoft) que é aprovada.</span><span class="sxs-lookup"><span data-stu-id="053c0-195">A green **Approved** notice indicates a Partner (non-Microsoft) offer that is approved.</span></span>
- <span data-ttu-id="053c0-196">Um aviso **aprovado** azul indica uma oferta da Microsoft (incluindo [distribuições de Linux endossadas)](/azure/virtual-machines/linux/endorsed-distros)que é aprovada.</span><span class="sxs-lookup"><span data-stu-id="053c0-196">A blue **Approved** notice indicates a Microsoft offer (including [Endorsed Linux distributions](/azure/virtual-machines/linux/endorsed-distros)) that is approved.</span></span>

<span data-ttu-id="053c0-197">Os utilizadores podem filtrar entre ofertas que são e não são aprovadas:</span><span class="sxs-lookup"><span data-stu-id="053c0-197">Users can filter between offers that are and are not approved:</span></span>

   :::image type="content" source="media/private-azure/filter-option-small.png" lightbox="media/private-azure/filter-option.png" alt-text="Mostra a opção de filtragem.":::

## <a name="buy-or-deploy-in-private-azure-marketplace"></a><span data-ttu-id="053c0-199">Comprar ou implementar no Private Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="053c0-199">Buy or deploy in Private Azure Marketplace</span></span>

<span data-ttu-id="053c0-200">Embora a experiência da página de detalhes do produto seja semelhante ao Azure Marketplace global, existem três cenários específicos do Private Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="053c0-200">While the product details page experience is similar to the global Azure Marketplace, there are three Private Azure Marketplace specific scenarios.</span></span>

- <span data-ttu-id="053c0-201">Quando um utilizador seleciona um plano aprovado, o botão **Criar** está ativado:</span><span class="sxs-lookup"><span data-stu-id="053c0-201">When a user selects an approved plan, the **Create** button is enabled:</span></span>

   :::image type="content" source="media/private-azure/button-create-enabled-small.png" lightbox="media/private-azure/button-create-enabled.png" alt-text="Mostra o banner de oferta observando que um plano pode ser criado.":::

- <span data-ttu-id="053c0-203">Se uma seleção de plano de produto não aparecer na página de detalhes do produto, mas o administrador aprovou um ou mais planos, um banner assinala quais os planos aprovados e o botão **Criar** está ativado:</span><span class="sxs-lookup"><span data-stu-id="053c0-203">If a product plan selection does not appear in the product details page but the admin approved one or more plans, a banner notes which plans are approved and the **Create** button is enabled:</span></span>

   :::image type="content" source="media/private-azure/button-create-enabled-and-plans-small.png" lightbox="media/private-azure/button-create-enabled-and-plans.png" alt-text="Mostra o banner da oferta notando que um plano pode ser criado e mostrando planos disponíveis.":::

- <span data-ttu-id="053c0-205">Quando um utilizador seleciona um plano não aprovado, um banner assinala o plano como não aprovado e o botão **Criar** é desativado.</span><span class="sxs-lookup"><span data-stu-id="053c0-205">When a user selects a non-approved plan, a banner notes the plan as not approved and the **Create** button is disabled.</span></span> <span data-ttu-id="053c0-206">O utilizador ainda pode solicitar a adição do plano à lista aprovada (ver secção seguinte).</span><span class="sxs-lookup"><span data-stu-id="053c0-206">The user can still request to add the plan to the approved list (see next section).</span></span>

## <a name="request-to-add-offers-or-plans"></a><span data-ttu-id="053c0-207">Pedido de adição de ofertas ou planos</span><span class="sxs-lookup"><span data-stu-id="053c0-207">Request to add offers or plans</span></span>

<span data-ttu-id="053c0-208">Pode solicitar a adição de uma oferta pública ou plano que não esteja atualmente aprovado no Mercado Privado Azure.</span><span class="sxs-lookup"><span data-stu-id="053c0-208">You can request to add a public offer or plan that is not currently approved in the Private Azure Marketplace.</span></span>

1. <span data-ttu-id="053c0-209">Selecione **Pedido para adicionar** no banner para abrir o formulário de pedido de **acesso**.</span><span class="sxs-lookup"><span data-stu-id="053c0-209">Select **Request to add** in the banner to open the **Access request form**.</span></span>

   :::image type="content" source="media/private-azure/request-banner-small.png" lightbox="media/private-azure/request-banner.png" alt-text="Mostra o banner com o link 'Pedido de adicionar'.":::

   :::image type="content" source="media/private-azure/access-request-form-small.png" lightbox="media/private-azure/access-request-form.png" alt-text="Mostra o formulário de pedido de acesso para ofertas ou planos.":::

1. <span data-ttu-id="053c0-212">Selecione quais os planos para adicionar ao pedido (**Qualquer Plano** diz ao administrador do Marketplace que você não tem uma preferência por um plano dentro de uma oferta).</span><span class="sxs-lookup"><span data-stu-id="053c0-212">Select which plans to add to the request (**Any Plan** tells the Marketplace admin that you don't have a preference for a plan within an offer).</span></span>

1. <span data-ttu-id="053c0-213">Adicione uma **Justificação** e selecione **Pedido** para submeter o seu pedido.</span><span class="sxs-lookup"><span data-stu-id="053c0-213">Add a **Justification** and select **Request** to submit your request.</span></span>

   :::image type="content" source="media/private-azure/access-request-form-filled-small.png" lightbox="media/private-azure/access-request-form-filled.png" alt-text="Mostra o formulário de pedido de acesso para ofertas ou planos com entradas de amostra.":::

1. <span data-ttu-id="053c0-215">Uma indicação para um pedido pendente aparecerá no formulário de pedido de Acesso com opção de **retirar o pedido.**</span><span class="sxs-lookup"><span data-stu-id="053c0-215">An indication for a pending request will appear in the Access request form with an option to **Withdraw request**.</span></span>

   :::image type="content" source="media/private-azure/approved-pending-plans-small.png" lightbox="media/private-azure/approved-pending-plans.png" alt-text="Mostra uma lista de planos aprovados ou pendentes com link Pedido de Retirada.":::

> [!NOTE]
> <span data-ttu-id="053c0-217">Uma vez apresentado, o formulário de pedido de aprovação será enviado ao [Centro de Notificação](#private-azure-marketplace-notification-center) do Administrador do Mercado para rever o pedido e tomar medidas.</span><span class="sxs-lookup"><span data-stu-id="053c0-217">Once submitted, the approval request form will be sent to the [Notification Center](#private-azure-marketplace-notification-center) for the Marketplace admin to review the request and take action.</span></span>

> [!CAUTION]
> <span data-ttu-id="053c0-218">A aprovação no Mercado Privado não indica a aquisição de uma solução.</span><span class="sxs-lookup"><span data-stu-id="053c0-218">Approval into Private Marketplace does not indicate procurement of a solution.</span></span>

## <a name="frequently-asked-questions-faqs"></a><span data-ttu-id="053c0-219">Perguntas frequentes (Perguntas Frequentes)</span><span class="sxs-lookup"><span data-stu-id="053c0-219">Frequently Asked Questions (FAQs)</span></span>

#### <a name="i-am-already-blocking-marketplace-third-party-application-through-azure-policy-how-is-this-different"></a><span data-ttu-id="053c0-220">Já estou a bloquear a aplicação de terceiros do Marketplace através da Política Azure.</span><span class="sxs-lookup"><span data-stu-id="053c0-220">I am already blocking Marketplace third-party application through Azure Policy.</span></span> <span data-ttu-id="053c0-221">Como é que isto é diferente?</span><span class="sxs-lookup"><span data-stu-id="053c0-221">How is this different?</span></span>

<span data-ttu-id="053c0-222">Existem atualmente duas formas de restringir os serviços de terceiros no Marketplace:</span><span class="sxs-lookup"><span data-stu-id="053c0-222">There are currently two ways to restrict third-party services in Marketplace:</span></span>

1. <span data-ttu-id="053c0-223">Através do portal EA ou do portal Azure, desative os serviços de terceiros ou limite-se apenas a "SKUs gratuitos ou BYOL".</span><span class="sxs-lookup"><span data-stu-id="053c0-223">Through EA portal or the Azure portal, disable third-party services or restrict to "Free or BYOL SKUs only".</span></span>

    :::image type="content" source="media/private-azure/disable-services.png" alt-text="Mostra como restringir os serviços no portal Azure.":::

    :::image type="content" source="media/private-azure/disable-services-other-view.png" alt-text="Mostra como restringir os serviços no portal E A.":::

2. <span data-ttu-id="053c0-226">Crie uma política Azure apenas para permitir VMs específicos.</span><span class="sxs-lookup"><span data-stu-id="053c0-226">Create an Azure policy to only allow specific VMs.</span></span> <span data-ttu-id="053c0-227">Para obter detalhes sobre como impor a política aos VMs Windows, consulte [aplicar políticas para Windows VMs com O Gestor de Recursos Azure](/azure/virtual-machines/windows/policy).</span><span class="sxs-lookup"><span data-stu-id="053c0-227">For details on how to enforce policy to Windows VMs, see [Apply policies to Windows VMs with Azure Resource Manager](/azure/virtual-machines/windows/policy).</span></span>

<span data-ttu-id="053c0-228">O Private Azure Marketplace permite uma maior flexibilidade na limitação e na possibilidade de ofertas e planos específicos.</span><span class="sxs-lookup"><span data-stu-id="053c0-228">Private Azure Marketplace allows more flexibility on restricting and allowing specific offers and plans.</span></span> <span data-ttu-id="053c0-229">Informa os utilizadores finais sobre a disponibilidade para implantação na galeria do mercado mesmo antes de tentarem implementar serviços de terceiros.</span><span class="sxs-lookup"><span data-stu-id="053c0-229">It informs end users on the availability for deployment in the marketplace gallery even before they try to deploy third-party services.</span></span> <span data-ttu-id="053c0-230">Para permitir a implantação de serviços de terceiros, defina o Azure Marketplace para On/Enabled no Portal EA e no portal Azure.</span><span class="sxs-lookup"><span data-stu-id="053c0-230">To allow deployment of third-party services, set Azure Marketplace to On/Enabled in EA Portal and the Azure portal.</span></span>

- <span data-ttu-id="053c0-231">O Private Azure Marketplace pode curar soluções parceiras não limitadas a máquinas virtuais.</span><span class="sxs-lookup"><span data-stu-id="053c0-231">Private Azure Marketplace can curate partner solutions not limited to virtual machines.</span></span>
- <span data-ttu-id="053c0-232">O Private Azure Marketplace pode ser curador ao nível do plano e pode ainda definir "Plano atual e futuro".</span><span class="sxs-lookup"><span data-stu-id="053c0-232">Private Azure Marketplace can curate at the plan level and can also set "Current and future plan".</span></span>
- <span data-ttu-id="053c0-233">O Private Azure Marketplace pode informar os utilizadores finais adiantado sobre o que pode ou não ser implementado.</span><span class="sxs-lookup"><span data-stu-id="053c0-233">Private Azure Marketplace can inform the end users up front on what can and cannot be deployed.</span></span>

#### <a name="whats-the-difference-between-a-private-offer-and-private-azure-marketplace"></a><span data-ttu-id="053c0-234">Qual é a diferença entre uma Oferta Privada e o Mercado Privado Azure?</span><span class="sxs-lookup"><span data-stu-id="053c0-234">What's the difference between a Private Offer and Private Azure Marketplace?</span></span>

<span data-ttu-id="053c0-235">Uma **Oferta Privada** permite que os editores criem planos que só são visíveis para clientes direcionados.</span><span class="sxs-lookup"><span data-stu-id="053c0-235">A **Private Offer** lets publishers create plans that are only visible to targeted customers.</span></span> <span data-ttu-id="053c0-236">Isto permite-lhes partilhar em privado soluções personalizadas com preços e condições negociados, termos e condições privados e configurações especializadas.</span><span class="sxs-lookup"><span data-stu-id="053c0-236">This lets them privately share customized solutions with negotiated pricing, private terms and conditions, and specialized configurations.</span></span> <span data-ttu-id="053c0-237">Para mais detalhes, consulte [ofertas privadas no mercado comercial.](/azure/marketplace/private-offers)</span><span class="sxs-lookup"><span data-stu-id="053c0-237">For details, see [Private offers in the commercial marketplace](/azure/marketplace/private-offers).</span></span>

<span data-ttu-id="053c0-238">**O Private Azure Marketplace** no portal Azure permite aos administradores pré-aprovarem quais as soluções de terceiros que os seus utilizadores podem implementar.</span><span class="sxs-lookup"><span data-stu-id="053c0-238">**Private Azure Marketplace** in the Azure portal lets administrators pre-approve which third-party solutions their users can deploy.</span></span> <span data-ttu-id="053c0-239">Com um Private Azure Marketplace, os utilizadores podem usufruir dos benefícios do Azure Marketplace, encontrando, comprando e implementando ofertas compatíveis.</span><span class="sxs-lookup"><span data-stu-id="053c0-239">With a Private Azure Marketplace, users can enjoy the benefits of Azure Marketplace by finding, buying, and deploying compliant offers.</span></span> <span data-ttu-id="053c0-240">Para gerir ofertas privadas baseadas em subscrições no Mercado Privado, o administrador do Marketplace deve ter um papel mínimo de "leitura" na subscrição específica.</span><span class="sxs-lookup"><span data-stu-id="053c0-240">To manage subscription-based Private Offers in Private Marketplace, the Marketplace admin must have a minimum of "read" role on the specific subscription.</span></span>

#### <a name="i-added-a-private-offer-to-the-private-azure-marketplace-why-is-it-not-showing-in-the-manage-marketplace-tab"></a><span data-ttu-id="053c0-241">Adicionei uma Oferta Privada ao Private Azure Marketplace, porque é que não está a aparecer no separador de mercado de gestão?</span><span class="sxs-lookup"><span data-stu-id="053c0-241">I added a Private Offer to the Private Azure Marketplace, why is it not showing in the manage marketplace tab?</span></span>

<span data-ttu-id="053c0-242">As Ofertas Privadas baseadas em subscrições são visíveis apenas para as subscrições listadas nas definições de Oferta Privada.</span><span class="sxs-lookup"><span data-stu-id="053c0-242">Subscription-based Private Offers are visible only for the listed subscriptions in the Private Offer settings.</span></span> <span data-ttu-id="053c0-243">Para ver a Oferta Privada, certifique-se de que o filtro global de subscrição está mostrando todas as subscrições.</span><span class="sxs-lookup"><span data-stu-id="053c0-243">To view the Private Offer, ensure the global subscription filter is showing all the subscriptions.</span></span>

   :::image type="content" source="media/private-azure/private-marketplace-filter.png" lightbox="media/private-azure/private-marketplace-filter.png" alt-text="Mostra o filtro do mercado privado.":::

#### <a name="can-we-include-custom-images-in-private-azure-marketplace"></a><span data-ttu-id="053c0-245">Podemos incluir imagens personalizadas no Private Azure Marketplace?</span><span class="sxs-lookup"><span data-stu-id="053c0-245">Can we include custom images in Private Azure Marketplace?</span></span>

<span data-ttu-id="053c0-246">N.º</span><span class="sxs-lookup"><span data-stu-id="053c0-246">No.</span></span> <span data-ttu-id="053c0-247">O Private Azure Marketplace permite que qualquer administrador de TI gere e cuide de soluções de terceiros a partir do Mercado Azure Global.</span><span class="sxs-lookup"><span data-stu-id="053c0-247">Private Azure Marketplace allows any IT administrator to manage and curate third-party solutions from global Azure Marketplace.</span></span> <span data-ttu-id="053c0-248">Uma vez que as imagens personalizadas não estão no Azure Marketplace global, o administrador de TI não pode escolher as suas imagens personalizadas.</span><span class="sxs-lookup"><span data-stu-id="053c0-248">Since custom images are not on global Azure Marketplace, the IT administrator cannot pick and choose your custom images.</span></span> <span data-ttu-id="053c0-249">Se quiser partilhar imagens personalizadas, utilize a [Galeria de Imagens Partilhadas.](/azure/virtual-machines/shared-image-galleries)</span><span class="sxs-lookup"><span data-stu-id="053c0-249">If you would like to share custom images, use [Shared Image Gallery](/azure/virtual-machines/shared-image-galleries).</span></span>

1. <span data-ttu-id="053c0-250">Guia passo a passo Criar uma Galeria de Imagem Partilhada (SIG)[(CLI,](/azure/virtual-machines/shared-images-cli) [PowerShell).](/azure/virtual-machines/shared-images-powershell)</span><span class="sxs-lookup"><span data-stu-id="053c0-250">Step-by-step guide Create a Shared Image Gallery (SIG) ([CLI](/azure/virtual-machines/shared-images-cli), [PowerShell](/azure/virtual-machines/shared-images-powershell)).</span></span>
2. <span data-ttu-id="053c0-251">Crie uma definição de imagem dentro de um SIG.</span><span class="sxs-lookup"><span data-stu-id="053c0-251">Create an image definition within a SIG.</span></span> <span data-ttu-id="053c0-252">O cliente deve escolher **generalizado** para o campo estado-OS.</span><span class="sxs-lookup"><span data-stu-id="053c0-252">Customer should choose **Generalized** for the OS-state field.</span></span> <span data-ttu-id="053c0-253">([CLI,](/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition) [PowerShell).](/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)</span><span class="sxs-lookup"><span data-stu-id="053c0-253">([CLI](/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition), [PowerShell](/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).</span></span>
3. <span data-ttu-id="053c0-254">Traga a imagem gerida para a Galeria de Imagens Partilhadas[(CLI,](/azure/virtual-machines/image-version-managed-image-cli) [PowerShell).](/azure/virtual-machines/image-version-managed-image-powershell)</span><span class="sxs-lookup"><span data-stu-id="053c0-254">Bring managed image into the Shared Image Gallery ([CLI](/azure/virtual-machines/image-version-managed-image-cli), [PowerShell](/azure/virtual-machines/image-version-managed-image-powershell)).</span></span>
4. <span data-ttu-id="053c0-255">As imagens SIG VM residiriam numa subscrição.</span><span class="sxs-lookup"><span data-stu-id="053c0-255">The SIG VM images would reside in one subscription.</span></span> <span data-ttu-id="053c0-256">Para disponibilizá-lo a outras subscrições, utilize um registo de aplicações[(CLI,](/azure/virtual-machines/linux/share-images-across-tenants) [PowerShell).](/azure/virtual-machines/windows/share-images-across-tenants)</span><span class="sxs-lookup"><span data-stu-id="053c0-256">To make it available to other subscriptions, use an app registration ([CLI](/azure/virtual-machines/linux/share-images-across-tenants), [PowerShell](/azure/virtual-machines/windows/share-images-across-tenants)).</span></span>

#### <a name="why-do-i-see-some-offers-approved-by-default-even-though-the-publisher-is-not-microsoft"></a><span data-ttu-id="053c0-257">Por que vejo algumas ofertas **aprovadas por padrão,** mesmo que a editora não seja a Microsoft?</span><span class="sxs-lookup"><span data-stu-id="053c0-257">Why do I see some offers **Approved by default** even though the publisher is not Microsoft?</span></span>

<span data-ttu-id="053c0-258">A Microsoft suporta o Linux e a tecnologia open-source em Azure.</span><span class="sxs-lookup"><span data-stu-id="053c0-258">Microsoft supports Linux and open-source technology in Azure.</span></span> <span data-ttu-id="053c0-259">[As distribuições de Linux endossadas](/azure/virtual-machines/linux/endorsed-distros) são suportadas no Azure e o preço está integrado em máquinas virtuais.</span><span class="sxs-lookup"><span data-stu-id="053c0-259">[Endorsed Linux distributions](/azure/virtual-machines/linux/endorsed-distros) are supported on Azure and the price is integrated in virtual machines.</span></span> <span data-ttu-id="053c0-260">Uma vez que o Agente Azure Linux já está pré-instalado no Azure Marketplace, é tratado como uma oferta da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="053c0-260">Because Azure Linux Agent is already pre-installed on Azure Marketplace, it is treated like a Microsoft offer.</span></span> <span data-ttu-id="053c0-261">Uma vez que as ofertas da Microsoft são aprovadas por padrão, as distribuições de Linux endossadas não podem ser geridas no Private Azure Marketplace e são aprovadas por padrão.</span><span class="sxs-lookup"><span data-stu-id="053c0-261">Since Microsoft offers are approved by default, endorsed Linux distributions cannot be managed in Private Azure Marketplace and are approved by default.</span></span>

## <a name="contact-support"></a><span data-ttu-id="053c0-262">Contactar o suporte</span><span class="sxs-lookup"><span data-stu-id="053c0-262">Contact support</span></span>

- <span data-ttu-id="053c0-263">Para obter suporte ao Azure Marketplace, visite [o Microsoft Q&A](/answers/products/).</span><span class="sxs-lookup"><span data-stu-id="053c0-263">For Azure Marketplace support, visit [Microsoft Q&A](/answers/products/).</span></span>