---
title: Definir um orçamento de despesas do Azure para os clientes
ms.topic: how-to
ms.date: 03/17/2021
description: Saiba como definir ou remover orçamentos mensais de gastos do Azure para os seus clientes, bem como ver os dados de gastos do Azure e definir notificações relacionadas com o orçamento.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: eaf54898d7a130ca38e5a2aaeba279fb722c9e66
ms.sourcegitcommit: e8e8362d2777d25efac3e1076af5939765ed13d0
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/20/2021
ms.locfileid: "104712754"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a><span data-ttu-id="8b1cb-103">Desconfiem, verifiquem ou removam os orçamentos mensais de gastos da Azure para os clientes no Partner Center</span><span class="sxs-lookup"><span data-stu-id="8b1cb-103">Set, check, or remove monthly Azure spending budgets for customers in Partner Center</span></span>

<span data-ttu-id="8b1cb-104">**Funções adequadas**</span><span class="sxs-lookup"><span data-stu-id="8b1cb-104">**Appropriate roles**</span></span>

- <span data-ttu-id="8b1cb-105">Agente administrativo</span><span class="sxs-lookup"><span data-stu-id="8b1cb-105">Admin agent</span></span>

<span data-ttu-id="8b1cb-106">Pode [definir um orçamento mensal de gastos da Azure para os seus clientes](#set-azure-spending-budget) no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="8b1cb-106">You can [set a monthly Azure spending budget for your customers](#set-azure-spending-budget) in Partner Center.</span></span> <span data-ttu-id="8b1cb-107">Isto ajuda os seus clientes a gerir os seus gastos com o Azure.</span><span class="sxs-lookup"><span data-stu-id="8b1cb-107">This helps your customers manage their Azure spending.</span></span> <span data-ttu-id="8b1cb-108">Esta opção permite comparar os gastos do Azure dos seus clientes com o orçamento durante o mês.</span><span class="sxs-lookup"><span data-stu-id="8b1cb-108">This option allows you to compare your customers' Azure spending to the budget during the month.</span></span> <span data-ttu-id="8b1cb-109">Também ajuda os seus clientes a orçamentar os seus gastos com o Azure para que a sua fatura mensal não seja maior do que antecipam.</span><span class="sxs-lookup"><span data-stu-id="8b1cb-109">It also helps your customers to budget their Azure spending so their monthly bill isn't higher than they anticipate.</span></span>

> [!NOTE]  
> <span data-ttu-id="8b1cb-110">Esta função não está disponível nas contas sandbox ou Test in Production (TIP).</span><span class="sxs-lookup"><span data-stu-id="8b1cb-110">This feature is not available in sandbox or Test in Production (TIP) accounts.</span></span>

<span data-ttu-id="8b1cb-111">Depois de [definir um orçamento de gastos da Azure para o seu cliente,s,](#set-azure-spending-budget)também pode rever o uso do cliente das seguintes formas.</span><span class="sxs-lookup"><span data-stu-id="8b1cb-111">After you [set an Azure spending budget for your customer(s)](#set-azure-spending-budget), you can also review customer usage in the following ways.</span></span> <span data-ttu-id="8b1cb-112">Estas opções podem ajudá-lo a detetar serviços mal configurados ou tendências incomuns que possam sugerir fraude.</span><span class="sxs-lookup"><span data-stu-id="8b1cb-112">These options may help you spot misconfigured services or unusual trends that might suggest fraud.</span></span> <span data-ttu-id="8b1cb-113">Em seguida, pode trabalhar com o(s) cliente(s) para identificar a causa raiz e gerir os custos.</span><span class="sxs-lookup"><span data-stu-id="8b1cb-113">You can then work with your customer(s) to identify the root cause and manage costs.</span></span> <span data-ttu-id="8b1cb-114">Se necessário, também pode [alterar o orçamento do cliente](#set-azure-spending-budget) para um valor mais elevado.</span><span class="sxs-lookup"><span data-stu-id="8b1cb-114">If necessary, you can also [change the customer's budget](#set-azure-spending-budget) to a higher amount.</span></span>

- [<span data-ttu-id="8b1cb-115">Verifique os gastos atuais do Azure</span><span class="sxs-lookup"><span data-stu-id="8b1cb-115">Check current Azure spending</span></span>](#check-current-azure-spending)

- [<span data-ttu-id="8b1cb-116">Ligue as notificações por e-mail para quando os gastos de um cliente estiverem próximos do seu limite orçamental</span><span class="sxs-lookup"><span data-stu-id="8b1cb-116">Turn on email notifications for when a customer's spending is nearing their budget limit</span></span>](#notifications-for-budget-limits)

- [<span data-ttu-id="8b1cb-117">Ver custos itemizados por serviço para subscrições baseadas em uso</span><span class="sxs-lookup"><span data-stu-id="8b1cb-117">View itemized costs by service for usage-based subscriptions</span></span>](#itemized-costs-by-service)

<span data-ttu-id="8b1cb-118">Também pode [remover um orçamento de gastos da Azure](#remove-azure-spending-budget) para clientes a qualquer momento.</span><span class="sxs-lookup"><span data-stu-id="8b1cb-118">You can also [remove an Azure spending budget](#remove-azure-spending-budget) for customer(s) at any time.</span></span>

## <a name="azure-spending-data"></a><span data-ttu-id="8b1cb-119">Dados de gastos do Azure</span><span class="sxs-lookup"><span data-stu-id="8b1cb-119">Azure spending data</span></span>

<span data-ttu-id="8b1cb-120">Os dados de gastos do Azure são uma *estimativa* e *os valores reais de faturação podem variar.*</span><span class="sxs-lookup"><span data-stu-id="8b1cb-120">The Azure spending data is an *estimate* and *actual billing amounts may vary*.</span></span> <span data-ttu-id="8b1cb-121">O valor dos dados *não reflete* impostos, créditos, ajustes ou outros encargos que possam ser aplicados.</span><span class="sxs-lookup"><span data-stu-id="8b1cb-121">The data's value *doesn't reflect* taxes, credits, adjustments, or other charges that may apply.</span></span>

<span data-ttu-id="8b1cb-122">Os dados de gastos são *atualizados uma vez por dia.*</span><span class="sxs-lookup"><span data-stu-id="8b1cb-122">The spending data is *refreshed once per day*.</span></span> <span data-ttu-id="8b1cb-123">Os seus clientes podem continuar a utilizar (e ser cobrados) serviços e recursos da Azure, a menos que altere as definições da sua conta no portal Azure.</span><span class="sxs-lookup"><span data-stu-id="8b1cb-123">Your customers can continue to use (and be charged for) Azure services and resources, unless you change their account settings in the Azure portal.</span></span>

## <a name="set-azure-spending-budget"></a><span data-ttu-id="8b1cb-124">Definir orçamento de gastos do Azure</span><span class="sxs-lookup"><span data-stu-id="8b1cb-124">Set Azure spending budget</span></span>

<span data-ttu-id="8b1cb-125">Pode *definir um orçamento mensal de gastos da Azure* para vários clientes no Partner Center:</span><span class="sxs-lookup"><span data-stu-id="8b1cb-125">You can *set a monthly Azure spending budget* for multiple customers in Partner Center:</span></span>

1. <span data-ttu-id="8b1cb-126">Inicie sessão no [dashboard do Centro de Parceiros](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="8b1cb-126">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="8b1cb-127">No menu à esquerda em **CSP,** escolha os gastos do **Azure**.</span><span class="sxs-lookup"><span data-stu-id="8b1cb-127">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="8b1cb-128">Na página de gastos do **Azure,** em **Clientes com subscrições Microsoft Azure,** selecione os clientes(s) para os quais pretende definir um orçamento.</span><span class="sxs-lookup"><span data-stu-id="8b1cb-128">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) for whom you want to set a budget.</span></span>

4. <span data-ttu-id="8b1cb-129">Introduza um valor para **o orçamento mensal.**</span><span class="sxs-lookup"><span data-stu-id="8b1cb-129">Enter a value for **Monthly budget**.</span></span>

5. <span data-ttu-id="8b1cb-130">Escolha **Aplicar** para guardar as suas alterações.</span><span class="sxs-lookup"><span data-stu-id="8b1cb-130">Choose **Apply** to save your changes.</span></span>

<span data-ttu-id="8b1cb-131">Também pode *definir um orçamento para um cliente individual* nas suas definições de subscrição:</span><span class="sxs-lookup"><span data-stu-id="8b1cb-131">You can also *set a budget for an individual customer* in their subscription settings:</span></span>

1. <span data-ttu-id="8b1cb-132">Inicie sessão no dashboard do Centro de Parceiros.</span><span class="sxs-lookup"><span data-stu-id="8b1cb-132">Sign in to the Partner Center dashboard.</span></span>

2. <span data-ttu-id="8b1cb-133">No menu à esquerda em **CSP,** escolha **Clientes**.</span><span class="sxs-lookup"><span data-stu-id="8b1cb-133">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="8b1cb-134">Na página **Clientes,** selecione o **nome da Empresa** do cliente.</span><span class="sxs-lookup"><span data-stu-id="8b1cb-134">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="8b1cb-135">Na página de **Subscrições** do cliente, na **subscrição baseada em utilização,** escolha **o orçamento change**.</span><span class="sxs-lookup"><span data-stu-id="8b1cb-135">On the customer's **Subscriptions** page, under **Usage-based subscription**, choose **Change budget**.</span></span>

5. <span data-ttu-id="8b1cb-136">Insira um valor para o orçamento.</span><span class="sxs-lookup"><span data-stu-id="8b1cb-136">Enter a value for the budget.</span></span>

6. <span data-ttu-id="8b1cb-137">Escolha **Aplicar** para guardar as suas alterações.</span><span class="sxs-lookup"><span data-stu-id="8b1cb-137">Choose **Apply** to save your changes.</span></span>

## <a name="remove-azure-spending-budget"></a><span data-ttu-id="8b1cb-138">Remover orçamento de gastos do Azure</span><span class="sxs-lookup"><span data-stu-id="8b1cb-138">Remove Azure spending budget</span></span>

<span data-ttu-id="8b1cb-139">Pode *remover um orçamento mensal de gastos da Azure* para o seu cliente(s) no Partner Center:</span><span class="sxs-lookup"><span data-stu-id="8b1cb-139">You can *remove a monthly Azure spending budget* for your customer(s) in Partner Center:</span></span>

1. <span data-ttu-id="8b1cb-140">Inicie sessão no [dashboard do Centro de Parceiros](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="8b1cb-140">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="8b1cb-141">No menu à esquerda em **CSP,** escolha os gastos do **Azure**.</span><span class="sxs-lookup"><span data-stu-id="8b1cb-141">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="8b1cb-142">Na página de gastos do **Azure,** em **Clientes com subscrições Microsoft Azure,** selecione os clientes(s) cujo orçamento pretende remover.</span><span class="sxs-lookup"><span data-stu-id="8b1cb-142">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) whose budget you want to remove.</span></span>

4. <span data-ttu-id="8b1cb-143">Escolha **Remover orçamento**.</span><span class="sxs-lookup"><span data-stu-id="8b1cb-143">Choose **Remove budget**.</span></span>

## <a name="check-current-azure-spending"></a><span data-ttu-id="8b1cb-144">Verifique os gastos atuais do Azure</span><span class="sxs-lookup"><span data-stu-id="8b1cb-144">Check current Azure spending</span></span>

<span data-ttu-id="8b1cb-145">Pode *acompanhar os gastos atuais do Azure e os orçamentos mensais dos seus clientes* a qualquer momento:</span><span class="sxs-lookup"><span data-stu-id="8b1cb-145">You can *track your customers' current Azure spending and monthly budgets* at any time:</span></span>

1. <span data-ttu-id="8b1cb-146">Inicie sessão no [dashboard do Centro de Parceiros](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="8b1cb-146">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="8b1cb-147">No menu à esquerda em **CSP,** escolha os gastos do **Azure**.</span><span class="sxs-lookup"><span data-stu-id="8b1cb-147">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="8b1cb-148">Na página de gastos do **Azure,** em **Clientes com subscrições microsoft Azure,** pode ver uma visão geral dos orçamentos mensais dos clientes, estimativas de gastos correntes e percentagem de orçamento utilizado.</span><span class="sxs-lookup"><span data-stu-id="8b1cb-148">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, you can see an overview of customers' monthly budgets, current spending estimates and percentage of budget used.</span></span>

## <a name="notifications-for-budget-limits"></a><span data-ttu-id="8b1cb-149">Notificações para limites orçamentais</span><span class="sxs-lookup"><span data-stu-id="8b1cb-149">Notifications for budget limits</span></span>

<span data-ttu-id="8b1cb-150">Pode *ligar notificações por e-mail* para quando os gastos mensais do seu cliente estiverem perto do limite orçamental.</span><span class="sxs-lookup"><span data-stu-id="8b1cb-150">You can *turn on email notifications* for when your customer's monthly spending is nearing their budget limit.</span></span> <span data-ttu-id="8b1cb-151">Quando ligar esta opção, será notificado quando os clientes utilizarem 80% ou mais do seu orçamento mensal.</span><span class="sxs-lookup"><span data-stu-id="8b1cb-151">When you turn on this option, you will be notified when customers use 80% or more of their monthly budget.</span></span> <span data-ttu-id="8b1cb-152">Esta opção ajuda-o a manter um olho na sua conta do Azure.</span><span class="sxs-lookup"><span data-stu-id="8b1cb-152">This option helps you can keep an eye on your Azure bill.</span></span> <span data-ttu-id="8b1cb-153">Para configurar notificações de e-mail:</span><span class="sxs-lookup"><span data-stu-id="8b1cb-153">To configure email notifications:</span></span>

1. <span data-ttu-id="8b1cb-154">Inicie sessão no Centro de Parceiros.</span><span class="sxs-lookup"><span data-stu-id="8b1cb-154">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="8b1cb-155">Ir para **Definições**.</span><span class="sxs-lookup"><span data-stu-id="8b1cb-155">Go to **Settings**.</span></span>

3. <span data-ttu-id="8b1cb-156">Selecione **as minhas preferências**.</span><span class="sxs-lookup"><span data-stu-id="8b1cb-156">Select **My preferences**.</span></span>

4. <span data-ttu-id="8b1cb-157">Configure um endereço de e-mail preferido se não tiver.</span><span class="sxs-lookup"><span data-stu-id="8b1cb-157">Configure a preferred email address if you haven't.</span></span>

5. <span data-ttu-id="8b1cb-158">Configurar a língua preferida para a notificação.</span><span class="sxs-lookup"><span data-stu-id="8b1cb-158">Configure the preferred language for the notification.</span></span>

6. <span data-ttu-id="8b1cb-159">Selecione o separador **CSP** na secção **de preferências de notificação.**</span><span class="sxs-lookup"><span data-stu-id="8b1cb-159">Select **CSP** tab under **Notification preferences** section.</span></span>

7. <span data-ttu-id="8b1cb-160">Consulte a opção E-mail para obter a notificação de gastos do **Azure** e **guarde**.</span><span class="sxs-lookup"><span data-stu-id="8b1cb-160">Check the Email option for **Azure Spending** notification, and **Save**.</span></span>


## <a name="itemized-costs-by-service"></a><span data-ttu-id="8b1cb-161">Custos itemados por serviço</span><span class="sxs-lookup"><span data-stu-id="8b1cb-161">Itemized costs by service</span></span>

<span data-ttu-id="8b1cb-162">Pode *ver os custos (e a utilização estimada) por serviço para subscrições baseadas em uso:*</span><span class="sxs-lookup"><span data-stu-id="8b1cb-162">You can *view itemized costs (and estimated usage) by service for usage-based subscriptions*:</span></span>

1. <span data-ttu-id="8b1cb-163">Inicie sessão no Centro de Parceiros.</span><span class="sxs-lookup"><span data-stu-id="8b1cb-163">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="8b1cb-164">No menu à esquerda em **CSP,** escolha **Clientes**.</span><span class="sxs-lookup"><span data-stu-id="8b1cb-164">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="8b1cb-165">Na página **Clientes,** selecione o **nome da Empresa** do cliente.</span><span class="sxs-lookup"><span data-stu-id="8b1cb-165">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="8b1cb-166">Na página de **Subscrições** do cliente, em **subscrições baseadas em uso,** selecione o nome da **Subscrição**.</span><span class="sxs-lookup"><span data-stu-id="8b1cb-166">On the customer's **Subscriptions** page, under **Usage-based subscriptions**, select the name of the **Subscription**.</span></span>

5. <span data-ttu-id="8b1cb-167">Na página da subscrição, pode rever os **custos itemizados** por serviço e a **utilização estimada** para o mês em curso.</span><span class="sxs-lookup"><span data-stu-id="8b1cb-167">On the subscription's page, you can review the **Itemized costs** by service, and the **Estimated usage** for the current month.</span></span>


## <a name="next-steps"></a><span data-ttu-id="8b1cb-168">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="8b1cb-168">Next steps</span></span>

- [<span data-ttu-id="8b1cb-169">Nova experiência comercial no CSP – faturação do Azure</span><span class="sxs-lookup"><span data-stu-id="8b1cb-169">New commerce experience in CSP - Azure billing</span></span>](azure-plan-billing.md)
