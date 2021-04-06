---
title: Faturação para compras recorrentes de & única
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Amostras de faturação do Partner Center para uma única vez e selecione compras recorrentes - quando compra subscrições, adiciona mais subscrições, adiciona ou remove licenças.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 329675e10205755819a19710976073d22f73eb58
ms.sourcegitcommit: 3d7d5064c5e021079ed7e6f93f03869cbf425a32
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/06/2021
ms.locfileid: "106502536"
---
# <a name="partner-center-billing-scenarios-for-one-time-and-select-recurring-purchases"></a>Cenários de faturação do Partner Center para uma única vez e selecione compras recorrentes

**Funções adequadas**

- Agente administrativo
- Administrador de faturação
- Agente helpdesk
- Agente comercial

Estes são [cenários comuns de faturação.](common-billing-scenarios.md) 

## <a name="purchase-a-subscription-and-add-a-license-on-the-same-day"></a>Compre uma subscrição e adicione uma licença no mesmo dia

No Cenário 1, você compra uma subscrição no dia 11 de junho a um preço unitário de $4. Mais tarde, nesse mesmo dia, comprou outra da mesma subscrição pelo mesmo preço.

O ficheiro de reconhecimento incluirá o seguinte:

- Nota de $4 para o período de serviço de 10 de junho a 9 de julho.
- $-4,00 provalorizado rebill para o período de serviço 11 de junho a 11 de junho. Este é o período em que se tem licença. Cálculo = (preço mensal/dia total no período de serviço) x dias no período de serviço provalorizado x número de licenças = (4/30) x 30 x 1 = 4,00.
- $8,00 provalorizado rebill para o período de serviço de 10 de junho a 9 de julho. Este é o período em que tinha duas licenças. Cálculo = (4/30) x 30 x 2 = 8,00.

|**Data de compra**   |**Início da carga** |**Fim da carga**  |**Preço unitário**  |**Quantidade**  |**Montante** |**Tipo de custo** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|6/11/2019      |6/10/2019   |7/09/2019         |$4                |1                 |$4            |Novo         |
|6/11/2019     | 6/10/2019    |7/09/2019        |$4        |1        | -$4       |adicionarQuantity           |
|6/11/2019     | 6/10/2019    |7/09/2019        |$4        | 2      |$8         |adicionarQuantity           |

## <a name="purchase-a-subscription-and-add-more-subscriptions-later"></a>Compre uma subscrição e adicione mais subscrições mais tarde

No Cenário 2, você compra uma subscrição no dia 11 de junho a um preço unitário de $4, e no dia 12 de junho você compra outra subscrição para o mesmo produto ao mesmo preço.

O ficheiro de reconhecimento incluirá o seguinte:

- Nota de $4 para o período de serviço de 10 de junho a 9 de julho.
- $-3,87 provalorizado rebill para o período de serviço de 11 de junho a 12 de junho. Este é o período em que se tem uma licença. Cálculo = (preço mensal/dia total no período de serviço) x dias no período de serviço provalorizado x número de licenças = (4/30) x 29 x 1 = 3,87.
- $7,74 provalorizado rebill para o período de serviço de 12 de junho a 9 de julho. Este é o período em que tinha duas licenças. Cálculo = (4/30) x 29 x 2 = 7,74.

|**Data de compra**   |**Início da carga** |**Fim da carga**  |**Preço unitário**  |**Quantidade**  |**Montante** |**Tipo de custo** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|6/11/2019 (tem uma licença)     |6/10/2019   |7/09/2019         |$4         |1        |$4            |Novo         |
|6/12/2019     | 6/10/2019    |7/09/2019        |$4        |1        | -$3,87       |adicionarQuantity           |
|6/12/2019     | 6/10/2019    |7/09/2019        |$4        | 2      |$7,74       |adicionarQuantity           |

## <a name="purchase-a-subscription-and-remove-a-license-on-the-same-day"></a>Compre uma subscrição e remova uma licença no mesmo dia

No Cenário 3, compra duas subscrições para o mesmo produto no dia 11 de junho a um preço unitário de $4. Mais tarde, nesse mesmo dia, retiras uma das licenças.  

O ficheiro de reconhecimento incluirá o seguinte:

- Nota de 8 dólares por duas licenças para o período de serviço de 10 de junho a 9 de julho.
- $-8,00 provalorizado rebill para o período de serviço 11 de junho a 11 de junho. Este é o período em que tinha duas licenças. Cálculo = (preço mensal/dia total no período de serviço) x dias no período de serviço provalorizado x número de licenças = (4/30) x 30 x 2 = 8,00.
- $4,00 provalorizado rebill para o período de serviço de 11 de junho a 9 de julho. Este é o período em que se tem uma licença. Cálculo = (4/30) x 30 x 1 = 4,00.

|**Data de compra**   |**Início da carga** |**Fim da carga**  |**Preço unitário**  |**Quantidade**  |**Montante** |**Tipo de custo** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|6/11/2019      |6/10/2019   |7/09/2019         |$4                |2                 |$8            |Novo         |
|6/11/2019     | 6/10/2019    |7/09/2019        |$4        |2        | -$8       |removerQuantidade           |
|6/11/2019     | 6/10/2019    |7/09/2019        |$4        | 1      |$4         |removerQuantidade           |

## <a name="purchase-a-subscription-and-remove-licenses-later"></a>Compre uma subscrição e retire licenças mais tarde

No cenário 4, compra duas subscrições no dia 11 de junho a um preço unitário de 4 dólares, e no dia 12 de junho retira uma das licenças.

O ficheiro de reconhecimento incluirá o seguinte:

- Nota de 8 dólares para o período de serviço de 10 de junho a 9 de julho.
- $-7,74 provalorizado rebill para o período de serviço de 11 de junho a 12 de junho. Este é o período em que tinha duas licenças. Cálculo = (preço mensal/dia total no período de serviço) x dias no período de serviço provalorizado x número de licenças = (4/30) x 29 x 2 = 7,74.
- $3,87 provalorizado rebill para o período de serviço de 12 de junho a 9 de julho. Este é o período em que se tem uma licença. Cálculo = (4/30) x 29 x 1 = 3,87.

|**Data de compra**   |**Início da carga** |**Fim da carga**  |**Preço unitário**  |**Quantidade**  |**Montante** |**Tipo de custo** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|6/11/2019 (tem duas licenças)     |6/10/2019   |7/09/2019         |$4         |2        |$8       |Novo       |
|6/12/2019     | 6/10/2019    |7/09/2019        |$4        |2        | -$7,74       |removerQuantidade           |
|6/12/2019 (tem uma licença)    | 6/10/2019    |7/09/2019   |$4    |1      |$3,87    |removerQuantidade |

## <a name="next-steps"></a>Passos seguintes

- [Experimente cenários de faturação mensal para novas subscrições, alteração dos valores das licenças ou suspensões](common-billing-scenarios-monthly.md)