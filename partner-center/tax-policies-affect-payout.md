---
title: Como as políticas fiscais afetam o pagamento do Azure Marketplace
description: Saiba como as políticas fiscais afetam o pagamento do Azure Marketplace.
ms.topic: conceptual
ms.service: partner-dashboard
author: mingshen-ms
ms.author: mingshen
ms.date: 02/09/2021
ms.openlocfilehash: 19acb085b601212f1bf94316aab2b72c54aecc1a
ms.sourcegitcommit: e8e8362d2777d25efac3e1076af5939765ed13d0
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/20/2021
ms.locfileid: "104712958"
---
# <a name="how-tax-policies-affect-payout-for-azure-marketplace"></a><span data-ttu-id="08bee-103">Como as políticas fiscais afetam o pagamento do Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="08bee-103">How tax policies affect payout for Azure Marketplace</span></span>

<span data-ttu-id="08bee-104">**Funções adequadas**</span><span class="sxs-lookup"><span data-stu-id="08bee-104">**Appropriate roles**</span></span>
-    <span data-ttu-id="08bee-105">Administrador global</span><span class="sxs-lookup"><span data-stu-id="08bee-105">Global admin</span></span>
-    <span data-ttu-id="08bee-106">Administrador de utilizadores</span><span class="sxs-lookup"><span data-stu-id="08bee-106">User admin</span></span>
-    <span data-ttu-id="08bee-107">Agente administrativo</span><span class="sxs-lookup"><span data-stu-id="08bee-107">Admin agent</span></span>

## <a name="introduction"></a><span data-ttu-id="08bee-108">Introdução</span><span class="sxs-lookup"><span data-stu-id="08bee-108">Introduction</span></span>

<span data-ttu-id="08bee-109">O mercado comercial da Microsoft tem alcance global.</span><span class="sxs-lookup"><span data-stu-id="08bee-109">The Microsoft commercial marketplace has global reach.</span></span> <span data-ttu-id="08bee-110">As transações ocorrem além-fronteiras e dependendo do local onde o ISV e o cliente estão localizados, as implicações fiscais podem variar.</span><span class="sxs-lookup"><span data-stu-id="08bee-110">Transactions occur across borders and depending on where the ISV and the customer are located, tax implications can vary.</span></span> <span data-ttu-id="08bee-111">O Microsoft AppSource e o Azure Marketplace utilizam as Informações de Perfil Fiscal do Centro de Parceiros para determinar o país do ISV.</span><span class="sxs-lookup"><span data-stu-id="08bee-111">Microsoft AppSource and Azure Marketplace use the Partner Center Tax Profile Information to determine the ISV's country.</span></span> <span data-ttu-id="08bee-112">Para determinar o país do cliente, utilize as informações de faturação do cliente ou, se o cliente estiver na UE, utilizamos duas informações diferentes.</span><span class="sxs-lookup"><span data-stu-id="08bee-112">To determine the customer's country, either use the customer's billing information or, if the customer is in the EU, we use two different pieces of information.</span></span>

<span data-ttu-id="08bee-113">Para melhor compreender os seguintes cenários, consulte a tabela [de detalhes fiscais,](tax-details-marketplace.md) que mostra se a Microsoft cobra e paga impostos em nome da editora ou se essa responsabilidade pertence à editora.</span><span class="sxs-lookup"><span data-stu-id="08bee-113">To better understand the following scenarios, refer to the [Tax details](tax-details-marketplace.md) table, which shows whether Microsoft collects and pays taxes on behalf of the publisher or if that responsibility belongs to the publisher.</span></span>

> [!NOTE]
> <span data-ttu-id="08bee-114">Todos os exemplos de valores de venda e percentagens fiscais neste tópico são apenas para fins ilustrativos, não números exatos.</span><span class="sxs-lookup"><span data-stu-id="08bee-114">All examples sale values and tax percentages in this topic are for illustrative purposes only, not exact figures.</span></span>

## <a name="publisher-transacts-in-microsoft-managed-tax-country"></a><span data-ttu-id="08bee-115">Transts editoriais no País Fiscal gerido pela Microsoft</span><span class="sxs-lookup"><span data-stu-id="08bee-115">Publisher Transacts in Microsoft-managed Tax Country</span></span>

<span data-ttu-id="08bee-116">**Cenário A** – Transações que ocorrem entre um editor e um cliente num [país fiscal gerido pela Microsoft.](tax-details-marketplace.md#microsoft-managed-countries)</span><span class="sxs-lookup"><span data-stu-id="08bee-116">**Scenario A** – Transactions that take place between a publisher and a customer in a [Microsoft-managed tax country](tax-details-marketplace.md#microsoft-managed-countries).</span></span> <span data-ttu-id="08bee-117">Estas transações terão o imposto aplicável adicionado no momento da venda e a Microsoft envia esse imposto para o país aplicável.</span><span class="sxs-lookup"><span data-stu-id="08bee-117">These transactions will have applicable tax added at the time of sale and Microsoft sends that tax to the applicable country.</span></span> <span data-ttu-id="08bee-118">Nenhum imposto é retido do pagamento e os cálculos de pagamento são exclusivos dos impostos.</span><span class="sxs-lookup"><span data-stu-id="08bee-118">No taxes are withheld from payout and payout calculations are tax exclusive.</span></span>

<span data-ttu-id="08bee-119">Consulte [o Cenário D](#foreign-publisher-transacts-with-us-customer) para transações entre um editor não americano e um cliente americano.</span><span class="sxs-lookup"><span data-stu-id="08bee-119">See [Scenario D](#foreign-publisher-transacts-with-us-customer) for transactions between a non-US publisher and a US customer.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-a.png" alt-text="Mostra fluxo de trabalho para o cenário de processo de pagamento A.":::

## <a name="publisher-transacts-in-microsoft-managed-tax-country-where-marketplace-fee-is-taxable-service"></a><span data-ttu-id="08bee-121">Transts editoriais no País Fiscal gerido pela Microsoft onde a Taxa de Mercado é serviço tributável</span><span class="sxs-lookup"><span data-stu-id="08bee-121">Publisher Transacts in Microsoft-managed Tax Country where Marketplace Fee is Taxable Service</span></span>

<span data-ttu-id="08bee-122">**Cenário B** – Transações que ocorrem entre um editor com sede nos EUA (conforme definido pela sua Informação de Perfil Fiscal do Partner Center) a um cliente num país fiscal gerido pela Microsoft onde o país impõe um imposto sobre a Taxa de Mercado (um serviço tributável).</span><span class="sxs-lookup"><span data-stu-id="08bee-122">**Scenario B** – Transactions that take place between a US-based publisher (as defined by their Partner Center Tax Profile Information) to a customer in a Microsoft-managed tax country where the country imposes a tax on the Marketplace Fee (a taxable service).</span></span> <span data-ttu-id="08bee-123">Neste cenário, o imposto sobre a taxa de serviço da loja é subtraído do pagamento da editora.</span><span class="sxs-lookup"><span data-stu-id="08bee-123">In this scenario, the tax on the store service fee is subtracted from the publisher's payout.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-b.png" alt-text="Mostra fluxo de trabalho para o cenário de processo de pagamento B.":::

## <a name="publisher-transacts-in-publisher-managed-tax-country"></a><span data-ttu-id="08bee-125">Publisher Transacts em País Fiscal gerido por editores</span><span class="sxs-lookup"><span data-stu-id="08bee-125">Publisher Transacts in Publisher-managed Tax Country</span></span>

<span data-ttu-id="08bee-126">**Cenário C** – Transações que ocorrem entre um editor e um cliente num país fiscal gerido por editores que não impõe uma retenção na fonte aos clientes.</span><span class="sxs-lookup"><span data-stu-id="08bee-126">**Scenario C** – Transactions that take place between a publisher and a customer in a publisher-managed tax country that does not impose a withholding tax on customers.</span></span> <span data-ttu-id="08bee-127">Os clientes não pagam imposto no ponto de venda e é obrigação da editora pagar todos os impostos aplicáveis.</span><span class="sxs-lookup"><span data-stu-id="08bee-127">Customers pay no tax at the point of sale and it is the publisher's obligation to pay all applicable taxes.</span></span>

<span data-ttu-id="08bee-128">Para obter mais informações sobre preços específicos de cada país (por exemplo, para compensar a tributação futura) consulte [planos e preços para ofertas de mercado comercial](/azure/marketplace/plans-pricing#custom-prices).</span><span class="sxs-lookup"><span data-stu-id="08bee-128">For more information on country-specific pricing (for example, to offset upcoming taxation) see [Plans and pricing for commercial marketplace offers](/azure/marketplace/plans-pricing#custom-prices).</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-c.png" alt-text="Mostra fluxo de trabalho para o cenário do processo de pagamento C.":::

## <a name="foreign-publisher-transacts-with-us-customer"></a><span data-ttu-id="08bee-130">Transtas de Editores Estrangeiros com Cliente dos EUA</span><span class="sxs-lookup"><span data-stu-id="08bee-130">Foreign Publisher Transacts with US Customer</span></span>

<span data-ttu-id="08bee-131">**Cenário D** – Todos os editores estrangeiros (conforme definido pela sua Informação de Perfil Fiscal do Partner Center) em países sem tratado dos EUA (ver [Cenário E)](#foreign-publisher-with-a-treaty-transacts-with-us-customer)fazendo uma venda a um cliente com sede nos EUA (conforme definido pelo endereço da sua conta de cliente).</span><span class="sxs-lookup"><span data-stu-id="08bee-131">**Scenario D** – All foreign publishers (as defined by their Partner Center Tax Profile Information) in countries without a US treaty (see [Scenario E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)) making a sale to a US-based customer (as defined by their customer account address).</span></span> <span data-ttu-id="08bee-132">O governo dos EUA exige que a Microsoft retenha o imposto em nome da editora.</span><span class="sxs-lookup"><span data-stu-id="08bee-132">US government requires that Microsoft withhold tax on behalf of the publisher.</span></span> <span data-ttu-id="08bee-133">O imposto retido do pagamento ao editor é calculado com base no preço da oferta.</span><span class="sxs-lookup"><span data-stu-id="08bee-133">Tax withheld from payout to publisher is calculated based on offer price.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-d.png" alt-text="Mostra fluxo de trabalho para o cenário de processo de pagamento D.":::

## <a name="foreign-publisher-with-a-treaty-transacts-with-us-customer"></a><span data-ttu-id="08bee-135">Editora estrangeira com um Tratado Transata com cliente dos EUA</span><span class="sxs-lookup"><span data-stu-id="08bee-135">Foreign publisher with a Treaty Transacts with US customer</span></span>

<span data-ttu-id="08bee-136">**Cenário E** – Todos os editores estrangeiros (conforme definido pela sua Informação de Perfil Fiscal do Partner Center) em países com um tratado dos EUA que faz uma venda a um cliente com sede nos EUA (conforme definido pelo seu endereço de conta de cliente).</span><span class="sxs-lookup"><span data-stu-id="08bee-136">**Scenario E** – All foreign publishers (as defined by their Partner Center Tax Profile Information) in countries with a US treaty making a sale to a US-based customer (as defined by their customer account address).</span></span> <span data-ttu-id="08bee-137">O governo dos EUA não exige que a Microsoft retenha o imposto em nome da editora.</span><span class="sxs-lookup"><span data-stu-id="08bee-137">US government does not require Microsoft to withhold tax on behalf of the publisher.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-e.png" alt-text="Mostra fluxo de trabalho para o cenário do processo de pagamento E.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-outside-ireland"></a><span data-ttu-id="08bee-139">Editora estrangeira vende a um cliente registado na UE com IVA num país gerido pela Microsoft (fora da Irlanda)</span><span class="sxs-lookup"><span data-stu-id="08bee-139">Foreign publisher sells to an EU VAT-registered customer in a Microsoft-managed country (outside Ireland)</span></span>

<span data-ttu-id="08bee-140">**Cenário F** – Todas as transações entre editores estrangeiros e clientes registados em IVA da UE (fora da Irlanda) num país Microsoft-Managed.</span><span class="sxs-lookup"><span data-stu-id="08bee-140">**Scenario F** – All transactions between foreign publishers and EU VAT-registered customers (outside Ireland) in a Microsoft-Managed country.</span></span> <span data-ttu-id="08bee-141">O cliente não paga imposto sobre a venda.</span><span class="sxs-lookup"><span data-stu-id="08bee-141">The customer does not pay tax on the sale.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-f.png" alt-text="Mostra fluxo de trabalho para o cenário do processo de pagamento F.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-in-ireland"></a><span data-ttu-id="08bee-143">Editora estrangeira vende a um cliente registado na UE com IVA num país gerido pela Microsoft (na Irlanda)</span><span class="sxs-lookup"><span data-stu-id="08bee-143">Foreign publisher sells to an EU VAT-registered customer in a Microsoft-managed country (in Ireland)</span></span>

<span data-ttu-id="08bee-144">**Cenário G** – Todas as transações entre editores estrangeiros e clientes registados em IVA da UE (dentro da Irlanda) num país Microsoft-Managed.</span><span class="sxs-lookup"><span data-stu-id="08bee-144">**Scenario G** – All transactions between foreign publishers and EU VAT-registered customers (inside Ireland) in a Microsoft-Managed country.</span></span> <span data-ttu-id="08bee-145">O cliente paga IVA irlandês e a Microsoft paga este imposto ao governo irlandês.</span><span class="sxs-lookup"><span data-stu-id="08bee-145">The customer pays Irish VAT and Microsoft pays this tax to the Irish government.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-g.png" alt-text="Mostra fluxo de trabalho para o cenário de processo de pagamento G.":::

## <a name="next-steps"></a><span data-ttu-id="08bee-147">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="08bee-147">Next steps</span></span>

- [<span data-ttu-id="08bee-148">Editor FAQ</span><span class="sxs-lookup"><span data-stu-id="08bee-148">Publisher FAQ</span></span>](/azure/marketplace/marketplace-faq-publisher-guide)
- [<span data-ttu-id="08bee-149">Instruções para criar perfis de pagamento e impostos</span><span class="sxs-lookup"><span data-stu-id="08bee-149">Instructions to create payment and tax profiles</span></span>](./set-up-your-payout-account.md?context=%2fazure%2fmarketplace%2fcontext%2fcontext#create-a-payment-profile)