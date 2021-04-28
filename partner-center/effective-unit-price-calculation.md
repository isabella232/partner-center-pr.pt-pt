---
title: Cálculo efetivo do preço por unidade
ms.topic: how-to
ms.date: 04/02/2021
description: Saiba mais sobre o preço unitário eficaz e como é calculado. Este artigo também inclui um cálculo de amostra.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1473b3c0b90cca1152b4dab0b8efec86dbc3d22d
ms.sourcegitcommit: f8fd51e1acdbfafdde86d6490bade66c63033ebd
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/28/2021
ms.locfileid: "108172222"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a>Cálculo efetivo dos preços unitários para o consumo do plano Azure

**Funções adequadas**

- Administrador de faturação

## <a name="the-effective-unit-price"></a>O preço unitário efetivo

O preço unitário efetivo é calculado ao nível do contador (ao contrário do nível de recursos), e é ajustado diariamente de acordo com a utilização do medidor.

Calculamos o preço unitário efetivo utilizando os seguintes três fatores:

- Consumo, que é monitorizado diariamente ao longo do ciclo de faturação
- Custo faturado para o contador
- Tiering (se aplicável)

Como monitorizamos o consumo diariamente ao longo do ciclo de faturação, o preço unitário efetivo irá oscilar. O preço final de um determinado ciclo de faturação estará disponível depois de pararmos o cálculo do consumo e fecharmos o período de faturação. Verá a maioria das mudanças no consumo após a quarta ou quinta decimal.

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a>Descubra se o seu contador utiliza preços hierárquicos

Se não sabe se o seu contador utiliza preços hierárquicos, use o procedimento abaixo para saber. 

1. Inicie sessão no [dashboard do Centro de Parceiros](https://partner.microsoft.com/dashboard/).
2. Selecione **Vender,** **selecione Preços e ofertas**, e, em seguida, selecione **preços do plano Azure**.
3. Localize o seu medidor por ID e, em seguida, descarregue os seus dados de preços. 

## <a name="sample-calculation"></a>Cálculo da amostra

O quadro abaixo dá um exemplo de como calculamos o preço unitário efetivo durante o período aberto.

Na tabela, aplicam-se os seguintes valores: 

- **UP** = Preço unitário do recurso/hora = 0,868

- **BCU** = Unidade de consumo alusário para o contador

- **BC** = Custo billable para o medidor = BCU * UP * 0,85. Isto reflete um ajustamento para o desconto de 15% do PEC. Em seguida, usamos o limite inferior da função para limitar o valor a dois dígitos após o ponto decimal, de modo a cobrar o valor mínimo. 

- **Preço unitário efetivo** = BCU/BC

>[!NOTE]

>Nota: O medidor neste exemplo não tem níveis de preços ou outros descontos — os fatores de Preço Unitário Efetivo em percentagens de desconto e outros ajustes.


| Data | BCU (unidade de consumo a cobrar) | BC (Custo faturado) | Preço unitário eficaz |
| ------ | ----------- | ----------- | ----------- |  
| 3-Ago | 29 | 21.39 | 0.737586206896552 |
| 10 ago | 210.950039 | 155.63 | 0.737757626107858 |
| 25 ago | 555.950039 | 410.17 | 0.737782122900436 |

## <a name="next-steps"></a>Passos seguintes

- [Faturação e impostos](billing.md)
