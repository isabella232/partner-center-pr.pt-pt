---
title: Criar e gerir o Private Azure Marketplace no portal Azure
description: Saiba como criar e gerir o Private Azure Marketplace (pré-visualização) no portal Azure.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: article
author: keferna
ms.author: keferna
ms.date: 09/18/2020
ms.openlocfilehash: c0a395a7c5bfe926cdc56d7386aaaebb0305fb68
ms.sourcegitcommit: d31c06022624ca2d1db12b3c60ef1d0a3861f763
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/19/2020
ms.locfileid: "92529759"
---
# <a name="create-and-manage-private-azure-marketplace-preview-in-the-azure-portal"></a><span data-ttu-id="155b0-103">Criar e gerir o Private Azure Marketplace (pré-visualização) no portal Azure</span><span class="sxs-lookup"><span data-stu-id="155b0-103">Create and manage Private Azure Marketplace (preview) in the Azure portal</span></span>

<span data-ttu-id="155b0-104">O Private Azure Marketplace (pré-visualização) permite aos administradores governar quais as soluções de terceiros que os seus utilizadores podem utilizar.</span><span class="sxs-lookup"><span data-stu-id="155b0-104">Private Azure Marketplace (preview) lets administrators govern which third-party solutions their users can use.</span></span> <span data-ttu-id="155b0-105">Fá-lo permitindo-lhe implementar apenas ofertas que aprove e que cumpram as políticas da sua empresa.</span><span class="sxs-lookup"><span data-stu-id="155b0-105">It does this by allowing you to deploy only offers that you approve and that comply with your enterprise's policies.</span></span> <span data-ttu-id="155b0-106">Com o Private Azure Marketplace, os seus utilizadores podem pesquisar na loja online ofertas compatíveis para comprar e implementar.</span><span class="sxs-lookup"><span data-stu-id="155b0-106">With Private Azure Marketplace, your users can search the online store for compliant offers to purchase and deploy.</span></span> 

<span data-ttu-id="155b0-107">Como administrador do Marketplace (papel atribuído), começará com uma Loja Privada desativada e vazia, onde poderá adicionar as suas ofertas e planos aprovados.</span><span class="sxs-lookup"><span data-stu-id="155b0-107">As a Marketplace admin (assigned role), you will start with a disabled and empty Private Store where you can add your approved offers and plans.</span></span> <span data-ttu-id="155b0-108">Este artigo explica como criar, gerir e ativar o Private Azure Marketplace para os seus utilizadores.</span><span class="sxs-lookup"><span data-stu-id="155b0-108">This article explains how to create, manage, and enable Private Azure Marketplace for your users.</span></span>

<span data-ttu-id="155b0-109">Notas:</span><span class="sxs-lookup"><span data-stu-id="155b0-109">Notes:</span></span>

- <span data-ttu-id="155b0-110">O Private Azure Marketplace está ao nível dos inquilinos, pelo que todos os utilizadores sob o inquilino verão a mesma lista com curadoria.</span><span class="sxs-lookup"><span data-stu-id="155b0-110">Private Azure Marketplace is at a tenant level, so all users under the tenant will see the same curated list.</span></span>
- <span data-ttu-id="155b0-111">Todas as soluções microsoft são automaticamente adicionadas ao Private Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="155b0-111">All Microsoft solutions are automatically added to Private Azure Marketplace.</span></span>

## <a name="assign-the-marketplace-admin-role"></a><span data-ttu-id="155b0-112">Atribuir o papel de administrador do Marketplace</span><span class="sxs-lookup"><span data-stu-id="155b0-112">Assign the Marketplace admin role</span></span>

<span data-ttu-id="155b0-113">O administrador global inquilino deve atribuir o papel **de administrador do Marketplace** ao administrador privado Azure Marketplace que irá gerir a loja privada.</span><span class="sxs-lookup"><span data-stu-id="155b0-113">The tenant Global administrator must assign the **Marketplace admin** role to the Private Azure Marketplace admin who will manage the private store.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="155b0-114">O acesso à gestão private Azure Marketplace só está disponível para administradores de TI com a função de administração do Marketplace atribuída.</span><span class="sxs-lookup"><span data-stu-id="155b0-114">Access to Private Azure Marketplace management is only available to IT admins with the Marketplace admin role assigned.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="155b0-115">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="155b0-115">Prerequisites</span></span>

<span data-ttu-id="155b0-116">Deve cumprir estes pré-requisitos antes de poder atribuir a função de Administrador do Marketplace a um utilizador no âmbito do arrendatário:</span><span class="sxs-lookup"><span data-stu-id="155b0-116">You must meet these prerequisites before you can assign the Marketplace Admin role to a user on the tenant scope:</span></span>

- <span data-ttu-id="155b0-117">Tem acesso a um utilizador **administrador global.**</span><span class="sxs-lookup"><span data-stu-id="155b0-117">You have access to a **Global administrator** user.</span></span>
- <span data-ttu-id="155b0-118">O arrendatário tem pelo menos uma Subscrição (pode ser qualquer tipo).</span><span class="sxs-lookup"><span data-stu-id="155b0-118">The tenant has at least one Subscription (can be any type).</span></span>
- <span data-ttu-id="155b0-119">O utilizador administrador Global é atribuído à função **Contribuinte** ou superior para a subscrição escolhida no passo 2.</span><span class="sxs-lookup"><span data-stu-id="155b0-119">The Global administrator user is assigned the **Contributor** role or higher for the subscription chosen in step 2.</span></span>
- <span data-ttu-id="155b0-120">O utilizador administrador global tem um acesso elevado definido para **Sim** (ver [elevate-access-global-admin).](/azure/role-based-access-control/elevate-access-global-admin)</span><span class="sxs-lookup"><span data-stu-id="155b0-120">The Global administrator user has elevated access set to **Yes** (see [elevate-access-global-admin](/azure/role-based-access-control/elevate-access-global-admin)).</span></span>

### <a name="assign-the-marketplace-admin-role-with-powershell"></a><span data-ttu-id="155b0-121">Atribuir o papel de administrador do Marketplace com o PowerShell</span><span class="sxs-lookup"><span data-stu-id="155b0-121">Assign the Marketplace admin role with PowerShell</span></span>

<span data-ttu-id="155b0-122">Utilize o seguinte script PowerShell para atribuir a função de Administrador marketplace; requer os seguintes parâmetros:</span><span class="sxs-lookup"><span data-stu-id="155b0-122">Use the following PowerShell script to assign the Marketplace Admin role; it requires the following parameters:</span></span>

- <span data-ttu-id="155b0-123">**TenantId:** A ID do inquilino em âmbito (a função de administrador do Marketplace é atribuível no âmbito do arrendatário).</span><span class="sxs-lookup"><span data-stu-id="155b0-123">**TenantId:** The ID of the tenant in scope (Marketplace admin role is assignable on the tenant scope).</span></span>
- <span data-ttu-id="155b0-124">**SubscriçãoId:** Uma subscrição da qual o administrador global tem **papel contributivo** ou superior atribuído.</span><span class="sxs-lookup"><span data-stu-id="155b0-124">**SubscriptionId:** A subscription of which the global admin has **Contributor** role or higher assigned.</span></span>
- <span data-ttu-id="155b0-125">**GlobalAdminUsername:** O nome de utilizador da administração global.</span><span class="sxs-lookup"><span data-stu-id="155b0-125">**GlobalAdminUsername:** The username of the global admin.</span></span>
- <span data-ttu-id="155b0-126">**Nome de utilizadorToAssignRoleFor:** O nome de utilizador ao qual será atribuída a função de administrador do Marketplace.</span><span class="sxs-lookup"><span data-stu-id="155b0-126">**UsernameToAssignRoleFor:** The user name to which the Marketplace admin role will be assigned.</span></span>

> [!NOTE]
> <span data-ttu-id="155b0-127">Para os utilizadores convidados convidados ao arrendatário, pode demorar até 48 horas até que a sua conta esteja disponível para atribuir o papel de administrador do Marketplace.</span><span class="sxs-lookup"><span data-stu-id="155b0-127">For guest users invited to the tenant, it may take up to 48 hours until their account is available for assigning the Marketplace admin role.</span></span> <span data-ttu-id="155b0-128">Para mais informações, consulte [propriedades de um utilizador de colaboração Azure Ative Directory B2B.](/azure/active-directory/b2b/user-properties)</span><span class="sxs-lookup"><span data-stu-id="155b0-128">For more information, see [Properties of an Azure Active Directory B2B collaboration user](/azure/active-directory/b2b/user-properties).</span></span>

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

$MarketPlaceAdminRole = Get-AzRoleDefinition $MarketplaceAdminRoleDefinitionName

if($MarketPlaceAdminRole -eq $null)
{
Write-Error -Message "'$($MarketplaceAdminRoleDefinitionName)' role is not available" -ErrorAction Stop
}
else
{
Write-Output -Message "'$($MarketplaceAdminRoleDefinitionName)' role is available"
}

Write-Output -Message "About to assign '$($MarketplaceAdminRoleDefinitionName)' role for $($UsernameToAssignRoleFor)..."

$elevatedAccessOnRoot = Get-AzRoleAssignment | where {$_.RoleDefinitionName -eq "User Access Administrator" -and $_.Scope -eq "/" -and $_.SignInName.Trim().ToLower() -eq $GlobalAdminUsername.Trim().ToLower() } | ft -Property SignInName

if($elevatedAccessOnRoot.Count -eq 0)
{
Write-Error -Message "$($GlobalAdminUsername) doesn't have permissions to assign '$($MarketplaceAdminRoleDefinitionName)'. Please verify it has elevated access 'On' in portal, https://docs.microsoft.com/en-us/azure/role-based-access-control/elevate-access-global-admin" -ErrorAction Stop
}
else
{
Write-Output "$GlobalAdminUsername has elevated access on root"
}

New-AzRoleAssignment -SignInName $UsernameToAssignRoleFor -RoleDefinitionName $MarketplaceAdminRoleDefinitionName -Scope "/providers/Microsoft.Marketplace"

}

Assign-MarketplaceAdminRole
```

<span data-ttu-id="155b0-129">Para obter mais informações sobre os cmdlets contidos no módulo Az.Portal PowerShell, consulte [microsoft Azure PowerShell: Portal Dashboard cmdlets](/powershell/module/az.portal/).</span><span class="sxs-lookup"><span data-stu-id="155b0-129">For more information about the cmdlets contained in the Az.Portal PowerShell module, see [Microsoft Azure PowerShell: Portal Dashboard cmdlets](/powershell/module/az.portal/).</span></span>

## <a name="create-private-azure-marketplace"></a><span data-ttu-id="155b0-130">Criar Mercado Privado Azure</span><span class="sxs-lookup"><span data-stu-id="155b0-130">Create Private Azure Marketplace</span></span>

1. <span data-ttu-id="155b0-131">Inicie sessão no [portal do Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="155b0-131">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="155b0-132">Selecione **Todos os serviços** e, em seguida, **Marketplace** .</span><span class="sxs-lookup"><span data-stu-id="155b0-132">Select **All services** and then **Marketplace** .</span></span>

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Janela principal do portal Azure.":::

3. <span data-ttu-id="155b0-134">Selecione **Private Marketplace** a partir das opções à esquerda.</span><span class="sxs-lookup"><span data-stu-id="155b0-134">Select **Private Marketplace** from the options on the left.</span></span>

    :::image type="content" source="media/private-azure/private-marketplace.png" alt-text="Selecionando o Private Marketplace na janela principal do portal Azure.":::

4. <span data-ttu-id="155b0-136">**Selecione Get Start** para criar Private Azure Marketplace (só tem de o fazer uma vez).</span><span class="sxs-lookup"><span data-stu-id="155b0-136">Select **Get Started** to create Private Azure Marketplace (you only have to do this once).</span></span>

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Selecionando Começar na janela principal do portal Azure.":::

    <span data-ttu-id="155b0-138">Se o Private Azure Marketplace já existir para este inquilino, **o Manage Marketplace** será selecionado por padrão.</span><span class="sxs-lookup"><span data-stu-id="155b0-138">If Private Azure Marketplace already exists for this tenant, **Manage Marketplace** will be selected by default.</span></span>

5. <span data-ttu-id="155b0-139">Uma vez concluído, terá um Mercado Privado Azure vazio e desativado.</span><span class="sxs-lookup"><span data-stu-id="155b0-139">Once completed you will have an empty and disabled Private Azure Marketplace.</span></span>

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="O ecrã vazio do Mercado Privado Azure.":::

## <a name="add-items-from-gallery"></a><span data-ttu-id="155b0-141">Adicione artigos da galeria</span><span class="sxs-lookup"><span data-stu-id="155b0-141">Add items from gallery</span></span>

<span data-ttu-id="155b0-142">Um item é uma combinação de uma oferta e um plano.</span><span class="sxs-lookup"><span data-stu-id="155b0-142">An item is a combination of an offer and a plan.</span></span> <span data-ttu-id="155b0-143">Pode pesquisar e adicionar artigo na página 'Gerir Mercado'.</span><span class="sxs-lookup"><span data-stu-id="155b0-143">You can search for and add item in the Manage Marketplace page.</span></span>

1. <span data-ttu-id="155b0-144">**Selecione Adicionar itens** .</span><span class="sxs-lookup"><span data-stu-id="155b0-144">Select **Add items** .</span></span>

2. <span data-ttu-id="155b0-145">Navegue na **Galeria** ou utilize o campo de pesquisa para encontrar o item que deseja.</span><span class="sxs-lookup"><span data-stu-id="155b0-145">Browse the **Gallery** or use the search field to find the item you want.</span></span>

    :::image type="content" source="media/private-azure/marketplace-gallery.png" alt-text="Navegue na galeria ou utilize o campo de pesquisa.":::

3. <span data-ttu-id="155b0-147">Como padrão, ao adicionar uma nova oferta, todos os planos atuais serão adicionados à lista permitida.</span><span class="sxs-lookup"><span data-stu-id="155b0-147">As default, when adding a new offer, all current plans will be added to the allowed list.</span></span> <span data-ttu-id="155b0-148">Para modificar a seleção do plano antes de adicionar os itens selecionados, selecione o menu suspenso no azulejo da oferta e atualize os planos necessários.</span><span class="sxs-lookup"><span data-stu-id="155b0-148">To modify the plan selection before adding the selected items, select the drop-down menu in the offer’s tile and update the required plans.</span></span>

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Atualização dos planos necessários.":::

4. <span data-ttu-id="155b0-150">Selecione **Feito** na parte inferior esquerda depois de ter feito as suas seleções.</span><span class="sxs-lookup"><span data-stu-id="155b0-150">Select **Done** at the bottom-left after you've made your selections.</span></span>

>[!Note]
> <span data-ttu-id="155b0-151">**Adicionar itens** ao Mercado estará disponível apenas para ofertas não microsoft.</span><span class="sxs-lookup"><span data-stu-id="155b0-151">**Add Items** to the Marketplace will be available for non-Microsoft offers only.</span></span> <span data-ttu-id="155b0-152">As ofertas da Microsoft são permitidas por padrão.</span><span class="sxs-lookup"><span data-stu-id="155b0-152">Microsoft offers are allowed by default.</span></span>

## <a name="edit-item-plans"></a><span data-ttu-id="155b0-153">Editar planos de artigos</span><span class="sxs-lookup"><span data-stu-id="155b0-153">Edit item plans</span></span>

<span data-ttu-id="155b0-154">Pode editar os planos de um item na página Manage Marketplace.</span><span class="sxs-lookup"><span data-stu-id="155b0-154">You can edit an item's plans in the Manage Marketplace page.</span></span>

1. <span data-ttu-id="155b0-155">Na coluna **Planos,** reveja os planos disponíveis do menu suspenso para esse item.</span><span class="sxs-lookup"><span data-stu-id="155b0-155">In the **Plans** column, review the available plans from the dropdown menu for that item.</span></span>
2. <span data-ttu-id="155b0-156">Selecione ou limpe as caixas de verificação para escolher quais os planos para disponibilizar aos seus utilizadores.</span><span class="sxs-lookup"><span data-stu-id="155b0-156">Select or clear the checkboxes to choose which plans to make available to your users.</span></span>

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="Selecionar ou limpar a caixa de verificação para o item necessário.":::

> [!NOTE]
> <span data-ttu-id="155b0-158">Cada oferta necessita de pelo menos um plano selecionado para que a atualização ocorra.</span><span class="sxs-lookup"><span data-stu-id="155b0-158">Each offer needs at least one plan selected in order for the update to occur.</span></span> <span data-ttu-id="155b0-159">Para remover todos os planos relacionados com uma oferta, elimine toda a oferta (ver secção seguinte).</span><span class="sxs-lookup"><span data-stu-id="155b0-159">To remove all plans related to an offer, delete the entire offer (see next section).</span></span>

## <a name="delete-offers"></a><span data-ttu-id="155b0-160">Excluir ofertas</span><span class="sxs-lookup"><span data-stu-id="155b0-160">Delete offers</span></span>

<span data-ttu-id="155b0-161">Na página Manage Marketplace, selecione a caixa de verificação ao lado do nome da oferta (ver ecrã acima) e selecione **Eliminar itens** .</span><span class="sxs-lookup"><span data-stu-id="155b0-161">In the Manage Marketplace page, select the check box next to the offer name (see screen above) and select **Delete items** .</span></span>

## <a name="enabledisable-private-azure-marketplace"></a><span data-ttu-id="155b0-162">Ativar/desativar o Mercado Privado de Azure</span><span class="sxs-lookup"><span data-stu-id="155b0-162">Enable/disable Private Azure Marketplace</span></span>

<span data-ttu-id="155b0-163">Na página Manage Marketplace você verá um destes banners, que mostram o estado atual do Mercado Privado Azure:</span><span class="sxs-lookup"><span data-stu-id="155b0-163">In the Manage Marketplace page you will see one of these banners, which show the current state of Private Azure Marketplace:</span></span>

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Desativar o banner do estado":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Ativar banner de estado":::

<span data-ttu-id="155b0-166">Pode ativar ou desativar o Private Azure Marketplace conforme necessário.</span><span class="sxs-lookup"><span data-stu-id="155b0-166">You can enable or disable Private Azure Marketplace as needed.</span></span>

1. <span data-ttu-id="155b0-167">Se estiver desativado, selecione **Enable Private Marketplace** para ativar.</span><span class="sxs-lookup"><span data-stu-id="155b0-167">If disabled, select **Enable Private Marketplace** to enable.</span></span>
2. <span data-ttu-id="155b0-168">Se estiver ativado, **selecione Desativar o Mercado Privado** para desativar.</span><span class="sxs-lookup"><span data-stu-id="155b0-168">If enabled, select **Disable Private Marketplace** to disable.</span></span>

## <a name="browsing-private-azure-marketplace"></a><span data-ttu-id="155b0-169">Navegar no Mercado Privado Azure</span><span class="sxs-lookup"><span data-stu-id="155b0-169">Browsing Private Azure Marketplace</span></span>

<span data-ttu-id="155b0-170">Quando o Private Azure Marketplace estiver ativado, os utilizadores verão quais os planos que o administrador do Marketplace permitiu.</span><span class="sxs-lookup"><span data-stu-id="155b0-170">When Private Azure Marketplace is enabled, users will see which plans the Marketplace admin has allowed.</span></span>

- <span data-ttu-id="155b0-171">Um aviso **verde Permitido** indica uma oferta de Parceiro (não-Microsoft) que é permitida.</span><span class="sxs-lookup"><span data-stu-id="155b0-171">A green **Allowed** notice indicates a Partner (non-Microsoft) offer that is allowed.</span></span>
- <span data-ttu-id="155b0-172">Um aviso azul **permitido** indica uma oferta da Microsoft que é permitida.</span><span class="sxs-lookup"><span data-stu-id="155b0-172">A blue **Allowed** notice indicates a Microsoft offer that is allowed.</span></span>

<span data-ttu-id="155b0-173">Os utilizadores podem filtrar entre ofertas que são e não são permitidas:</span><span class="sxs-lookup"><span data-stu-id="155b0-173">Users can filter between offers that are and are not allowed:</span></span>

:::image type="content" source="media/private-azure/filter-option.png" alt-text="Opção de filtragem.":::

## <a name="buy-or-deploy-in-private-azure-marketplace"></a><span data-ttu-id="155b0-175">Comprar ou implementar no Private Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="155b0-175">Buy or deploy in Private Azure Marketplace</span></span>

<span data-ttu-id="155b0-176">Embora a experiência da página de detalhes do produto seja semelhante ao público Azure Marketplace, existem três cenários específicos do Private Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="155b0-176">While the product details page experience is similar to the public Azure Marketplace, there are three Private Azure Marketplace specific scenarios.</span></span>

- <span data-ttu-id="155b0-177">Quando um utilizador seleciona um plano permitido, o botão **Criar** está ativado:</span><span class="sxs-lookup"><span data-stu-id="155b0-177">When a user selects an allowed plan, the **Create** button is enabled:</span></span>

    :::image type="content" source="media/private-azure/button-create-enabled.png" alt-text="Ofereça banner notando que um plano pode ser criado.":::

- <span data-ttu-id="155b0-179">Quando um utilizador seleciona um plano não permitido, um banner nota que o plano não é permitido e o botão **Criar** é desativado.</span><span class="sxs-lookup"><span data-stu-id="155b0-179">When a user selects a non-allowed plan, a banner notes that the plan is not allowed and the **Create** button is disabled.</span></span>

   :::image type="content" source="media/private-azure/button-create-disabled.png" alt-text="Oferecer banner notando que um plano não pode ser criado.":::

- <span data-ttu-id="155b0-181">Se uma seleção de plano de produto não aparecer na página de detalhes do produto, mas o administrador aprovou um ou mais planos, um banner nota quais os planos permitidos e o botão **Criar** está ativado:</span><span class="sxs-lookup"><span data-stu-id="155b0-181">If a product plan selection does not appear in the product details page but the admin approved one or more plans, a banner notes which plans are allowed and the **Create** button is enabled:</span></span>

    :::image type="content" source="media/private-azure/button-create-enabled-and-plans.png" alt-text="Ofereça banner observando que um plano pode ser criado e mostrando planos disponíveis.":::

## <a name="contact-support"></a><span data-ttu-id="155b0-183">Contactar o suporte</span><span class="sxs-lookup"><span data-stu-id="155b0-183">Contact support</span></span>

<span data-ttu-id="155b0-184">Para obter suporte ao Azure Marketplace, visite [o Microsoft Q&A](/answers/products/).</span><span class="sxs-lookup"><span data-stu-id="155b0-184">For Azure Marketplace support, visit [Microsoft Q&A](/answers/products/).</span></span> 
