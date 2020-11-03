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
# <a name="create-and-manage-private-azure-marketplace-preview-in-the-azure-portal"></a>Criar e gerir o Private Azure Marketplace (pré-visualização) no portal Azure

O Private Azure Marketplace (pré-visualização) permite aos administradores governar quais as soluções de terceiros que os seus utilizadores podem utilizar. Fá-lo permitindo-lhe implementar apenas ofertas que aprove e que cumpram as políticas da sua empresa. Com o Private Azure Marketplace, os seus utilizadores podem pesquisar na loja online ofertas compatíveis para comprar e implementar. 

Como administrador do Marketplace (papel atribuído), começará com uma Loja Privada desativada e vazia, onde poderá adicionar as suas ofertas e planos aprovados. Este artigo explica como criar, gerir e ativar o Private Azure Marketplace para os seus utilizadores.

Notas:

- O Private Azure Marketplace está ao nível dos inquilinos, pelo que todos os utilizadores sob o inquilino verão a mesma lista com curadoria.
- Todas as soluções microsoft são automaticamente adicionadas ao Private Azure Marketplace.

## <a name="assign-the-marketplace-admin-role"></a>Atribuir o papel de administrador do Marketplace

O administrador global inquilino deve atribuir o papel **de administrador do Marketplace** ao administrador privado Azure Marketplace que irá gerir a loja privada.

>[!IMPORTANT]
> O acesso à gestão private Azure Marketplace só está disponível para administradores de TI com a função de administração do Marketplace atribuída.

### <a name="prerequisites"></a>Pré-requisitos

Deve cumprir estes pré-requisitos antes de poder atribuir a função de Administrador do Marketplace a um utilizador no âmbito do arrendatário:

- Tem acesso a um utilizador **administrador global.**
- O arrendatário tem pelo menos uma Subscrição (pode ser qualquer tipo).
- O utilizador administrador Global é atribuído à função **Contribuinte** ou superior para a subscrição escolhida no passo 2.
- O utilizador administrador global tem um acesso elevado definido para **Sim** (ver [elevate-access-global-admin).](/azure/role-based-access-control/elevate-access-global-admin)

### <a name="assign-the-marketplace-admin-role-with-powershell"></a>Atribuir o papel de administrador do Marketplace com o PowerShell

Utilize o seguinte script PowerShell para atribuir a função de Administrador marketplace; requer os seguintes parâmetros:

- **TenantId:** A ID do inquilino em âmbito (a função de administrador do Marketplace é atribuível no âmbito do arrendatário).
- **SubscriçãoId:** Uma subscrição da qual o administrador global tem **papel contributivo** ou superior atribuído.
- **GlobalAdminUsername:** O nome de utilizador da administração global.
- **Nome de utilizadorToAssignRoleFor:** O nome de utilizador ao qual será atribuída a função de administrador do Marketplace.

> [!NOTE]
> Para os utilizadores convidados convidados ao arrendatário, pode demorar até 48 horas até que a sua conta esteja disponível para atribuir o papel de administrador do Marketplace. Para mais informações, consulte [propriedades de um utilizador de colaboração Azure Ative Directory B2B.](/azure/active-directory/b2b/user-properties)

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

Para obter mais informações sobre os cmdlets contidos no módulo Az.Portal PowerShell, consulte [microsoft Azure PowerShell: Portal Dashboard cmdlets](/powershell/module/az.portal/).

## <a name="create-private-azure-marketplace"></a>Criar Mercado Privado Azure

1. Inicie sessão no [portal do Azure](https://portal.azure.com/).
2. Selecione **Todos os serviços** e, em seguida, **Marketplace** .

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Janela principal do portal Azure.":::

3. Selecione **Private Marketplace** a partir das opções à esquerda.

    :::image type="content" source="media/private-azure/private-marketplace.png" alt-text="Janela principal do portal Azure.":::

4. **Selecione Get Start** para criar Private Azure Marketplace (só tem de o fazer uma vez).

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Janela principal do portal Azure.":::

    Se o Private Azure Marketplace já existir para este inquilino, **o Manage Marketplace** será selecionado por padrão.

5. Uma vez concluído, terá um Mercado Privado Azure vazio e desativado.

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="Janela principal do portal Azure.":::

## <a name="add-items-from-gallery"></a>Adicione artigos da galeria

Um item é uma combinação de uma oferta e um plano. Pode pesquisar e adicionar artigo na página 'Gerir Mercado'.

1. **Selecione Adicionar itens** .

2. Navegue na **Galeria** ou utilize o campo de pesquisa para encontrar o item que deseja.

    :::image type="content" source="media/private-azure/marketplace-gallery.png" alt-text="Janela principal do portal Azure.":::

3. Como padrão, ao adicionar uma nova oferta, todos os planos atuais serão adicionados à lista permitida. Para modificar a seleção do plano antes de adicionar os itens selecionados, selecione o menu suspenso no azulejo da oferta e atualize os planos necessários.

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Janela principal do portal Azure.":::

4. Selecione **Feito** na parte inferior esquerda depois de ter feito as suas seleções.

>[!Note]
> **Adicionar itens** ao Mercado estará disponível apenas para ofertas não microsoft. As ofertas da Microsoft são permitidas por padrão.

## <a name="edit-item-plans"></a>Editar planos de artigos

Pode editar os planos de um item na página Manage Marketplace.

1. Na coluna **Planos,** reveja os planos disponíveis do menu suspenso para esse item.
2. Selecione ou limpe as caixas de verificação para escolher quais os planos para disponibilizar aos seus utilizadores.

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="Janela principal do portal Azure.":::

> [!NOTE]
> Cada oferta necessita de pelo menos um plano selecionado para que a atualização ocorra. Para remover todos os planos relacionados com uma oferta, elimine toda a oferta (ver secção seguinte).

## <a name="delete-offers"></a>Excluir ofertas

Na página Manage Marketplace, selecione a caixa de verificação ao lado do nome da oferta (ver ecrã acima) e selecione **Eliminar itens** .

## <a name="enabledisable-private-azure-marketplace"></a>Ativar/desativar o Mercado Privado de Azure

Na página Manage Marketplace você verá um destes banners, que mostram o estado atual do Mercado Privado Azure:

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Janela principal do portal Azure.":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Janela principal do portal Azure.":::

Pode ativar ou desativar o Private Azure Marketplace conforme necessário.

1. Se estiver desativado, selecione **Enable Private Marketplace** para ativar.
2. Se estiver ativado, **selecione Desativar o Mercado Privado** para desativar.

## <a name="browsing-private-azure-marketplace"></a>Navegar no Mercado Privado Azure

Quando o Private Azure Marketplace estiver ativado, os utilizadores verão quais os planos que o administrador do Marketplace permitiu.

- Um aviso **verde Permitido** indica uma oferta de Parceiro (não-Microsoft) que é permitida.
- Um aviso azul **permitido** indica uma oferta da Microsoft que é permitida.

Os utilizadores podem filtrar entre ofertas que são e não são permitidas:

:::image type="content" source="media/private-azure/filter-option.png" alt-text="Janela principal do portal Azure.":::

## <a name="buy-or-deploy-in-private-azure-marketplace"></a>Comprar ou implementar no Private Azure Marketplace

Embora a experiência da página de detalhes do produto seja semelhante ao público Azure Marketplace, existem três cenários específicos do Private Azure Marketplace.

- Quando um utilizador seleciona um plano permitido, o botão **Criar** está ativado:

    :::image type="content" source="media/private-azure/button-create-enabled.png" alt-text="Janela principal do portal Azure.":::

- Quando um utilizador seleciona um plano não permitido, um banner nota que o plano não é permitido e o botão **Criar** é desativado.

   :::image type="content" source="media/private-azure/button-create-disabled.png" alt-text="Janela principal do portal Azure.":::

- Se uma seleção de plano de produto não aparecer na página de detalhes do produto, mas o administrador aprovou um ou mais planos, um banner nota quais os planos permitidos e o botão **Criar** está ativado:

    :::image type="content" source="media/private-azure/button-create-enabled-and-plans.png" alt-text="Janela principal do portal Azure.":::

## <a name="contact-support"></a>Contactar o suporte

Para obter suporte ao Azure Marketplace, visite [o Microsoft Q&A](/answers/products/). 
