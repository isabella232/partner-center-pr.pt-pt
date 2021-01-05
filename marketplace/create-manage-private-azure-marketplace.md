---
title: Criar e gerir o Private Azure Marketplace no portal Azure
description: Saiba como criar e gerir o Private Azure Marketplace (pré-visualização) no portal Azure. O Private Azure Marketplace (pré-visualização) permite aos administradores governar quais as soluções de terceiros que os seus utilizadores podem utilizar.
ms.prod: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 12/22/2020
ms.openlocfilehash: 09f7bcb29dc619e4e31c0aa3d5c73fade5218819
ms.sourcegitcommit: 30d154cdf40aa75400be7805cd9b2685b66a1382
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/24/2020
ms.locfileid: "97760827"
---
# <a name="create-and-manage-private-azure-marketplace-preview-in-the-azure-portal"></a><span data-ttu-id="4c122-104">Criar e gerir o Private Azure Marketplace (pré-visualização) no portal Azure</span><span class="sxs-lookup"><span data-stu-id="4c122-104">Create and manage Private Azure Marketplace (preview) in the Azure portal</span></span>

<span data-ttu-id="4c122-105">O Private Azure Marketplace (pré-visualização) permite aos administradores governar quais as soluções de terceiros que os seus utilizadores podem utilizar.</span><span class="sxs-lookup"><span data-stu-id="4c122-105">Private Azure Marketplace (preview) lets administrators govern which third-party solutions their users can use.</span></span> <span data-ttu-id="4c122-106">Fá-lo permitindo-lhe implementar apenas ofertas que aprove e que cumpram as políticas da sua empresa.</span><span class="sxs-lookup"><span data-stu-id="4c122-106">It does this by allowing you to deploy only offers that you approve and that comply with your enterprise's policies.</span></span> <span data-ttu-id="4c122-107">Com o Private Azure Marketplace, os seus utilizadores podem pesquisar na loja online ofertas compatíveis para comprar e implementar.</span><span class="sxs-lookup"><span data-stu-id="4c122-107">With Private Azure Marketplace, your users can search the online store for compliant offers to purchase and deploy.</span></span> 

<span data-ttu-id="4c122-108">Como administrador do Marketplace (papel atribuído), começará com uma Loja Privada desativada e vazia, onde poderá adicionar as suas ofertas e planos aprovados.</span><span class="sxs-lookup"><span data-stu-id="4c122-108">As a Marketplace admin (assigned role), you will start with a disabled and empty Private Store where you can add your approved offers and plans.</span></span> <span data-ttu-id="4c122-109">Este artigo explica como criar, gerir e ativar o Private Azure Marketplace para os seus utilizadores.</span><span class="sxs-lookup"><span data-stu-id="4c122-109">This article explains how to create, manage, and enable Private Azure Marketplace for your users.</span></span>

<span data-ttu-id="4c122-110">Notas:</span><span class="sxs-lookup"><span data-stu-id="4c122-110">Notes:</span></span>

- <span data-ttu-id="4c122-111">O Private Azure Marketplace está ao nível dos inquilinos, pelo que todos os utilizadores sob o inquilino verão a mesma lista com curadoria.</span><span class="sxs-lookup"><span data-stu-id="4c122-111">Private Azure Marketplace is at a tenant level, so all users under the tenant will see the same curated list.</span></span>
- <span data-ttu-id="4c122-112">Todas as soluções microsoft são automaticamente adicionadas ao Private Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="4c122-112">All Microsoft solutions are automatically added to Private Azure Marketplace.</span></span>

## <a name="assign-the-marketplace-admin-role"></a><span data-ttu-id="4c122-113">Atribuir o papel de administrador do Marketplace</span><span class="sxs-lookup"><span data-stu-id="4c122-113">Assign the Marketplace admin role</span></span>

<span data-ttu-id="4c122-114">O administrador global inquilino deve atribuir o papel **de administrador do Marketplace** ao administrador privado Azure Marketplace que irá gerir a loja privada.</span><span class="sxs-lookup"><span data-stu-id="4c122-114">The tenant Global administrator must assign the **Marketplace admin** role to the Private Azure Marketplace admin who will manage the private store.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="4c122-115">O acesso à gestão private Azure Marketplace só está disponível para administradores de TI com a função de administração do Marketplace atribuída.</span><span class="sxs-lookup"><span data-stu-id="4c122-115">Access to Private Azure Marketplace management is only available to IT admins with the Marketplace admin role assigned.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="4c122-116">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4c122-116">Prerequisites</span></span>

<span data-ttu-id="4c122-117">Deve cumprir estes pré-requisitos antes de poder atribuir a função de Administrador do Marketplace a um utilizador no âmbito do arrendatário:</span><span class="sxs-lookup"><span data-stu-id="4c122-117">You must meet these prerequisites before you can assign the Marketplace Admin role to a user on the tenant scope:</span></span>

- <span data-ttu-id="4c122-118">Tem acesso a um utilizador **administrador global.**</span><span class="sxs-lookup"><span data-stu-id="4c122-118">You have access to a **Global administrator** user.</span></span>
- <span data-ttu-id="4c122-119">O arrendatário tem pelo menos uma subscrição (pode ser qualquer tipo).</span><span class="sxs-lookup"><span data-stu-id="4c122-119">The tenant has at least one subscription (can be any type).</span></span>
- <span data-ttu-id="4c122-120">O utilizador administrador Global é atribuído à função **Contribuinte** ou superior para a subscrição escolhida.</span><span class="sxs-lookup"><span data-stu-id="4c122-120">The Global administrator user is assigned the **Contributor** role or higher for the chosen subscription.</span></span>

### <a name="assign-the-marketplace-admin-role-with-iam"></a><span data-ttu-id="4c122-121">Atribuir o papel de administrador do Marketplace com o IAM</span><span class="sxs-lookup"><span data-stu-id="4c122-121">Assign the Marketplace admin role with IAM</span></span>

1. <span data-ttu-id="4c122-122">Inicie sessão no [portal do Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="4c122-122">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
1. <span data-ttu-id="4c122-123">Selecione **Todos os serviços** e, em seguida, **Marketplace**.</span><span class="sxs-lookup"><span data-stu-id="4c122-123">Select **All services** and then **Marketplace**.</span></span>

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Janela principal do portal Azure.":::

3. <span data-ttu-id="4c122-125">Selecione **Private Marketplace** a partir das opções à esquerda.</span><span class="sxs-lookup"><span data-stu-id="4c122-125">Select **Private Marketplace** from the options on the left.</span></span>
1. <span data-ttu-id="4c122-126">Selecione **o controlo de acesso (IAM)** para atribuir a função de administração do Marketplace.</span><span class="sxs-lookup"><span data-stu-id="4c122-126">Select **Access control (IAM)** to assign the Marketplace admin role.</span></span>

    :::image type="content" source="media/private-azure/access-control-iam.png" alt-text="Ecrã de controlo de acesso IAM.":::

1. <span data-ttu-id="4c122-128">Selecione **+ Adicionar** > **Adicionar atribuição de função**.</span><span class="sxs-lookup"><span data-stu-id="4c122-128">Select **+ Add** > **Add role assignment**.</span></span>
1. <span data-ttu-id="4c122-129">Under **Role**, escolha **Marketplace Admin**.</span><span class="sxs-lookup"><span data-stu-id="4c122-129">Under **Role**, choose **Marketplace Admin**.</span></span>

    :::image type="content" source="media/private-azure/iam-role-assignment.png" alt-text="Menu de atribuição de funções.":::

1. <span data-ttu-id="4c122-131">Selecione o utilizador desejado da lista de retirada e, em seguida, selecione **'Fazer'.**</span><span class="sxs-lookup"><span data-stu-id="4c122-131">Select the desired user from the dropdown list, then select **Done**.</span></span>

### <a name="assign-the-marketplace-admin-role-with-powershell"></a><span data-ttu-id="4c122-132">Atribuir o papel de administrador do Marketplace com o PowerShell</span><span class="sxs-lookup"><span data-stu-id="4c122-132">Assign the Marketplace admin role with PowerShell</span></span>

<span data-ttu-id="4c122-133">Utilize o seguinte script PowerShell para atribuir a função de Administrador marketplace; requer os seguintes parâmetros:</span><span class="sxs-lookup"><span data-stu-id="4c122-133">Use the following PowerShell script to assign the Marketplace Admin role; it requires the following parameters:</span></span>

- <span data-ttu-id="4c122-134">**TenantId:** A ID do inquilino em âmbito (a função de administrador do Marketplace é atribuível no âmbito do arrendatário).</span><span class="sxs-lookup"><span data-stu-id="4c122-134">**TenantId:** The ID of the tenant in scope (Marketplace admin role is assignable on the tenant scope).</span></span>
- <span data-ttu-id="4c122-135">**SubscriçãoId:** Uma subscrição da qual o administrador global tem **papel contributivo** ou superior atribuído.</span><span class="sxs-lookup"><span data-stu-id="4c122-135">**SubscriptionId:** A subscription of which the global admin has **Contributor** role or higher assigned.</span></span>
- <span data-ttu-id="4c122-136">**GlobalAdminUsername:** O nome de utilizador da administração global.</span><span class="sxs-lookup"><span data-stu-id="4c122-136">**GlobalAdminUsername:** The username of the global admin.</span></span>
- <span data-ttu-id="4c122-137">**Nome de utilizadorToAssignRoleFor:** O nome de utilizador ao qual será atribuída a função de administrador do Marketplace.</span><span class="sxs-lookup"><span data-stu-id="4c122-137">**UsernameToAssignRoleFor:** The user name to which the Marketplace admin role will be assigned.</span></span>

> [!NOTE]
> <span data-ttu-id="4c122-138">Para os utilizadores convidados convidados ao arrendatário, pode demorar até 48 horas até que a sua conta esteja disponível para atribuir o papel de administrador do Marketplace.</span><span class="sxs-lookup"><span data-stu-id="4c122-138">For guest users invited to the tenant, it may take up to 48 hours until their account is available for assigning the Marketplace admin role.</span></span> <span data-ttu-id="4c122-139">Para mais informações, consulte [propriedades de um utilizador de colaboração Azure Ative Directory B2B.](/azure/active-directory/b2b/user-properties)</span><span class="sxs-lookup"><span data-stu-id="4c122-139">For more information, see [Properties of an Azure Active Directory B2B collaboration user](/azure/active-directory/b2b/user-properties).</span></span>

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

<span data-ttu-id="4c122-140">Para obter mais informações sobre os cmdlets contidos no módulo Az.Portal PowerShell, consulte [microsoft Azure PowerShell: Portal Dashboard cmdlets](/powershell/module/az.portal/).</span><span class="sxs-lookup"><span data-stu-id="4c122-140">For more information about the cmdlets contained in the Az.Portal PowerShell module, see [Microsoft Azure PowerShell: Portal Dashboard cmdlets](/powershell/module/az.portal/).</span></span>

## <a name="create-private-azure-marketplace"></a><span data-ttu-id="4c122-141">Criar Mercado Privado Azure</span><span class="sxs-lookup"><span data-stu-id="4c122-141">Create Private Azure Marketplace</span></span>

1. <span data-ttu-id="4c122-142">Inicie sessão no [portal do Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="4c122-142">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="4c122-143">Selecione **Todos os serviços** e, em seguida, **Marketplace**.</span><span class="sxs-lookup"><span data-stu-id="4c122-143">Select **All services** and then **Marketplace**.</span></span>

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Janela principal do portal Azure.":::

3. <span data-ttu-id="4c122-145">Selecione **Private Marketplace** a partir das opções à esquerda.</span><span class="sxs-lookup"><span data-stu-id="4c122-145">Select **Private Marketplace** from the options on the left.</span></span>

    :::image type="content" source="media/private-azure/private-marketplace.png" alt-text="Selecionando o Private Marketplace na janela principal do portal Azure.":::

4. <span data-ttu-id="4c122-147">**Selecione Get Start** para criar Private Azure Marketplace (só tem de o fazer uma vez).</span><span class="sxs-lookup"><span data-stu-id="4c122-147">Select **Get Started** to create Private Azure Marketplace (you only have to do this once).</span></span>

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Selecionando Começar na janela principal do portal Azure.":::

    <span data-ttu-id="4c122-149">Se o Private Azure Marketplace já existir para este inquilino, **o Manage Marketplace** será selecionado por padrão.</span><span class="sxs-lookup"><span data-stu-id="4c122-149">If Private Azure Marketplace already exists for this tenant, **Manage Marketplace** will be selected by default.</span></span>

5. <span data-ttu-id="4c122-150">Uma vez concluído, terá um Mercado Privado Azure vazio e desativado.</span><span class="sxs-lookup"><span data-stu-id="4c122-150">Once completed you will have an empty and disabled Private Azure Marketplace.</span></span>

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="O ecrã vazio do Mercado Privado Azure.":::

## <a name="add-items-from-gallery"></a><span data-ttu-id="4c122-152">Adicione artigos da galeria</span><span class="sxs-lookup"><span data-stu-id="4c122-152">Add items from gallery</span></span>

<span data-ttu-id="4c122-153">Um item é uma combinação de uma oferta e um plano.</span><span class="sxs-lookup"><span data-stu-id="4c122-153">An item is a combination of an offer and a plan.</span></span> <span data-ttu-id="4c122-154">Pode pesquisar e adicionar artigo na página 'Gerir Mercado'.</span><span class="sxs-lookup"><span data-stu-id="4c122-154">You can search for and add item in the Manage Marketplace page.</span></span>

1. <span data-ttu-id="4c122-155">**Selecione Adicionar itens**.</span><span class="sxs-lookup"><span data-stu-id="4c122-155">Select **Add items**.</span></span>

2. <span data-ttu-id="4c122-156">Navegue na **Galeria** ou utilize o campo de pesquisa para encontrar o item que deseja.</span><span class="sxs-lookup"><span data-stu-id="4c122-156">Browse the **Gallery** or use the search field to find the item you want.</span></span>

    :::image type="content" source="media/private-azure/marketplace-gallery.png" alt-text="Navegue na galeria ou utilize o campo de pesquisa.":::

3. <span data-ttu-id="4c122-158">Como padrão, ao adicionar uma nova oferta, todos os planos atuais serão adicionados à lista permitida.</span><span class="sxs-lookup"><span data-stu-id="4c122-158">As default, when adding a new offer, all current plans will be added to the allowed list.</span></span> <span data-ttu-id="4c122-159">Para modificar a seleção do plano antes de adicionar os itens selecionados, selecione o menu suspenso no azulejo da oferta e atualize os planos necessários.</span><span class="sxs-lookup"><span data-stu-id="4c122-159">To modify the plan selection before adding the selected items, select the drop-down menu in the offer’s tile and update the required plans.</span></span>

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Atualização dos planos necessários.":::

4. <span data-ttu-id="4c122-161">Selecione **Feito** na parte inferior esquerda depois de ter feito as suas seleções.</span><span class="sxs-lookup"><span data-stu-id="4c122-161">Select **Done** at the bottom-left after you've made your selections.</span></span>

>[!Note]
> <span data-ttu-id="4c122-162">**Adicionar itens** ao Mercado estará disponível apenas para ofertas não microsoft.</span><span class="sxs-lookup"><span data-stu-id="4c122-162">**Add Items** to the Marketplace will be available for non-Microsoft offers only.</span></span> <span data-ttu-id="4c122-163">As ofertas da Microsoft são permitidas por padrão.</span><span class="sxs-lookup"><span data-stu-id="4c122-163">Microsoft offers are allowed by default.</span></span>

## <a name="edit-item-plans"></a><span data-ttu-id="4c122-164">Editar planos de artigos</span><span class="sxs-lookup"><span data-stu-id="4c122-164">Edit item plans</span></span>

<span data-ttu-id="4c122-165">Pode editar os planos de um item na página Manage Marketplace.</span><span class="sxs-lookup"><span data-stu-id="4c122-165">You can edit an item's plans in the Manage Marketplace page.</span></span>

1. <span data-ttu-id="4c122-166">Na coluna **Planos,** reveja os planos disponíveis do menu suspenso para esse item.</span><span class="sxs-lookup"><span data-stu-id="4c122-166">In the **Plans** column, review the available plans from the dropdown menu for that item.</span></span>
2. <span data-ttu-id="4c122-167">Selecione ou limpe as caixas de verificação para escolher quais os planos para disponibilizar aos seus utilizadores.</span><span class="sxs-lookup"><span data-stu-id="4c122-167">Select or clear the checkboxes to choose which plans to make available to your users.</span></span>

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="Selecionar ou limpar a caixa de verificação para o item necessário.":::

> [!NOTE]
> <span data-ttu-id="4c122-169">Cada oferta necessita de pelo menos um plano selecionado para que a atualização ocorra.</span><span class="sxs-lookup"><span data-stu-id="4c122-169">Each offer needs at least one plan selected in order for the update to occur.</span></span> <span data-ttu-id="4c122-170">Para remover todos os planos relacionados com uma oferta, elimine toda a oferta (ver secção seguinte).</span><span class="sxs-lookup"><span data-stu-id="4c122-170">To remove all plans related to an offer, delete the entire offer (see next section).</span></span>

## <a name="delete-offers"></a><span data-ttu-id="4c122-171">Excluir ofertas</span><span class="sxs-lookup"><span data-stu-id="4c122-171">Delete offers</span></span>

<span data-ttu-id="4c122-172">Na página Manage Marketplace, selecione a caixa de verificação ao lado do nome da oferta (ver ecrã acima) e selecione **Eliminar itens**.</span><span class="sxs-lookup"><span data-stu-id="4c122-172">In the Manage Marketplace page, select the check box next to the offer name (see screen above) and select **Delete items**.</span></span>

## <a name="enabledisable-private-azure-marketplace"></a><span data-ttu-id="4c122-173">Ativar/desativar o Mercado Privado de Azure</span><span class="sxs-lookup"><span data-stu-id="4c122-173">Enable/disable Private Azure Marketplace</span></span>

<span data-ttu-id="4c122-174">Na página Manage Marketplace você verá um destes banners, que mostram o estado atual do Mercado Privado Azure:</span><span class="sxs-lookup"><span data-stu-id="4c122-174">In the Manage Marketplace page you will see one of these banners, which show the current state of Private Azure Marketplace:</span></span>

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Desativar o banner do estado":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Ativar banner de estado":::

<span data-ttu-id="4c122-177">Pode ativar ou desativar o Private Azure Marketplace conforme necessário.</span><span class="sxs-lookup"><span data-stu-id="4c122-177">You can enable or disable Private Azure Marketplace as needed.</span></span>

- <span data-ttu-id="4c122-178">Se estiver desativado, selecione **Enable Private Marketplace** para ativar.</span><span class="sxs-lookup"><span data-stu-id="4c122-178">If disabled, select **Enable Private Marketplace** to enable.</span></span>
- <span data-ttu-id="4c122-179">Se estiver ativado, **selecione Desativar o Mercado Privado** para desativar.</span><span class="sxs-lookup"><span data-stu-id="4c122-179">If enabled, select **Disable Private Marketplace** to disable.</span></span>

## <a name="browsing-private-azure-marketplace"></a><span data-ttu-id="4c122-180">Navegar no Mercado Privado Azure</span><span class="sxs-lookup"><span data-stu-id="4c122-180">Browsing Private Azure Marketplace</span></span>

<span data-ttu-id="4c122-181">Quando o Private Azure Marketplace estiver ativado, os utilizadores verão quais os planos que o administrador do Marketplace permitiu.</span><span class="sxs-lookup"><span data-stu-id="4c122-181">When Private Azure Marketplace is enabled, users will see which plans the Marketplace admin has allowed.</span></span>

- <span data-ttu-id="4c122-182">Um aviso **verde Permitido** indica uma oferta de Parceiro (não-Microsoft) que é permitida.</span><span class="sxs-lookup"><span data-stu-id="4c122-182">A green **Allowed** notice indicates a Partner (non-Microsoft) offer that is allowed.</span></span>
- <span data-ttu-id="4c122-183">Um aviso azul **permitido** indica uma oferta da Microsoft que é permitida.</span><span class="sxs-lookup"><span data-stu-id="4c122-183">A blue **Allowed** notice indicates a Microsoft offer that is allowed.</span></span>

<span data-ttu-id="4c122-184">Os utilizadores podem filtrar entre ofertas que são e não são permitidas:</span><span class="sxs-lookup"><span data-stu-id="4c122-184">Users can filter between offers that are and are not allowed:</span></span>

:::image type="content" source="media/private-azure/filter-option.png" alt-text="Opção de filtragem.":::

## <a name="buy-or-deploy-in-private-azure-marketplace"></a><span data-ttu-id="4c122-186">Comprar ou implementar no Private Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="4c122-186">Buy or deploy in Private Azure Marketplace</span></span>

<span data-ttu-id="4c122-187">Embora a experiência da página de detalhes do produto seja semelhante ao público Azure Marketplace, existem três cenários específicos do Private Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="4c122-187">While the product details page experience is similar to the public Azure Marketplace, there are three Private Azure Marketplace specific scenarios.</span></span>

- <span data-ttu-id="4c122-188">Quando um utilizador seleciona um plano permitido, o botão **Criar** está ativado:</span><span class="sxs-lookup"><span data-stu-id="4c122-188">When a user selects an allowed plan, the **Create** button is enabled:</span></span>

    :::image type="content" source="media/private-azure/button-create-enabled.png" alt-text="Ofereça banner notando que um plano pode ser criado.":::

- <span data-ttu-id="4c122-190">Quando um utilizador seleciona um plano não permitido, um banner nota que o plano não é permitido e o botão **Criar** é desativado.</span><span class="sxs-lookup"><span data-stu-id="4c122-190">When a user selects a non-allowed plan, a banner notes that the plan is not allowed and the **Create** button is disabled.</span></span>

   :::image type="content" source="media/private-azure/button-create-disabled.png" alt-text="Oferecer banner notando que um plano não pode ser criado.":::

- <span data-ttu-id="4c122-192">Se uma seleção de plano de produto não aparecer na página de detalhes do produto, mas o administrador aprovou um ou mais planos, um banner nota quais os planos permitidos e o botão **Criar** está ativado:</span><span class="sxs-lookup"><span data-stu-id="4c122-192">If a product plan selection does not appear in the product details page but the admin approved one or more plans, a banner notes which plans are allowed and the **Create** button is enabled:</span></span>

    :::image type="content" source="media/private-azure/button-create-enabled-and-plans.png" alt-text="Ofereça banner notando que um plano pode ser criado e mostrando planos disponíveis.":::

## <a name="contact-support"></a><span data-ttu-id="4c122-194">Contactar o suporte</span><span class="sxs-lookup"><span data-stu-id="4c122-194">Contact support</span></span>

<span data-ttu-id="4c122-195">Para obter suporte ao Azure Marketplace, visite [o Microsoft Q&A](/answers/products/).</span><span class="sxs-lookup"><span data-stu-id="4c122-195">For Azure Marketplace support, visit [Microsoft Q&A](/answers/products/).</span></span> 
