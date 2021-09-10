---
title: Visão geral da faturação do Partner Center
ms.topic: article
ms.date: 01/28/2021
description: Aprenda informações básicas de faturação e fatura para parceiros CSP no Partner Center. Inclui como cobrar aos clientes e como encontrar e ler a sua fatura.
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
author: sodeb
ms.author: sodeb
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: f594b7d39234080e2c3f99c05a2e64fdaa18f0dd
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/09/2021
ms.locfileid: "123960050"
---
# <a name="billing-overview-for-csp-program-partners-working-in-partner-center"></a>Descrição geral da faturação para parceiros do programa CSP que trabalham no Centro de Parceiros 

**Funções adequadas**: Agente administrador | Administrador de faturação | Administração global | Agente helpdesk | Agente comercial

Este artigo fornece a informação básica de faturação e fatura para parceiros CSP no Partner Center, incluindo como faturar os clientes e como encontrar e ler a sua fatura.


## <a name="find-your-bill"></a>Encontre a sua conta

Para encontrar a sua conta:

1. Inicie sessão no [dashboard](https://partner.microsoft.com/dashboard/home) do Centro de Parceiros.

2. No menu Partner Center, escolha **Faturação.**

3. Na página **de Faturação,** você pode baixar a sua conta mais recente ou baixar as contas anteriores na secção de histórico de **Faturação.**

## <a name="bill-your-customers"></a>Cobrar os seus clientes

A Microsoft não tem requisitos nem condições sobre a forma como lida com a sua própria faturação.

Para determinar a utilização de um cliente, consulte os seus ficheiros de [reconciliação](#find-your-bill). Utilize o nome do cliente e outros campos relevantes para determinar a utilização.

### <a name="billing-types"></a>Tipos de faturação

Os tipos de faturação no Partner Center incluem **faturação baseada em licenças,** **faturação baseada em uso** e **faturação única.** 

### <a name="billing-currency"></a>Moeda de faturação

**Faturação baseada em licenças e com base em uso**: Você será cobrado para produtos(s) na moeda do país ou região em que você está localizado. É cobrado o mesmo independentemente da localização do cliente a quem vendeu o produto.

**Faturação única**: A partir de agosto de 2021, todos os parceiros serão faturados na moeda de localização do parceiro, independentemente da localização do cliente a quem vendeu o produto. Leia mais sobre [uma vez e recorrente.](azure-plan-billing.md) 

## <a name="invoices"></a>Faturas

A sua fatura é um resumo de todos os encargos relativos ao período de faturação em curso. Isto inclui taxas em todo o programa, todos os produtos e todos os clientes. Por exemplo, cenários de faturação mensal e anual, consulte [cenários comuns de faturação](common-billing-scenarios.md)

Para a faturação baseada na utilização e na licença, a fatura fica disponível no prazo de dois (2) dias da data de faturação selecionada no fuso horário UTC. Por exemplo, se tiver uma data de faturação de 12 de setembro, o processo de geração de faturas começará às 00:00 UTC no dia 13 e completará até às 00:00 UTC no dia 14. 

Para a faturação única e recorrente, o período de faturação está alinhado com o mês de calendário e a fatura/ficheiros de reconciliação estarão disponíveis, o mais tardar, no 8.º dia de cada mês. Para mais informações leia [a faturação do plano Azure.](azure-plan-billing.md) 

## <a name="price-lists"></a>Listas de preços

As listas de preços são atualizadas mensalmente. As listas de preços de pré-visualização estão disponíveis com um (1) mês de antecedência.

Para ver os mais recentes programas e ofertas de Fornecedor de Soluções em Nuvem, a partir do painel de instrumentos do Portal dos **Parceiros,** vá ao Sell > Preços e Ofertas . Encontrará listas de preços separadas para os diferentes tipos de produtos disponíveis. As seguintes listas de preços estão disponíveis na página **de Preços e Ofertas:**

Os preços **baseados na licença** são garantidos para o prazo da subscrição, geralmente 12 meses a partir da data de compra. 

**Os preços baseados na utilização** podem ser alterados mensalmente.

**Os preços dos produtos, serviços e subscrições de software** são garantidos através da duração da subscrição. No entanto, os preços podem mudar quando renovar.

Verá **ajustes** e **créditos** em atraso na sua próxima fatura de faturação após a aplicação do crédito ou ajuste.

## <a name="payment-terms"></a>Termos de pagamento

As condições de pagamento são líquidas de 60 dias. As faturas devem ser pagas pela data de vencimento da fatura (60 dias após a data de faturação), ou a sua conta será delinquente, o que poderá ter impacto na sua inscrição na CSP. 

Pode recuperar a funcionalidade completa das suas contas suspensas quando pagar o valor devido do passado.

Uma vez fornecidas as informações de faturação corrigidas, o seu pagamento será visível na página de faturação do Partner Center no prazo de 5 dias úteis.

### <a name="taxes-and-vat"></a>Impostos e IVA

É tributado com base nos seus dados (não nos detalhes dos seus clientes) porque a relação de faturação é entre a Microsoft e você. Pode submeter o seu identificador de impostos durante o processo de configuração da conta ou através de um pedido de apoio mais tarde. Verá as mudanças refletidas no seu próximo ciclo de faturação.

Para **retenção na fonte e isenção de imposto sobre vendas,** deve apresentar documentação fiscal através de um pedido de apoio. Você verá as alterações e reembolsos apropriados no seu próximo ciclo de faturação. Saiba mais informações sobre [a submissão de impostos sobre retenção na fonte.](withholding-tax-credit-form.md) 

Para **isenção de imposto sobre o valor acrescentado (IVA),** deve submeter o seu ID de IVA (validado pela Microsoft) através de um pedido de serviço.  Se o ID do IVA for submetido após a configuração da conta (através de um pedido de apoio), as suas faturas anteriores a esse pedido não terão um ID de IVA carimbado na fatura PDF. Verá as mudanças no seu próximo ciclo de faturação.

Pode encontrar mais detalhes fiscais do seu fisco local ou consultor fiscal.

### <a name="adjustmentscreditscancellations"></a>Ajustes/Créditos/Cancelamentos

Os créditos de cancelamento de serviços licenciados são pro-rated para dias não reutilizados para cancelamentos de meio ciclo (assim como diminui a licença de acordo com esta fórmula:

[ROUND((ROUND(Preço unitário * Quantidade / Número de dias no mês pró-nominal, 2) * Número de dias pró-avaliados) / Quantidade, 2) * Quantidade] 

A Microsoft não cobra taxas de rescisão antecipada pelo cancelamento de serviços baseados em licenças.

### <a name="billing-rules"></a>Regras de faturação

Existem hoje dois tipos de frequências de faturação: Anual & Monthly.  
As taxas de serviço medidos podem ser alteradas dentro do ciclo da fatura.

#### <a name="annual-billing-rules"></a>Regras anuais de faturação 

- As assinaturas são anuais e autorrenovadas.  

- A faturação está em 12 pagamentos mensais ou um pagamento anual por subscrição anual. 

- É cobrado com antecedência para o próximo período de faturação de serviços baseados em licenças, com base no número de licenças no final do período de faturação anterior. 

- Você é cobrado/creditado em atraso para quaisquer alterações no número de licenças (cálculo pró-rata com base em dias de licença). Pro-rata utiliza a seguinte fórmula: 

  - [ROUND((ROUND(Preço unitário * Quantidade / Número de dias no mês pró-nominal, 2) * Número de dias pró-avaliados) / Quantidade, 2) * Quantidade] 

- Os pagamentos são cobrados para licenças vendidas, não para licenças provisões 

#### <a name="monthly-billing-rules"></a>Regras mensais de faturação 

- As subscrições são mensais e renovam-se automaticamente com as novas taxas de serviço medidos. É cobrado todos os meses pelo uso do mês anterior. 

- As taxas de serviço medidos podem ser alteradas dentro do ciclo da fatura. 

- A fatura que receber só terá os encargos que são acumulados para esse mês. 


### <a name="credit-notes"></a>Notas de crédito

Poderá ter de solicitar um crédito ou rebill pelas seguintes razões:

- Tem de fazer correções de morada ou de compra.
- Foi aplicada uma restituição fiscal após a geração da fatura. Você pode solicitar um crédito ou rebill para obter o reembolso de imposto reenusado de volta para a fatura original. O mesmo se aplica também aos reembolsos. Você pode solicitar um crédito ou rebill da fatura original, em seguida, puxar um reembolso.

**Para todas as transações pontuais e recorrentes,** a Microsoft pode emitir uma nota de crédito quando solicitar um crédito ou um rebill. A fatura é cancelada quando o crédito é emitido. 

## <a name="next-steps"></a>Passos seguintes

- [Compreenda o seu projeto de lei e arquivo de reconciliação](read-your-bill.md)
- [Cenários comuns de faturação para parceiros do programa CSP](common-billing-scenarios.md)
- [Change billing frequency](common-billing-scenarios.md) (Alterar a frequência de faturação)
- [Histórico de pedidos de clientes](csp-offers.md) 
- [Preços e ofertas](pricing-and-offers.md)
