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
ms.openlocfilehash: 14e901f51841e58b28a3cbbb1b7a19ce89d7c324
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855357"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a><span data-ttu-id="7cc36-103">Desconfiem, verifiquem ou removam os orçamentos mensais de gastos da Azure para os clientes no Partner Center</span><span class="sxs-lookup"><span data-stu-id="7cc36-103">Set, check, or remove monthly Azure spending budgets for customers in Partner Center</span></span>

<span data-ttu-id="7cc36-104">**Funções adequadas**: Agente administrativo</span><span class="sxs-lookup"><span data-stu-id="7cc36-104">**Appropriate roles**: Admin agent</span></span>

<span data-ttu-id="7cc36-105">Pode [definir um orçamento mensal de gastos da Azure para os seus clientes](#set-azure-spending-budget) no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="7cc36-105">You can [set a monthly Azure spending budget for your customers](#set-azure-spending-budget) in Partner Center.</span></span> <span data-ttu-id="7cc36-106">Isto ajuda os seus clientes a gerir os seus gastos com o Azure.</span><span class="sxs-lookup"><span data-stu-id="7cc36-106">This helps your customers manage their Azure spending.</span></span> <span data-ttu-id="7cc36-107">Esta opção permite comparar os gastos do Azure dos seus clientes com o orçamento durante o mês.</span><span class="sxs-lookup"><span data-stu-id="7cc36-107">This option allows you to compare your customers' Azure spending to the budget during the month.</span></span> <span data-ttu-id="7cc36-108">Também ajuda os seus clientes a orçamentar os seus gastos com o Azure para que a sua fatura mensal não seja maior do que antecipam.</span><span class="sxs-lookup"><span data-stu-id="7cc36-108">It also helps your customers to budget their Azure spending so their monthly bill isn't higher than they anticipate.</span></span>

> [!NOTE]  
> <span data-ttu-id="7cc36-109">Esta função não está disponível nas contas sandbox ou Test in Production (TIP).</span><span class="sxs-lookup"><span data-stu-id="7cc36-109">This feature is not available in sandbox or Test in Production (TIP) accounts.</span></span>

<span data-ttu-id="7cc36-110">Depois de [definir um orçamento de gastos da Azure para o seu cliente,s,](#set-azure-spending-budget)também pode rever o uso do cliente das seguintes formas.</span><span class="sxs-lookup"><span data-stu-id="7cc36-110">After you [set an Azure spending budget for your customer(s)](#set-azure-spending-budget), you can also review customer usage in the following ways.</span></span> <span data-ttu-id="7cc36-111">Estas opções podem ajudá-lo a detetar serviços mal configurados ou tendências incomuns que possam sugerir fraude.</span><span class="sxs-lookup"><span data-stu-id="7cc36-111">These options may help you spot misconfigured services or unusual trends that might suggest fraud.</span></span> <span data-ttu-id="7cc36-112">Em seguida, pode trabalhar com o(s) cliente(s) para identificar a causa raiz e gerir os custos.</span><span class="sxs-lookup"><span data-stu-id="7cc36-112">You can then work with your customer(s) to identify the root cause and manage costs.</span></span> <span data-ttu-id="7cc36-113">Se necessário, também pode [alterar o orçamento do cliente](#set-azure-spending-budget) para um valor mais elevado.</span><span class="sxs-lookup"><span data-stu-id="7cc36-113">If necessary, you can also [change the customer's budget](#set-azure-spending-budget) to a higher amount.</span></span>

- [<span data-ttu-id="7cc36-114">Verifique os gastos atuais do Azure</span><span class="sxs-lookup"><span data-stu-id="7cc36-114">Check current Azure spending</span></span>](#check-current-azure-spending)

- [<span data-ttu-id="7cc36-115">Ligue as notificações por e-mail para quando os gastos de um cliente estiverem próximos do seu limite orçamental</span><span class="sxs-lookup"><span data-stu-id="7cc36-115">Turn on email notifications for when a customer's spending is nearing their budget limit</span></span>](#notifications-for-budget-limits)

- [<span data-ttu-id="7cc36-116">Ver custos itemizados por serviço para subscrições baseadas em uso</span><span class="sxs-lookup"><span data-stu-id="7cc36-116">View itemized costs by service for usage-based subscriptions</span></span>](#itemized-costs-by-service)

<span data-ttu-id="7cc36-117">Também pode [remover um orçamento de gastos da Azure](#remove-azure-spending-budget) para clientes a qualquer momento.</span><span class="sxs-lookup"><span data-stu-id="7cc36-117">You can also [remove an Azure spending budget](#remove-azure-spending-budget) for customer(s) at any time.</span></span>

## <a name="azure-spending-data"></a><span data-ttu-id="7cc36-118">Dados de gastos do Azure</span><span class="sxs-lookup"><span data-stu-id="7cc36-118">Azure spending data</span></span>

<span data-ttu-id="7cc36-119">Os dados de gastos do Azure são uma *estimativa* e *os valores reais de faturação podem variar.*</span><span class="sxs-lookup"><span data-stu-id="7cc36-119">The Azure spending data is an *estimate* and *actual billing amounts may vary*.</span></span> <span data-ttu-id="7cc36-120">O valor dos dados *não reflete* impostos, créditos, ajustes ou outros encargos que possam ser aplicados.</span><span class="sxs-lookup"><span data-stu-id="7cc36-120">The data's value *doesn't reflect* taxes, credits, adjustments, or other charges that may apply.</span></span>

<span data-ttu-id="7cc36-121">Os dados de gastos são *atualizados uma vez por dia.*</span><span class="sxs-lookup"><span data-stu-id="7cc36-121">The spending data is *refreshed once per day*.</span></span> <span data-ttu-id="7cc36-122">Os seus clientes podem continuar a utilizar (e ser cobrados) serviços e recursos da Azure, a menos que altere as definições da sua conta no portal Azure.</span><span class="sxs-lookup"><span data-stu-id="7cc36-122">Your customers can continue to use (and be charged for) Azure services and resources, unless you change their account settings in the Azure portal.</span></span>

## <a name="set-azure-spending-budget"></a><span data-ttu-id="7cc36-123">Definir orçamento de gastos do Azure</span><span class="sxs-lookup"><span data-stu-id="7cc36-123">Set Azure spending budget</span></span>

<span data-ttu-id="7cc36-124">Pode *definir um orçamento mensal de gastos da Azure* para vários clientes no Partner Center:</span><span class="sxs-lookup"><span data-stu-id="7cc36-124">You can *set a monthly Azure spending budget* for multiple customers in Partner Center:</span></span>

1. <span data-ttu-id="7cc36-125">Inicie sessão no [dashboard do Centro de Parceiros](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="7cc36-125">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="7cc36-126">No menu à esquerda em **CSP,** escolha os gastos do **Azure**.</span><span class="sxs-lookup"><span data-stu-id="7cc36-126">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="7cc36-127">Na página de gastos do **Azure,** em **Clientes com subscrições Microsoft Azure,** selecione os clientes(s) para os quais pretende definir um orçamento.</span><span class="sxs-lookup"><span data-stu-id="7cc36-127">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) for whom you want to set a budget.</span></span>

4. <span data-ttu-id="7cc36-128">Introduza um valor para **o orçamento mensal.**</span><span class="sxs-lookup"><span data-stu-id="7cc36-128">Enter a value for **Monthly budget**.</span></span>

5. <span data-ttu-id="7cc36-129">Escolha **Aplicar** para guardar as suas alterações.</span><span class="sxs-lookup"><span data-stu-id="7cc36-129">Choose **Apply** to save your changes.</span></span>

<span data-ttu-id="7cc36-130">Também pode *definir um orçamento para um cliente individual* nas suas definições de subscrição:</span><span class="sxs-lookup"><span data-stu-id="7cc36-130">You can also *set a budget for an individual customer* in their subscription settings:</span></span>

1. <span data-ttu-id="7cc36-131">Inicie sessão no dashboard do Centro de Parceiros.</span><span class="sxs-lookup"><span data-stu-id="7cc36-131">Sign in to the Partner Center dashboard.</span></span>

2. <span data-ttu-id="7cc36-132">No menu à esquerda em **CSP,** escolha **Clientes**.</span><span class="sxs-lookup"><span data-stu-id="7cc36-132">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="7cc36-133">Na página **Clientes,** selecione o **nome da Empresa** do cliente.</span><span class="sxs-lookup"><span data-stu-id="7cc36-133">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="7cc36-134">Na página de **Subscrições** do cliente, na **subscrição baseada em utilização,** escolha **o orçamento change**.</span><span class="sxs-lookup"><span data-stu-id="7cc36-134">On the customer's **Subscriptions** page, under **Usage-based subscription**, choose **Change budget**.</span></span>

5. <span data-ttu-id="7cc36-135">Insira um valor para o orçamento.</span><span class="sxs-lookup"><span data-stu-id="7cc36-135">Enter a value for the budget.</span></span>

6. <span data-ttu-id="7cc36-136">Escolha **Aplicar** para guardar as suas alterações.</span><span class="sxs-lookup"><span data-stu-id="7cc36-136">Choose **Apply** to save your changes.</span></span>

## <a name="remove-azure-spending-budget"></a><span data-ttu-id="7cc36-137">Remover orçamento de gastos do Azure</span><span class="sxs-lookup"><span data-stu-id="7cc36-137">Remove Azure spending budget</span></span>

<span data-ttu-id="7cc36-138">Pode *remover um orçamento mensal de gastos da Azure* para o seu cliente(s) no Partner Center:</span><span class="sxs-lookup"><span data-stu-id="7cc36-138">You can *remove a monthly Azure spending budget* for your customer(s) in Partner Center:</span></span>

1. <span data-ttu-id="7cc36-139">Inicie sessão no [dashboard do Centro de Parceiros](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="7cc36-139">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="7cc36-140">No menu à esquerda em **CSP,** escolha os gastos do **Azure**.</span><span class="sxs-lookup"><span data-stu-id="7cc36-140">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="7cc36-141">Na página de gastos do **Azure,** em **Clientes com subscrições Microsoft Azure,** selecione os clientes(s) cujo orçamento pretende remover.</span><span class="sxs-lookup"><span data-stu-id="7cc36-141">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) whose budget you want to remove.</span></span>

4. <span data-ttu-id="7cc36-142">Escolha **Remover orçamento**.</span><span class="sxs-lookup"><span data-stu-id="7cc36-142">Choose **Remove budget**.</span></span>

## <a name="check-current-azure-spending"></a><span data-ttu-id="7cc36-143">Verifique os gastos atuais do Azure</span><span class="sxs-lookup"><span data-stu-id="7cc36-143">Check current Azure spending</span></span>

<span data-ttu-id="7cc36-144">Pode *acompanhar os gastos atuais do Azure e os orçamentos mensais dos seus clientes* a qualquer momento:</span><span class="sxs-lookup"><span data-stu-id="7cc36-144">You can *track your customers' current Azure spending and monthly budgets* at any time:</span></span>

1. <span data-ttu-id="7cc36-145">Inicie sessão no [dashboard do Centro de Parceiros](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="7cc36-145">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="7cc36-146">No menu à esquerda em **CSP,** escolha os gastos do **Azure**.</span><span class="sxs-lookup"><span data-stu-id="7cc36-146">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="7cc36-147">Na página de gastos do **Azure,** em **Clientes com subscrições microsoft Azure,** pode ver uma visão geral dos orçamentos mensais dos clientes, estimativas de gastos correntes e percentagem de orçamento utilizado.</span><span class="sxs-lookup"><span data-stu-id="7cc36-147">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, you can see an overview of customers' monthly budgets, current spending estimates and percentage of budget used.</span></span>

## <a name="notifications-for-budget-limits"></a><span data-ttu-id="7cc36-148">Notificações para limites orçamentais</span><span class="sxs-lookup"><span data-stu-id="7cc36-148">Notifications for budget limits</span></span>

<span data-ttu-id="7cc36-149">Pode *ligar notificações por e-mail* para quando os gastos mensais do seu cliente estiverem perto do limite orçamental.</span><span class="sxs-lookup"><span data-stu-id="7cc36-149">You can *turn on email notifications* for when your customer's monthly spending is nearing their budget limit.</span></span> <span data-ttu-id="7cc36-150">Quando ligar esta opção, será notificado quando os clientes utilizarem 80% ou mais do seu orçamento mensal.</span><span class="sxs-lookup"><span data-stu-id="7cc36-150">When you turn on this option, you will be notified when customers use 80% or more of their monthly budget.</span></span> <span data-ttu-id="7cc36-151">Esta opção ajuda-o a manter um olho na sua conta do Azure.</span><span class="sxs-lookup"><span data-stu-id="7cc36-151">This option helps you can keep an eye on your Azure bill.</span></span> <span data-ttu-id="7cc36-152">Para configurar notificações de e-mail:</span><span class="sxs-lookup"><span data-stu-id="7cc36-152">To configure email notifications:</span></span>

1. <span data-ttu-id="7cc36-153">Inicie sessão no Centro de Parceiros.</span><span class="sxs-lookup"><span data-stu-id="7cc36-153">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="7cc36-154">Ir para **Definições**.</span><span class="sxs-lookup"><span data-stu-id="7cc36-154">Go to **Settings**.</span></span>

3. <span data-ttu-id="7cc36-155">Selecione **as minhas preferências**.</span><span class="sxs-lookup"><span data-stu-id="7cc36-155">Select **My preferences**.</span></span>

4. <span data-ttu-id="7cc36-156">Configure um endereço de e-mail preferido se não tiver.</span><span class="sxs-lookup"><span data-stu-id="7cc36-156">Configure a preferred email address if you haven't.</span></span>

5. <span data-ttu-id="7cc36-157">Configurar a língua preferida para a notificação.</span><span class="sxs-lookup"><span data-stu-id="7cc36-157">Configure the preferred language for the notification.</span></span>

6. <span data-ttu-id="7cc36-158">Selecione o separador **CSP** na secção **de preferências de notificação.**</span><span class="sxs-lookup"><span data-stu-id="7cc36-158">Select **CSP** tab under **Notification preferences** section.</span></span>

7. <span data-ttu-id="7cc36-159">Consulte a opção E-mail para obter a notificação de gastos do **Azure** e **guarde**.</span><span class="sxs-lookup"><span data-stu-id="7cc36-159">Check the Email option for **Azure Spending** notification, and **Save**.</span></span>


## <a name="itemized-costs-by-service"></a><span data-ttu-id="7cc36-160">Custos itemados por serviço</span><span class="sxs-lookup"><span data-stu-id="7cc36-160">Itemized costs by service</span></span>

<span data-ttu-id="7cc36-161">Pode *ver os custos (e a utilização estimada) por serviço para subscrições baseadas em uso:*</span><span class="sxs-lookup"><span data-stu-id="7cc36-161">You can *view itemized costs (and estimated usage) by service for usage-based subscriptions*:</span></span>

1. <span data-ttu-id="7cc36-162">Inicie sessão no Centro de Parceiros.</span><span class="sxs-lookup"><span data-stu-id="7cc36-162">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="7cc36-163">No menu à esquerda em **CSP,** escolha **Clientes**.</span><span class="sxs-lookup"><span data-stu-id="7cc36-163">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="7cc36-164">Na página **Clientes,** selecione o **nome da Empresa** do cliente.</span><span class="sxs-lookup"><span data-stu-id="7cc36-164">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="7cc36-165">Na página de **Subscrições** do cliente, em **subscrições baseadas em uso,** selecione o nome da **Subscrição**.</span><span class="sxs-lookup"><span data-stu-id="7cc36-165">On the customer's **Subscriptions** page, under **Usage-based subscriptions**, select the name of the **Subscription**.</span></span>

5. <span data-ttu-id="7cc36-166">Na página da subscrição, pode rever os **custos itemizados** por serviço e a **utilização estimada** para o mês em curso.</span><span class="sxs-lookup"><span data-stu-id="7cc36-166">On the subscription's page, you can review the **Itemized costs** by service, and the **Estimated usage** for the current month.</span></span>


## <a name="next-steps"></a><span data-ttu-id="7cc36-167">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="7cc36-167">Next steps</span></span>

- [<span data-ttu-id="7cc36-168">Nova experiência comercial no CSP – faturação do Azure</span><span class="sxs-lookup"><span data-stu-id="7cc36-168">New commerce experience in CSP - Azure billing</span></span>](azure-plan-billing.md)
