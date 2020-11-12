---
title: Horários de pagamento e detalhes da política - Mercado Azure
description: Saiba mais sobre detalhes relacionados com as políticas de pagamento de mercado comercial, incluindo horários e recuperação.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: conceptual
author: eunjkim520
ms.author: eunjkim
ms.date: 11/06/2020
ms.openlocfilehash: 9c03878ec69b9df06795054464ef7f76e038e780
ms.sourcegitcommit: cc30a06abe55b9da32177a24e74bfd6fc7d8bbb9
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/12/2020
ms.locfileid: "94531992"
---
# <a name="payout-schedules-and-policy-details"></a>Horários de pagamento e detalhes da política

Este artigo discute o processo de pagamento da Microsoft, o calendário de pagamentos, onde encontrar o estado de um pagamento, e o processo de não pagamento do cliente.

## <a name="payment-schedules"></a>Horários de pagamento

As seguintes secções descrevem o nosso processo de pagamentos para **o Contrato de Empresa** e transações de **cartões de crédito/fatura.**

### <a name="enterprise-agreement-transactions"></a>Transações do Acordo de Empresa

Quando um cliente compra um produto do Microsoft AppSource ou do Azure Marketplace utilizando o seu atual Microsoft Enterprise Agreement para transações, emitiremos pagamentos no próximo ciclo de pagamentos de 30 dias após a fatura do cliente. As transações em que um cliente utiliza um cartão de crédito têm um período de detenção de 30 dias antes do pagamento.

Um pagamento ocorrerá frequentemente antes de a Microsoft receber o pagamento do cliente. Consulte [o Processo de não pagamento do cliente](#process-for-customer-non-payment) abaixo para as ações que tomamos se o cliente não pagar à Microsoft, mas já emitimos um pagamento.

| Evento | Description | Visibilidade reportando | Timing* |
| --- | --- | --- | --- |
| Utilização ou Mês de Transação | O cliente usa ou compra um serviço. | [Painel de utilização](/azure/marketplace/partner-center-portal/usage-dashboard) ou [ordem](/azure/marketplace/partner-center-portal/orders-dashboard) | **Mês 1** |
| A Ordem de Compra é criada | Determinar a utilização total, as transações totais | [Painel de utilização](/azure/marketplace/partner-center-portal/usage-dashboard) ou [ordem](/azure/marketplace/partner-center-portal/orders-dashboard) | **Mês 2** |
| Isv Payout Earning isv é criado | Determinar taxas de agência e ganhos de pagamento | Marcado como não processado no histórico de transações na Declaração de Pagamento | **Mês 3 (1ª semana)** |
| Preparar o Pagamento | Os ganhos estão preparados para o pagamento mensal | Marcado como O Próximo no Histórico de Transações na Declaração de Pagamento | **Mês 3 (1ª semana)** |
| **Data de Pagamento** | **O pagamento é enviado para editor** | **Marcada como Enviada no Histórico de Transações e na secção de Pagamentos da Declaração de Pagamento** | **Mês 3 (o mais tardar no dia 15)** |
| Fatura paga pelo Cliente | Microsoft recolhe pagamento do cliente | Sem alterações | **Mês 4 a 12** |
|

\* A data de pagamento está na Hora Padrão do Pacífico (PST).

### <a name="customers-who-pay-using-credit-card-or-invoice"></a>Clientes que pagam com cartão de crédito ou fatura

Todas as compras com cartão de crédito ou fatura mensal têm um período de detenção de 30 dias para garantir que os fundos são recolhidos junto do cliente.

| Evento | Description | Visibilidade reportando | Timing* |
| --- | --- | --- | --- |
| Utilização ou Mês de Transação | O cliente usa ou compra um serviço. | [Painel de utilização](/azure/marketplace/partner-center-portal/usage-dashboard) ou [ordem](/azure/marketplace/partner-center-portal/orders-dashboard) | **Mês 1** |
| Fatura paga pelo Cliente | Determine o uso total, o valor total da transação e a fatura do cliente | [Painel de utilização](/azure/marketplace/partner-center-portal/usage-dashboard) ou [ordem](/azure/marketplace/partner-center-portal/orders-dashboard) | **Mês 2** |
| Isv Payout Earning isv é criado | Determinar taxas de agência e ganhos de pagamento | Marcado como não processado no histórico de transações na Declaração de Pagamento | **Mês 2** |
| Período de detenção de 30 dias | Garantir a recolha de fundos, possíveis pedidos de reembolso e reembolso | Marcado como não processado no histórico de transações na Declaração de Pagamento | **3 mês** |
| Preparar o Pagamento | Os ganhos estão preparados para o pagamento mensal | Marcado como O Próximo no Histórico de Transações na Declaração de Pagamento | **Primeira semana do Mês 4** |
| **Data de Pagamento** | **O pagamento é enviado para editor** | **Marcada como Enviada no Histórico de Transações e na secção de Pagamentos da Declaração de Pagamento** | **Mês 4 (o mais tardar no dia 15)** |
|

\* A data de pagamento é na Hora Padrão do Pacífico (PST).

## <a name="process-for-customer-non-payment"></a>Processo de não pagamento de clientes

Em raras ocasiões, a Microsoft não consegue cobrar pagamentos aos clientes pelas suas compras no mercado comercial. Quando um cliente não paga à Microsoft de acordo com o seu calendário de faturação, iniciamos o processo de cobranças. Este processo demora aproximadamente quatro meses e envolve uma comunicação persistente da Microsoft. Se o pagamento não for recebido até ao final deste processo, a Microsoft anula os fundos como incobráveis.

De acordo com o processo de pagamento aqui articulado, a Microsoft pode já ter pago fundos a editores (você) que são, em última análise, incobráveis. Portanto, temos um processo de conciliação destes montantes. Para garantir que tem avisado que o seu (já recebido) pagamento pode ser reconciliado, será notificado quando um cliente estiver no processo de cobranças e as compras são suscetíveis de ser amortizadas.

A Microsoft recuperará quaisquer pagamentos já pagos utilizando um dos seguintes métodos: (1) A Microsoft pode subtrair os montantes não pagos de pagamentos futuros; por exemplo, se $1.000 em pagamentos forem considerados incobráveis e anulados, os seus pagamentos futuros serão retidos até que os $1.000 sejam recuperados, ou (2) a Microsoft pode solicitar um reembolso ou editores de fatura para quaisquer valores não cobrados.

Segue-se um exemplo de calendário:

| Evento | Data aproximada* | Visibilidade do parceiro |
| --- | --- | --- |
| Data de pagamento de exemplo | 10/15/2020 | Marcado como **Enviado** no Histórico de Transações e na secção de Pagamentos no Painel de Pagamentos |
| <font color="red">Se o cliente não pagar à Microsoft</font> | 12/2/2020 – 12/5/2020 | Sem mudanças, como acima |
| Cliente recebe primeiro e-mail de pagamento em atraso | 12/6/2020 | Nenhum |
| Cliente recebe e-mails regulares de urgência crescente | 12/7/2020 – 1/31/2021 | Nenhum |
| Editor é notificado write-off é provável | 1/7/2021 | E-mail notificação enviada ao editor que o seu cliente ainda não enviou o pagamento. O ID de transação e o valor em dólares estão incluídos. |
| Cliente recebe aviso de rescisão | 2/1/2021 | Nenhum |
| Fim do processo de recolha / os fundos são anulados | 2/15/2021 | E-mail notificação enviada ao editor de que os fundos foram anulados. O ID de transação e o valor em dólares estão incluídos. |
| O pagamento é deduzido | 3/1/2021 | Editor verá transação negativa em Declaração de Pagamento do Partner Center |
| O pagamento é retido | 3/15/2021 | Os pagamentos futuros serão mostrados na Declaração de Pagamento do Centro Parceiro. A editora não receberá o pagamento até que o saldo não seja mais negativo.  |
|||

\* A data de pagamento é na Hora Padrão do Pacífico (PST).

## <a name="number-of-days-for-payments-to-reach-a-payout-account"></a>Número de dias para pagamentos chegarem a uma conta de pagamento

Normalmente enviamos qualquer pagamento devido num dado mês no 15º dia desse mês, mas leva tempo adicional para o pagamento chegar à sua conta. O número de dias depende do método de pagamento que utilizamos para a sua conta, conforme descrito abaixo.

> [!NOTE]
> Os dias abaixo apresentados são aproximados; qualquer pagamento pode demorar um tempo maior ou mais curto para chegar à sua conta.

| Método de pagamento     | Número de dias para chegar à conta de pagamento     |
|--------------------|--------------------------------------------|
| PayPal             | 1 dia útil                             |
| ACH/SEPA           | 2-3 dias úteis                          |
| Transferência bancária      | 7-10 dias úteis                         |
|

## <a name="next-steps"></a>Passos seguintes

Saiba mais detalhes [fiscais.](tax-details-marketplace.md)
