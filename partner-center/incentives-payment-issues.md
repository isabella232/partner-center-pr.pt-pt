---
title: Resolver problemas de pagamentos e ganhos
ms.topic: article
ms.date: 02/05/2021
description: Saiba como resolver problemas como ganhos em falta ou incorretos, problemas de elegibilidade e como conciliar os seus ganhos de incentivos.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.openlocfilehash: 971b053119a263ed5c7f8e25fb532b4137e1cb13
ms.sourcegitcommit: 2d1f0d7bc897278ef37af6d43c1a088f5ca14807
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/08/2021
ms.locfileid: "99834888"
---
# <a name="troubleshooting-missing-payments-incorrect-earnings-and-other-issues"></a>Resolução de problemas em falta de pagamentos, ganhos incorretos e outras questões

**Aplica-se a:**

- Partner Center

**Funções adequadas:**

- Administradores de incentivos

Este artigo irá ajudá-lo a resolver quaisquer problemas de ganhos ou pagamentos no seu programa de incentivos. Os tópicos abordados incluem o tempo de pagamento, a verificação da elegibilidade dos seus ganhos e a importância de configurar corretamente os seus perfis de pagamento e impostos.

## <a name="who-can-create-or-update-payout-and-tax-profiles-for-my-organization"></a>Quem pode criar ou atualizar o pagamento e os perfis fiscais para a minha organização?

Os utilizadores que tenham o papel de administrador de incentivo no Partner Center para o programa de incentivos relevante e a localização mpn podem atualizar e ver o pagamento e os perfis fiscais para a organização.

## <a name="how-long-does-it-take-for-microsoft-to-approve-my-pending-payout-andor-tax-profiles"></a>Quanto tempo demora a Microsoft a aprovar os meus perfis de pagamento e/ou fiscais pendentes?

A validação pode demorar até 48 horas. Durante este período, o estado do perfil na página Descrição geral será apresentado como A validar a inscrição. Uma vez concluído o processo, o estado mostrará como **matriculado** se for bem sucedido, ou **Ação Necessária – Atualizar pagamento e/ou detalhes fiscais,** se necessário.

## <a name="how-do-i-know-if-i-have-completed-my-payout-and-tax-profile-correctly"></a>Como sei se preenchi corretamente o meu perfil de pagamento e perfil fiscal?

O estado da inscrição é apresentado na página Descrição geral. Quando terminar de criar os seus perfis, o seu estado será **validar a inscrição.** Assim que validarmos a sua informação, o seu estado muda para **Inscrição.** Este estado indica que o seu perfil de pagamento e de impostos e a sua inscrição foram concluídos com sucesso.

## <a name="why-do-i-need-to-update-my-tax-profile-to-use-it-with-a-new-incentive-program"></a>Por que preciso de atualizar o meu perfil fiscal para o utilizar com um novo programa de incentivos?

Pagamos incentivos a partir de diferentes localizações, dependendo do tipo de incentivo. Estas diferentes localizações podem exigir informações fiscais adicionais, com base nas regras do programa de incentivos, para que o processo decorra de forma correta.

## <a name="how-can-i-delete-a-payment-andor-tax-profile"></a>Como posso eliminar um perfil de pagamento e/ou fiscal?

Atualmente, a Microsoft não suporta a opção de eliminar os perfis de pagamento e perfis fiscais existentes.

## <a name="my-payment-is-missing-or-incorrect"></a>O meu pagamento está em falta ou incorreto.

Os pagamentos em falta ou incorretos devem-se frequentemente a um dos seguintes motivos:

- **Pode não ser elegível.**  Os ganhos só estarão disponíveis se cumprir os Requisitos de Elegibilidade Operacionais, ou seja, se se tiver inscrito no respetivo período de ganhos do programa.
- **Pode não ter cumprido os requisitos.**  Verifique se cumpriu as regras de elegibilidade e de receitas elegíveis correspondentes ao incentivo que procura.

  **Para verificar a sua elegibilidade**

  1. Inscreva-se nos [incentivos do Parceiro](https://partner.microsoft.com/membership/partner-incentives).

  2. Percorra os documentos do seu programa.
  
  3. Selecione o link de documento que deseja e, em seguida, reveja as secções 

**Elegibilidade do parceiro** e **regras de receitas elegíveis.**

- **O seu perfil de pagamento pode estar incompleto.** Your incentive earnings start date will be the first day of the month in which you’ve completed all of the eligibility requirements, including onboarding with payout and tax details. Os ganhos não estarão disponíveis nos meses anteriores ao preenchimento dos dados de pagamento e fiscais. Por exemplo, se completar todos os requisitos durante o mês de abril de 2020, a data de início dos ganhos será 1 de abril de 2020.
- **Pode ter uma ação excecional.**  Os incentivos podem não estar a ser processados por existir uma ação pendente associada.

  **Para ver as suas ações pendentes**

  1. Inscreva-se nos [incentivos do Parceiro](https://partner.microsoft.com/membership/partner-incentives).
  2. Abra a página **de histórico de transações.** Reveja os campos desta página para que quaisquer ações pendentes sejam concluídas, tais como **o perfil de Imposto Pendente,** o perfil de pagamento **pendente,** ou **a submissão pendente da fatura fiscal.**

Se estas ações não ajudarem e os seus pagamentos continuarem em falta ou incorretos, [contacte o suporte](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives).

## <a name="how-can-i-reconcile-my-adjustments"></a>Como posso reconciliar os meus ajustes?

Pode localizar e conciliar os seus ajustes descarregando os seus dados de ganhos e transações.

1. Inicie sessão no [dashboard do Centro de Parceiros](https://partner.microsoft.com/dashboard/).
2. Na barra de navegação superior, selecione o ícone do dinheiro e, em seguida, selecione **o histórico de Transações**.
3. Aplique os filtros apropriados. (Ver a nota **importante** abaixo.)
4. Depois de filtrar os seus dados, selecione **Iniciar o download** e, em seguida, selecione **dados de Exportação**. Os seus dados serão abertos num ficheiro CSV.
5. No ficheiro CSV, navegue para a Coluna P, **Tipo De Ganho**.
6. Filtrar esta coluna para **o Ajuste-Redução**. Pode ver o mês de cada ajuste na Coluna S.

>[!IMPORTANT]
>Os ajustamentos aplicados aos períodos de ganhos anteriores não serão visíveis nos ganhos do mês em que o ajustamento foi aplicado. Os ajustamentos refletir-se-ão sempre no relatório de resultados do mês a que o ajustamento foi aplicado.
>
>Por exemplo, um ajustamento para janeiro de 2019 que foi processado em setembro de 2019 não vai refletir no valor dos ganhos de setembro de 2019. No entanto, quando o pagamento de setembro de 2019 for recebido, incluirá o ajustamento para janeiro de 2019 que foi aplicado em setembro. Neste cenário, você precisaria de baixar os detalhes da transação para janeiro de 2019 para ver o ajuste que foi aplicado.
>
>Tenha isto em mente quando definir os filtros da data. Como acima referido, os ajustamentos relativos a períodos anteriores só serão visíveis no mês em que o ajustamento foi aplicado. Verifique duas vezes se o intervalo de datas selecionado corresponde ao mês do ajuste que está a tentar localizar. Pode ser necessário selecionar **Limpar tudo** para remover os filtros e, em seguida, aplicar os novos.

## <a name="why-are-my-co-op-claim-payments-made-in-two-different-currencies"></a>Porque é que os meus pagamentos de pedidos de cooperação são feitos em duas moedas diferentes?

Quando os fundos de cooperação são obtidos por diferentes entidades da Microsoft, os pagamentos são feitos na moeda local de cada entidade.  

## <a name="why-was-i-paid-in-a-currency-other-than-my-co-op-claim-currency"></a>Por que me pagaram numa moeda diferente da minha moeda do pedido de cooperação?

Cada programa de incentivos tem um perfil bancário que foi criado durante a configuração. A moeda especificada nesse perfil é a moeda na qual receberá os pagamentos.

## <a name="i-dont-see-earnings-for-a-certain-period"></a>Não vejo ganhos por um certo período.

Quando não se vê ganhos para um período em que são esperados, é geralmente devido a uma das seguintes questões:

- **Pode não ser elegível.**  Os ganhos só estarão disponíveis se cumprir os Requisitos de Elegibilidade Operacionais, ou seja, se se tiver inscrito no respetivo período de ganhos do programa.

- **O seu perfil de pagamento pode estar incompleto.**  Your incentive earnings start date will be the first day of the month in which you’ve completed all of the eligibility requirements, including onboarding with payout and tax details. Os ganhos não estarão disponíveis nos meses anteriores ao preenchimento dos dados de pagamento e fiscais. Por exemplo, se completar todos os requisitos durante o mês de abril de 2020, a data de início dos ganhos será 1 de abril de 2020.

Se tiver cumprido os requisitos de elegibilidade, incluindo embarque com pagamento e detalhes fiscais a tempo, e os ganhos ainda estiverem em falta, [suporte de](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives)contato .

## <a name="my-earnings-are-missing-or-incorrect"></a>Os meus ganhos estão em falta ou incorretos.

Os ganhos em falta ou incorretos podem ser causados por um dos seguintes problemas:

- **Pode não ter cumprido os requisitos.**  Verifique se cumpriu as regras de [elegibilidade](#my-payment-is-missing-or-incorrect) e de receitas elegíveis correspondentes ao incentivo que procura.

- **Pode existir uma discrepância.**  Se cumprir os [requisitos](incentives-confirm-your-earnings-eligibility.md) de [elegibilidade](incentives-determined-your-program-eligibility.md) do programa e os seus ganhos ainda parecem estar incorretos, as seguintes informações podem ajudá-lo a recuperar os seus dados.

Os ganhos são apresentados tanto na página de histórico de **Transações** como na página **Pagamentos.** Pode aceder a ambas as páginas selecionando o ícone **Payout** na barra de navegação no Partner Center.

:::image type="content" source="images/incentives/paymenticon.png" alt-text="Informações sobre transações":::

Os valores de ganho mensal na vista do histórico de transações podem não estar alinhados com o valor de pagamento recebido por um mês específico. Tal deve-se a recálculos e ajustamentos relativos a períodos de ganhos anteriores que são aplicados a pagamentos futuros.

Por exemplo, um ajustamento para janeiro de 2019 que foi processado em setembro de 2019 não se refletirá no valor dos proveitos de setembro de 2019; no entanto, quando o pagamento de setembro de 2019 for recebido, incluirá o ajustamento para janeiro de 2019 que foi aplicado em setembro.

Neste cenário, você precisaria de baixar os detalhes da transação para obter uma visão completa de todos os ganhos incluídos no seu pagamento.  Além disso, pode navegar para a vista pagamentos para descarregar transações para cada pagamento.

### <a name="transaction-history"></a>Histórico de transações

Esta visão mostra as tendências de ganhos e pagamentos por mês, ganhos por estado e detalhes de transação, juntamente com o estado de pagamento de cada transação. Os dados só são visíveis para os programas e IDs MPN para os quais é um utilizador de incentivo ou administrador.

### <a name="payments"></a>Pagamentos

Esta vista permite-lhe visualizar pagamentos para todos os programas e IDs MPN. Os dados só são visíveis para os programas e IDs MPN para os quais é um utilizador de incentivo ou administrador. A partir desta vista, você pode baixar remessas ou ver detalhes de transação por pagamento.

| Para efetuar isto | Clique aqui |
| ------ | :----------- | 
| Consulte as suas informações de pagamento por linha, incluindo valores de ganhos e pagamentos em moeda local  | Consulte o campo **Lista de Pagamentos**   |
| Faça o download de uma carta de remessa   |  Selecione remessa **de pagamento**  |
| Ver detalhes do nível de transação para um pagamento específico |  Selecione **Ver**  |
| Detalhes de transações de exportação para o Excel  |  Selecione **Iniciar o download** e, em seguida, clique em **Dados de Exportação**. Note que todos os filtros selecionados serão aplicados aos dados exportados. Uma vez alterado o estado para Completed, selecione **Download** e siga as instruções para exportar o relatório de transações detalhadas. Refresque a página se o estado não for atualizado dentro de cinco minutos.  |

### <a name="missing-or-incorrect-earnings-and-payments"></a>Ganhos e pagamentos em falta ou incorretos

Se não conseguir localizar um pagamento ou dados de transação, verifique se aplicou os filtros corretos. Note que uma vez que alguns nomes do programa mudaram (por exemplo, CSP 1T Direct Partner é agora CSP Direct Bill Partner), poderá ter de utilizar várias seleções.

Se ainda não conseguir encontrar os seus ganhos ou acreditar que os ganhos apresentados estão incorretos, contacte [o Support](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives).

## <a name="how-do-i-reconcile-my-earnings"></a>Como posso conciliar os meus ganhos?

Se existir alguma discrepância nos ganhos, execute os seguintes passos:

1. **Verifique se é elegível para ganhos**.  Os ganhos só estarão disponíveis se cumprir a [elegibilidade](incentives-determined-your-program-eligibility.md) do programa e [a elegibilidade dos ganhos.](incentives-confirm-your-earnings-eligibility.md)

2. **Verifique se o perfil de pagamento está completo.**  Your incentive earnings start date will be the first day of the month in which you’ve completed all of the eligibility requirements, including onboarding with payout and tax details. Os ganhos não estarão disponíveis nos meses anteriores ao preenchimento dos dados de pagamento e fiscais. Por exemplo, se completar todos os requisitos durante o mês de abril de 2020, a data de início dos ganhos será 1 de abril de 2020. 

3. **Verifique se cumpriu os requisitos.**  Verifique se cumpriu as regras de [elegibilidade](#my-payment-is-missing-or-incorrect) e receitas elegíveis para o seu programa de incentivos.

Se estas ações não ajudarem e os seus ganhos ainda não forem reconciliados, contacte [o Support](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives).

## <a name="where-can-i-find-my-rates"></a>Onde posso encontrar as minhas tarifas?

1. Inscreva-se nos [incentivos do Parceiro](https://partner.microsoft.com/membership/partner-incentives).

2. Percorra para baixo para aceder aos documentos do seu programa.

3. Selecione o link do documento para o respetivo programa.

4. No documento, consulte a **estrutura e tarifas** do programa de secção .

## <a name="next-steps"></a>Passos seguintes

- [Gerir queixas de co-op](incentives-managing-co-op-claims.md)