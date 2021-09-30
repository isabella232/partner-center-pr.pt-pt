---
title: Novos add-ons de comércio
ms.topic: article
ms.date: 09/29/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Conheça novas experiências de comércio para comprar addons.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 355c7ae3d4832764f6201613c040eebca998c3b6
ms.sourcegitcommit: a59e1abb470f4847e8f8337ffa4ba705514a0424
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/29/2021
ms.locfileid: "129249337"
---
# <a name="introduction-new-commerce-add-ons"></a>Introdução: Novos complementos de comércio

**Funções adequadas**: Agente administrador | Agente comercial | Administrador global

> [!NOTE]
> As novas mudanças na experiência de comércio estão atualmente disponíveis apenas para parceiros que fazem parte da Microsoft 365/Dynamics 365 nova experiência técnica de experiência técnica.

Os parceiros podem adquirir addons em novo comércio para permitir outros serviços que complementem um produto previamente comprado. Alguns exemplos de addons são planos de chamada, mais espaço em disco, ou outras funcionalidades que podem ser adicionadas se o cliente tiver os serviços base.

## <a name="add-ons-in-new-commerce"></a>Suplementos em novo comércio

Os novos complementos de comércio incluem conceitos semelhantes aos suplementos tradicionais baseados em licenças. Novos complementos de comércio, como as tradicionais baseadas em licenças, incluem o conceito de pré-requisitos. Os requisitos prévios são o produto SKUs que o cliente deve ter para que o add-on funcione corretamente. Os pré-requisitos para um addon podem ser encontrados o catálogo APIs para um dado SKU e no catálogo do Partner Center experiência de utilizador. A aquisição de suplementos requer que exista um ou mais dos pré-requisitos para o cliente.

A principal diferença entre os suplementos de comércio tradicionais e os novos é a **forma como** são comprados. Os parceiros aplicam o complemento à subscrição da oferta base em cenários tradicionais baseados em licenças. Parceiro comprar novos add-ons de comércio do próprio catálogo. Esta experiência de compra alinha a descoberta adicional à oferta base, facilitando a procura e compra dos addons.

Muitos dos conceitos sobre como funcionam os complementos, do ponto de vista dos serviços, permanecem verdadeiros em todo o comércio tradicional e novo. Tanto as transações comerciais tradicionais como as novas transações de comércio registam e prestam os serviços adicionais, o provisionamento ocorre da mesma forma em ambos os casos. Além disso, um único serviço de addon pode complementar mais do que um produto base SKU o add-on é projetado para trabalhar com.

## <a name="identifying-add-ons"></a>Identificar addons

Os parceiros podem identificar Add-ons e obter listas de pré-requisitos, revendo os detalhes do SKU ao obter SKUs através da API. Os addons também são identificados na nova lista de preços baseados em licenças de comércio na coluna Tags. A matriz de oferta inclui a lista de pré-requisitos para cada produto adicionador SKU.

## <a name="purchasing-add-ons"></a>Aquisição de suplementos

Existem complementos tanto para experiências tradicionais baseadas em licenças como para novas experiências de comércio. A diferença chave é como os addons são descobertos. Novos addons de comércio são descobertos e compra do catálogo, o mesmo local onde se encontram as ofertas base ou os pré-requisitos. Os addons tradicionais baseados em licenças só são detetáveis e adicionados indo para a página de detalhes de subscrição da oferta base. 

Novos add-ons de experiência de comércio são descobertos e comprados no próprio catálogo. Os parceiros podem filtrar por novos addons de comércio selecionando o dropdown do tipo de produto. Os produtos adicionais são identificados pelo ícone de informação ao lado do produto SKU. Os parceiros podem clicar neste ícone para obter mais informações sobre os pré-requisitos do add-on.

Os parceiros podem obter mais detalhes sobre os produtos necessários para um addon clicando em **Ver subscrições de produtos base compatíveis** para mostrar uma lista de SKUs de produto que deve existir para o parceiro comprar um dado addon.

## <a name="add-on-enforcement"></a>Aplicação de complementos

Os parceiros verão informações úteis sobre addons ao tentar comprar um novo produto de complemento de comércio quando o cliente não tiver os pré-requisitos. Os parceiros podem validar se existem pré-requisitos de um addon no catálogo do Partner Center e experiências de página de revisão. Se o addon não tiver os pré-requisitos de suporte, a interface do utilizador apresentará uma mensagem "O addon não é purivel sem um produto base compatível". Os parceiros que utilizam a API CreateCart verão um erro no item da linha do carrinho se o add-on não tiver os SKUs do produto necessário. O código de erro será 400041 com a descrição "O addon não é purificável sem um produto base compatível".

## <a name="important-details-when-purchasing-add-ons"></a>Detalhes importantes na compra de addons

Os addons são adquiridos como SKUs de produto distinto se o cliente satisfizer os requisitos prévios. As subscrições adicionais têm o seu próprio alinhamento de termo distinto. Os parceiros que comprarem addons notarão o termo e a data de fim associada pode não ser o mesmo que o pré-requisito. Enquanto ambas as subscrições renovarem automaticamente para novos termos, os suplementos e suplementos pré-necessários continuarão a funcionar corretamente. Se o parceiro decidir terminar o prazo pré-requisito não renovando automaticamente, então o addon também deve ser atualizado para não renovar automaticamente no final do prazo de adição se o parceiro concluir que já não é necessário.  Os parceiros convertem um produto SKU para um SKU mais alto que já tem os serviços adicionais pode arquivar um pedido de serviço com suporte para desligar um add-on.

Espera-se que os parceiros gerem as datas limite de prazo para os addons que adquirem para garantir que há alinhamento conforme necessário às ofertas base.
