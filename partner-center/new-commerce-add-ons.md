---
title: Novos add-ons de comércio
ms.topic: article
ms.date: 09/03/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Conheça novas experiências de comércio para comprar addons.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c944dc5de89ad0e9d6332252d722de90250c82c6
ms.sourcegitcommit: d731813da1d31519dc2dc583d17899e5cf4ec1b2
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/27/2021
ms.locfileid: "129072770"
---
# <a name="introduction-new-commerce-add-ons"></a>Introdução: Novos complementos de comércio

**Funções adequadas**: Agente administrador | Agente comercial | Administrador global

> [!NOTE]
> As novas mudanças na experiência de comércio estão atualmente disponíveis apenas para parceiros que fazem parte da Microsoft 365/Dynamics 365 nova experiência técnica de experiência técnica.

Os parceiros podem adquirir addons em novo comércio para permitir outros serviços que complementem um produto previamente comprado. Alguns exemplos destes são planos de chamada, mais espaço em disco, ou outras funcionalidades que podem ser adicionadas se o cliente tiver os serviços base.

## <a name="add-ons-in-new-commerce"></a>Suplementos em novo comércio

Os novos complementos de comércio incluem conceitos semelhantes aos suplementos tradicionais baseados em licenças. Novos complementos de comércio, como as tradicionais baseadas em licenças, incluem o conceito de pré-requisitos. Estes são SKUs de produto que o cliente deve ter para que o add-on funcione corretamente. Os pré-requisitos para um addon podem ser encontrados o catálogo APIs para um dado SKU e no catálogo do Partner Center experiência de utilizador. A aquisição de suplementos requer que exista um ou mais dos pré-requisitos para o cliente.

A grande diferença na compra de complementos entre licenças tradicionais e novo comércio está na *forma como* são comprados. Na licença tradicional, o parceiro aplica o complemento a uma subscrição de oferta de base existente. No novo comércio, os parceiros compram os addons do próprio catálogo, já não tendo uma experiência bifurcada de compra para ofertas base e addons, tudo está no catálogo em novo comércio.

Muitos dos conceitos sobre como funcionam os complementos, do ponto de vista dos serviços, permanecem verdadeiros em todo o comércio tradicional e novo. Tanto o registo como a prestação dos serviços adicionais, não há nada de diferente na forma como o provisionamento acontece. Além disso, um único serviço de addon pode complementar mais do que um produto base SKU o add-on é projetado para trabalhar com.

## <a name="identifying-add-ons"></a>Identificar addons

Os parceiros podem identificar Add-ons e obter listas de pré-requisitos, revendo os detalhes do SKU ao obter SKUs através da API. Os addons também são identificados na nova lista de preços baseados em licenças de comércio na coluna Tags. A matriz de oferta inclui a lista de pré-requisitos para cada produto adicionador SKU.

## <a name="purchasing-add-ons"></a>Aquisição de suplementos

Existem complementos tanto para experiências tradicionais baseadas em licenças como para novas experiências de comércio. A principal diferença é que o novo comércio permite a descoberta e a compra do catálogo, o mesmo local onde se encontram as ofertas base ou os pré-requisitos. Os addons tradicionais baseados em licenças só são detetáveis e adquiridos indo para a página de detalhes de subscrição da oferta base. Depois de um addon ser listado lá, o parceiro aplica o addon desejado.

Novos add-ons de experiência de comércio são descobertos e comprados no próprio catálogo. Os parceiros podem filtrar por novos addons de comércio selecionando o dropdown do tipo de produto. Os produtos adicionais também são fáceis de ver, uma vez que têm um ícone de informação ao seu lado, o que explica o seu estado de Add-on e significado.

Os parceiros podem obter mais detalhes sobre os produtos necessários para um addon clicando em *Ver subscrições de produtos base compatíveis* para mostrar uma lista de SKUs de produto que deve existir para o parceiro comprar um dado addon.

## <a name="add-on-enforcement"></a>Aplicação de complementos

Os parceiros verão erros ao tentar comprar um novo produto de complemento de comércio onde o cliente não tenha nenhum dos requisitos prévios. Os parceiros podem validar um cliente que cumpre os requisitos pré-requisitos, ligando para a validação da APIaddon no centro de parceiros.

## <a name="important-details-when-purchasing-add-ons"></a>Detalhes importantes na compra de addons

Os addons são adquiridos como SKUs de produto distinto se o cliente satisfizer os requisitos prévios. As subscrições adicionais têm o seu próprio alinhamento de termo distinto. Os parceiros que comprarem addons notarão o termo e a data de fim associada pode não ser o mesmo que o pré-requisito. Desde que ambas as subscrições renovam automaticamente para novos termos, os suplementos pré-requisitos e adicionais funcionarão muito bem. Se o parceiro decidir terminar o prazo pré-requisito não renovando automaticamente, então o addon também deve ser atualizado para não renovar automaticamente no final do prazo de adição se o parceiro concluir que já não é necessário.  Os parceiros convertem um produto SKU para um SKU mais alto que já tem os serviços adicionais pode arquivar um pedido de serviço com suporte para desligar um add-on.

Espera-se que os parceiros gerem as datas limite de prazo para os addons que adquirem para garantir que há alinhamento conforme necessário às ofertas base.
