---
title: Resumo das receitas no painel de instrumentos do Partner Center
description: Pode utilizar o resumo do Resumo das Receitas ver receitas e ganhos e exportar dados sobre quaisquer transações não elegíveis.
author: satinder37
ms.author: sabaja
ms.service: partner-dashboard
ms.topic: conceptual
ms.date: 10/04/2021
ms.custom: template-concept
customer intent: As an incentive user or incentive admin, I want to be able to read and export revenue data from Partner Center so I can see our earnings and learn why any transactions were reported ineligible.
ms.openlocfilehash: 9ec9d64127f537ac74615a8fbe17499ebb5872dd
ms.sourcegitcommit: cf8c78e0c8831371432007d5ab05f934f15a77b5
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/05/2021
ms.locfileid: "129528663"
---
# <a name="revenue-summary"></a>Resumo das receitas

Pode utilizar o resumo da Receita para entender como a receita gerada pelo consumo de clientes dos serviços Azure contribui para os seus ganhos, e por que algumas receitas podem ser determinadas não elegíveis para ganhos.

:::image type="content" source="images/revenue-summary/revenue-reporting-diagram.png" alt-text="Diagrama de como as receitas são avaliadas e reportadas no Partner Center":::

O resumo da Receita só é atualizado depois de avaliadas as transações, pelo que o consumo do Azure que ocorre em outubro só aparece no resumo das Receitas em novembro, por exemplo.

O resumo da Receita está no espaço de trabalho dos Pagamentos, juntamente com a página [de histórico de Transações](https://partner.microsoft.com/dashboard/payouts/reports/transactionhistory) e [Pagamentos.](https://partner.microsoft.com/dashboard/payouts/reports/incentivepayments)

## <a name="using-the-revenue-summary"></a>Usando o resumo da receita

Utilizando o resumo das receitas, pode:

- Procure receitas elegíveis, e o montante dos ganhos resultantes, por cliente ou subscrição.
- Complemente o que aprende com o histórico de [Transações](https://partner.microsoft.com/dashboard/payouts/reports/transactionhistory)  com insights sobre os montantes das receitas subjacentes.
- Procure qualquer receita não elegível e saiba a razão pela qual essa receita foi classificada como inelegível.
- Dados de exportação sobre transações não elegíveis, incluindo razões de [inelegibilidade](#ineligibility-reasons) e [atributos,](#exported-data-attributes)o que o ajuda a entender por que essas transações não ganharam incentivos.

## <a name="access-roles-and-permissions"></a>Funções e permissões de acesso

Os utilizadores de incentivos e os administradores de incentivo têm acesso ao resumo das Receitas.
A informação disponível no resumo depende das combinações do programa e da Microsoft Partner Network (MPN) a que os utilizadores e administradores têm acesso (tal como nas páginas de histórico de Transações e Pagamentos). (Ver [Atribuir funções e permissões](permissions-overview.md) para saber mais sobre a configuração dos utilizadores com funções e palavras-passe.)

## <a name="when-data-is-available"></a>Quando os dados estão disponíveis

Os dados do consumo do Azure são normalmente avaliados várias semanas após o mês em que ocorrem transações. A informação do resumo das receitas só é atualizada quando essa avaliação estiver concluída. Isto resulta num atraso entre quando as transações ocorrem e quando são reportadas, para que não possa ver o consumo para o mês em curso no resumo da Receita. Como exemplo, os dados relativos a março seriam normalmente avaliados na terceira semana de abril, e as informações de resumo das receitas seriam normalmente atualizadas pouco depois.

## <a name="customer-summary-view"></a>Vista sumária do cliente

A visão sumária do Cliente mostra receitas agregadas pelo nome do cliente e programa/noivado.

Os insights de resumo do cliente incluem:

- **O top 10 por receitas elegíveis** mostra os 10 melhores clientes que contribuem para o máximo de receitas elegíveis.
- **O top 10 por receitas não elegíveis** mostra os 10 melhores clientes que contribuem para o máximo de receitas não elegíveis.
- **O top 10 por ganhos** mostra os 10 melhores clientes a contribuir para o máximo de ganhos.

Pode procurar informações sobre qualquer cliente no resumo do cliente, e não apenas o top 10.

## <a name="eligible-transactions"></a>Transações elegíveis

*As transações elegíveis* são transações que produzem receitas elegíveis para pagamentos de ganhos.

Pode pesquisar informações sobre transações elegíveis por ID do cliente ou ID de assinatura. No entanto, não é possível exportar dados sobre transações elegíveis.

## <a name="ineligible-transactions"></a>Transações não elegíveis

*As transações não elegíveis* são transações que não são elegíveis para pagamentos de rendimentos.

- As razões pelas quais quaisquer transações são consideradas não elegíveis para ganhos estão listadas na secção de razões de [inelegibilidade](#ineligibility-reasons) deste artigo.
- Pode pesquisar e  [exportar dados](#exporting-data) sobre quaisquer transações não elegíveis para ajudá-lo a descobrir por que pode não ter ganho incentivos mcI.
- O resumo da Receita apresenta sempre a mais recente classificação de receitas (para que não possa ver como uma transação foi classificada um mês antes). Uma transação marcada como inelegível num mês poderia ser marcada como elegível no mês seguinte.

As transações não elegíveis listadas no resumo das Receitas têm atributos que incluem:

- produto
- Receitas não elegíveis
- [razão de inelegibilidade](#ineligibility-reasons)
- ID da subscrição
- nome do cliente (normalmente disponível após a faturação de uma subscrição)

Pode pesquisar transações não elegíveis pelo nome do cliente e iD de assinatura. (O número de registos apresentados é limitado a 10.) Se a informação que encontrar não responder às suas perguntas, contacte o suporte para ajuda.

## <a name="ineligibility-reasons"></a>Razões de inelegibilidade

*Razões* de inelegibilidade nas tabelas que se seguem indicam por que razão as receitas foram classificadas como inelegíveis para os ganhos. Cada linha nas tabelas também tem uma explicação sobre se e como um parceiro com ganhos não elegíveis pode tornar-se elegível novamente para ganhos.

Algumas razões de inelegibilidade nestas tabelas podem não ser aplicáveis a um determinado compromisso.

Existem três categorias de inelegibilidade:

- [Cliente inelegível](#ineligible-customer)
- [Parceiro não elegível](#ineligible-partner)
- [Transação não elegível](#ineligible-transaction)

### <a name="ineligible-customer"></a>Cliente inelegível

|Razão de inelegibilidade|A ação do parceiro é necessária?|Como voltar a ser elegível|
|---------|---------|---------|
|Cliente é setor público|Sim, se o cliente estiver nos Estados Unidos, Porto Rico ou Índia|Se respondeu a um pedido de prova de execução (POE) e foi rejeitado, não pode voltar a ser elegível. (Quando um POE é rejeitado, o e-mail é enviado explicando porquê.)<br><br>Pode solicitar outro POE no prazo de 90 dias a contar da data de transação/ganho. (Certifique-se de confirmar a receção do e-mail POE quando chegar.) Também pode contestar a inelegibilidade no prazo de 90 dias, contactando o suporte com a razão de inelegibilidade, informação de subscrição e cliente, e razão de litígio.|
|Receitas da China não devem pertencer a parceiro não-China|No|O parceiro não pode voltar a ser elegível por política.|

### <a name="ineligible-partner"></a>Parceiro não elegível

|Razão de inelegibilidade|Ação do parceiro necessária|Como voltar a ser elegível|
|---------|---------|---------|
|Requisito avançado de especialização não cumprido|Yes|[Conheça as especializações avançadas](advanced-specializations.md)|
|Estatuto de competência não cumprido ou caducado|Yes|Veja o seu estatuto de competência nas [Competências.](https://partner.microsoft.com/pcv/partnership/competencies) Veja as competências necessárias para o seu envolvimento na [Incentives Engagements](https://partner.microsoft.com/dashboard/incentives/engagements/ux)|
|Acordo mpa expirou ou não assinou|Yes|Verifique e assine o acordo mpa por orientação sobre [o Acordo de Parceiro da Microsoft para parceiros de programas CSP](microsoft-partner-agreement.md)|
|Co-venda de elegibilidade expirada ou não estabelecida|Yes|Ver [Co-vender com equipas de vendas da Microsoft e visão geral dos parceiros](/azure/marketplace/co-sell-overview)|
|A localização do parceiro não é elegível para incentivos|No|Parceiro não pode voltar a ser elegível por política|
|MPN ID não elegível para participar no noivado|No|Parceiro não pode voltar a ser elegível por política|

### <a name="ineligible-transaction"></a>Transação não elegível

|Razão de inelegibilidade|A ação do parceiro é necessária?|Como voltar a ser elegível|
|---------|---------|---------|
|A prova de execução não é aprovada|Sim, se não respondeu a um parceiro digital de prova de execução exigida (POE) da Microsoft|O pedido de prova de execução é aplicável apenas para o sector público ou para a DPOR. A partir de 1 de outubro de 2021, a DPOR já não é incentivada para o Azure, pelo que os pedidos de POE não são enviados.<br><br>Se respondeu ao e-mail com o tema "Prova de execução necessária" e a sua resposta foi rejeitada, não pode voltar a ser elegível.|

## <a name="exporting-data"></a>Exportar dados

Você pode baixar informações sobre transações não elegíveis (mas não elegível) no resumo do Rendimento.

:::image type="content" source="images/revenue-summary/export-data-page.png" alt-text="Screenshot da página de dados de exportação no Partner Center":::

### <a name="exported-data-attributes"></a>Atributos de dados exportados

Os atributos de transações não elegíveis incluem:

|Nome do atributo  |Description  |
|---------|---------|
|agreementNumber|Número do contrato (disponível apenas conforme aplicável)|
|customerId|Identidade do cliente associado a uma subscrição/recurso. (Para o consumo do Azure, esta informação não está disponível para os primeiros 30 a 45 dias de uma nova subscrição, a menos que a primeira fatura tenha sido criada.)|
|CustomerIdType|TPID ou ID MCAPI|
|nome do cliente|Nome do cliente|
|faturaNumber|Número de fatura (disponível apenas para parceiros, liderados por campo e orientados pelo cliente)|
|partnerCountryCode|Localização MPN inscrita|
|partnerId|ID MPN do parceiro inscrito|
|nome parceiro|Nome do parceiro|
|productId|Nome do produto do comércio|
|produtoAmily|Família de produtos|
|reason|Razão para a inelegibilidade|
|subscriptionId|ID da subscrição|
|transacçãoAmountUSD|Valor do consumo em dólares americanos|
|transacçõesDate|Data de consumo ou faturação
|não merecidoId|Identificador único que pode ajudá-lo a criar um inquérito de apoio|
|workload|Nome de serviço ou nome da carga de trabalho|

## <a name="next-steps"></a>Passos seguintes

Para obter mais informações sobre transações, receitas, ganhos e pagamentos, consulte os seguintes artigos.

- Consulte a página [de histórico de Transações](https://partner.microsoft.com/dashboard/payouts/reports/transactionhistory) para ver os resultados e os detalhes de transações associados para todos os seus programas com o respetivo estado de pagamento.
- Consulte a [página pagamentos](https://partner.microsoft.com/dashboard/payouts/reports/incentivepayments) para ver os pagamentos concluídos e pendentes de todos os seus programas.
- Consulte a página [de declarações do Payout](payout-statement.md) para obter uma visão geral dos seus pagamentos a partir de ofertas vendidas através do mercado comercial.
