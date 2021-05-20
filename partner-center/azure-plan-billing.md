---
title: Faturação do plano Azure - fatura & arquivos de reconhecimento
ms.topic: article
ms.date: 05/19/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como aceder e compreender a estrutura de ficheiros de fatura e reconciliação relacionada com a faturação do plano Azure.
author: khpavan
ms.author: sakhanda
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 5ab086a4d15d16f094e33d19b81f1c93711916dc
ms.sourcegitcommit: e0444145d7720df948b9d02ae2469206db48dba5
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110201430"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a>Nova experiência comercial no CSP – faturação do Azure 

**Funções adequadas**: Agente administrador | Administrador de faturação | Administração global

Este artigo explica como aceder e compreender a estrutura de ficheiros de fatura e reconciliação relacionada com a faturação do plano Azure. A faturação ao abrigo do plano Azure é uma experiência de faturação simplificada usando uma data de faturação única alinhada e período de faturação de um mês de calendário.

## <a name="summary-of-billing-essentials"></a>Resumo do essencial da faturação

- **Data da fatura**: A fatura e o ficheiro de reconciliação estarão disponíveis no painel de instrumentos/API do Centro Parceiro até ao dia 8 (meia-noite UTC).

- **Período de faturação**: O período de faturação está alinhado com o mês civil, por exemplo, 10/1-10/31, 11/1-11/30.

- **Períodos de serviço de cobrança**: As taxas irão alinhar-se com o mês civil. Por exemplo, se o parceiro faturado adicionar serviços Azure através de um plano Azure em 10/15 e o cliente iniciar o consumo de serviços Azure em 10/15, então o parceiro faturado receberá fatura/reconhecimento em 11/8 para consumo de clientes para o período de serviço 10/15 - 10/31. A fatura do próximo mês que será gerada em 12/8 contém todos os encargos para o período de serviço 11/1- 11/31.

- **Prazo de pagamento da fatura:** Líquido 60 dias.

- **Moeda de fatura**: A partir de 28 de janeiro de 2021, os parceiros da região UE/EFTA e reino unido que tenham novos clientes e clientes CSP existentes que adquiram novas ofertas de comércio pela primeira vez, cujos inquilinos foram criados antes de 11 de maio de 2020, serão cobrados para essas compras em moeda de localização parceira. Os parceiros situados fora da região UE/EFTA e reino unido continuarão a ser faturados em moeda de localização de parceiros.

- **Incentivos ao parceiro**: Pago 45 dias a partir do final do mês de fatura.

## <a name="access-your-invoices-and-reconciliation-files"></a>Aceda às suas faturas e ficheiros de reconciliação

O administrador global ou administrador de faturação da sua empresa receberá um e-mail quando uma fatura estiver pronta para ver.

Para aceder à fatura e ao ficheiro de reconciliação:

1. Inicie sessão no [dashboard](https://partner.microsoft.com/dashboard/) do Centro de Parceiros.

2. No menu Partner Center, selecione **Billing**.

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

   :::image type="content" source="images/azure/invoice1.png" alt-text="fatura":::

## <a name="read-the-invoice-reconciliation-file"></a>Leia o ficheiro de reconciliação da fatura

1. Cada plano Azure e combinação de contadores podem ter até duas linhas de faturação no ficheiro de reconhecimento.

2. Se o contador se qualificar para qualquer tipo de desconto ou crédito (como descontos hierárquicos ou o Parceiro ganhou crédito pelos serviços geridos) durante todo o mês civil, então o ficheiro de reconhecimento conterá apenas uma linha de faturação. A coluna **PriceAdjusmentDescription** referenciará o desconto ou o crédito auferido.

3. Se não houver recursos para um determinado contador que se qualiou para desconto ou parceiro ganhou crédito, então o ficheiro de reconhecimento conterá apenas uma linha de faturação e o preço unitário efetivo será o preço de venda ao público (que é o preço unitário).

4. Se o contador, ou quaisquer recursos que emitem esse contador, se qualificasse para **Partner a ganhar crédito pelos serviços geridos** durante uma parte do mês, o ficheiro de reconhecimento conterá duas linhas de faturação. Uma linha representará os dias em que o contador se qualificou e a segunda linha representará os dias em que o contador não se qualificou.

>[!NOTE]
>Pode conciliar o seu consumo de Azure no seu ficheiro de reconhecimento de compra única. Para isso, vá ao seu arquivo de reconhecimento de utilização diária e procure a sua SubscriçãoID. Isto mostrará todos os custos associados ao seu ID do Plano Azure. O seu Azure SubscriptionID é apresentado como o EntitlementID.

## <a name="read-the-daily-usage-file"></a>Leia o ficheiro de utilização diária

- Os contadores de subscrição ao abrigo de um plano Azure são avaliados, e são acumulados, diariamente.

- **O parceiro que ganhou crédito pelos serviços geridos** é determinado e aplicado diariamente.

- Cada contador de assinaturas terá uma linha para cada dia do mês onde houve consumo.

- No exemplo abaixo:

  - O medidor qualificado para **Parceiro ganhou crédito por serviços geridos** de 7/1 - 7/3 (note que o preço unitário efetivo é o preço de venda a retalho menos parceiro ganho crédito.

  - A Meter não se qualificou para **o Partner a ganhar crédito pelos serviços geridos** de 7/4 - 7/7 (note que o preço unitário efetivo é o preço de venda ao público).

  - O medidor qualificado para **Partner ganhou crédito por serviços geridos** de 7/8 - 7/31 (note que o preço unitário efetivo é o preço de venda a retalho menos parceiro ganho crédito).

   :::image type="content" source="images/azure/pecfinal.png" alt-text="recon2":::

## <a name="invoice-in-customer-currency"></a>Fatura em moeda de cliente

Os serviços Azure através de um plano Azure serão avaliados em USD e faturados na moeda atribuída pelo país cliente. Se a moeda de faturação não for USD, então a taxa cambial (FX) utilizada será mostrada na última página da fatura. As tarifas FX são determinadas mensalmente e aplicadas à seguinte fatura. Para obter uma lista completa de moedas de país, por favor, veja o [novo comércio oferece disponibilidade do país e matriz de moeda de cliente.](https://go.microsoft.com/fwlink/?linkid=2112354)

A Microsoft segue a Bolsa de Valores de Londres para conversão. Usamos a taxa de câmbio, que é igual à taxa de câmbio capturada no último segundo do último dia útil do mês na Bolsa de Valores de Londres. As tarifas de FX serão atualizadas e disponíveis na véspera do primeiro dia do mês para o qual se candidatam.

## <a name="azure-reservations"></a>Reservas do Azure


Se comprar [reservas do Azure](azure-reservations.md) através de um plano Azure, pode escolher faturação única ou mensal.


## <a name="azure-spending"></a>Despesas do Azure

A experiência de gastos azure existente é atualizada para apoiar a nova faturação do plano Azure no Partner Center. Isto permite que os parceiros:

- Ver, gerir e receber alertas de orçamento definidos ao nível do cliente 

- Ver os gastos totais estimados num plano Azure (discriminado pelo nível de recursos e contadores)

Uma vez que o modelo de faturação dos serviços Azure através de um plano Azure é o consumo pós-pagamento, para evitar uma fatura maior do que o previsto, os parceiros podem aplicar um orçamento mensal e acompanhar a percentagem de utilização. Um orçamento pode ser aplicado a um cliente ou a vários clientes de uma só vez. 

:::image type="content" source="images/azure/azurespend.png" alt-text="Despesas do Azure":::

## <a name="next-steps"></a>Passos seguintes

- Veja como o parceiro obteve crédito (PEC) é calculado. Inscreva-se no [painel do](https://partner.microsoft.com/dashboard/) Partner Center e localize a lista de preços disponíveis.

- Conheça [a compra do plano Azure](purchase-azure-plan.md)

- Veja a [tabela de preços para a nova experiência de comércio na CSP](azure-plan-price-list.md)
