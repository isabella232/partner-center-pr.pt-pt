---
title: Criar e gerir coleções Private Azure Marketplace no portal Azure
description: Criar e gerir o Private Azure Marketplace (pré-visualização) no portal Azure com a nova vista Coleções. O Private Azure Marketplace (pré-visualização) permite aos administradores governar quais as soluções de terceiros que os seus utilizadores podem utilizar.
ms.service: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 08/10/2021
ms.openlocfilehash: 74550d814657a117f62d1e3eae45d46bae040356
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/13/2021
ms.locfileid: "126246683"
---
# <a name="create-and-manage-private-azure-marketplace-collections-in-the-azure-portal"></a>Criar e gerir coleções Private Azure Marketplace no portal Azure

> [!NOTE]
> Este artigo abrange coleções private Azure Marketplace. A vista do legado é, em vez disso, abordada no [artigo original.](create-manage-private-azure-marketplace.md)

O Private Azure Marketplace permite aos administradores governar quais as soluções de terceiros que os seus utilizadores podem utilizar. Fá-lo permitindo que o utilizador implemente apenas ofertas que sejam aprovadas pelo administrador e cumpram as políticas da sua empresa. Com o Private Azure Marketplace, os utilizadores podem pesquisar na loja online ofertas compatíveis para comprar e implementar.

Como administrador do Marketplace (papel atribuído), começará com um Mercado Privado desativado e vazio e uma coleção onde poderá adicionar as suas ofertas e planos aprovados. Este artigo explica como atribuir a função necessária, criar uma loja privada, gerir coleções e itens, aprovar pedidos de utilizador e ativar o Private Azure Marketplace para os seus utilizadores.

> [!NOTE]
> - O Private Azure Marketplace está ao nível dos inquilinos; uma vez ativado, definirá a política para todos os utilizadores sob o inquilino.
> - Gerir a lista aprovada a nível de subscrição utilizando coleções.
> - Todas as soluções microsoft (incluindo [as distribuições de Linux endossadas)](/azure/virtual-machines/linux/endorsed-distros)são automaticamente adicionadas ao Private Azure Marketplace.

## <a name="assign-the-marketplace-admin-role"></a>Atribuir o papel de administrador do Marketplace

O administrador global inquilino deve atribuir o papel **de administrador do Marketplace** ao administrador privado Azure Marketplace que irá gerir a loja privada.

>[!IMPORTANT]
> O acesso à gestão private Azure Marketplace só está disponível para administradores de TI com a função de administração do Marketplace atribuída.

### <a name="prerequisites"></a>Pré-requisitos

Estes pré-requisitos são necessários antes de poder atribuir a função de Administrador do Mercado a um utilizador no âmbito do arrendatário:

- Tem acesso a um utilizador **administrador global.**
- O arrendatário tem pelo menos uma subscrição (pode ser qualquer tipo).
- O utilizador administrador Global é atribuído à função **Contribuinte** ou superior para a subscrição escolhida.

### <a name="assign-the-marketplace-admin-role-with-access-control-iam"></a>Atribuir a função de administrador do Marketplace com controlo de acesso (IAM)

1. Inicie sessão no [portal do Azure](https://portal.azure.com/).

1. Selecione **Todos os serviços** e, em seguida, **Marketplace**.

1. Selecione **Private Marketplace** a partir do menu à esquerda.

   :::image type="content" source="media/private-azure/private-marketplace.png" lightbox="media/private-azure/private-marketplace-zoom.png" alt-text="Mostra a opção de menu de mercado privado no lado esquerdo do Mercado.":::

1. Selecione **o controlo de acesso (IAM)** para atribuir a função de administração do Marketplace.

   :::image type="content" source="media/private-azure-new/access-control-iam.png" alt-text="Mostra o ecrã de controlo de acesso I A M.":::

1. Selecione **+ Adicionar** > **Adicionar atribuição de função**.

1. Under **Role**, escolha **Marketplace Admin**.

    :::image type="content" source="media/private-azure/iam-role-assignment.png" alt-text="Mostra o menu de atribuição de funções.":::

1. Selecione o utilizador desejado da lista de retirada e, em seguida, selecione **'Fazer'.**

### <a name="assign-the-marketplace-admin-role-with-powershell"></a>Atribuir o papel de administrador do Marketplace com o PowerShell

Utilize o seguinte script PowerShell para atribuir a função de Administrador marketplace; requer os seguintes parâmetros:

- **TenantId:** A ID do inquilino em âmbito (a função de administrador do Marketplace é atribuível no âmbito do arrendatário).
- **SubscriçãoId:** Uma subscrição da qual o administrador global tem **papel contributivo** ou superior atribuído.
- **GlobalAdminUsername:** O nome de utilizador da administração global.
- **Nome de utilizadorToAssignRoleFor:** O nome de utilizador ao qual será atribuída a função de administrador do Marketplace.

> [!NOTE]
> Para os utilizadores convidados convidados ao arrendatário, pode demorar até 48 horas até que a sua conta esteja disponível para atribuir o papel de Administrador do Mercado. Para mais informações, consulte [as propriedades de um utilizador de colaboração B2B Azure Ative Directory.](/azure/active-directory/b2b/user-properties)

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

Para obter mais informações sobre os cmdlets contidos no módulo Az.Portal PowerShell, consulte [Microsoft Azure PowerShell: Cmdlets portal Dashboard](/powershell/module/az.portal/).

## <a name="create-private-azure-marketplace"></a>Criar Mercado Privado Azure

1. Inicie sessão no [portal do Azure](https://portal.azure.com/).
2. Selecione **Todos os serviços** e, em seguida, **Marketplace**.

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Mostra a janela principal do portal Azure.":::

3. Selecione **Private Marketplace** a partir do menu de navegação à esquerda.

4. Selecione **Introdução** para criar o Private Azure Marketplace (só tem de o fazer uma vez).

    :::image type="content" source="media/private-azure-new/private-marketplace-get-started.png" alt-text="Mostra como selecionar a 'Introdução na janela principal do portal Azure'.":::

    Se o Private Azure Marketplace já existir para este inquilino, **o Manage Marketplace** será selecionado por padrão.

5. Uma vez concluído, terá um Mercado Azure Privado desativado com uma **Coleção Padrão.**

    :::image type="content" source="media/private-azure-new/new-private-marketplace.png" alt-text="Mostra o ecrã vazio do Mercado Privado Azure.":::

    > [!NOTE]
    > - **A Predefinição de Recolha** é um conjunto de recolha gerado pelo sistema com o âmbito de todas as subscrições sob o mesmo inquilino.
    > - O nome e o âmbito da Coleção Padrão não podem ser alterados e a recolha não pode ser eliminada.

## <a name="add-collection-items-from-gallery"></a>Adicione artigos de coleção da galeria

Um item é uma combinação de uma oferta e um plano. Pode pesquisar e adicionar itens na página da recolha.

1. Selecione o nome da coleção para gerir esta coleção.

2. **Selecione Adicionar itens**.

3. Navegue na **Galeria** ou utilize o campo de pesquisa para encontrar o item que deseja.

   :::image type="content" source="media/private-azure/marketplace-gallery.png" lightbox="media/private-azure/marketplace-gallery-zoom.png" alt-text="Mostra como navegar na galeria ou utilizar o campo de pesquisa.":::

4. Como padrão, ao adicionar uma nova oferta, todos os planos atuais serão adicionados à lista aprovada. Para modificar a seleção do plano antes de adicionar os itens selecionados, selecione o menu suspenso no azulejo da oferta e atualize os planos necessários.

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Mostra como atualizar os planos necessários.":::

5. Selecione **Feito** na parte inferior esquerda depois de ter feito as suas seleções.

>[!Note]
> **Adicionar itens** ao Mercado estará disponível apenas para ofertas não microsoft. As soluções da Microsoft (incluindo [as Distribuições Linux endossadas)](/azure/virtual-machines/linux/endorsed-distros)serão marcadas como "Aprovadas por padrão" e não podem ser geridas no Private Marketplace.

## <a name="edit-item-plans"></a>Editar planos de artigos

Edite os planos de um item na página de recolha.

1. Na coluna **Planos,** reveja os planos disponíveis do menu suspenso para esse item.

2. Selecione ou limpe as caixas de verificação para escolher quais os planos para disponibilizar aos seus utilizadores.

   :::image type="content" source="media/private-azure-new/edit-items.png" alt-text="Mostra como selecionar ou limpar a caixa de verificação para o item necessário.":::

   > [!NOTE]
   > Cada oferta precisa de pelo menos um plano selecionado para que a atualização ocorra. Para remover todos os planos relacionados com uma oferta, elimine toda a oferta (ver secção seguinte).

### <a name="delete-items"></a>Eliminar itens

Na página de recolha, verifique a caixa ao lado do nome da oferta e selecione **Eliminar itens**.

:::image type="content" source="media/private-azure-new/delete-item.png" alt-text="Mostra como selecionar a caixa de verificação e escolher 'Eliminar itens'.":::

### <a name="copy-items"></a>Copiar itens

1. Na página de cobrança de gestão, verifique a caixa ao lado do nome da oferta e selecione **itens de cópia.**  

   :::image type="content" source="media/private-azure-new/copy-items.png" lightbox="media/private-azure/marketplace-notifications.png" alt-text="Mostra o botão Itens de Cópia.":::

1. No painel direito, selecione a coleção de destino (se necessário, crie uma nova coleção selecionando **Criar nova coleção).**

   :::image type="content" source="media/private-azure-new/create-new-collection.png" alt-text="Mostra a caixa de diálogo Criar uma Coleção.":::

1. Selecione **Copiar**.

### <a name="enabledisable-a-collection"></a>Ativar/desativar uma coleção

1. A página **de recolha Manage** apresentará um banner que mostra o estado atual da coleção:

   :::image type="content" source="media/private-azure-new/collection-disabled.png" alt-text="Mostra o banner de desativação de coleção.":::
   :::image type="content" source="media/private-azure-new/collection-enabled.png" alt-text="Mostra o banner &quot;Collection Enabled&quot;.":::

1. Na página **Manage Marketplace,** selecione a coleção e use a barra de ação superior para ativar ou desativar a coleção.

   :::image type="content" source="media/private-azure-new/action-bar.png" alt-text="Mostra a barra de ação Manage Marketplace com botões de recolha ativado e desativado.":::

### <a name="enabledisable-private-azure-marketplace"></a>Ativar/desativar o Mercado Privado de Azure

A página Manage Marketplace exibe um destes banners que mostra o estado atual do Mercado Privado Azure:

   :::image type="content" source="media/private-azure-new/state-disable.png" alt-text="Mostra o banner private Azure Marketplace Disabled.":::
   :::image type="content" source="media/private-azure-new/state-enable.png" alt-text="Mostra o banner Private Azure Marketplace Enabled.":::

Para ativar ou desativar o Mercado Privado Azure:

1. Selecione **Definições** no menu de navegação à esquerda.
1. Selecione o botão de rádio para o estado desejado.
1. **Selecione Aplicar** na parte inferior da página.

### <a name="add-new-collection"></a>Adicionar nova coleção

Com coleções, o Marketplace Admin (papel atribuído) pode criar várias listas de itens aprovados que estarão disponíveis para diferentes subscrições em toda a sua organização.

1. Selecione **Adicionar a coleção**.

2. Diga o nome da sua coleção.

3. Selecione subscrições do menu suspenso.

4. Selecione **Criar** na parte inferior (não mostrado abaixo) depois de ter feito as suas seleções.

    :::image type="content" source="media/private-azure-new/create-collection.png" alt-text="Mostra a caixa de diálogo Create a Collection.":::

5. Isto cria uma nova coleção privada vazia e desativada. Selecione um nome de coleção para geri-lo.

    :::image type="content" source="media/private-azure-new/new-empty-collection.png" alt-text="Mostra uma nova e vazia janela de Itens de Coleção.":::

### <a name="update-collection-properties"></a>Atualizar propriedades de recolha

1. Selecione o nome da coleção que pretende gerir.
2. Selecione **as propriedades** de coleção do menu de navegação à esquerda.

    :::image type="content" source="media/private-azure-new/collection-properties.png" alt-text="Mostra a janela Collection Properties.":::

3. Atualize o nome e as subscrições selecionadas conforme necessário.
4. **Selecione Aplicar** (não mostrado).

### <a name="delete-a-collection"></a>Delete a collection (Eliminar uma coleção)

Na página Manage Marketplace, verifique a caixa ao lado do nome da recolha e selecione **a coleção Delete**.

:::image type="content" source="media/private-azure-new/collection-delete.png" alt-text="Mostra o ecrã Private Azure Marketplace com o botão 'Delete collection' em destaque.":::

> [!NOTE]
> **A Predefinição de Recolha** é uma coleção gerada pelo sistema e não pode ser eliminada.

## <a name="private-azure-marketplace-notification-center"></a>Centro de notificação private Azure Marketplace

O Centro de Notificação é composto por três tipos de notificações e permite ao administrador do Marketplace tomar medidas com base na notificação:

- Pedidos de aprovação dos utilizadores para itens que não constam da lista aprovada (ver [Pedido de adicionar ofertas ou planos](#request-to-add-offers-or-plans) abaixo).
- Novas notificações de plano para ofertas que já tenham um ou mais planos na lista aprovada.
- Removidos notificações do plano para itens que estão na lista aprovada, mas foram removidos do mercado global de Azure.

Para aceder ao centro de notificação:

1. Selecione **Notificações** do menu de navegação à esquerda.

   :::image type="content" source="media/private-azure-new/marketplace-notifications-small.png" lightbox="media/private-azure/marketplace-notifications.png" alt-text="Mostra o menu notificações.":::

1. Selecione um menu de elipses à direita para mais ações.

    :::image type="content" source="media/private-azure/notifications-more-options.png" alt-text="Mostra os resultados do menu Mais Opções.":::

1. Para pedidos de plano, **os pedidos do Show** abrem o formulário de pedido de aprovação onde pode rever todos os pedidos do utilizador para a oferta específica.

1. Selecione **Aprovar** ou **Rejeitar**.

   :::image type="content" source="media/private-azure-new/notifications-approve-reject-small.png" lightbox="media/private-azure/notifications-approve-reject.png" alt-text="Mostra as opções de aprovação e rejeição.":::

1. Selecione o plano para aprovar no menu suspenso.

1. Selecione a coleção para adicionar as ofertas/planos para.

1. Adicione um comentário e **selecione Enviar por isso.**

## <a name="browsing-private-azure-marketplace-user-experience"></a>Navegar no Private Azure Marketplace (experiência do utilizador)

Quando o Private Azure Marketplace estiver ativado, os utilizadores verão quais os planos que o administrador do Marketplace aprovou.

- Um **aviso** aprovado verde indica uma oferta de Parceiro (não Microsoft) que é aprovada.
- Um aviso **aprovado** azul indica uma oferta da Microsoft (incluindo [distribuições de Linux endossadas)](/azure/virtual-machines/linux/endorsed-distros)que é aprovada.

Os utilizadores podem filtrar entre ofertas que são e não são aprovadas:

   :::image type="content" source="media/private-azure/filter-option-small.png" lightbox="media/private-azure/filter-option.png" alt-text="Mostra a opção de filtragem.":::

## <a name="buy-or-deploy-in-private-azure-marketplace"></a>Comprar ou implementar no Private Azure Marketplace

Embora a experiência da página de detalhes do produto seja semelhante ao Azure Marketplace global, existem três cenários específicos do Private Azure Marketplace.

- Quando um utilizador seleciona uma combinação de plano aprovado e subscrição aprovada, o botão **Criar** está ativado:

   :::image type="content" source="media/private-azure/button-create-enabled-small.png" lightbox="media/private-azure/button-create-enabled.png" alt-text="Mostra o banner de oferta observando que um plano pode ser criado.":::

- Se uma seleção de plano de produto não aparecer na página de detalhes do produto, mas o administrador aprovou um ou mais planos, um banner assinala quais os planos aprovados e o botão **Criar** está ativado:

   :::image type="content" source="media/private-azure/button-create-enabled-and-plans-small.png" lightbox="media/private-azure/button-create-enabled-and-plans.png" alt-text="Mostra o banner da oferta notando que um plano pode ser criado e mostrando planos disponíveis.":::

- Quando um utilizador seleciona um plano ou subscrição não aprovado, um banner assinala o plano como não aprovado para a subscrição selecionada e o botão **Criar** é desativado. O utilizador ainda pode solicitar a adição do plano à lista aprovada (ver secção seguinte).

## <a name="request-to-add-offers-or-plans"></a>Pedido de adição de ofertas ou planos

Pode solicitar a adição de uma oferta pública ou plano que não esteja atualmente aprovado no Mercado Privado Azure.

1. Selecione **Pedido para adicionar** no banner para abrir o formulário de pedido de **acesso**.

   :::image type="content" source="media/private-azure-new/access-request-form-small.png" lightbox="media/private-azure/access-request-form.png" alt-text="Mostra o formulário de pedido de acesso para ofertas ou planos.":::

1. Selecione quais os planos a adicionar ao pedido (**Qualquer Plano** diz ao administrador do Marketplace que não tem preferência por um plano específico dentro de uma oferta).

1. Adicione uma **Justificação** e selecione **Pedido** para submeter o seu pedido.

1. Uma indicação para um pedido pendente aparecerá no formulário de pedido de Acesso com opção de **retirar o pedido.**

   :::image type="content" source="media/private-azure/approved-pending-plans-small.png" lightbox="media/private-azure/approved-pending-plans.png" alt-text="Mostra uma lista de planos aprovados ou pendentes com link Pedido de Retirada.":::

> [!NOTE]
> Uma vez apresentado, o formulário de pedido de aprovação será enviado ao [Centro de Notificação](#private-azure-marketplace-notification-center) do Administrador do Mercado para rever o pedido e tomar medidas.

> [!CAUTION]
> A aprovação no Mercado Privado não indica a aquisição de uma solução.

## <a name="frequently-asked-questions-faqs"></a>Perguntas frequentes (Perguntas Frequentes)

#### <a name="i-am-already-blocking-marketplace-third-party-application-through-azure-policy-how-is-this-different"></a>Já estou a bloquear a aplicação de terceiros do Marketplace através da Política Azure. Como é que isto é diferente?

Existem atualmente duas formas de restringir os serviços de terceiros no Marketplace:

1. Através do portal EA ou do portal Azure, desative os serviços de terceiros ou limite-se apenas a "SKUs gratuitos ou BYOL".

    :::image type="content" source="media/private-azure/disable-services.png" alt-text="Mostra como restringir os serviços no portal Azure.":::

    :::image type="content" source="media/private-azure/disable-services-other-view.png" alt-text="Mostra como restringir os serviços no portal E A.":::

2. Crie uma política Azure apenas para permitir VMs específicos. Para obter detalhes sobre como impor a política aos VMs Windows, consulte [aplicar políticas para Windows VMs com O Gestor de Recursos Azure](/azure/virtual-machines/windows/policy).

O Private Azure Marketplace permite uma maior flexibilidade na limitação e na possibilidade de ofertas e planos específicos. Informa os utilizadores finais sobre a disponibilidade para implantação na galeria do mercado mesmo antes de tentarem implementar serviços de terceiros. Para permitir a implantação de serviços de terceiros, defina o Azure Marketplace para On/Enabled no Portal EA e no portal Azure.

- O Private Azure Marketplace pode curar soluções parceiras não limitadas a máquinas virtuais.
- O Private Azure Marketplace pode ser curador ao nível do plano e pode ainda definir "Plano atual e futuro".
- O Private Azure Marketplace pode informar os utilizadores finais adiantado sobre o que pode ou não ser implementado.

#### <a name="whats-the-difference-between-a-private-offer-and-private-azure-marketplace"></a>Qual é a diferença entre uma Oferta Privada e o Mercado Privado Azure?

Uma **Oferta Privada** permite que os parceiros criem planos que só são visíveis para clientes direcionados. Isto permite-lhes partilhar em privado soluções personalizadas com preços e condições negociados, termos e condições privados e configurações especializadas. Para mais detalhes, consulte [ofertas privadas no mercado comercial.](/azure/marketplace/private-offers)

**O Private Azure Marketplace** no portal Azure permite aos administradores pré-aprovarem quais as soluções de terceiros que os seus utilizadores podem implementar. Com um Private Azure Marketplace, os utilizadores podem usufruir dos benefícios do Azure Marketplace, encontrando, comprando e implementando ofertas compatíveis. Para gerir ofertas privadas baseadas em subscrições no Mercado Privado, o administrador do Marketplace deve ter um papel mínimo de "leitura" na subscrição específica.

#### <a name="i-added-a-private-offer-to-the-private-azure-marketplace-why-is-it-not-showing-in-the-manage-marketplace-tab"></a>Adicionei uma Oferta Privada ao Private Azure Marketplace, porque é que não está a aparecer no separador de mercado de gestão?

As Ofertas Privadas baseadas em subscrições são visíveis apenas para as subscrições listadas nas definições de Oferta Privada. Para ver a Oferta Privada, certifique-se de que o filtro global de subscrição está mostrando todas as subscrições.

   :::image type="content" source="media/private-azure/private-marketplace-filter.png" lightbox="media/private-azure/private-marketplace-filter.png" alt-text="Mostra o filtro do mercado privado.":::

#### <a name="can-we-include-custom-images-in-private-azure-marketplace"></a>Podemos incluir imagens personalizadas no Private Azure Marketplace?

N.º O Private Azure Marketplace permite que qualquer administrador de TI gere e cuide de soluções de terceiros a partir do Mercado Azure Global. Uma vez que as imagens personalizadas não estão no Azure Marketplace global, o administrador de TI não pode escolher as suas imagens personalizadas. Se quiser partilhar imagens personalizadas, utilize a [Galeria de Imagens Partilhadas.](/azure/virtual-machines/shared-image-galleries)

1. Guia passo a passo Criar uma Galeria de Imagem Partilhada (SIG)[(CLI,](/azure/virtual-machines/shared-images-cli) [PowerShell).](/azure/virtual-machines/shared-images-powershell)
2. Crie uma definição de imagem dentro de um SIG. O cliente deve escolher **generalizado** para o campo estado-OS. ([CLI,](/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition) [PowerShell).](/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)
3. Traga a imagem gerida para a Galeria de Imagens Partilhadas[(CLI,](/azure/virtual-machines/image-version-managed-image-cli) [PowerShell).](/azure/virtual-machines/image-version-managed-image-powershell)
4. As imagens SIG VM residiriam numa subscrição. Para disponibilizá-lo a outras subscrições, utilize um registo de aplicações[(CLI,](/azure/virtual-machines/linux/share-images-across-tenants) [PowerShell).](/azure/virtual-machines/windows/share-images-across-tenants)

#### <a name="why-do-i-see-some-offers-approved-by-default-even-though-the-partner-is-not-microsoft"></a>Por que vejo algumas ofertas **aprovadas por padrão,** mesmo que o parceiro não seja a Microsoft?

A Microsoft suporta o Linux e a tecnologia open-source em Azure. [As distribuições de Linux endossadas](/azure/virtual-machines/linux/endorsed-distros) são suportadas no Azure e o preço está integrado em máquinas virtuais. Uma vez que o Agente Azure Linux já está pré-instalado no Azure Marketplace, é tratado como uma oferta da Microsoft. Uma vez que as ofertas da Microsoft são aprovadas por padrão, as distribuições de Linux endossadas não podem ser geridas no Private Azure Marketplace e são aprovadas por padrão.

## <a name="contact-support"></a>Contactar o suporte

- Para obter suporte ao Azure Marketplace, visite [o Microsoft Q&A](/answers/products/).
<!-- images to delete when we retire old version: request-banner-small and access-request-form-filled-small>
