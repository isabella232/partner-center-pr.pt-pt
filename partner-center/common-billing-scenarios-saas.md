---
title: Faturação - transações saaS baseadas em licenças
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
description: Conheça os cenários comuns de faturação no Partner Center para transações baseadas em licenças, software-as-a-service (SaaS).
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 85b5b4c33226236b7fcc3ce6b4833c3d58aba58ebb281b80576c9f26d04ecfe3
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/06/2021
ms.locfileid: "115682254"
---
# <a name="common-billing-scenarios-for-license-based-saas-transactions-in-partner-center"></a>Cenários comuns de faturação para transações saaS baseadas em licenças no Partner Center

**Funções adequadas**: Agente administrador | Administrador de faturação | Agente helpdesk | Agente comercial


Estes [cenários de faturação comuns](common-billing-scenarios.md) são aplicáveis a software baseado em licenças como subscrições de serviço (SaaS) no Partner Center.

## <a name="convert-a-free-trial-saas-subscription-to-a-paid-subscription"></a>Converter uma subscrição gratuita do SaaS para uma subscrição paga

Este cenário descreve a faturação para a renovação de uma subscrição saas de teste gratuito baseada em licença. A renovação converte o teste gratuito para uma subscrição paga no final do período experimental gratuito.

Neste exemplo, comprou um teste gratuito de uma subscrição saaS (software como serviço) baseada em licença no dia 10 de junho. Este teste gratuito foi automaticamente renovado como uma subscrição paga quando o período experimental gratuito terminar.

Os ficheiros de reconhecimento incluirão os seguintes encargos:

| Data de compra | Data de início da carga | Data de fim da carga | Preço unitário | Quantidade unitária | Montante total | Tipo de custo | Descrição da subscrição |
| ------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | 06/10/2019 | 07/09/2019 | $0 | 1 | $0 | Novo | Avaliação gratuita |
| 07/10/2019 | 07/10/2019 | 08/09/2019 | $2 | 1 | $2 | Renovar | Subscrição paga |

## <a name="cancel-a-free-trial-saas-subscription"></a>Cancelar uma subscrição gratuita do SaaS

> [!TIP]
> Pode cancelar uma subscrição saaS de teste gratuito baseada na licença a qualquer momento, mesmo durante o período de teste gratuito.

Neste cenário, comprou uma assinatura SaaS de teste gratuito baseada em licença no dia 1 de julho e depois cancelou-a imediatamente no Partner Center.

O ficheiro de reconhecimento incluirá as seguintes acusações:

| Data de compra | Data de início da carga | Data de fim da carga | Preço unitário | Quantidade unitária | Montante total | Tipo de custo | Descrição da subscrição |
| ------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | 06/10/2019 | 07/09/2019 | $0 | 11 | $0 | Novo | Avaliação gratuita |
| 06/10/2019 | 06/10/2019 | 07/09/2019 | $0 | 11 | $0 | Cancelar | Avaliação gratuita |

## <a name="convert-custom-meter-saas-subscription-to-another-sku"></a>Converter a subscrição do medidor personalizado SaaS para outro SKU

Este cenário descreve como converter uma subscrição de medidor personalizado SaaS de uma unidade de stock (SKU) para outra SKU para o mesmo produto, na mesma data.

Neste cenário, comprou um SKU (Silver) sob um produto e converteu-o para outro SKU (Bronze) disponível ao abrigo deste produto na mesma data.

O ficheiro de reconhecimento incluirá as seguintes acusações:

| Data de compra | SKU | Data de início da carga | Data de fim da carga | Preço unitário | Quantidade unitária | Montante total | Tipo de custo | Descrição da subscrição |
| ------------- | ----------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | Silver | 06/10/2019 | 06/10/2019 | $20 | 1 | $20 | Novo | Assinatura saaS do medidor personalizado |
| 06/10/2019 | Silver | 06/10/2019 | 06/10/2019 | $20 | 1 | -$20 | Converter | Rebill procitado para assinatura saas de medidor personalizado |
| 06/10/2019 | Bronze | 06/10/2019 | 06/10/2019 | 10 € | 1 | 10 € | Converter | Assinatura saaS do medidor personalizado |

## <a name="purchase-and-cancel-a-customer-meter-saas-subscription-on-same-date"></a>Comprar e cancelar uma assinatura saaS do medidor de clientes na mesma data

Este cenário descreve a faturação de uma subscrição do Medidor de Cliente SaaS que adquiriu e cancelou através do portal Azure na mesma data.

Neste cenário, comprou uma assinatura SaaS de medidor personalizado no portal Azure. Em seguida, cancelou a assinatura na mesma data.

| Data de compra | SKU | Data de início da carga | Data de fim da carga | Preço unitário | Quantidade unitária | Montante total | Tipo de custo | Descrição da subscrição |
| ------------- | ------------- |----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | Bronze | 06/10/2019 | 06/10/2019 | 10 € | 1 | 10 € | Novo | Assinatura saaS do medidor personalizado |
| 06/10/2019 | Bronze | 06/10/2019 | 06/10/2019 | 10 € | 1 | -$10 | CancelImmediate | Assinatura saaS do medidor personalizado |
