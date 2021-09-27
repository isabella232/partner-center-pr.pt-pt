---
title: Ser pago no Centro de Parceiros
description: Saiba como receber pagamentos por ganhos como parceiro da Microsoft, como por exemplo através de ofertas de marketplace comercial, programas de incentivo e o programa Fornecedor de Soluções em Nuvem. Inclui política de pagamento, estatuto de detenção de pagamento e declarações de pagamento.
ms.service: partner-dashboard
ms.subservice: partnercenter-payouts
ms.topic: conceptual
ms.date: 09/21/2021
author: eunjkim520
ms.author: eunjkim
ms.openlocfilehash: 5a98a4ef3c1064a64dd2af46ce3a83a0a73589d6
ms.sourcegitcommit: d731813da1d31519dc2dc583d17899e5cf4ec1b2
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/27/2021
ms.locfileid: "129075264"
---
# <a name="getting-paid-in-partner-center"></a>Ser pago no Centro de Parceiros

**Funções adequadas**: Administração de contas | Administrador global

Este artigo tem informações importantes sobre receber o pagamento das suas ofertas, suplementos e ganhos publicitários. Resume a política de pagamentos, os passos necessários antes de serem pagos, e a visão geral do pagamento.

## <a name="payout-policies-and-agreements"></a>Políticas e acordos de pagamento

Ser pago requer que cumpra os acordos e a política de pagamentos.

- [Microsoft Azure Acordo de Publisher do Mercado:](/legal/marketplace/msft-publisher-agreement)Antes de ser pago, tem de aceitar este acordo de editor. Este acordo explica a relação entre si e a Microsoft, uma vez que se refere às ofertas de vendedores no mercado comercial, incluindo a taxa de loja que a Microsoft cobra por cada venda feita.
- [A política de pagamentos](payout-policy-details.md) mostra as políticas de pagamento, incluindo o calendário de pagamentos e os métodos de pagamento. A política também explica o processo de não pagamentos de clientes.
- [Os detalhes fiscais](tax-details-marketplace.md) explicam a consideração fiscal para a seleção de preços e responsabilidade fiscal ao abrigo do [Acordo de Publisher microsoft](/legal/marketplace/msft-publisher-agreement).
- **As taxas de** loja são oficialmente fornecidas nas [Taxas de Mercado Comercial.](/azure/marketplace/marketplace-commercial-transaction-capabilities-and-considerations)
- **Os pagamentos** são efetuados mensalmente (desde que o limiar de pagamento tenha sido cumprido). Normalmente enviamos qualquer pagamento devido num dado mês até ao 15º dia desse mês. Os pagamentos geralmente demoram 3 a 10 dias úteis adicionais para chegar à sua conta de pagamento. Para mais informações, consulte [limiares de pagamento, métodos e prazos.](payment-thresholds-methods-timeframes.md)

## <a name="prerequisite-steps-before-getting-paid"></a>Passos pré-requisitos antes de ser pago

Antes de ser pago pela primeira vez, deve configurar a sua conta de pagamento e preencher os formulários bancários e fiscais necessários. Nos formulários bancários e fiscais, irá fornecer os seus métodos de pagamento preferidos e os formulários fiscais para retenção na fonte. Os formulários bancários e fiscais são necessários antes de podermos pagar-lhe. Para mais informações, consulte [configurar a sua conta de pagamento e formulários fiscais.](set-up-your-payout-account.md)

### <a name="payout-hold-status"></a>Estatuto de detenção de pagamento

Por padrão, enviaremos pagamentos mensalmente, conforme descrito acima. No entanto, pode colocar os seus pagamentos para um programa em espera, e a Microsoft não libertará os seus pagamentos na sua conta. Se optar por colocar os seus pagamentos em espera, continuaremos a registar quaisquer ganhos na página **de Pagamentos.** No entanto, não enviaremos quaisquer pagamentos para a sua conta até que remova o porão.

Para colocar os seus pagamentos em espera, selecione o ícone de engrenagem **Definições** no topo direito e, em seguida, **as definições de Conta**. Selecione **Payout e tax** no menu esquerdo, e na secção de atribuição de pagamento e perfil **fiscal,** localize o programa para o qual você gostaria de pagamentos realizados. Selecione a caixa de verificação **Hold my Payment** para guardar pagamentos para este programa. Pode alterar o seu estado de detenção a qualquer momento, mas a sua decisão afetará o próximo pagamento mensal. Por exemplo, se quiser manter o pagamento de abril, certifique-se de definir o seu estado de detenção de pagamento para **On** antes do final de março.

Uma vez definido o seu estado de detenção de pagamento para **On,** todos os pagamentos para este programa estarão em espera até que você limpe a caixa de verificação para **Off**. Quando o fizer, será incluído durante o próximo ciclo mensal de pagamento (desde que o limite de pagamento tenha sido cumprido). Se já teve os seus pagamentos em espera, mas gostaria de ter um pagamento gerado em junho, então limpe a caixa de verificação para **off** antes do final de maio.

>[!Note]
> O seu estatuto de detenção de Payout aplica-se individualmente a cada programa (Microsoft Store, publicidade, Azure Marketplace, e assim por diante). Se desejar realizar pagamentos para todos os seus programas, guarde o pagamento em cada programa individualmente.

## <a name="payout-statements"></a>Declaração de dividendos

O depoimento mostra os seus ganhos com as vendas das suas ofertas e complementos no histórico de transações. Também pode ver detalhes de pagamento e relatórios de descarregamento em formato TSV ou CSV. Consulte [as declarações do Payout](payout-statement.md) para saber mais sobre como aceder à declaração de pagamento e aos detalhes do histórico de transações e relatórios de pagamento. Além disso, pode utilizar a [API de Pagamentos de Parceiros](https://apidocs.microsoft.com/services/partnerpayouts) para retirar sistematicamente os relatórios de pagamento.

## <a name="next-steps"></a>Passos seguintes

- [API de Pagamentos de Parceiros](https://apidocs.microsoft.com/services/partnerpayouts)
- [FAQ sobre dividendos](payout-faq.yml)