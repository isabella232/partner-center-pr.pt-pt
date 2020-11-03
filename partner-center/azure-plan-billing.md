---
title: Faturação do plano Azure - fatura & arquivos de reconhecimento
ms.topic: article
ms.date: 07/02/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como aceder e compreender a estrutura de ficheiros de fatura e reconciliação relacionada com a faturação do plano Azure.
author: khpavan
ms.author: sakhanda
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 5d8bb85357d796ae4917faf91c93db8fef4369c2
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/22/2020
ms.locfileid: "92529828"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a>Nova experiência de comércio em CSP - Faturação Azure 

**Funções adequadas:**

- Agente administrativo
- Administrador de faturação
- Administrador global

A faturação ao abrigo do plano Azure é uma experiência de faturação simplificada usando uma data de faturação única alinhada e período de faturação de um mês de calendário.

## <a name="summary-of-billing-essentials"></a>Resumo do essencial da faturação

- **Data da fatura** : A fatura e o ficheiro de reconciliação estarão disponíveis no painel de instrumentos/API do Centro Parceiro até ao dia 8 (meia-noite UTC).

- **Período de faturação** : O período de faturação está alinhado com o mês civil, por exemplo, 10/1-10/31, 11/1-11/30.

- **Períodos de serviço de cobrança** : As taxas irão alinhar-se com o mês civil. Por exemplo, se o parceiro faturado adicionar serviços Azure através de um plano Azure em 10/15 e o cliente iniciar o consumo de serviços Azure em 10/15, então o parceiro faturado receberá fatura/reconhecimento em 11/8 para consumo de clientes para o período de serviço 10/15 - 10/31. A fatura do próximo mês que será gerada em 12/8 contém todos os encargos para o período de serviço 11/1- 11/31.

- **Prazo de pagamento da fatura:** Líquido 60 dias.

- **Moeda de fatura** : Os parceiros continuarão a ser faturados na moeda atribuída ao cliente. Por exemplo, se o parceiro faturado estiver na Irlanda com clientes no Reino Unido, Noruega e Alemanha, então o parceiro faturado receberá uma fatura/reconhecimento de EUROS.

- **Incentivos ao parceiro** : Pago 45 dias a partir do final do mês de fatura.

## <a name="access-your-invoices-and-reconciliation-files"></a>Aceda às suas faturas e ficheiros de reconciliação

O administrador global ou administrador de faturação da sua empresa receberá um e-mail quando uma fatura estiver pronta para ver.

Para aceder à fatura e ao ficheiro de reconciliação:

1. Inscreva-se no painel do Centro [de Parceiros.](https://partner.microsoft.com/dashboard/)

2. No menu Partner Center, selecione **Billing** .

3. Selecione o separador para o **Recorrente** e **uma vez** e a moeda em que está interessado.

   :::image type="content" source="images/azure/billing3.png" alt-text="faturação":::

4. Selecione o ficheiro **Fatura** ou **Reconciliação.**  

   Para ver faturas históricas e ficheiros de reconhecimento expande a linha de história de Billing abaixo.

## <a name="understanding-usage-data"></a>Compreender os dados de utilização 

1. O plano Azure é a raiz ou o recipiente de nível superior para utilização. Todo o uso está ligado a um único plano Azure.

2. Dentro de um plano, haverá uma ou mais subscrições da Azure. Estes são recipientes utilizados para a gestão e implantação de recursos. 

3. Dentro de uma subscrição, os grupos de recursos adicionam recursos de grupo. Todos os recursos são implantados num grupo de recursos. 

4. Exemplos de recursos incluem máquinas virtuais e contas de armazenamento. 

5. Contadores de recursos: Os contadores são medições de consumo de um recurso, e um recurso pode emitir uso para vários metros. Os contadores são identificados por um ProductId, SKUId e AvailabilityId. 

### <a name="hierarchy-of-subscription-resource-groups-and-metering"></a>Hierarquia dos grupos de recursos de subscrição e da medição

**Conta Azure (inquilino)**

- Assinatura A
    - Grupo de Recursos 1
        - Máquina virtual (recurso)
            - Contador de cálculo
        - Rede virtual (recurso)
            - Sem medidor de faturação

    - Grupo de Recursos 2
        - Máquina virtual (recurso)
            - Medidor de computador
        - Disco gerido por SSD premium (recurso)
            - Contador de capacidade de armazenamento
            - Contador de operações de armazenamento

- Assinatura B -ResourceGroup 1 - Azure SQL (recurso) - Medidor DTU - VPN Gateway (recurso) - Medidor de gateway VPN

    - Grupo de Recursos 2
        - Interface de rede virtual (recurso)
            - Sem medidor de faturação

## <a name="read-the-invoice"></a>Leia a fatura

1. A fatura estará disponível o mais tardar no oitavo de cada mês.

2. Os sócios têm 60 dias para pagar.

3. O período de faturação abrangerá um determinado mês civil, por exemplo, 10/1-10/31.

4. Os encargos são líquidos de ajustamentos (o montante é líquido de "Partner earned credit for services managed").

5. Reveja o ficheiro de reconhecimento de fatura e o ficheiro de utilização nominal diário para obter detalhes adicionais de faturação.

   :::image type="content" source="images/azure/invoice1.png" alt-text="faturação":::

## <a name="read-the-invoice-reconciliation-file"></a>Leia o ficheiro de reconciliação da fatura

1. Cada plano Azure e combinação de contadores podem ter até duas linhas de faturação no ficheiro de reconhecimento.

2. Se o contador se qualificar para qualquer tipo de desconto ou crédito (como descontos hierárquicos ou o Parceiro ganhou crédito pelos serviços geridos) durante todo o mês civil, então o ficheiro de reconhecimento conterá apenas uma linha de faturação. A coluna **PriceAdjusmentDescription** referenciará o desconto ou o crédito auferido.

3. Se não houver recursos para um determinado contador que se qualiou para desconto ou parceiro ganhou crédito, então o ficheiro de reconhecimento conterá apenas uma linha de faturação e o preço unitário efetivo será o preço de venda ao público (que é o preço unitário).

4. Se o contador, ou quaisquer recursos que emitem esse contador, se qualificasse para **Partner a ganhar crédito pelos serviços geridos** durante uma parte do mês, o ficheiro de reconhecimento conterá duas linhas de faturação. Uma linha representará os dias em que o contador se qualificou e a segunda linha representará os dias em que o contador não se qualificou.

## <a name="read-the-daily-usage-file"></a>Leia o ficheiro de utilização diária

- Os contadores de subscrição ao abrigo de um plano Azure são avaliados, e são acumulados, diariamente.

- **O parceiro que ganhou crédito pelos serviços geridos** é determinado e aplicado diariamente.

- Cada contador de assinaturas terá uma linha para cada dia do mês onde houve consumo.

- No exemplo abaixo:

  - O medidor qualificado para **Parceiro ganhou crédito por serviços geridos** de 7/1 - 7/3 (note que o preço unitário efetivo é o preço de venda a retalho menos parceiro ganho crédito.

  - A Meter não se qualificou para **o Partner a ganhar crédito pelos serviços geridos** de 7/4 - 7/7 (note que o preço unitário efetivo é o preço de venda ao público).

  - O medidor qualificado para **Partner ganhou crédito por serviços geridos** de 7/8 - 7/31 (note que o preço unitário efetivo é o preço de venda a retalho menos parceiro ganho crédito).

   :::image type="content" source="images/azure/pecfinal.png" alt-text="faturação":::

## <a name="invoice-in-customer-currency"></a>Fatura em moeda de cliente

Os serviços Azure através de um plano Azure serão avaliados em USD e faturados na moeda atribuída pelo país cliente. Se a moeda de faturação não for USD, então a taxa cambial (FX) utilizada será mostrada na última página da fatura. As tarifas FX são determinadas mensalmente e aplicadas à seguinte fatura. Para obter uma lista completa de moedas de país, por favor, veja o [novo comércio oferece disponibilidade do país e matriz de moeda de cliente.](https://go.microsoft.com/fwlink/?linkid=2112354)

A Microsoft usará a Thomson Reuters para determinar as taxas FX utilizadas para determinar a moeda de preços para a conversão de moeda de faturação. As tarifas de FX serão atualizadas e disponíveis na véspera do primeiro dia do mês para o qual se candidatam.

**Exemplo:** As taxas de utilização para o período de serviço de 1 de agosto a 31 de agosto serão faturadas através da taxa FX publicada a 31 de julho. Estes encargos aparecerão na fatura de setembro e a taxa FX será anotado na última página da fatura.

## <a name="azure-reservations"></a>Reservas do Azure


Se comprar [reservas do Azure](azure-reservations.md) através de um plano Azure, pode escolher faturação única ou mensal.


## <a name="azure-spending"></a>Despesas do Azure

A experiência de gastos azure existente é atualizada para apoiar a nova faturação do plano Azure no Partner Center. Isto permite que os parceiros:

- Ver, gerir e receber alertas de orçamento definidos ao nível do cliente 

- Ver os gastos totais estimados num plano Azure (discriminado pelo nível de recursos e contadores)

Uma vez que o modelo de faturação dos serviços Azure através de um plano Azure é o consumo pós-pagamento, para evitar uma fatura maior do que o previsto, os parceiros podem aplicar um orçamento mensal e acompanhar a percentagem de utilização. Um orçamento pode ser aplicado a um cliente ou a vários clientes de uma só vez. 

:::image type="content" source="images/azure/azurespend.png" alt-text="faturação":::

## <a name="next-steps"></a>Passos seguintes

- Veja como o parceiro obteve crédito (PEC) é calculado. Inscreva-se no [painel do](https://partner.microsoft.com/dashboard/) Partner Center e localize a lista de preços disponíveis.

- Conheça [a compra do plano Azure](purchase-azure-plan.md)

- Veja a [tabela de preços para a nova experiência de comércio na CSP](azure-plan-price-list.md)
