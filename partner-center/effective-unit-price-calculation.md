---
title: Cálculo efetivo do preço por unidade
ms.topic: how-to
ms.date: 09/27/2021
description: Saiba mais sobre o preço unitário eficaz e como é calculado. Este artigo também inclui um cálculo de amostra.
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 252ec080dcc7e521e1db74eb5bdd668d8cd081e7
ms.sourcegitcommit: d731813da1d31519dc2dc583d17899e5cf4ec1b2
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/27/2021
ms.locfileid: "129071505"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a>Cálculo efetivo dos preços unitários para o consumo do plano Azure

**Funções apropriadas**: Administrador de Faturação

## <a name="the-effective-unit-price"></a>O preço unitário efetivo

O preço unitário efetivo é calculado ao nível do contador (ao contrário do nível de recursos), e é ajustado diariamente de acordo com a utilização do contador.

Calculamos o preço unitário efetivo utilizando os seguintes três fatores:

- Consumo, que é monitorizado diariamente ao longo do ciclo de faturação
- Custo faturado para o contador
- Tiering (se aplicável)

Como monitorizamos o consumo diariamente ao longo do ciclo de faturação, o preço unitário efetivo vai oscilar. O preço final de um determinado ciclo de faturação estará disponível depois de pararmos o cálculo do consumo e fecharmos o período de faturação. Verá a maioria das mudanças no consumo após a quarta ou quinta casa decimal.

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a>Descubra se o seu contador utiliza preços hierárquicos

Se não sabe se o seu contador utiliza preços hierárquicos, use o procedimento abaixo para descobrir.

> [!NOTE]
> A interface de pré-visualização do Partner Center proporciona-lhe uma experiência de utilizador mais eficiente e produtiva através de espaços de trabalho agrupados logicamente. Para saber mais sobre a interface dos espaços de trabalho e como ligá-lo, consulte [Getting around Partner Center](get-around-partner-center.md#turn-workspaces-on-and-off).

#### <a name="workspaces-view"></a>[Vista de espaços de trabalho](#tab/workspaces-view)

1. Inicie sessão no [dashboard do Centro de Parceiros](https://partner.microsoft.com/dashboard/).

2. Selecione o **azulejo de preços** e, em seguida, selecione os preços do plano **Azure**.

3. Localize o seu medidor por ID e, em seguida, baixe os seus dados de preços.

#### <a name="current-view"></a>[Vista atual](#tab/current-view)

1. Inicie sessão no [dashboard do Centro de Parceiros](https://partner.microsoft.com/dashboard/).

2. Selecione **Vender,** **selecione Preços e ofertas**, e, em seguida, selecione **preços do plano Azure**.

3. Localize o seu medidor por ID e, em seguida, baixe os seus dados de preços.

* * *

## <a name="sample-calculation"></a>Cálculo da amostra

O quadro abaixo dá um exemplo de como calculamos o preço unitário efetivo durante o período aberto.

Na tabela, aplicam-se os seguintes valores: 

- **UP** = Preço unitário do recurso/hora = 0,868

- **BCU** = Unidade de consumo alusário para o contador

- **BC** = Custo billable para o medidor = BCU * UP * 0,85. Isto reflete um ajustamento para o desconto de 15% do PEC. Em seguida, usamos o limite inferior da função para limitar o valor a dois dígitos após o ponto decimal, de modo a cobrar o valor mínimo. 

- **Preço unitário efetivo** = BCU/BC

> [!NOTE]
> O medidor neste exemplo não tem níveis de preços ou outros descontos - os fatores de Preço Unitário Efetivo em percentagens de desconto e outros ajustes.

| Data | BCU (unidade de consumo a cobrar) | BC (custo de faturação) | Preço unitário eficaz |
| ------ | ----------- | ----------- | ----------- |  
| 3-ago | 29 | 21.39 | 0.737586206896552 |
| 10 ago | 210.950039 | 155.63 | 0.737757626107858 |
| 25 ago | 555.950039 | 410.17 | 0.737782122900436 |

## <a name="next-steps"></a>Passos seguintes

- [Faturação e impostos](billing.md)
