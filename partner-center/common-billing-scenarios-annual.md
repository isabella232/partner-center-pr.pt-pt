---
title: Faturação anual - cenários comuns
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
description: Partner Center faturação anual - quando adicionar novas subscrições, adicionar licenças antes da data de faturação, alterar a quantidade de licença ou suspender/reativar subscrições.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 9cf6ddd8ed73fcd9a7ee20a180072ad51cc5b7c4
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/09/2021
ms.locfileid: "123960039"
---
# <a name="common-annual-billing-scenarios-in-partner-center"></a>Cenários comuns de faturação anual no Centro de Parceiros

**Funções adequadas**: Agente administrador | Administrador de faturação | Agente helpdesk | Agente comercial

Estes [cenários de faturação comuns](common-billing-scenarios.md) são aplicáveis se utilizar a faturação anual no Partner Center.

## <a name="new-annual-subscription"></a>Nova subscrição anual

A sua data de faturação é dia 15 de cada mês. No dia 13 de janeiro, você compra uma nova subscrição com uma licença por $4/mês e seleciona faturação anual. O ficheiro de reconciliação baseado na licença de 15 de janeiro conterá a seguinte linha de faturação:

|Data de início do carregamento |Data de Fim de Carga |Tipo de carga |Preço Unitário |Quantidade |Montante |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Taxas de prorate na compra|48.00|1|48.00

## <a name="add-license-after-subscription-anniversary-date-but-before-billing-date"></a>Adicionar licença após data de aniversário de subscrição, mas antes da data de faturação

Você compra uma nova subscrição em 2/11/17 com uma licença por $211,20/ano. O seu aniversário de subscrição está definido como o dia 11 de cada mês. O sistema de faturação da Microsoft cria as seguintes linhas de faturação:

- Taxa de $211,20 para o período 2/11/17 – 2/10/18.

No dia 2/12/17, compra uma segunda licença. A sua data de faturação é 2/14/17. Uma fatura e um ficheiro de reconciliação são gerados. O ficheiro de reconciliação conterá as seguintes linhas de faturação:

|Data de início do carregamento  |Data de Fim de Carga  |Tipo de carga  |Preço Unitário |Quantidade | Montante |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|2/11/2017 |2/10/2018 |Taxas de prorate ao comprar |211.20 |1 | 211.20 |

No seu aniversário de subscrição, 3/11/17, o sistema de faturação da Microsoft cria as seguintes linhas de faturação para o aumento da licença em 2/12/17:

- Crédito de $211,20 para o período 2/11/17 – 2/10/18.
- $0,58 taxa procorrida por licença por uma licença para o período 2/11/17 – 2/11/17.
- $15,62 taxa por licença para duas licenças para o período 2/12/17 – 3/10/2017.
- $195,00 de cobrança por licença por duas licenças para o período 3/11/2017 – 2/10/2018.

No dia 2/11/17, compra uma subscrição. No dia 2/12/17, adiciona-se uma licença. A sua data de faturação é 2/14/17. Em 2/11/18 a sua subscrição renova.

A sua próxima data de faturação é 3/14/17, e uma fatura e arquivo de reconciliação são gerados. O ficheiro de reconciliação conterá as seguintes linhas de faturação:

|Data de início do carregamento  |Data de Fim de Carga  |Tipo de carga  |Preço Unitário |Quantidade | Montante |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|2/11/2017 |2/10/2018 |Prorate de instância de ciclo |-211.20 |1 |-211.20 |
|2/11/2017 |2/11/2017 |Prorate de instância de ciclo |0.58 |1 |0.58 |
|2/12/2017 |3/10/2017 |Prorate de instância de ciclo |15.62 |2 |31.25 |
|3/11/2017 |2/10/2018 |Prorate de instância de ciclo |195.00 |2 |390.00 |

Em 2/11/18 a subscrição renova por mais 12 meses de mandato.

## <a name="change-license-quantity"></a>Alterar quantidade de licenças

A sua data de faturação é dia 15 de cada mês. No dia 13 de janeiro, você compra uma nova subscrição com uma licença por $4/mês e seleciona faturação anual. O ficheiro de reconciliação baseado na licença de 15 de janeiro conterá a seguinte linha de faturação:

|Data de início do carregamento |Data de Fim de Carga |Tipo de carga |Preço Unitário |Quantidade |Montante |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Taxas de prorate na compra|48.00|1|48.00

No dia 1 de fevereiro, aumenta a quantidade de licença de um para dois. O ficheiro de reconciliação baseado em licenças de 15 de fevereiro conterá as seguintes linhas de faturação:

|Data de início do carregamento |Data de Fim de Carga |Tipo de carga |Preço Unitário |Quantidade |Montante |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Prorate de instância de ciclo|-48.00|1|-48.00
1/13/2018|1/31/2018|Prorate de instância de ciclo|2.47|1|2.47
01/02/2018|1/12/2019|Prorate de instância de ciclo|44.98|2|89.96

O preço anual é de 48,00, o que equivale ao preço diário de 0,13 (48.00/365).

Preço unitário = dias no período de serviço x preço diário x número de licenças.

São 19 dias no período de serviço 1/13/2018 – 1/31/2018.

Portanto, preço unitário = 2,47 (19x0.13x1)

São 346 dias no período de serviço 2/1/2018 – 1/12/2019.

Portanto, preço unitário = 44,98 (346x0.13x2)

## <a name="suspend-before-30-days"></a>Suspender antes de 30 dias

A sua data de faturação é dia 15 de cada mês. No dia 13 de janeiro, você compra uma nova subscrição com uma licença por $4/mês e seleciona faturação anual. O ficheiro de reconciliação baseado na licença de 15 de janeiro conterá a seguinte linha de faturação:

|Data de início do carregamento |Data de Fim de Carga |Tipo de carga |Preço Unitário |Quantidade |Montante |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Taxas de prorate na compra|48.00|1|48.00

No dia 1 de fevereiro, suspende a sua assinatura. O ficheiro de reconciliação baseado na licença de 15 de fevereiro conterá a seguinte linha de faturação:

|Data de início do carregamento |Data de Fim de Carga |Tipo de carga |Preço Unitário |Quantidade |Montante |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Taxa de Cancelamento|-48.00|1|-48.00

## <a name="suspend-after-30-days"></a>Suspender após 30 dias

A sua data de faturação é dia 15 de cada mês. No dia 13 de janeiro, você compra uma nova subscrição com uma licença por $4/mês e seleciona faturação anual. O ficheiro de reconciliação baseado na licença de 15 de janeiro conterá a seguinte linha de faturação:

|Data de início do carregamento |Data de Fim de Carga |Tipo de carga |Preço Unitário |Quantidade |Montante |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Taxas de prorate na compra|48.00|1|48.00

O ficheiro de reconciliação baseado em licenças de 15 de fevereiro não conterá quaisquer linhas de faturação para esta subscrição.
No dia 1 de março, suspende a sua assinatura. O ficheiro de reconciliação baseado na licença de 15 de março conterá a seguinte linha de faturação:

|Data de início do carregamento |Data de Fim de Carga |Tipo de carga |Preço Unitário |Quantidade |Montante |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
3/1/2018|1/12/2019|Taxa de Cancelamento|-41.34|1|-41.34

O preço anual é de 48,00, o que equivale ao preço diário de 0,13 (48.00/365).

Preço unitário = dias no período de serviço x preço diário x número de licenças.

São 318 dias no período de serviço 3/1/2018 – 1/12/2019.

Portanto, preço unitário = 41,34 (318x0.13x1). Porque este é um crédito o preço unitário é -41.34.

## <a name="suspend-and-reactivate"></a>Suspender e reativar

A sua data de faturação é dia 15 de cada mês. No dia 13 de janeiro, você compra uma nova subscrição com uma licença por $4/mês e seleciona faturação anual. O ficheiro de reconciliação baseado na licença de 15 de janeiro conterá a seguinte linha de faturação:

|Data de início do carregamento |Data de Fim de Carga |Tipo de carga |Preço Unitário |Quantidade |Montante |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Taxas de prorate na compra|48.00|1|48.00

No dia 1 de fevereiro, suspende a sua assinatura. O ficheiro de reconciliação baseado na licença de 15 de fevereiro conterá a seguinte linha de faturação:

|Data de início do carregamento |Data de Fim de Carga |Tipo de carga |Preço Unitário |Quantidade |Montante |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Taxa de Cancelamento|-48.00|1|-48.00

No dia 1 de março, reativa a sua assinatura. O ficheiro de reconciliação baseado na licença de 15 de março conterá a seguinte linha de faturação:

|Data de início do carregamento |Data de Fim de Carga |Tipo de carga |Preço Unitário |Quantidade |Montante |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
3/1/2018|1/12/2019|Taxas de prorate na compra|41.34|1|41.34

O preço anual é de 48,00, o que equivale ao preço diário de 0,13 (48.00/365).

Preço unitário = dias no período de serviço x preço diário x número de licenças.

São 318 dias no período de serviço 3/1/2018 – 1/12/2019.

Portanto, preço unitário = 41,34 (318x0.13x1).
