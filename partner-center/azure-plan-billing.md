---
title: Faturação do plano Azure - fatura & arquivos de reconhecimento
ms.topic: article
ms.date: 09/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
description: Saiba como aceder e compreender a estrutura de ficheiros de fatura e reconciliação relacionada com a faturação do plano Azure.
author: khpavan
ms.author: sakhanda
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: ad04b7af67bb4cf664b2a552c94fc96fa25e5349
ms.sourcegitcommit: e1da62b36420d78bf44e3962358d0af65ebc3402
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/27/2021
ms.locfileid: "129089271"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a>Nova experiência comercial no CSP – faturação do Azure

**Funções adequadas**: Agente administrador | Administrador de faturação | Administrador global

Este artigo explica como aceder e compreender a estrutura de ficheiros de fatura e reconciliação relacionada com a faturação do plano Azure. A faturação ao abrigo do plano Azure é uma experiência de faturação simplificada usando uma data de faturação única alinhada e período de faturação de um mês de calendário.

## <a name="summary-of-billing-essentials"></a>Resumo do essencial da faturação

- **Data da fatura**: O ficheiro de fatura e reconciliação estará disponível no painel de instrumentos/API do Centro De Parceiros até ao dia 8 (meia-noite UTC).

- **Período de faturação**: O período de faturação está alinhado com o mês civil, por exemplo, 10/1-10/31, 11/1-11/30.

- **Períodos de serviço de cobrança**: As taxas alinhar-se-ão ao mês civil. Por exemplo, se o parceiro faturado adicionar serviços Azure através de um plano Azure em 10/15 e o cliente iniciar o consumo de serviços Azure em 10/15, então o parceiro faturado receberá fatura/reconhecimento em 11/8 para consumo de clientes para o período de serviço 10/15 - 10/31. A fatura do próximo mês que será gerada em 12/8 contém todos os encargos para o período de serviço 11/1- 11/31.

- **Prazo de pagamento da fatura:** Líquido 60 dias.

- **Moeda de fatura**: A partir de agosto de 2021, todos os parceiros serão faturados na moeda de localização do parceiro, independentemente da localização do cliente a quem vendeu o(s).

- **Incentivos ao parceiro**: Pago 45 dias a partir do final do mês de fatura.

## <a name="access-your-invoices-and-reconciliation-files"></a>Aceda às suas faturas e ficheiros de reconciliação

O administrador global ou administrador de faturação da sua empresa receberá um e-mail quando uma fatura estiver pronta para ver.

Para aceder à fatura e ao ficheiro de reconciliação:

> [!NOTE]
> Para saber mais sobre a interface de espaços de trabalho, consulte [o Centro de Parceiros.](get-around-partner-center.md#turn-workspaces-on-and-off)

#### <a name="workspaces-view"></a>[Vista de espaços de trabalho](#tab/workspaces-view)

1. A partir do [painel Partner Center,](https://partner.microsoft.com/dashboard/)selecione o azulejo **de Faturação.**

2. Selecione o separador para o **Recorrente** e **uma vez** e a moeda em que está interessado.

   :::image type="content" source="images/azure/billing-workspace-1.png" alt-text="Screenshot mostrando o histórico de faturação.":::

3. Selecione o ficheiro **Fatura** ou **Reconciliação**.

   Para ver faturas históricas e ficheiros de reconciliação, expanda a linha de história da Billing abaixo.

#### <a name="current-view"></a>[Vista atual](#tab/current-view)

1. A partir do [painel partner center](https://partner.microsoft.com/dashboard/), selecione **Billing**.

2. Selecione o separador para o **Recorrente** e **uma vez** e a moeda em que está interessado.

   :::image type="content" source="images/azure/billing3.png" alt-text="faturação.":::

3. Selecione o ficheiro **Fatura** ou **Reconciliação**.

   Para ver faturas históricas e ficheiros de reconciliação, expanda a linha de história da Billing abaixo.

* * *

## <a name="about-usage-data"></a>Sobre os dados de utilização

- O plano Azul é o recipiente de raiz ou de nível superior para utilização. Todo o uso está ligado a um único plano Azure.

- Dentro de um plano, haverá uma ou mais subscrições da Azure. Estes são recipientes utilizados para a gestão e implantação de recursos.

- Dentro de uma subscrição, os grupos de recursos adicionam recursos de grupo. Todos os recursos são implantados num grupo de recursos.

- Exemplos de recursos incluem máquinas virtuais e contas de armazenamento.

- Contadores de recursos: Os contadores são medições de consumo de um recurso, e um recurso pode emitir uso para vários metros. Os contadores são identificados por um ProductId, SKUId e AvailabilityId.

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
        - Premium Disco gerido por SSD (recurso)
            - contador de capacidade Armazenamento
            - contador de operações Armazenamento

- Assinatura B -Grupo de Recursos 1 - Azure SQL (recurso) - Medidor DTU - VPN Gateway (recurso) - Medidor de gateway VPN

    - Grupo de Recursos 2
        - Interface de rede virtual (recurso)
            - Sem medidor de faturação

## <a name="about-your-invoice"></a>Sobre a sua fatura

- A fatura estará disponível o mais tardar no oitavo de cada mês.

- Os sócios têm 60 dias para pagar.

- O período de faturação abrangerá um determinado mês civil, por exemplo, 10/1-10/31.

- Os encargos são líquidos de ajustamentos (o montante é líquido de "Parceiro auferido crédito pelos serviços geridos").

- Reveja o ficheiro de reconhecimento de fatura e o ficheiro de utilização nominal diário para obter detalhes adicionais de faturação.

   :::image type="content" source="images/azure/invoice1.png" alt-text="fatura.":::

## <a name="about-your-invoice-reconciliation-file"></a>Sobre o seu arquivo de reconciliação de fatura

- Cada plano Azure e combinação de contadores podem ter até duas linhas de faturação no ficheiro de reconciliação (recon).

- Se o contador se qualificar para qualquer tipo de desconto ou crédito (como descontos hierárquicos ou o Parceiro ganhou crédito pelos serviços geridos) durante todo o mês civil, então o ficheiro de reconhecimento conterá apenas uma linha de faturação. A coluna **PriceAdjusmentDescription** referenciará o desconto ou o crédito auferido.

- Se não houver recursos para um determinado contador que se qualiou para desconto ou parceiro ganhou crédito, então o ficheiro de reconhecimento conterá apenas uma linha de faturação e o preço unitário efetivo será o preço de venda ao público (que é o preço unitário).

- Se o contador, ou quaisquer recursos que emitem esse contador, se qualificassem para **Partner a ganhar crédito pelos serviços geridos** durante uma parte do mês, o ficheiro de reconhecimento conterá duas linhas de faturação. Uma linha representará os dias em que o contador se qualificou e a segunda linha representará os dias em que o contador não se qualificou.

> [!NOTE]
> Pode conciliar o seu consumo de Azure no seu ficheiro de reconhecimento de compra única. Para isso, vá ao seu arquivo de reconhecimento de uso diário e procure o seu SubscriçãoID. Isto mostrará todos os custos associados ao seu ID do plano Azure. O seu Azure SubscriptionID é apresentado como o EntitlementID.

## <a name="read-the-daily-usage-file"></a>Leia o ficheiro de utilização diária

- Os contadores de subscrição ao abrigo de um plano Azure são avaliados e são acumulados diariamente.

- **O parceiro que ganhou crédito pelos serviços geridos** é determinado e aplicado diariamente.

- Cada contador de assinaturas terá uma linha para cada dia do mês onde houve consumo.

- No exemplo abaixo:

  - O medidor qualificado para **Parceiro ganhou crédito por serviços geridos** de 7/1 - 7/3 (note que o preço unitário efetivo é o preço de venda a retalho menos parceiro ganho crédito.

  - A Meter não se qualificou para **o Partner a ganhar crédito pelos serviços geridos** de 7/4 - 7/7 (note que o preço unitário efetivo é o preço de venda ao público).

  - O medidor qualificado para **Parceiro ganhou crédito por serviços geridos** de 7/8 - 7/31 (note que o preço unitário efetivo é o preço de venda a retalho menos parceiro ganho crédito).

   :::image type="content" source="images/azure/pecfinal.png" alt-text="recon2.":::

## <a name="invoice-in-partner-location-currency"></a>Fatura na moeda de localização do parceiro

Os serviços Azure através de um plano Azure serão avaliados em USD e faturados na moeda atribuída pelo país parceiro. Se a moeda de faturação não for USD, então a taxa cambial (FX) utilizada será mostrada na última página da fatura. As tarifas FX são determinadas mensalmente e aplicadas à seguinte fatura. Para obter uma lista completa das moedas do país, por favor, veja o [novo comércio oferece disponibilidade de país e matriz de moeda parceira.](https://go.microsoft.com/fwlink/?linkid=2112354)

A Microsoft aplica uma taxa de câmbio pré-determinada para basear os preços de USD para chegar aos custos totais incorridos pelos serviços Azure comprados ou consumidos todos os meses. A taxa de câmbio mensal é a taxa média publicada pela Thomson Reuters (tipicamente) dois dias úteis antes do final do mês anterior às 16:00 GMT.

**Por exemplo,** A taxa de câmbio de dezembro da Microsoft seria a taxa média da Thomson Reuters em 29 de novembro ou por volta de 29 de novembro para uma determinada moeda. Essa taxa será aplicada a todas as compras nessa moeda de 1 de dezembro a 31 de dezembro.

## <a name="azure-reservations"></a>Reservas do Azure

Se comprar [reservas do Azure](azure-reservations.md) através de um plano Azure, pode escolher faturação única ou mensal.

## <a name="azure-spending"></a>Despesas do Azure

A experiência de gastos azure existente é atualizada para apoiar a nova faturação do plano Azure no Partner Center. Isto permite que os parceiros:

- Ver, gerir e receber alertas de orçamento definidos ao nível do cliente

- Ver os gastos totais estimados num plano Azure (discriminado pelo nível de recursos e contadores)

Uma vez que o modelo de faturação dos serviços Azure através de um plano Azure é o consumo pós-pagamento, para evitar uma fatura maior do que o previsto, os parceiros podem aplicar um orçamento mensal e acompanhar a percentagem de utilização. Um orçamento pode ser aplicado a um cliente ou a vários clientes de uma só vez.

:::image type="content" source="images/azure/azurespend.png" alt-text="Gastos azure.":::

## <a name="next-steps"></a>Passos seguintes

- Veja como o parceiro obteve crédito (PEC) é calculado. Inscreva-se no painel de [instrumentos](https://partner.microsoft.com/dashboard/) do Partner Center e selecione o azulejo **de preços** para encontrar listas de preços disponíveis.

- Conheça [a compra do plano Azure](purchase-azure-plan.md)

- Veja a [tabela de preços para a nova experiência de comércio na CSP](azure-plan-price-list.md)
