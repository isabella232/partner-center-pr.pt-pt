---
title: Faturação anual - cenários comuns
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
description: Contação anual do Partner Center - quando adicionar novas subscrições, adicionar licenças antes da data de faturação, alterar a quantidade de licença ou suspender/reativar subscrições.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 0f97c36c821955570965fcebb006610f4c5c0c79
ms.sourcegitcommit: e1da62b36420d78bf44e3962358d0af65ebc3402
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/27/2021
ms.locfileid: "129089492"
---
# <a name="common-annual-billing-scenarios-in-partner-center"></a>Cenários comuns de faturação anual no Centro de Parceiros

**Funções adequadas**: Agente administrador | Administrador de faturação | Agente helpdesk | Agente comercial

Estes [cenários de faturação comuns](common-billing-scenarios.md) são aplicáveis se utilizar a faturação anual no Partner Center.

## <a name="new-annual-subscription"></a>Nova subscrição anual

A sua data de faturação é dia 15 de cada mês. No dia 13 de janeiro, você compra uma nova subscrição com uma licença por $4 por mês e seleciona faturação anual. O ficheiro de reconciliação baseado em licenças de 15 de janeiro conterá a seguinte linha de faturação:

|Data de início do carregamento |Data de fim de carga |Tipo de carga |Preço Unitário |Quantidade |Montante |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13 de janeiro de 2018|12 de janeiro de 2019|Taxas de prorate na compra|48.00|1|48.00

## <a name="add-license-after-subscription-anniversary-date-but-before-billing-date"></a>Adicionar licença após data de aniversário de assinatura, mas antes da data de faturação

Você compra uma nova subscrição em 11 de fevereiro de 2017 com uma licença por $211,20 por ano. O seu aniversário de subscrição está definido como o dia 11 de cada mês. O sistema de faturação da Microsoft cria as seguintes linhas de faturação:

- $211,20 de taxa para o período 11 de fevereiro de 2017 - 10 de fevereiro de 2018.

Em 12 de fevereiro de 2017, compra uma segunda licença. Sua data de faturação é 14 de fevereiro de 2017. Uma fatura e um ficheiro de reconciliação são gerados. O ficheiro de reconciliação conterá as seguintes linhas de faturação:

|Data de início do carregamento  |Data de fim de carga  |Tipo de carga  |Preço Unitário |Quantidade | Montante |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|11 de fevereiro de 2017 |10 de fevereiro de 2018 |Taxas de prorate ao comprar |211.20 |1 | 211.20 |

No seu aniversário de subscrição, 11 de março de 2017, o sistema de faturação da Microsoft cria as seguintes linhas de faturação para o aumento da licença em 12 de fevereiro de 2017:

- Crédito de $211,20 para o período de 11 de fevereiro de 2017 a 10 de fevereiro de 2018.
- $0,58 taxa procorrida por licença por uma licença para o período 11 de fevereiro de 2017 a 11 de fevereiro de 2017.
- $15,62 taxa procorrida por licença para duas licenças para o período 12 de fevereiro de 2017 a 10 de março.
- $195,00 taxa procorrida por licença para duas licenças para o período 11 de março de 2017 a 10 de fevereiro de 2018.

No dia 11 de fevereiro de 2017, compra uma subscrição. Em 12 de fevereiro de 2017, você adiciona uma licença. Sua data de faturação é 14 de fevereiro de 2017. No dia 11 de fevereiro de 2018 a sua subscrição renova.

A sua próxima data de faturação é 14 de março de 2017, e uma fatura e arquivo de reconciliação são gerados. O ficheiro de reconciliação conterá as seguintes linhas de faturação:

|Data de início do carregamento  |Data de fim de carga  |Tipo de carga  |Preço Unitário |Quantidade | Montante |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|11 de fevereiro de 2017 |10 de fevereiro de 2018 |Prorate de instância de ciclo |-211.20 |1 |-211.20 |
|11 de fevereiro de 2017 |11 de fevereiro de 2017 |Prorate de instância de ciclo |0.58 |1 |0.58 |
|12 de fevereiro de 2017 |10 de março de 2017 |Prorate de instância de ciclo |15.62 |2 |31.25 |
|11 de março de 2017 |10 de fevereiro de 2018 |Prorate de instância de ciclo |195.00 |2 |390.00 |

Em 11 de fevereiro de 2018 a subscrição renova por mais um período de 12 meses.

## <a name="change-license-quantity"></a>Alterar quantidade de licenças

A sua data de faturação é dia 15 de cada mês. No dia 13 de janeiro, você compra uma nova subscrição com uma licença por $4 por mês e seleciona faturação anual. O ficheiro de reconciliação baseado em licenças de 15 de janeiro conterá a seguinte linha de faturação:

|Data de início do carregamento |Data de fim de carga |Tipo de carga |Preço Unitário |Quantidade |Montante |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13 de janeiro de 2018|12 de janeiro de 2019|Taxas de prorate ao comprar|48.00|1|48.00

No dia 1 de fevereiro, aumenta a quantidade de licença de um para dois. O ficheiro de reconciliação baseado em licenças de 15 de fevereiro conterá as seguintes linhas de faturação:

|Data de início do carregamento |Data de fim de carga |Tipo de carga |Preço Unitário |Quantidade |Montante |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13 de janeiro de 2018|12 de janeiro de 2019|Prorate de instância de ciclo|-48.00|1|-48.00
13 de janeiro de 2018|31 de janeiro de 2018|Prorate de instância de ciclo|2.47|1|2.47
1 de fevereiro de 2018|12 de janeiro de 2019|Prorate de instância de ciclo|44.98|2|89.96

O preço anual é $48,00, o que equivale ao preço diário de $0,13 ($48,00 / 365).

Preço unitário = dias no período de serviço x preço diário x número de licenças.

São 19 dias de serviço de 13 de janeiro de 2018 a 31 de janeiro de 2018.

Assim, o preço unitário é $2,47 (19 x 0,13 x 1)

São 346 dias no período de serviço 1 de fevereiro de 2018 a 12 de janeiro de 2019.

Assim, o preço unitário é $44.98 (346 x 0,13 x 2)

## <a name="suspend-before-30-days"></a>Suspender antes de 30 dias

A sua data de faturação é dia 15 de cada mês. No dia 13 de janeiro, você compra uma nova subscrição com uma licença por $4 por mês, e seleciona faturação anual. O ficheiro de reconciliação baseado em licenças de 15 de janeiro conterá a seguinte linha de faturação:

|Data de início do carregamento |Data de fim de carga |Tipo de carga |Preço Unitário |Quantidade |Montante |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13 de janeiro de 2018|12 de janeiro de 2019|Taxas de prorate na compra|48.00|1|48.00

No dia 1 de fevereiro, suspende a sua assinatura. O ficheiro de reconciliação baseado em licença de 15 de fevereiro conterá a seguinte linha de faturação:

|Data de início do carregamento |Data de fim de carga |Tipo de carga |Preço Unitário |Quantidade |Montante |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13 de janeiro de 2018|12 de janeiro de 2019|Taxa de Cancelamento|-48.00|1|-48.00

## <a name="suspend-after-30-days"></a>Suspender após 30 dias

A sua data de faturação é dia 15 de cada mês. No dia 13 de janeiro, você compra uma nova subscrição com uma licença por $4/mês e seleciona faturação anual. O ficheiro de reconciliação baseado em licenças de 15 de janeiro conterá a seguinte linha de faturação:

|Data de início do carregamento |Data de fim de carga |Tipo de carga |Preço Unitário |Quantidade |Montante |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13 de janeiro de 2018|12 de janeiro de 2019|Taxas de prorate ao comprar|48.00|1|48.00

O ficheiro de reconciliação baseado em licenças de 15 de fevereiro não conterá quaisquer linhas de faturação para esta subscrição.
No dia 1 de março, suspende a sua assinatura. O ficheiro de reconciliação baseado na licença de 15 de março conterá a seguinte linha de faturação:

|Data de início do carregamento |Data de fim de carga |Tipo de carga |Preço Unitário |Quantidade |Montante |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1 de março de 2018|12 de janeiro de 2019|Taxa de Cancelamento|-41.34|1|-41.34

O preço anual é de $48,00, o que equivale ao preço diário de 0,13 (48,00 / 365).

Preço unitário = dias no período de serviço x preço diário x número de licenças.

São 318 dias no período de serviço 1 de março de 2018 a 12 de janeiro de 2019.

Assim, o preço unitário é de $41,34 (318 x 0,13 x 1). Porque isto é um crédito, o preço unitário é de $41,34.

## <a name="suspend-and-reactivate"></a>Suspender e reativar

A sua data de faturação é dia 15 de cada mês. No dia 13 de janeiro, você compra uma nova subscrição com uma licença por $4 por mês e seleciona faturação anual. O ficheiro de reconciliação baseado em licenças de 15 de janeiro conterá a seguinte linha de faturação:

|Data de início do carregamento |Data de fim de carga |Tipo de carga |Preço Unitário |Quantidade |Montante |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13 de janeiro de 2018|12 de janeiro de 2019|Taxas de prorate na compra|48.00|1|48.00

No dia 1 de fevereiro, suspende a sua assinatura. O ficheiro de reconciliação baseado em licença de 15 de fevereiro conterá a seguinte linha de faturação:

|Data de início do carregamento |Data de fim de carga |Tipo de carga |Preço Unitário |Quantidade |Montante |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13 de janeiro de 2018|12 de janeiro de 2019|Taxa de Cancelamento|-48.00|1|-48.00

No dia 1 de março, reativa a sua assinatura. O ficheiro de reconciliação baseado na licença de 15 de março conterá a seguinte linha de faturação:

|Data de início do carregamento |Data de fim de carga |Tipo de carga |Preço Unitário |Quantidade |Montante |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1 de março de 2018|12 de janeiro de 2019|Taxas de prorate na compra|41.34|1|41.34

O preço anual é de 48,00, o que equivale ao preço diário de 0,13 (48.00/365).

Preço unitário = dias no período de serviço x preço diário x número de licenças.

São 318 dias no período de serviço 1 de março de 2018 a 12 de janeiro de 2019.

Assim, o preço unitário é de $41,34 (318 x 0,13 x 1).

## <a name="multiyear-offers-with-annual-billing"></a>Ofertas plurianuais com faturação anual

Para ofertas plurianuais com faturação anual, os encargos começam na data de compra e continuam por um ano.

(No [exemplo da faturação plurianual](#example-of-multiyear-billing) que se segue, no primeiro ano as taxas começam em 20 de março de 2020, e terminam um ano depois, em 19 de março de 2021.)

Os encargos pelo segundo ano começam um mês antes da data limite de cobrança do primeiro ano.

(No exemplo, os encargos para o segundo ano começam em 20 de fevereiro de 2021, um mês antes da data de fim do primeiro ano de 19 de março de 2021.)

Este processo anual de faturação tem uma diferença de um mês entre a data de fim da subscrição e a data de fim da cobrança para o terceiro ano. No entanto, a subscrição permanece ativa até à data final da subscrição.

(No exemplo, a data de fim da subscrição de 19 de março de 2023 no terceiro ano é um mês após a data de fim da taxa de 19 de fevereiro de 2023.)

### <a name="example-of-multiyear-billing"></a>Exemplo de faturação plurianual

Para uma oferta de 36 meses comprada em 20 de março de 2020 mostrada nas tabelas que se seguem, o ficheiro de reconciliação seria:

#### <a name="first-year"></a>Primeiro ano

|Data de início da subscrição  |Data de fim da assinatura  |Data de início da carga  |Data de fim da carga  |Tipo de custo  |
|:-:|:-:|:-:|:-:|:-:|
|20 de março de 2020|19 de março de 2023|20 de março de 2020|19 de março de 2021|Taxas de prorate quando compradas|

#### <a name="second-year"></a>Segundo ano

|Data de início da subscrição  |Data de fim da assinatura  |Data de início da carga  |Data de fim da carga  |Tipo de custo  |
|:-:|:-:|:-:|:-:|:-:|
|20 de março de 2020|19 de março de 2023|20 de fevereiro de 2021|19 de fevereiro de 2022|Taxa de ciclo|

#### <a name="third-year"></a>Terceiro ano

|Data de início da subscrição  |Data de fim da assinatura  |Data de início da carga  |Data de fim da carga  |Tipo de custo  |
|:-:|:-:|:-:|:-:|:-:|
|20 de março de 2020|19 de março de 2023|20 de fevereiro de 2022|19 de fevereiro de 2023|Taxa de ciclo|
