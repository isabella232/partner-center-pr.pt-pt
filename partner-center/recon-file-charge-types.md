---
title: Tipos de encargos de ficheiro de reconciliação
ms.topic: article
ms.date: 06/05/2020
description: Descubra os tipos de encargos (tais como, baseados em licenças, baseados em uso e uma vez), créditos e descontos em ficheiros de reconciliação do Partner Center.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: ba42ac5beb28a3cf819c54a86385fb79853cdcd0
ms.sourcegitcommit: 700150044ea4f1a0b96cb4caeb97d7197da29ef6
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/25/2021
ms.locfileid: "105549231"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a>Compreenda os diferentes tipos de carga nos ficheiros de reconciliação do Partner Center

**Aplica-se a**

- Centro de Parceiros para a nuvem do Governo da Microsoft

**Funções adequadas**

- Agente administrativo
- Administrador de faturação
- Administrador global

Este artigo descreve os mapeamentos entre uma secção de fatura e tipos de carga associados que podem estar no seu ficheiro de reconciliação. A sua fatura fornece um resumo das taxas. O seu ficheiro de reconciliação fornece uma desagregação detalhada das transações de item de linha, incluindo tipos de carga. Para obter mais informações sobre ficheiros de reconciliação, [consulte como utilizar ficheiros de reconciliação](use-the-reconciliation-files.md).

Tanto os [ficheiros de reconciliação baseados na utilização](usage-based-recon-files.md) como [os ficheiros de reconciliação baseados em licenças](license-based-recon-files.md) apenas mostram transações e encargos relacionados com o uso (unidades consumidas e encargos relacionados).

> [!NOTE]
> Créditos pontuais, descontos ou reembolsos que apareçam na fatura, uma vez que os **ajustes** não constam do ficheiro de reconciliação.

## <a name="map-charge-types-to-invoice-charges"></a>Tipos de carga de mapa para cobrar faturas

Para cruzar os valores de carga entre a sua fatura e o ficheiro de reconciliação, utilize as opções de filtro no Microsoft Excel. Filtrar por tipos de carga no seu ficheiro de reconciliação para mapear os encargos da fatura para um conjunto de avarias de carga no ficheiro de reconciliação.

## <a name="license-based-charges"></a>Encargos baseados em licença

Para mapear estes encargos baseados na licença para a sua fatura, em suma a coluna **Valor** a partir do ficheiro baseado em licença.

| Descrição da carga (coluna ChargeType no ficheiro de reconciliação) | Explicação de cobrança |
| ------------------------------------------------------------- | ------------------ |
| Taxa de ativação | O valor cobrado ao cliente quando utiliza a subscrição após a compra. |
| Taxa de cancelamento | Encargos procitados reembolsados ao cliente quando as licenças associadas são alteradas. |
| Cancelar caso prorate | Os encargos procitados cancelados quando o cliente com subscrição mensal tem subscrição suspensa e as licenças associadas alteradas no mesmo mês. |
| Taxa de ciclo | Encargos periódicos para uma subscrição. |
| Prorate de instância de ciclo | Encargos procitados avaliados pelo cliente quando as licenças associadas são alteradas. |
| Taxas de prorate quando cancela | Reembolso prostimado para parte não utilizada do serviço após cancelamento. |
| Taxas de prorate quando convertidas fora da oferta atual | Taxas prostimadas após a conversão da subscrição mensal atual para uma subscrição anual. |
| Taxas de prorate quando convertidas para uma nova oferta | Taxas prostimadas após converter uma subscrição mensal para uma nova subscrição anual. |
| Taxas de prorate na compra | O tipo de cobrança de uma subscrição quando se utiliza faturação mensal ou anual. |
| Taxa de prorate ao renovar | Taxas prostimadas após a renovação da subscrição. |
| Taxa de renovação | Cobrança pela renovação de uma subscrição |
| Taxas de prorate quando ativadas | Taxas prostimadas desde a ativação até ao final do período de faturação. |

## <a name="one-time-charges"></a>Encargos únicos

Para mapear estes encargos únicos para a sua fatura, em suma a coluna **Valor** a partir do ficheiro baseado na licença.

| Descrição da carga (coluna ChargeType no ficheiro de reconciliação) | Explicação de cobrança |
| ------------------------------------------------------------- | ------------------ |
| Novo | Usado quando uma nova compra é criada. |
| adicionarQuantity | Utilizado tanto no reembolso da compra original como na nova quantidade após um aumento. |
| removerQuantidade | Utilizado tanto no reembolso da compra original como na nova quantidade após uma diminuição. |
| Cancelar | Usado quando uma subscrição é cancelada. |
| Converter | Usado quando uma licença é atualizada, mas o número de licenças permanece inalterado. |

## <a name="usage-charges"></a>Custos de utilização

Para mapear estes custos de utilização na sua fatura, em suma a coluna **PretaxCharges** a partir do ficheiro baseado em utilização.

| Descrição da carga (coluna ChargeType no ficheiro de reconciliação) | Explicação de cobrança |
| ------------------------------------------------------------- | ------------------ |
| Avaliar a taxa de utilização ao cancelar | Taxa de utilização de acesso após cancelamento de uso não pago durante o período de faturação atual. |
| Avaliar a taxa de utilização do ciclo atual | Taxa de utilização de acesso para o período de faturação atual. |

### <a name="credits"></a>Créditos

Para mapear estes créditos na sua fatura:

- Em suma, o **TotalForCustomer** do ficheiro baseado na licença.
- Em suma, a coluna **PostTaxTotal** a partir do ficheiro baseado na utilização.

| Descrição da carga (coluna ChargeType no ficheiro de reconciliação) | Explicação de cobrança |
| ------------------------------------------------------------- | ------------------ |
| Compensar um item de linha | Reembolso parcial ou total a um item de linha, incluindo impostos. |

### <a name="usage-based-discounts"></a>Descontos baseados na utilização

Para mapear estes descontos baseados na sua fatura, em suma a coluna **PretaxCharges** a partir do ficheiro baseado em utilização.

| Descrição da carga (coluna ChargeType no ficheiro de reconciliação) | Explicação de cobrança |
| ------------------------------------------------------------- | ------------------ |
| Desconto de ativação | Desconto aplicado quando a subscrição é ativada. |
| Desconto de ciclo | Desconto aplicado em encargos periódicos. |
| Renovar desconto | Desconto aplicado quando a subscrição renovada. |
| Cancelar desconto | Encargos aplicados quando os descontos são cancelados. |

### <a name="license-based-discounts"></a>Descontos baseados em licenças

Para mapear descontos baseados em licenças na sua fatura, em suma a coluna **TotalOtherDiscount** a partir do ficheiro baseado na licença.

*Os descontos baseados na licença podem ser aplicados a vários tipos de carga.*
