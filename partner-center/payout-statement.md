---
title: Declaração de pagamento para o mercado comercial no Partner Center
description: Saiba mais sobre as demonstrações e resumos de pagamento, e como ver e exportar os seus dados de pagamento para o mercado comercial
ms.subservice: partnercenter-marketplace-publisher
ms.service: marketplace
ms.topic: article
author: mingshen-ms
ms.author: mingshen
ms.date: 09/23/2020
ms.openlocfilehash: 460a7b1992d7db40e0f45d3aeb7e2236e9495e07
ms.sourcegitcommit: a84812b650ec8b6d0513c46c04840e4bbb0c8460
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/25/2020
ms.locfileid: "92530128"
---
# <a name="payout-statements"></a>Declaração de dividendos

A **declaração do Payout** apresenta uma visão geral dos seus pagamentos a partir de ofertas vendidas através do mercado comercial. Mostra o histórico transacional dos seus ganhos, estima o seu próximo pagamento e mostra as tendências de pagamento. Também pode baixar o histórico de transações e as demonstrações de pagamento. Este artigo explica como aceder ao seu depoimento de pagamento, e às diferentes páginas de pagamento e downloads acessíveis a si no Partner Center.

## <a name="roles-and-permissions"></a>Funções e permissões

Para aceder a uma demonstração de pagamento, é necessário atribuir-lhe a **função de titular** da Conta ou **contribuinte financeiro.**

| Relatórios/Páginas | Proprietário de Conta | Gestor | Programador | Contribuinte de negócios | Contribuinte financeiro | Marketer |
| --- | --- | --- | --- | --- | --- | --- |
| Relatório de aquisição (incluindo dados quase em tempo real) | Pode ver | Pode ver | Sem acesso | Sem acesso | Pode ver | Sem acesso |
| Relatório de feedback/respostas | Pode ver e enviar feedback | Pode ver e enviar feedback | Pode ver e enviar feedback | Sem acesso | Sem acesso | Pode ver e enviar feedback |
| Relatório de saúde (incluindo dados quase em tempo real) | Pode ver | Pode ver | Pode ver | Pode ver | Sem acesso | Sem acesso |
| Relatório de utilização | Pode ver | Pode ver | Pode ver | Pode ver | Sem acesso | Sem acesso |
| Conta de pagamento | Pode atualizar | Sem acesso | Sem acesso | Sem acesso | Pode atualizar | Sem acesso |
| Perfil fiscal | Pode atualizar | Sem acesso | Sem acesso | Sem acesso | Pode atualizar | Sem acesso |
| Resumo dos dividendos | Pode ver | Sem acesso | Sem acesso | Sem acesso | Pode ver | Sem acesso |
|

## <a name="access-your-payout-statement"></a>Aceda ao seu dado de pagamento

Inscreva-se no [Partner Center](https://partner.microsoft.com/dashboard/home) e selecione o ícone de pagamento no canto superior direito do ecrã para aceder a estes diferentes resumos:

- Histórico de transações
- Pagamentos
- Exportar dados

:::image type="content" source="images/payouts/payout-overview.png" alt-text="Ilustra o ícone payout no canto superior direito do portal Partner Center":::

Também pode utilizar a [API de Pagamento de Parceiros](https://apidocs.microsoft.com/services/partnerpayouts) para conectar e obter dados de transações e pagamentos diretamente.


## <a name="transaction-history"></a>Histórico de transações

A página de histórico de **transações** mostra o resumo dos seus ganhos, o próximo pagamento estimado, e a tendência dos seus ganhos e pagamentos ao longo dos últimos 36 meses. Também pode baixar detalhes de transações a partir desta secção.

:::image type="content" source="images/payouts/transaction-overview.png" alt-text="Ilustra o ícone payout no canto superior direito do portal Partner Center":::

- **Resultados enviados este ano** – Total de ganhos e desagregação dos ganhos que foram pagos e serão pagos no próximo mês.
- **Mês estimado de pagamento** – Lucros totais esperados para os próximos meses.
- **Tendência de ganhos e pagamentos** – Os valores mensais de ganhos e pagamentos dos últimos 36 meses.
- **Baixar** - Baixar detalhes de transações em formato .csv ou .tsv.

Utilize a seleção da gama de datas no canto superior direito da página para filtrar a saída da página para mostrar os últimos 3, 6, 12 ou 36 meses. Ou, selecione um intervalo de data personalizada até 36 meses. O intervalo de data por defeito é de 12 meses.

:::image type="content" source="images/payouts/search-filter.png" alt-text="Ilustra o ícone payout no canto superior direito do portal Partner Center":::

### <a name="transaction-history-summary"></a>Resumo do histórico de transações

Isto mostra detalhes de ganhos, incluindo a origem do ganho do produto vendido datas de ganho, estado e mês de pagamento estimado.

:::image type="content" source="images/payouts/transaction-history.png" alt-text="Ilustra o ícone payout no canto superior direito do portal Partner Center":::

- **Data ganha** - A data de compra.
- **Tipo de ganho** – O tipo de ganho, como Venda, Desconto ou Cooperativa.
- **Valor total** – O valor líquido do resultado. No mercado comercial, isto significa depois de deduzir a taxa normal de mercado.
- **Estado** – Tem três opções:
    - **A seguir** – Os ganhos estão em período de arrefecimento pendente.
    - **Processado** – Os ganhos estão preparados para o próximo pagamento.
    - **Enviados** – Os ganhos foram pagos.
- **Mês estimado de pagamento** – O mês em que os ganhos deverão ser pagos.

As transações de ganhos são mostradas assim que a transação satisfaz a elegibilidade do pagamento. Para entender por que pode ter ganhos em falta ou inesperados, consulte [questões comuns sobre pagamentos de mercado comercial.](payout-faq.md#why-are-my-earnings-missing)

### <a name="transaction-history-download"></a>Download do histórico de transações

Para ver mais detalhes sobre um ganho, selecione **Baixar** no topo da página. A tabela seguinte explica cada coluna do relatório.

| Nome da coluna | Descrição | Aplicabilidade para programas de incentivo/mercados |
| --- | --- | --- |
| agreementEndDate | Data limite do acordo | Incentivos - apenas alguns programas |
| agreementNumber | Número do contrato | Incentivos - apenas alguns programas |
| agreementStartDate | Data de início do acordo | Incentivos - apenas alguns programas |
| cálculoDate | Data em que o ganho foi calculado no sistema | Todos |
| claimId | Identificador único para reclamação | Incentivos - apenas alguns programas |
| clienteCountry | País/região do cliente | mercados |
| customerEmail |  |  |
| nome do cliente | Estará sempre em branco. | Apenas programas de incentivo (exceção: OEM) e mercados |
| customerTenantId |  |  |
| distribuidorId | Identificador de distribuidor | Incentivos - apenas alguns programas |
| nome distribuidorna | Nome do distribuidor | Incentivos - apenas alguns programas |
| earningAmount | Valor de Ganho na moeda de transação original | Todos |
| earningAmountInLastPaymentCurrency | Valor da obtenção na última moeda de pagamento (o campo estará vazio se não tiverem sido pagos pagamentos prévios) |  |
| earningAmountUSD | Valor de Ganho em USD | Todos |
| ganhandoDate | Data do ganho | Todos |
| earningExchangeRate | Taxa de câmbio utilizada para mostrar o montante correspondente de USD | Todos |
| earningId | Identificador único para cada ganho | Todos |
| ganhoSArtra | Taxa de incentivos aplicada no valor da transação para gerar um ganho | Todos |
| tipo de ganhos | Indica se é taxa, desconto, cooperativa, venda, e assim por diante | Todos |
| exchangeRateDate | Data de câmbio utilizada para calcular O Resultado Amount USD | Todos |
| externoReferênciaId | Identificador único para o programa | Programas direct Pay (incentivos e mercados) |
| externoReferenceIdLabel | Rótulo de identificador único | Programas direct Pay (incentivos e mercados) |
| instantâneoRebateAmount |  |  |
| faturaDate |  |  |
| faturaNumber | Número de fatura (aplicável apenas para empresa) | Incentivos e mercados - apenas alguns programas |
| última Procuração | Última moeda de pagamento (o campo estará vazio se não tiver sido pago nenhum pagamento prévio) |  |
| alavanca | Indica regra de negócio para o ganho | Todos |
| LicenciamentoProgramName | Nome do programa de licenciamento |  |
| LineItemId | Linha individual na fatura de um cliente |  |
| LocalProviderSeller | Fornecedor local/vendedor de registos |  |
| Mês de Maturidade | O mês de pagamento estimado | Todos |
| OrderId | Diz respeito à fatura de um cliente  | mercados |
| parentProductId | Identificador de produto único. Se não houver um produto-mãe para a transação, então iD do produto-mãe = ID do produto. | mercados |
| nome de produto parental | Nome do produto-mãe. Se não houver um produto-mãe para a transação, então o nome do produto principal = nome do produto. | mercados |
| participanteId | A identidade primária do parceiro que ganha ao abrigo do programa | Todos |
| ParticipanteIdType | Principalmente iD de programa para programas de incentivo e Vendedor IF para mercados | Todos |
| nome participante | Nome do parceiro de ganhos | Todos |
| partnerCountryCode | Localização/país/região do parceiro de ganhos | Todos |
| partNumber | Estará sempre em branco. | Alguns programas de incentivo e mercados |
| pagamentoId | Identificador único para o pagamento. Este número é geralmente visível no seu extrato bancário | Pagamentos SAP apenas |
| estatísticas de pagamentos | Estado dos pagamentos | Todos |
| subscrição de pagamentosSdededesimento | Descrição amigável do estado do pagamento | Todos |
| productId | Identificador de produto único | mercados |
| produtoName | Nome do produto ligado à transação | Todos |
| productType | Tipo de produto, como App, Add-on ou Game | mercados |
| Código do Programa | Cadeia para mapear com o nome do programa |  |
| programaName | Nome do programa de incentivo/loja | Todos |
| comprarOrderCoverageEndDate | Estará sempre em branco. | Programa de incentivos - CRI |
| comprarOrderCoverageStartDate | Estará sempre em branco. | Programa de incentivos - CRI |
| purchaseOrderType | Estará sempre em branco. | Programa de incentivos - CRI |
| comprarTypeCode | Estará sempre em branco. | Programa de incentivos - CRI |
| quantidade | Varia com base no programa. Indica quantidade faturada para programas transacionais | Todos |
| reasonCode |  |  |
| revendedorCountry |  |  |
| revendedorId | Identificador de revendedor | Incentivos - apenas alguns programas |
| revendedorName | Nome do revendedor |  |
| SkuId | SKU ID como definido durante a publicação. Uma oferta pode ter muitos SKUs, mas um SKU só pode ser associado a uma única oferta. Incentivos - apenas alguns programas |  |
| storeFee | O valor retido pela Microsoft como uma taxa para disponibilizar a app ou o addon na Loja | mercados |
| subscriçãoEndDate | Data de fim da assinatura | Incentivos - apenas alguns programas |
| subscriptionId | Identificador de assinatura associado ao cliente | Incentivos - apenas alguns programas |
| subscriçãoStartDate | Data de início da subscrição | Incentivos - apenas alguns programas |
| taxCity |  |  |
| imposto País |  |  |
| taxRemitModel | Parte responsável pela remessa de impostos (taxas de venda, utilização ou IVA/GST) | mercados |
| imposto Remetido | Montante dos impostos remetidos (taxas de venda, utilização ou IVA/GST) | mercados |
| taxState | Estado do cliente |  |
| taxZipCode | Código postal/postal do cliente |  |
| tpan | Indica a rede de anúncios de terceiros | mercados Anúncios apenas |
| transacçõesAmonte | Valor da transação na moeda de transação original com base no qual os ganhos são gerados | Todos |
| transactionAmountUSD | Valor da transação em USD | Todos |
| transacçãoCountryCode | Código país/região em que a transação aconteceu |  |
| transacçõesAcorrency | Moeda em que ocorreu a transação original do cliente (esta não é moeda de localização de parceiros) | Todos |
| transacçõesDate | Data da transação. Útil para programas onde muitas transações contribuem para um ganho | Todos |
| transacçãoExchangeRate | Data de câmbio utilizada para mostrar o valor correspondente da transação USD | Todos |
| transactionId | Identificador único para a transação | Todos |
| transactionPaymentMethod | Instrumento de pagamento do cliente utilizado para a transação, como Cartão, Faturação de Transportadora Móvel ou PayPal | mercados |
| tipo de transação | Tipo de transação, tais como compra, reembolso, reversão ou cobrança | mercados |
| workload | Carga de trabalho | Incentivos - apenas alguns programas |
|

## <a name="payments"></a>Pagamentos

A página **pagamentos** detalha o dinheiro que ganhou com a Microsoft. Também mostra quando e quanto te pagarão.

>[!Note]
> Para ser elegível para pagamento, as suas receitas devem atingir o limiar de [pagamento](payment-thresholds-methods-timeframes.md) de $50. Para obter mais informações, consulte o [Microsoft Publisher Agreement](https://go.microsoft.com/fwlink/?LinkID=699560).

:::image type="content" source="images/payouts/payments-overview.png" alt-text="Ilustra o ícone payout no canto superior direito do portal Partner Center":::

- **Total pago este ano** – O total combinado pago este ano, em dólares americanos, por todos os seus programas.
- **Próximo pagamento estimado** – O próximo pagamento que lhe chega (mesmo que haja outros em breve), em dólares americanos.
- **Último pagamento** – O valor (em dólares americanos), nome do programa e programa do seu pagamento mais recente.
- **Pagamento por fonte** – Montante de pagamentos (em dólares americanos), por programa, nos últimos 12 meses.

### <a name="payments-list"></a>Lista de pagamentos

A **tabela lista de pagamentos** mostra pagamentos pagos e pendentes. Você pode baixar informações sobre taxas de serviço em formato PDF e ver os detalhes de ganho para um dado pagamento.

:::image type="content" source="images/payouts/list-of-payments.png" alt-text="Ilustra o ícone payout no canto superior direito do portal Partner Center":::

- **Pago** – Todos os pagamentos enviados com sucesso. Escolha o ano no menu suspenso para filtrar os pagamentos lançados nesse ano.
- **Pendentes** – Próximos pagamentos.
- **Imposto sobre a taxa de serviço (formulário PDF)** – Disponível para os pagamentos sujeitos ao imposto sobre a taxa de serviço. Os impostos sobre a taxa de serviço são indicados em **Outros impostos.**
- **Ver** – Redirecionamentos para o histórico de transações com uma lista de ganhos incluídos no pagamento.

Para entender por que pode ter ganhos em falta ou inesperados, consulte [questões comuns sobre pagamentos de mercado comercial.](payout-faq.md#why-are-my-earnings-missing)

### <a name="payment-status"></a>Estado dos pagamentos

A tabela seguinte explica os diferentes estados de ganho.

| Estado de ganho | Razão | A ação do parceiro é necessária? |
| --- | --- | --- |
| Não processado | O ganho é elegível para pagamento. Permanece neste estado por um período de arrefecimento, conforme definido no guia do programa para o programa Incentivos. | No |
| A seguir | Ordem de pagamento gerada até revisões internas antes do pagamento ser processado. | No |
| Fatura fiscal pendente | A sua fatura fiscal é incompleta ou inválida. | Precisa atualizar a sua fatura fiscal antes de poder ser paga |
| Rejeitado durante a revisão | O pagamento foi rejeitado durante a revisão. | Contacte o suporte da Microsoft para obter mais detalhes |
| Com falhas | O pagamento falhou devido a um erro no sistema da Microsoft. | Contacte o suporte da Microsoft para obter mais detalhes |
| Em curso | O pagamento está em andamento. | No |
| Pagamento incorreto | A recuperação dos pagamentos está em curso. | No |
| Enviados | O pagamento foi enviado para o seu banco. | No |
| Reprocessamento | O pagamento encontrou um erro no sistema da Microsoft e está a ser reprocessado. | No |
| Invertido | O pagamento foi revertido pelo seu banco e será remetido no próximo ciclo de pagamentos. | No |
| Fatura fiscal rejeitada | A sua fatura fiscal foi rejeitada durante a revisão. Todos os pagamentos pendentes estarão suspensos até que a revisão da fatura fiscal esteja completa. | Contacte o suporte da Microsoft para obter mais detalhes |
| Fatura fiscal em análise | A sua fatura fiscal está a ser revista. O seu pagamento será liberado assim que a fatura do imposto tiver sido aprovada. | No |
| Rejeitado | O pagamento foi rejeitado pelo seu banco. | Contacte o seu banco para obter mais detalhes. |
|

### <a name="payments-download"></a>Transferência de pagamentos

Para ver mais detalhes sobre os seus pagamentos, selecione **Baixar** no topo da página. A tabela seguinte explica cada coluna do relatório.

| Nome da coluna | Descrição |
| --- | --- |
| id participante | A identidade primária do parceiro que ganha ao abrigo do programa |
| IDType participante | Normalmente programa ID para programas de incentivos e ID do vendedor para programas de loja |
| nome participante | Nome do parceiro de ganhos |
| programaName | Nome do programa de incentivos/loja |
| merecido | Valor auferido na moeda Pay To para esse programa/participanteID |
| earnedusd | Valor ganho para o ID do programa/participante, em USD |
| retidoTax | Montante do imposto retido na moeda Pay To para o programa/participanteID |
| salesTax | Montante total do imposto sobre as vendas na moeda Pay To para o programa/participanteID (aplicável apenas para programas de incentivos) |
| serviceFeeTax | Montante total do serviçoFeeTax em Moeda Paga para o programa/participanteID (aplicável apenas para programas de loja e apenas Azure Marketplace) |
| total de pagamento | Pagamento total em moeda local, excluindo a retenção na fonte e incluindo o imposto sobre as vendas (se aplicável) para o programa/participanteID |
| currencyCode | Pagar para código de moeda |
| pagamentoMethod | O método usado para pagar ao parceiro, por exemplo, transferência bancária eletrónica, nota de crédito |
| paymentID | Identificador único para o pagamento. Este número é geralmente visível no seu extrato bancário (aplicável apenas para pagamentos SAP). |
| estatísticas de pagamentos | Estado dos pagamentos |
| subscrição de pagamentosSdededesimento | Descrição amigável do estado do pagamento |
| pagamentoDate | O pagamento da data foi enviado da Microsoft |
|

## <a name="export-data"></a>Exportar dados

A página **de dados de exportação** não se atualiza por si só. Poderá ser necessário atualizar a página manualmente para ver os dados mais recentes. Selecione a partir dos três separadores para exportar o **histórico de transações,** **pagamentos,** **resumo de transações** ou **declaração histórica.**

O filtro pode resultar num erro **de não dados disponíveis.** Isto pode acontecer se deixar o período de tempo predefinido selecionado em três meses e, em seguida, selecionar um ID de pagamento de um ganho que está fora desse período. Se isto acontecer, expanda o seu período de tempo e tente novamente.

Aqui está uma amostra de pagamentos exportação:

:::image type="content" source="images/payouts/pc-export-payments.png" alt-text="Ilustra o ícone payout no canto superior direito do portal Partner Center":::

### <a name="historical-statements"></a>Declarações históricas

O resumo **dos dados relativos** às exportações também dá acesso a declarações históricas.

> [!NOTE]
> Uma afirmação histórica é um instantâneo e não é refrescada. Por favor contacte [o suporte](https://partner.microsoft.com/support/v2/?stage=1) e solicite os dados mais recentes, se necessário.

:::image type="content" source="images/payouts/pc-export-statements.png" alt-text="Ilustra o ícone payout no canto superior direito do portal Partner Center" na história moderna, exceto que exclui todos os ganhos com estatuto igual a "Pagamento Enviado".
- Filtros como 3M, 6M ou 12M não se aplicam à secção de declarações históricas.

### <a name="historical-statement-downloads"></a>Downloads de declarações históricas

A tabela seguinte explica cada coluna numa declaração histórica.

| Nome do campo | Descrição |
| --- | --- |
| Fonte de Receitas | A fonte das suas receitas com base no local onde ocorreu a transação, como a Microsoft Store, Windows Phone Store, Windows Store 8 ou publicidade |
| ID da Encomenda | Identificador de ordem único. Este ID permite identificar transações de compra com as respetivas transações não-compra, tais como reembolsos ou reembolsos. Ambos terão a mesma identificação de encomenda. Além disso, se houver uma taxa dividida em que foram utilizados vários métodos de pagamento para uma única compra, permite-lhe ligar as transações de compra. |
| ID de Transação | Identificador de transações único. |
| Data de Data de Transação | A data e a hora da transação ocorreu (UTC). |
| ID do produto parental | Identificador de produto único. Se não houver um produto-mãe para a transação, então iD do produto-mãe = ID do produto. |
| ID do Produto | Identificador de produto único. |
| Nome do produto principal | Nome do produto-mãe. Se não houver um produto-mãe para a transação, então o nome do produto principal = nome do produto. |
| Nome do Produto | Nome do produto |
| Tipo de Produto | Tipo de produto, como App, Add-on ou Game |
| Quantidade | Quando a Fonte de Receita é a Microsoft Store para Negócios, a Quantidade representa o número de licenças adquiridas. Para todas as outras Fontes de Receita, a Quantidade será sempre 1. Mesmo quando uma única transação é dividida em dois itens de linha porque foram utilizados dois métodos de pagamento diferentes, cada item de linha mostrará uma quantidade de 1. |
| Tipo de Transação | Tipo de transação, tais como compra, reembolso, reversão ou cobrança |
| Método de Pagamento | Instrumento de pagamento do cliente utilizado para a transação, como Cartão, Faturação de Transportadora Móvel ou PayPal |
| País / Região | País/região onde ocorreu a transação |
| Fornecedor Local / Vendedor | Fornecedor local/vendedor de registos |
| Moeda de Transação | Moeda da transação |
| Valor da Transação | Montante da transação |
| Imposto Remetido | Montante dos impostos remetidos (taxas de venda, utilização ou IVA/GST) |
| Recibos Líquidos | Valor de transação menos imposto remetido |
| Taxa de Loja | A percentagem de Recibos Líquidos retidos pela Microsoft como uma taxa para disponibilizar a app ou o addon na Loja |
| Receitas da App | Recibos líquidos menos a Taxa de Loja |
| Impostos Retidos | Montante do imposto sobre o rendimento retido (ot incluído no ficheiro CSV **reservado)** |
| Payment | A App Procede menos qualquer retenção na fonte de imposto sobre o rendimento aplicável (valor indicado em Moeda de Transação). Não incluído no ficheiro CSV **reservado.** |
| Taxa FX | Taxa cambial utilizada para converter moeda de transação em moeda de pagamento |
| Moeda de Pagamento | Moeda em que o seu pagamento é feito |
| Pagamento Convertido | Valor de pagamento convertido em Moeda de Pagamento utilizando a Taxa FX |
| Modelo de remessa fiscal | Parte responsável pela remessa de impostos (taxas de venda, utilização ou IVA/GST) |
| Data de elegibilidade | A data e a hora em que as transações prosseguem tornam-se elegíveis para pagamento (UTC). Quando um pagamento é criado, inclui receitas de transações com uma data de elegibilidade antes da data de criação do pagamento (apenas incluída no ficheiro CSV **reservado).** |
| Cobranças | Apresenta uma repartição de todos os detalhes de cobrança agregados na coluna Transaction Amount (apenas incluído para O Mercado Azure; não incluído no ficheiro CSV **reservado).** |
|||

## <a name="next-steps"></a>Passos seguintes

- [API de Pagamento de Parceiro](https://apidocs.microsoft.com/services/partnerpayouts)
- [Detalhes da política de dividendos](payout-policy-details.md)
- Para suporte à faturação, contacte o suporte de [editores](https://partner.microsoft.com/support/v2/?stage=1)de marketplace comercial.