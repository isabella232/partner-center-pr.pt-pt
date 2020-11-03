---
title: Pagamento de FAQ para o mercado comercial da Microsoft
description: Obtenha respostas a perguntas comuns sobre pagamentos no mercado comercial. Inclui respostas sobre o porquê dos seus ganhos serem diferentes do que esperava.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: article
author: keferna
ms.author: keferna
ms.date: 09/11/2020
ms.openlocfilehash: 44bd7f488e3d4e79c45cb2746c7e2a6da449a310
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/19/2020
ms.locfileid: "92530572"
---
# <a name="common-questions-about-commercial-marketplace-payouts"></a>Questões comuns sobre pagamentos de mercado comercial

Este artigo responde frequentemente a perguntas sobre pagamentos no mercado comercial.

## <a name="earnings-incorrect-or-missing"></a>Ganhos incorretos ou em falta

#### <a name="why-are-my-earnings-missing"></a>Porque é que os meus ganhos estão em falta?

- A encomenda do cliente talvez ainda não seja elegível para pagamento. Para pedidos de clientes não empresariais, a Microsoft tem de receber o pagamento do cliente antes de os ganhos do publicador ficarem elegíveis. Para encomendas de clientes empresariais, os seus ganhos estarão disponíveis 1-2 dias após a data da Nota de encomenda. Verifique o estado da Encomenda em [Relatórios de encomendas](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/order).
- Os ganhos de transações antes de julho de 2019 podem não ser mostrados no relatório do histórico de transações. Verifique as Declarações do Histórico em [Transferência de Pagamento](https://partner.microsoft.com/dashboard/payouts/reports/incentiveexport).
- Verifique o [prazo do ciclo de pagamento](payment-thresholds-methods-timeframes.md) e compreenda quando os seus ganhos devem aparecer na declaração de pagamento.

#### <a name="why-is-my-earnings-amount-different-than-what-i-expected"></a>Porque é que os meus ganhos são diferentes do que esperava?

- Se a encomenda foi parcialmente paga pelo seu cliente, o seu valor de ganho basear-se-á no valor parcialmente pago após a dedução da taxa e do imposto adequado.
- Verifique a responsabilidade fiscal por país. No caso de países em que o imposto seja da responsabilidade da Microsoft, a Microsoft cobra e deduz o imposto dos ganhos do publicador. O montante da transação mostrado na declaração é após o montante do imposto. Veja [Detalhes fiscais](tax-details-marketplace.md).
- As ofertas da SaaS e da IaaS têm uma taxa de agência descontada de 10% em vez dos 20% padrão, deixando uma taxa de ganhos de 90%. Esta promoção está em vigor até 30 de junho de 2021.

**Continuar a ler** [Acordo de Editor de Mercado Comercial](https://go.microsoft.com/fwlink/p/?LinkID=699560), [Detalhes da política de pagamento,](payout-policy-details.md) [limiar de pagamento, método e prazo,](payment-thresholds-methods-timeframes.md) [Ser pago no mercado comercial,](marketplace-get-paid.md) [detalhes fiscais,](tax-details-marketplace.md) [declarações de pagamento,](payout-statement.md) [dashboard de encomendas em análise de mercado comercial](/azure/marketplace/partner-center-portal/orders-dashboard)

## <a name="earnings-reconciliation"></a>Reconciliação dos ganhos
### <a name="how-do-i-reconcile-payout-statements-to-order-or-usage-reports-in-analytics"></a>Como devo proceder para reconciliar as declarações de dividendos para relatórios de encomendas ou de utilização nas análises?
Utilize o AssetID, o orderID e o ID do item de linha que aparece no relatório do histórico de transações de pagamento com ordens analíticas e relatórios de utilização. Utilize este mapeamento:

- Histórico de Transações de Dividendos.AssetID = order.OrderID
- Histórico de Transações de Dividendos.OrderID & LineItem = Usage.UsageReferenceID [OrderID:LineItemID]

### <a name="how-do-i-know-when-to-expect-payments-for-my-customer-orders"></a>Como devo proceder para saber quando esperar pagamentos para as encomendas de clientes?
- Em primeiro lugar, utilizando o seu activoID, consulte as encomendas de clientes nos [relatórios encomendas](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/order).
- Verifique o canal de cliente para a subscrição do seu cliente no [relatório de clientes.](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/customer)
- Para os clientes empresariais, os ganhos dos editores aparecem no comunicado 1-2 dias após a data da Encomenda de Compra.
- Para clientes não empresariais, os ganhos dos editores aparecem no comunicado 1-2 dias após o pagamento do cliente.

**Continuar a ler** [Declarações de pagamento](payout-statement.md), Dashboard de encomendas em análise de mercado [comercial](/azure/marketplace/partner-center-portal/orders-dashboard)

## <a name="payout-policies"></a>Políticas de dividendos

#### <a name="how-do-i-find-the-current-agency-fee-and-the-payout-rate"></a>Como devo proceder para encontrar a tarifa da agência atual e a taxa de dividendos?

- Verifique o Contrato do Editor do marketplace comercial. A tarifa da agência padrão é de 20%. As transações elegíveis Co-Sell SaaS têm uma taxa descontada de 10%. Verifique se existem anúncios de tarifas promocionais da agência.
- Na sua demonstração de pagamento, a Taxa de Ganhos especifica a taxa de pagamento real para uma determinada transação.

#### <a name="when-can-i-expect-a-payment-from-microsoft-once-earnings-appear-on-my-statement"></a>Quando posso esperar um pagamento da Microsoft, assim que os ganhos aparecerem na minha declaração?
- Assim que os ganhos estiverem no estado não processado, pode verificar a data de vencimento referente ao mês em que os ganhos serão processados para pagamento. Uma vez preparado o seu pagamento, o seu estado de ganho mudará para "processado".  A Microsoft lança os pagamentos no 15º dia do mês de vencimento.
- Para encomendas pagas com cartão de crédito, a Microsoft detém pagamentos de 30 dias até que o ganho seja amadurecido.

 **Continuar a ler** [Acordo de Editor de Mercado Comercial](https://go.microsoft.com/fwlink/p/?LinkID=699560), Detalhes da política de [pagamento,](payout-policy-details.md) [detalhes fiscais,](tax-details-marketplace.md) [limiar de pagamento, método e prazo](payment-thresholds-methods-timeframes.md)

## <a name="payments-and-adjustments"></a>Pagamentos e ajustamentos

#### <a name="why-is-my-payment-missing"></a>Porque é que o meu pagamento está em falta?

- Certifique-se de que o seu estado de pagamento e o estado do perfil do imposto são apresentados como *válidos* na [página geral.](https://partner.microsoft.com/dashboard/commercial-marketplace/overview)
- Pode não ter cumprido o limiar mínimo para um pagamento. Os ganhos têm ser de, pelo menos, 50 USD para receber um pagamento.


#### <a name="how-do-i-set-my-account-to-not-receive-payment"></a>Como posso definir a minha conta para não receber o pagamento?
Pode realizar pagamentos no [Perfil de Pagamento;](https://partner.microsoft.com/dashboard/commercial-marketplace/overview) basta verificar **Hold** . A Microsoft irá reter-lhe o pagamento até que liberte o porão.

#### <a name="why-do-i-receive-in-a-different-currency-than-the-purchase-currency"></a>Porque recebo numa moeda diferente da moeda de compra?

A moeda de pagamento é baseada na moeda selecionada no perfil de pagamento. A moeda de compra é baseada na moeda paga pelo cliente.

#### <a name="how-do-i-reconcile-adjustments"></a>Como faço a reconciliação de ajustes?

Os ajustes de pagamento são correções de pagamento para acomodar os ajustes de compensação, como problemas do sistema. Na instrução do pagamento, ReasonCode especificará o motivo do ajuste. Estes não se destinam a reconciliar diretamente transações individuais.

**Continuar a ler** [Acordo de Editor de Mercado Comercial](https://go.microsoft.com/fwlink/p/?LinkID=699560), Detalhes da política de [pagamento,](payout-policy-details.md) [detalhes fiscais,](tax-details-marketplace.md) [limiar de pagamento, método e prazo](payment-thresholds-methods-timeframes.md)

## <a name="taxes"></a>Impostos

#### <a name="how-do-we-identify-tax-remit-responsibility-between-microsoft-or-publisher-in-the-payout-statement"></a>Como identificamos a responsabilidade da Cobrança de Impostos entre a Microsoft ou o Publicador na declaração de pagamento?

Na transferência do histórico de transações, localize a coluna Modelo de imposto. Deste modo, mostra Gerido pela MS ou Gerido pelo ISV. Veja as regras de impostos específicas do país e implicações de pagamento em [Detalhes do imposto](tax-details-marketplace.md).

#### <a name="how-do-i-download-service-fee-tax-forms"></a>Como transfiro formulários do Imposto da Tarifa de Serviço?

Aceda à página **Pagamentos** e, em seguida, à secção **Lista de Pagamentos** . Uma ligação para o formulário do imposto da Tarifa de Serviço é apresentado para um pagamento que tem o Imposto da Tarifa de Serviço.

#### <a name="how-do-i-download-a-withholding-tax-form-in-pdf"></a>Como transfiro um formulário de Imposto retido em PDF?

Aceda à página *Pagamentos* e, em seguida, à secção **Lista de Pagamentos** . Uma ligação para um formulário de imposto retido é apresentado junto a um pagamento.

#### <a name="where-do-i-find-year-end-tax-forms"></a>Onde encontro os formulários de imposto de fim de ano?

Aceda à [página Perfil](https://partner.microsoft.com/dashboard/payee/profiles/partner/manage) para ver os seus formulários de imposto de fim de ano.

#### <a name="how-do-i-find-withholding-tax-for-a-transaction"></a>Como fazer localizar a Retenção de imposto de uma transação?
A retenção de imposto é aplicável a publicadores norte-americanos que preencheram um formulário W-9. A retenção de imposto é calculada com base num pagamento mensal.

**Continuar a ler** [Acordo de Editor de Mercado Comercial,](https://go.microsoft.com/fwlink/p/?LinkID=699560) [Detalhes da política de pagamento](payout-policy-details.md)

## <a name="payout-statement-access"></a>Acesso a declaração de pagamento

#### <a name="how-do-i-access-a-payout-statement"></a>Como devo proceder para aceder a uma declaração de pagamento?

1. Verifique as funções. Tem de ter a função de *contribuidor financeiro* ou de *proprietário da conta* para aceder à declaração de pagamento.
2. Na navegação superior direita, selecione o ícone **Payout** para ver a sua declaração de pagamento. Escolha entre **Histórico de Transações,** **Pagamento** e **Download.**

**Continuar a ler** [Funções e permissões de pagamento,](payout-statement.md#roles-and-permissions) [declarações de pagamento](payout-statement.md) 

## <a name="payout-statement-report"></a>Relatório de declaração de pagamento

#### <a name="what-does-each-field-in-the-transaction-download-mean"></a>O que significa cada campo na transferência da transação?

Consulte [as declarações de Payout](payout-statement.md) para obter uma lista detalhada dos atributos e dos seus significados.

#### <a name="what-is-earning-status"></a>Qual é o estado dos ganhos?

Isto mostra os seus ganhos como não processados, processados ou enviados.

- **Não processados** – os ganhos estão em período de caução até à data de vencimento.
- **Processado** – Os ganhos amadureceram e estão preparados para um pagamento mensal. Os pagamentos são liberados até dia 15 de cada mês.
- **Enviado** – O pagamento foi liberado com sucesso para o seu banco com base no seu perfil de pagamento.

#### <a name="how-do-i-download-service-fee-tax-forms"></a>Como transfiro formulários do Imposto da Tarifa de Serviço?

Aceda à página **Pagamentos** e, em seguida, à secção **Lista de Pagamentos** . Uma ligação para o formulário do imposto da Tarifa de Serviço é apresentado para um pagamento que tem o Imposto da Tarifa de Serviço.

#### <a name="how-do-i-download-a-withholding-tax-form-in-pdf"></a>Como faço o download de um formulário de retenção na fonte em PDF?

Aceda à página **Pagamentos** e, em seguida, à secção **Lista de Pagamentos** . Uma ligação para um formulário de imposto retido é apresentado junto a um pagamento.

#### <a name="where-do-i-find-year-end-tax-forms"></a>Onde encontro os formulários de imposto de fim de ano?

Aceda à [página Perfil](https://partner.microsoft.com/dashboard/payee/profiles/partner/manage) para ver os seus formulários de imposto de fim de ano.

**Continuar a ler** [Declarações de pagamento,](payout-statement.md) [download do histórico de transações](payout-statement.md#transaction-history-download)

## <a name="historical-statements"></a>Declarações históricas

#### <a name="how-do-i-view-historical-information"></a>Como vejo informação histórica?

A declaração do histórico mostrará o instantâneo dos dados de pagamento a partir de outubro de 2019. Infelizmente, a informação sobre o pagamento aqui não se atualiza. Para receber as últimas informações, envie um bilhete de apoio para os dados mais recentes.

**Continuar a ler** [Declarações de pagamento,](payout-statement.md) [download do histórico de transações](payout-statement.md#transaction-history-download)

## <a name="payout-export-api"></a>Pagamento exportar API

#### <a name="how-do-i-download-payout-data"></a>Como transfiro dados de pagamento?

Utilize a [API de Pagamento de Parceiros.](https://apidocs.microsoft.com/services/partnerpayouts)

## <a name="next-steps"></a>Passos seguintes

- [Receber pagamento no marketplace comercial](marketplace-get-paid.md)
