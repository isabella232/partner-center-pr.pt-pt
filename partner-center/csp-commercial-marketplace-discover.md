---
title: Descubra ofertas - mercado comercial
ms.topic: how-to
ms.date: 09/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Saiba como os parceiros da CSP podem usar o Partner Center para visualizar ou pesquisar no mercado ofertas ou preços de Fornecedores de Software Independentes (ISVs).
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 991839f3675fb77c40ab08af623094e02521d6b3
ms.sourcegitcommit: d731813da1d31519dc2dc583d17899e5cf4ec1b2
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/27/2021
ms.locfileid: "129072252"
---
# <a name="discover-offers-and-pricing-in-partner-center-commercial-marketplace"></a>Descubra ofertas e preços no mercado comercial partner Center

**Funções adequadas**: Administração global | Agente administrativo

Quando os Fornecedores independentes de Software (ISV) optarem por publicar uma oferta no mercado comercial, também podem decidir se querem que a oferta seja disponibilizada no programa CSP. Se optarem por vender a oferta através do programa CSP, os parceiros da CSP deverão ver a oferta na área do Partner Center Marketplace.

Se uma oferta ISV não aparecer como espera no Partner Center, pode ser porque:

- O ISV decidiu não vender a oferta através do programa CSP. Por exemplo, alguns produtos ISV podem ter sido disponibilizados noutras áreas do mercado comercial (como no [Microsoft AppSource](https://appsource.microsoft.com/) e [Azure Marketplace),](https://azuremarketplace.microsoft.com/)mas podem não aparecer para parceiros no programa CSP no mercado partner Center.

- O ISV decidiu tornar a oferta exclusiva apenas para um número selecionado de parceiros CSP. Para mais informações sobre ofertas exclusivas, consulte mais tarde neste tópico de ajuda.

- O tipo de oferta pode não ser transacionável através do Partner Center ou do portal Azure (por exemplo, contentores ou algumas ofertas baseadas em uso).

- O país de faturação dos seus clientes associados não pode ser suportado para esta oferta ISV.

## <a name="view-marketplace-offers-in-partner-center"></a>Ver ofertas do Marketplace no Partner Center

Para visualizar as ofertas de mercado comercial disponíveis no programa CSP:

> [!NOTE]
> A interface de pré-visualização do Partner Center proporciona-lhe uma experiência de utilizador mais eficiente e produtiva através de espaços de trabalho agrupados logicamente. Para saber mais sobre a interface dos espaços de trabalho e como ligá-lo, consulte [Getting around Partner Center](get-around-partner-center.md#turn-workspaces-on-and-off).

#### <a name="workspaces-view"></a>[Vista de espaços de trabalho](#tab/workspaces-view)

1. Inscreva-se no [painel partner center](https://partner.microsoft.com/dashboard) e selecione o azulejo de **preços.**

2. Selecione **Marketplace**. Por padrão, verá produtos de todos os tipos e categorias.

3. Selecione um filtro por tipo ou categoria. Também pode utilizar **a Pesquisa** para encontrar palavras-chave específicas, oferecer nomes ou nomes de editores ISV.

4. Selecione uma oferta específica de produto da lista. Isto irá levá-lo a um separador de visão geral do produto onde poderá saber mais sobre a oferta. As informações sobre este separador podem incluir:

    - Uma descrição do produto ou oferta

    - Mais informações sobre a editora ISV

    - Links para documentação ou materiais de marketing carregados pela editora ISV

    - Outros possíveis contactos ISV para apoio ao cliente, engenharia ou um contacto para o programa CSP

5. Para ver mais informações sobre os planos disponíveis de uma oferta, SKUs ou preços, selecione o **separador Planos + Preços.** Este separador irá mostrar-lhe:

    - Os mercados onde esta oferta está disponível para si

    - Uma lista de SKUs ou planos disponíveis para a oferta

    - Preços para cada SKU ou Plano disponível

#### <a name="current-view"></a>[Vista atual](#tab/current-view)

1. Inscreva-se no painel partner [center](https://partner.microsoft.com/dashboard)e, em seguida, selecione **CSP** do menu de navegação à esquerda.

2. Selecione **Venda,** seguido do **Marketplace**. Por padrão, verá produtos de todos os tipos e categorias.

3. Selecione um filtro por tipo ou categoria. Também pode utilizar **a Pesquisa** para encontrar palavras-chave específicas, oferecer nomes ou nomes de editores ISV.

4. Selecione uma oferta específica de produto da lista. Isto irá levá-lo a um separador de visão geral do produto onde poderá saber mais sobre a oferta. As informações sobre este separador podem incluir:

    - Uma descrição do produto ou oferta

    - Mais informações sobre a editora ISV

    - Links para documentação ou materiais de marketing carregados pela editora ISV

    - Outros possíveis contactos ISV para apoio ao cliente, engenharia ou um contacto para o programa CSP

5. Para ver mais informações sobre os planos disponíveis de uma oferta, SKUs ou preços, selecione o **separador Planos + Preços.** Este separador irá mostrar-lhe:

    - Os mercados onde esta oferta está disponível para si

    - Uma lista de SKUs ou planos disponíveis para a oferta

    - Preços para cada SKU ou Plano disponível

* * *

## <a name="view-marketplace-offers-via-partner-center-apis"></a>Ver Ofertas do Marketplace através de APIs do Partner Center

Os parceiros do programa CSP também podem usar APIs para devolver uma lista de ofertas elegíveis. As ofertas elegíveis serão apenas as ofertas saaS ISV disponíveis para o parceiro vender através do mercado Partner Center. Para os parceiros que utilizam APIs para identificar ofertas no catálogo, consulte as orientações para [obter uma lista de ofertas para um mercado](/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market).

## <a name="view-the-latest-marketplace-offer-pricing-in-partner-center"></a>Veja os preços mais recentes da oferta de marketplace no Partner Center

Siga estes passos para os mais recentes detalhes de preços associados a uma oferta:

> [!NOTE]
> A interface de pré-visualização do Partner Center proporciona-lhe uma experiência de utilizador mais eficiente e produtiva através de espaços de trabalho agrupados logicamente. Para saber mais sobre a interface dos espaços de trabalho e como ligá-lo, consulte [Getting around Partner Center](get-around-partner-center.md#turn-workspaces-on-and-off).

#### <a name="workspaces-view"></a>[Vista de espaços de trabalho](#tab/workspaces-view)

1. Inscreva-se no [painel partner center](https://partner.microsoft.com/dashboard) e selecione o azulejo de **preços.**

2. Selecione **Marketplace**. Por padrão, verá produtos de todos os tipos e categorias.

3. Percorra a secção **Marketplace,** selecione uma localização e baixe **os preços do Marketplace**. Isto gera uma folha de cálculo com os dados de preços mais recentes para o SaaS, ofertas baseadas em licenças e ofertas com contadores disponíveis a partir de editores ISV. Alguns preços de aplicação Azure também podem aparecer aqui. Estas informações são atualizadas diariamente, para que possa verificar se existem preços correntes sempre que quiser.

4. Se um produto ISV incluir um período experimental gratuito, a folha de cálculo apresentará duas linhas para esse produto:

    - Uma linha mostra o preço de teste gratuito de zero. Isto significa que está disponível um período experimental gratuito.

    - A outra linha mostra o preço e os termos que se aplicarão após o fim do período experimental gratuito.

Como parceiro de programa CSP, poderá ser elegível para outros incentivos associados a determinadas ofertas de mercado comercial. Para obter mais informações sobre outros incentivos, consulte o [guia de incentivos da CSP](https://aka.ms/partnerincentives) (requer login CSP).

#### <a name="current-view"></a>[Vista atual](#tab/current-view)

1. Inscreva-se no painel partner [center](https://partner.microsoft.com/dashboard)e, em seguida, selecione **CSP** do menu de navegação à esquerda.

2. Selecione **Venda,** seguido **de Preços e ofertas**.

3. Percorra a secção **Marketplace,** selecione uma localização e baixe **os preços do Marketplace**. Isto gera uma folha de cálculo com os dados de preços mais recentes para o SaaS, ofertas baseadas em licenças e ofertas com contadores disponíveis a partir de editores ISV. Alguns preços de aplicação Azure também podem aparecer aqui. Estas informações são atualizadas diariamente, para que possa verificar se existem preços correntes sempre que quiser.

4. Se um produto ISV incluir um período experimental gratuito, a folha de cálculo apresentará duas linhas para esse produto:

    - Uma linha mostra o preço de teste gratuito de zero. Isto significa que está disponível um período experimental gratuito.

    - A outra linha mostra o preço e os termos que se aplicarão após o fim do período experimental gratuito.

Como parceiro de programa CSP, poderá ser elegível para outros incentivos associados a determinadas ofertas de mercado comercial. Para obter mais informações sobre outros incentivos, consulte o [guia de incentivos da CSP](https://aka.ms/partnerincentives) (requer login CSP).

* * *

## <a name="learn-about-marketplace-exclusive-offers"></a>Conheça as ofertas exclusivas do marketplace

Os ISVs têm a opção de disponibilizar as suas ofertas apenas a parceiros específicos no programa CSP. Isto é conhecido como uma oferta exclusiva. Todos os parceiros do programa CSP ainda podem ver todas as ofertas isv no mercado comercial partner Center, incluindo as ofertas marcadas como Exclusive.

Se uma oferta **não** estiver marcada como Exclusiva, todos os parceiros podem comprar essa oferta (assumindo que o país de faturação do cliente selecionado corresponde à disponibilidade do país da oferta do ISV).

Para qualquer oferta marcada exclusivamente, no entanto, apenas os parceiros selecionados pelo ISV poderão adquirir essa oferta.

> [!NOTE]
> Se vir uma oferta marcada exclusivamente que gostaria de vender aos seus clientes, contacte diretamente o ISV e peça permissão para vender a oferta exclusiva. Quando visualizar os detalhes de uma oferta exclusiva, poderá ver um link **Contato ISV** que pode selecionar.

Para saber mais sobre a experiência ISV no mercado comercial, leia a [Cloud Solution Providers.](/azure/marketplace/cloud-solution-providers)

Para obter mais informações sobre a experiência da CSP no mercado, leia a [visão geral do mercado comercial.](csp-commercial-marketplace-overview.md)

## <a name="next-steps"></a>Passos seguintes

- [Comprar ofertas de mercado comercial](csp-commercial-marketplace-purchase.md)