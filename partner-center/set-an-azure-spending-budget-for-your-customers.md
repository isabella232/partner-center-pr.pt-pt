---
title: Definir um orçamento de despesas do Azure para os clientes
ms.topic: how-to
ms.date: 09/27/2021
description: Saiba como definir ou remover orçamentos mensais de gastos do Azure para os seus clientes, e também para ver os dados de gastos do Azure e definir notificações relacionadas com o orçamento.
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: add447f6d9b0332bea9bbddd0ccf66efc5e146fd
ms.sourcegitcommit: e1da62b36420d78bf44e3962358d0af65ebc3402
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/27/2021
ms.locfileid: "129088778"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a>Desconfiem, verifiquem ou removam os orçamentos mensais de gastos da Azure para os clientes no Partner Center

**Funções adequadas**: Agente administrativo

Pode definir um [orçamento mensal de gastos da Azure](#set-azure-spending-budget) para os seus clientes no Partner Center. Isto ajuda os seus clientes a gerir os seus gastos com o Azure. Esta opção permite comparar os gastos do Azure dos seus clientes com o orçamento durante o mês. Também ajuda os seus clientes a orçamentar os seus gastos com o Azure para que a sua fatura mensal não seja maior do que antecipam.

> [!NOTE]  
> Esta função não está disponível nas contas sandbox ou Test in Production (TIP).

Depois de definir um orçamento de gastos Azure para o seu cliente, também pode rever o uso do cliente. Estas opções podem ajudá-lo a detetar serviços mal configurados ou tendências incomuns que possam sugerir fraude. Em seguida, pode trabalhar com o(s) cliente(s) para identificar a causa raiz e gerir os custos. Se necessário, também pode alterar o orçamento do cliente para um valor mais elevado.

## <a name="azure-spending-data"></a>Dados de gastos do Azure

Os dados de gastos do Azure são uma *estimativa* e *os valores reais de faturação podem variar*. O valor dos dados *não reflete* impostos, créditos, ajustes ou outros encargos que possam ser aplicados.

Os dados de gastos são *atualizados uma vez por dia.* Os seus clientes podem continuar a utilizar (e ser cobrados) serviços e recursos da Azure, a menos que altere as definições da sua conta no portal Azure.

## <a name="set-azure-spending-budget"></a>Definir orçamento de gastos do Azure

> [!NOTE]
> Para saber mais sobre a interface de espaços de trabalho, consulte [o Centro de Parceiros.](get-around-partner-center.md#turn-workspaces-on-and-off)

#### <a name="workspaces-view"></a>[Vista de espaços de trabalho](#tab/workspaces-view)

Pode *definir um orçamento mensal de gastos da Azure* para vários clientes no Partner Center:

1. Inicie sessão no [dashboard do Centro de Parceiros](https://partner.microsoft.com/dashboard/).

2. Selecione o **azulejo de Faturação** e, em seguida, escolha **os gastos do Azure**.

3. Na página de gastos do **Azure,** em **Clientes com Microsoft Azure subscrições,** selecione os clientes(s) para os quais pretende definir um orçamento.

4. Introduza um valor para **o orçamento mensal.**

5. Escolha **Aplicar** para guardar as suas alterações.

Pode *definir um orçamento para um cliente individual* nas suas definições de subscrição.

1. Inicie sessão no [dashboard do Centro de Parceiros](https://partner.microsoft.com/dashboard/).

2. Selecione **o** azulejo cliente.

3. Na página **Clientes,** selecione o **nome da Empresa** do cliente.

4. Na página de **Subscrições** do cliente, na **subscrição baseada em utilização,** escolha **o orçamento change**.

5. Insira um valor para o orçamento.

6. Escolha **Aplicar** para guardar as suas alterações.

Pode *remover um orçamento mensal de gastos da Azure* para os seus clientes no Partner Center.

1. Inicie sessão no [dashboard do Centro de Parceiros](https://partner.microsoft.com/dashboard/).

2. Selecione o azulejo **de Faturação** e, em seguida, selecione **gastos do Azure**.

3. Na página de gastos do **Azure,** em **Clientes com Microsoft Azure subscrições,** selecione os clientes(s) cujo orçamento pretende remover.

4. Escolha **Remover orçamento**.

Pode *acompanhar os gastos atuais do Azure e os orçamentos mensais dos seus clientes a* qualquer momento.

1. Inicie sessão no [dashboard do Centro de Parceiros](https://partner.microsoft.com/dashboard/).

2. Selecione o azulejo **de Faturação** e, em seguida, selecione **gastos do Azure**.

3. Na página de gastos do **Azure,** em **Clientes com Microsoft Azure subscrições,** pode ver uma visão geral dos orçamentos mensais dos clientes, estimativas correntes de gastos e percentagem do orçamento utilizado.

#### <a name="current-view"></a>[Vista atual](#tab/current-view)

Pode *definir um orçamento mensal de gastos da Azure* para vários clientes:

1. Inicie sessão no [dashboard do Centro de Parceiros](https://partner.microsoft.com/dashboard/).

2. No menu à esquerda em **CSP,** escolha **os gastos do Azure**.

3. Na página de gastos do **Azure,** em **Clientes com Microsoft Azure subscrições,** selecione os clientes(s) para os quais pretende definir um orçamento.

4. Introduza um valor para **o orçamento mensal.**

5. Escolha **Aplicar** para guardar as suas alterações.

Pode *definir um orçamento para um cliente individual* nas suas definições de subscrição.

1. Inicie sessão no [dashboard do Centro de Parceiros](https://partner.microsoft.com/dashboard/).

2. No menu à esquerda em **CSP,** escolha **Clientes**.

3. Na página **Clientes,** selecione o **nome da Empresa** do cliente.

4. Na página de **Subscrições** do cliente, na **subscrição baseada em utilização,** escolha **o orçamento change**.

5. Insira um valor para o orçamento.

6. Escolha **Aplicar** para guardar as suas alterações.

**Remover orçamento de gastos do Azure**

Pode *remover um orçamento mensal de gastos da Azure* para o seu cliente(s) no Partner Center:

1. Inicie sessão no [dashboard do Centro de Parceiros](https://partner.microsoft.com/dashboard/).

2. No menu à esquerda em **CSP,** escolha **os gastos do Azure**.

3. Na página de gastos do **Azure,** em **Clientes com Microsoft Azure subscrições,** selecione os clientes(s) cujo orçamento pretende remover.

4. Escolha **Remover orçamento**.

* * *

## <a name="notifications-for-budget-limits"></a>Notificações para limites orçamentais

Pode *ligar notificações por e-mail* para quando os gastos mensais do seu cliente estiverem perto do limite de orçamento. Quando ligar esta opção, será notificado quando os clientes utilizarem 80% ou mais do seu orçamento mensal. Esta opção ajuda-o a manter um olho na sua conta Azure. Para configurar notificações de email:

1. Inicie sessão no Centro de Parceiros.

2. Selecione o ícone de engrenagem Definições e, em seguida, selecione **As minhas preferências**.

3. Configure um endereço de e-mail preferido se não tiver.

4. Configure a língua preferida para a notificação.

5. Selecione o separador **CSP** na secção **de preferências de notificação.**

6. Consulte a opção E-mail para a notificação **de gastos do Azure** e **guarde**.

## <a name="itemized-costs-by-service"></a>Custos itemados por serviço

Pode ver os custos (e a utilização estimada) por serviço para subscrições baseadas em uso*:

> [!NOTE]
> Para saber mais sobre a interface de espaços de trabalho, consulte [o Centro de Parceiros.](get-around-partner-center.md#turn-workspaces-on-and-off)

#### <a name="workspaces-view"></a>[Vista de espaços de trabalho](#tab/workspaces-view)

1. Inicie sessão no [dashboard do Centro de Parceiros](https://partner.microsoft.com/dashboard).

2. Selecione **o** azulejo cliente.

3. Selecione o **nome da Empresa** do cliente.

4. Na página de **Subscrições** do cliente, em **subscrições baseadas em uso,** selecione o nome da **Subscrição**.

5. Na página da subscrição, pode rever os **custos itemizados** por serviço e a **utilização estimada** para o mês em curso.

#### <a name="current-view"></a>[Vista atual](#tab/current-view)

1. Inicie sessão no [dashboard do Centro de Parceiros](https://partner.microsoft.com/dashboard).

2. No menu à esquerda em **CSP,** escolha **Clientes**.

3. Na página **Clientes,** selecione o **nome da Empresa** do cliente.

4. Na página de **Subscrições** do cliente, em **subscrições baseadas em uso,** selecione o nome da **Subscrição**.

5. Na página da subscrição, pode rever os **custos itemizados** por serviço e a **utilização estimada** para o mês em curso.

* * *

## <a name="next-steps"></a>Passos seguintes

- [Nova experiência comercial no CSP – faturação do Azure](azure-plan-billing.md)
