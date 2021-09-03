---
title: Lista de preços de planos do Azure para parceiros CSP
ms.topic: how-to
ms.date: 07/21/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Saiba como os parceiros de programas da CSP podem usar o Partner Center para ver a lista de preços das subscrições ao abrigo do plano Azure.
author: brentserbus
ms.author: brserbus
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 73b47b62ce996156c7e780450bada1bdbec9f4b0
ms.sourcegitcommit: 09d2c10491244775e656b48fce35b5648262ce59
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/03/2021
ms.locfileid: "123457617"
---
# <a name="price-list-for-the-new-commerce-experience-in-csp-for-azure"></a>Lista de preços da nova experiência comercial no CSP para Azure

**Funções adequadas**: Agente administrador | Administrador de faturação | Administração global | Agente helpdesk | Agente comercial | Administração de gestão de utilizadores

Os preços em tempo real para a nova experiência de comércio Azure em CSP são entregues dinamicamente em tempo real no Partner Center. Os preços são mostrados apenas em USD. A partir de agosto de 2021, todos os parceiros serão faturados na moeda de localização do parceiro, independentemente da localização do cliente a quem vendeu o produto. Para mais informações, consulte [o plano Azure - faturação](azure-plan-billing.md).

Como parte da nova experiência de comércio do Azure no CSP, introduzimos uma [nova oferta do Azure](./azure-plan-lp.md). Para datas importantes relacionadas com a oferta do Azure anterior (MS-AZR-0145p), veja o [documento da oferta](https://go.microsoft.com/fwlink/p/?linkid=2164140).

Se se matriculou *antes* de 21 de julho de 2021
- Você continuará a ver a oferta anterior do Azure na lista de preços.

Se se matriculou *em ou depois de* 21 de julho de 2021
- *Não* verá a oferta anterior do Azure na lista de preços.

## <a name="see-pricing-for-subscriptions-under-the-azure-plan-pricing"></a>Ver preços para subscrições ao abrigo do plano Azure

1.  A partir do menu Partner Center, selecione **Venda,** em **seguida, Preços e ofertas**.
2.  De acordo com **o plano Azure, os preços de consumo** e o plano **Azure planeiam a fixação de preços**, selecione o país e, em seguida, o link de descarregamento.
   - Para **taxas de câmbio estrangeiras,** selecione o link de descarregamento na secção.

   > [!NOTE] 
   > **As tarifas de FX** não são específicas do país.

   :::image type="content" source="images/azure/pricing-new.png" alt-text="Screenshot de Preços e ofertas mostrando a nova experiência de comércio.":::

   > [!NOTE] 
   > Pode exportar duas listas de preços diferentes: preços do plano Azure e preços de terceiros do Marketplace.

## <a name="azure-price-list-specifics"></a>Detalhes da lista de preços do Azure

- Os preços do plano Azure estarão disponíveis a partir da página **de Preços e ofertas** no Partner Center, em **Sell.**

- As exportações estarão disponíveis para os serviços de consumo do plano Azure, reservas Azure e taxas DE FX.

- As opções de exportação incluem:

  - **Preços correntes**: Esta opção inclui todos os contadores e preços desde o primeiro do mês até à data atual do mês, como novos preços, preços alterados ou preços removidos. Todos os preços terão datas de início e fim eficazes para explicar se são novos ou removidos.

  - **Preço do mês anterior**: Os downloads de cada tipo de recurso serão por mês. Para os ficheiros de preços, isto incluirá todos os contadores que estavam disponíveis durante esse mês. Se um novo medidor aparecer em meados do mês, eu apareci como um medidor com uma data efetiva que reflete a sua disponibilidade. Semelhante aos preços que são descontinuados, mostrando com uma data final efetiva descrevendo quando já não estão disponíveis.

  - **Tarifas FX**: As tarifas FX estarão disponíveis para download na véspera do dia 1 do mês, 18h PST. Por exemplo, se quiser as tarifas para novembro, baixe as tarifas no dia 31 de outubro. As tarifas de FX do mês anterior também estarão disponíveis.

- Os preços nas tabelas de preços são preços diretos. Alguns parceiros podem ser elegíveis para sócios que ganharam créditos. Para obter informações sobre como o parceiro obteve crédito é calculado, leia [como o parceiro obteve crédito é calculado e pago](partner-earned-credit-explanation.md).

- **Serviços elegíveis**: O crédito auferido pelo parceiro é aplicável aos serviços listados no **plano Azure que** os parceiros de preços de consumo podem exportar a partir da página de preços do [plano Azure.](https://partner.microsoft.com/commerce/sales)
   > [!NOTE]
   > Existem exceções, incluindo, mas não se limitando a, produtos de **terceiros identificados** como "Terceiros" na coluna Tags da lista de preços de consumo do plano Azure e reservas do plano Azure.

## <a name="price-list-data"></a>Dados da lista de preços

|**Campo**   |**Descrição**   |
|--------------------------|:---------------------------|
|Instituto de Produtos  |Título ou nome do produto|
|ProductID   |ID do produto|
|SKuId|ID do SKU|
|SkuTitle|Título ou nome da SKU|
|Publisher|A primeira parte será sempre a Microsoft.|
|SkuDescription|Descrição do SKU|
|UnitOfMeasure|As unidades que serão cobradas ou faturadas|
|TermoDuração|Para produtos de base a prazo, a duração do termo, aplicável às reservas|
|Mercado|Mercado dos preços|
|Moeda|Moeda do preço|
|UnitPrice|Preço por unidade|
|PreçosTierRangeMin|Para preços diferenciados, o preço mínimo aplica-se|
|PreçosTierRangeMax|Para preços diferenciados, o preço máximo aplica-se|
|EficazStartDate|Data de início dos preços|
|Efê-Térmo|Data de fim do preço|
|Meterids|Identificação do medidor do produto SKU|
|Medidor deTipo|Tipo de Medidor|
|Etiquetas|Propriedades para o item, para preços do plano Azure este será Azure ou Azure e Reservas (especificamente para reservas)|

As listas de preços do plano Azure podem ser exportadas a partir da [página de Preços e ofertas](https://partner.microsoft.com/dashboard/sell/pricingandoffers) no Partner Center.

## <a name="tiered-pricing"></a>Preços hierárquicos

Alguns serviços de consumo de plano Azure apoiam preços diferenciados. Os parceiros podem encontrar estes produtos e SKUs na lista de preços do plano Azure. Os itens que têm valores nas colunas de gama de preços permitem aos parceiros compreender o preço com base na utilização. No exemplo abaixo, usando dados de amostra, temos um produto SKU com três níveis de preços.

|**ProductId**   |**SkuId**   |**UnitPrice**   |**PreçosTierRangeMin**   |**PreçosTierRangeMax**   |
|:---------------|:-----------|:---------------|:-------------------------|:-------------------------|
|DDD123456ABC|01AB|0.50|100001|9223372036854780000|
|DDD123456ABC|01AB|0.80|101|100000|
|DDD123456ABC|01AB|1|1|100|

Neste exemplo, se 101 unidades forem usadas, a carga seria de 100,80. As primeiras 100 unidades são uma cada e a próxima unidade é carregada a 0,80.

## <a name="pricing-api-for-azure-plan"></a>API de preços para plano Azure

Você pode usar o [preço API](/partner/develop/pricing) para recuperar preços do plano Azure para consumo e reservas programáticamente. Também pode recuperar as taxas de câmbio.

A API de preços está num ponto final diferente dos APIs do Centro De Parceiros. As informações sobre preços incluem preços de contadores em USD para recursos do plano Azure e preços de reservas aplicados às subscrições do plano Azure.

Esta API também permite que os parceiros recuperem taxas de câmbio mensais porque os preços do plano Azure estão apenas em USD. Pode utilizar as APIs para recuperar os preços e as taxas de câmbio para o mês em curso ou meses anteriores.

> [!NOTE]
> A API de preços é específica para os preços do plano Azure. Você ainda deve usar a API do RateCard existente e as listas de preços postadas na página "Preços e ofertas" do Partner Center para recursos Azure ou reservas implantadas para subscrições de planos não-Azure. O plano Azure que fixa preços API não suporta software, marketplace ou preços baseados em licenças, tais como Microsoft 365 ou Dynamics 365.

Para obter mais informações sobre os preços do plano Azure e as APIs cambiais, consulte a documentação completa da [API sobre preços](/partner/develop/pricing).

## <a name="next-steps"></a>Passos seguintes

- [Manage subscriptions and resources under the Azure plan](azure-plan-manage.md) (Gerir subscrições e recursos ao abrigo do plano do Azure)
