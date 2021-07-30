---
title: Cenários comuns de faturação mensal
ms.topic: article
ms.date: 05/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
description: Cenários comuns no Partner Center quando utiliza faturação mensal - inclui a adição de novas subscrições, alteração da quantidade de licença e suspensão de subscrições.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: dad132f9ad749076dc52a45f1ce77f23839e8671
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/29/2021
ms.locfileid: "114840710"
---
# <a name="sample-monthly-billing-scenarios-for-new-subscriptions-changing-license-amounts-or-suspensions"></a>Experimente cenários de faturação mensal para novas subscrições, alteração dos valores das licenças ou suspensões

**Funções adequadas**: Agente administrador | Administrador de faturação | Agente helpdesk | Agente comercial

Estes [cenários de faturação comuns](common-billing-scenarios.md) são aplicáveis se utilizar a faturação mensal no Partner Center.

## <a name="new-monthly-subscription"></a>Nova subscrição mensal

A sua data de faturação é dia 15 de cada mês. No dia 13 de janeiro, você compra uma nova subscrição com uma licença por $4/mês e seleciona faturação mensal. O ficheiro de reconciliação baseado na licença de 15 de janeiro conterá as seguintes linhas de faturação:

|Data de início do carregamento |Data de Fim de Carga |Tipo de carga |Preço Unitário |Quantidade |Montante |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |2/12/2018    |Taxa de ciclo   |4.00       |1        |4.00 |

O ficheiro de reconciliação baseado na licença de 15 de fevereiro conterá a seguinte linha de faturação:

|Data de início do carregamento |Data de Fim de Carga |Tipo de carga |Preço Unitário |Quantidade |Montante |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|2/13/2018         |3/12/2018    |Taxa de ciclo   |4.00       |1        |4.00 |

## <a name="change-license-quantity"></a>Alterar quantidade de licenças

A sua data de faturação é dia 15 de cada mês. No dia 13 de janeiro, você compra uma nova subscrição com uma licença por $4/mês e seleciona faturação mensal. O ficheiro de reconciliação baseado na licença de 15 de janeiro conterá as seguintes linhas de faturação:

|Data de início do carregamento |Data de Fim de Carga |Tipo de carga |Preço Unitário |Quantidade |Montante |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |2/12/2018    |Taxa de ciclo   |4.00       |1        |4.00    |

No dia 1 de fevereiro, aumenta a quantidade de licença de um para dois. O ficheiro de reconciliação baseado em licenças de 15 de fevereiro conterá as seguintes linhas de faturação:

|Data de início do carregamento |Data de Fim de Carga |Tipo de carga |Preço Unitário |Quantidade |Montante |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
| 1/13/2018        |2/12/2018    |Prorate de instância de ciclo   |-4.00       |1        |-4.00   |
|1/13/2018         |1/31/2018    | Prorate de instância de ciclo   |2.45       |1        |2.45    |
|01/02/2018         |2/12/2018    | Prorate de instância de ciclo   |1,55       |2        |3.10    |
|2/13/2018         |3/12/2018    | Prorate de instância de ciclo   |4.00       |2        |8.00    |

O preço mensal é de 4,00 e há 31 dias no período de serviço 1/13/2018 – 2/12/2018. Isto equivale a um preço diário de 0.129 (4/31).

São 19 dias no período de proseção 1/13/2018 – 1/31/2018.

Preço unitário de proção = 2.451 = 19 x 0,129

São 12 dias no período de proseção 2/1/2018 – 2/12/2018.

Preço unitário de proção = 1,54 = 12 x 0,129

## <a name="suspend-before-30-days"></a>Suspender antes de 30 dias

A sua data de faturação é dia 15 de cada mês. No dia 13 de janeiro, você compra uma nova subscrição com uma licença por $4/mês e seleciona faturação mensal. O ficheiro de reconciliação baseado na licença de 15 de janeiro conterá as seguintes linhas de faturação:

|Data de início do carregamento |Data de Fim de Carga |Tipo de carga |Preço Unitário |Quantidade |Montante |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |2/12/2018    |Taxa de ciclo   |4.00       |1        |4.00    |

No dia 1 de fevereiro, suspende-se uma assinatura. O ficheiro de reconciliação baseado na licença de 15 de fevereiro conterá a seguinte linha de faturação:

|Data de início do carregamento |Data de Fim de Carga |Tipo de carga |Preço Unitário |Quantidade |Montante |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|2/12/2018|Taxa de Cancelamento|-4.00|1|-4.00

## <a name="suspend-after-30-days"></a>Suspender após 30 dias

A sua data de faturação é dia 15 de cada mês. No dia 13 de janeiro, você compra uma nova subscrição com uma licença por $4/mês e seleciona faturação mensal. O ficheiro de reconciliação baseado na licença de 15 de janeiro conterá as seguintes linhas de faturação:

|Data de início do carregamento |Data de Fim de Carga |Tipo de carga |Preço Unitário |Quantidade |Montante |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|2/12/2018|Taxa de ciclo|4.00|1|4.00

O ficheiro de reconciliação baseado na licença de 15 de fevereiro conterá a seguinte linha de faturação:

|Data de início do carregamento |Data de Fim de Carga |Tipo de carga |Preço Unitário |Quantidade |Montante |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
2/13/2018|3/12/2018|Taxa de ciclo|4.00|1|4.00

No dia 1 de março, suspende a subscrição. O ficheiro de reconciliação baseado na licença de 15 de março conterá a seguinte linha de faturação:

|Data de início do carregamento |Data de Fim de Carga |Tipo de carga |Preço Unitário |Quantidade |Montante |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
3/1/2018|3/12/2018|Taxa de Cancelamento|-1.72|1|-1.72

O preço mensal é de 4,00 e há 28 dias no período de serviço 2/13/2018 – 3/12/2018. Isto equivale a um preço diário de 0.143 (4/28).

Preço unitário = dias no período de serviço x preço diário x número de licenças.

São 12 dias no período de cancelamento 3/1/2018 – 3/12/2018.

Portanto, o preço unitário = -1.716 (12 x 0,143 x (-1)).

## <a name="next-steps"></a>Passos seguintes

- [Cenários de faturação para uma única vez e selecione compras recorrentes](common-billing-scenarios-onetime-recurring.md)