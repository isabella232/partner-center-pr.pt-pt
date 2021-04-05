---
title: Cálculo efetivo do preço por unidade
ms.topic: how-to
ms.date: 04/02/2021
description: Saiba mais sobre o preço unitário eficaz e como é calculado. Este artigo também inclui um cálculo de amostra.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a662e0b815c979b3454762c5b35eb510887c96ad
ms.sourcegitcommit: c6c741475604b8daf386fb54bb2795a6445ac887
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/05/2021
ms.locfileid: "106374403"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a><span data-ttu-id="11f21-104">Cálculo efetivo dos preços unitários para o consumo do plano Azure</span><span class="sxs-lookup"><span data-stu-id="11f21-104">Effective unit price calculation for Azure plan consumption</span></span>

## <a name="the-effective-unit-price"></a><span data-ttu-id="11f21-105">O preço unitário efetivo</span><span class="sxs-lookup"><span data-stu-id="11f21-105">The effective unit price</span></span>

<span data-ttu-id="11f21-106">O preço unitário efetivo é calculado ao nível do contador (ao contrário do nível de recursos), e é ajustado diariamente de acordo com a utilização do medidor.</span><span class="sxs-lookup"><span data-stu-id="11f21-106">The effective unit price is calculated at the meter level (as opposed to the resource level), and is adjusted daily according to meter usage.</span></span>

<span data-ttu-id="11f21-107">Calculamos o preço unitário efetivo utilizando os seguintes três fatores:</span><span class="sxs-lookup"><span data-stu-id="11f21-107">We calculate the effective unit price using the following three factors:</span></span>

- <span data-ttu-id="11f21-108">Consumo, que é monitorizado diariamente ao longo do ciclo de faturação</span><span class="sxs-lookup"><span data-stu-id="11f21-108">Consumption, which is monitored daily throughout the billing cycle</span></span>
- <span data-ttu-id="11f21-109">Custo faturado para o contador</span><span class="sxs-lookup"><span data-stu-id="11f21-109">Billable cost for the meter</span></span>
- <span data-ttu-id="11f21-110">Tiering (se aplicável)</span><span class="sxs-lookup"><span data-stu-id="11f21-110">Tiering (if applicable)</span></span>

<span data-ttu-id="11f21-111">Como monitorizamos o consumo diariamente ao longo do ciclo de faturação, o preço unitário efetivo irá oscilar.</span><span class="sxs-lookup"><span data-stu-id="11f21-111">Because we monitor consumption daily throughout the billing cycle, the effective unit price will fluctuate.</span></span> <span data-ttu-id="11f21-112">O preço final de um determinado ciclo de faturação estará disponível depois de pararmos o cálculo do consumo e fecharmos o período de faturação.</span><span class="sxs-lookup"><span data-stu-id="11f21-112">The final price for a given billing cycle will be available after we stop the consumption calculation and close the billing period.</span></span> <span data-ttu-id="11f21-113">Verá a maioria das mudanças no consumo após a quarta ou quinta decimal.</span><span class="sxs-lookup"><span data-stu-id="11f21-113">You’ll see most changes in consumption after the fourth or fifth decimal place.</span></span>

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a><span data-ttu-id="11f21-114">Descubra se o seu contador utiliza preços hierárquicos</span><span class="sxs-lookup"><span data-stu-id="11f21-114">Find out whether your meter uses tiered pricing</span></span>

<span data-ttu-id="11f21-115">Se não sabe se o seu contador utiliza preços hierárquicos, use o procedimento abaixo para saber.</span><span class="sxs-lookup"><span data-stu-id="11f21-115">If you don’t know whether your meter uses tiered pricing, use the procedure below to find out.</span></span> 

1. <span data-ttu-id="11f21-116">Inicie sessão no [dashboard do Centro de Parceiros](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="11f21-116">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="11f21-117">Selecione **Vender,** **selecione Preços e ofertas**, e, em seguida, selecione **preços do plano Azure**.</span><span class="sxs-lookup"><span data-stu-id="11f21-117">Select **Sell**, select **Pricing and offers**, and then select **Azure plan pricing**.</span></span>
3. <span data-ttu-id="11f21-118">Localize o seu medidor por ID e, em seguida, descarregue os seus dados de preços.</span><span class="sxs-lookup"><span data-stu-id="11f21-118">Locate your meter by ID, and then download your pricing data.</span></span> 

## <a name="sample-calculation"></a><span data-ttu-id="11f21-119">Cálculo da amostra</span><span class="sxs-lookup"><span data-stu-id="11f21-119">Sample calculation</span></span>

<span data-ttu-id="11f21-120">O quadro abaixo dá um exemplo de como calculamos o preço unitário efetivo durante o período aberto.</span><span class="sxs-lookup"><span data-stu-id="11f21-120">The table below gives an example of how we calculate the effective unit price during the open period.</span></span>

<span data-ttu-id="11f21-121">Na tabela, aplicam-se os seguintes valores:</span><span class="sxs-lookup"><span data-stu-id="11f21-121">In the table, the following values apply:</span></span> 

- <span data-ttu-id="11f21-122">**UP** = Preço unitário do recurso/hora = 0,868</span><span class="sxs-lookup"><span data-stu-id="11f21-122">**UP** = Unit price of the resource/hour = 0.868</span></span>

- <span data-ttu-id="11f21-123">**BCU** = Unidade de consumo alusário para o contador</span><span class="sxs-lookup"><span data-stu-id="11f21-123">**BCU** = Billable consumption unit for the meter</span></span>

- <span data-ttu-id="11f21-124">**BC** = Custo billable para o medidor = BCU \* UP \* 0,85.</span><span class="sxs-lookup"><span data-stu-id="11f21-124">**BC** = Billable cost for the meter = BCU \* UP \* 0.85.</span></span> <span data-ttu-id="11f21-125">Isto reflete um ajustamento para o desconto de 15% do PEC.</span><span class="sxs-lookup"><span data-stu-id="11f21-125">This reflects an adjustment for the 15% PEC discount.</span></span> <span data-ttu-id="11f21-126">Em seguida, usamos o limite inferior da função para limitar o valor a dois dígitos após o ponto decimal, de modo a cobrar o valor mínimo.</span><span class="sxs-lookup"><span data-stu-id="11f21-126">We then use the lower limit of the function to limit the value to two digits after the decimal point, in order to charge the minimum amount.</span></span> 

- <span data-ttu-id="11f21-127">**Preço unitário efetivo** = BCU/BC</span><span class="sxs-lookup"><span data-stu-id="11f21-127">**Effective unit price** = BCU/BC</span></span>

>[!NOTE]
><span data-ttu-id="11f21-128">O medidor neste exemplo não tem níveis de preços.</span><span class="sxs-lookup"><span data-stu-id="11f21-128">The meter in this example does not have tiers in pricing.</span></span> <span data-ttu-id="11f21-129">Os fatores de preço unitário efetivo em percentagens de desconto e outros ajustamentos.</span><span class="sxs-lookup"><span data-stu-id="11f21-129">The Effective Unit Price factors in discount percentages and other adjustments.</span></span>

| <span data-ttu-id="11f21-130">Data</span><span class="sxs-lookup"><span data-stu-id="11f21-130">Date</span></span> | <span data-ttu-id="11f21-131">BCU (unidade de consumo a cobrar)</span><span class="sxs-lookup"><span data-stu-id="11f21-131">BCU (Billable consumption unit)</span></span> | <span data-ttu-id="11f21-132">BC (Custo faturado)</span><span class="sxs-lookup"><span data-stu-id="11f21-132">BC (Billable cost)</span></span> | <span data-ttu-id="11f21-133">Preço unitário eficaz</span><span class="sxs-lookup"><span data-stu-id="11f21-133">Effective unit price</span></span> |
| ------ | ----------- | ----------- | ----------- |  
| <span data-ttu-id="11f21-134">3-Ago</span><span class="sxs-lookup"><span data-stu-id="11f21-134">3-Aug</span></span> | <span data-ttu-id="11f21-135">29</span><span class="sxs-lookup"><span data-stu-id="11f21-135">29</span></span> | <span data-ttu-id="11f21-136">21.39</span><span class="sxs-lookup"><span data-stu-id="11f21-136">21.39</span></span> | <span data-ttu-id="11f21-137">0.737586206896552</span><span class="sxs-lookup"><span data-stu-id="11f21-137">0.737586206896552</span></span> |
| <span data-ttu-id="11f21-138">10 ago</span><span class="sxs-lookup"><span data-stu-id="11f21-138">10-Aug</span></span> | <span data-ttu-id="11f21-139">210.950039</span><span class="sxs-lookup"><span data-stu-id="11f21-139">210.950039</span></span> | <span data-ttu-id="11f21-140">155.63</span><span class="sxs-lookup"><span data-stu-id="11f21-140">155.63</span></span> | <span data-ttu-id="11f21-141">0.737757626107858</span><span class="sxs-lookup"><span data-stu-id="11f21-141">0.737757626107858</span></span> |
| <span data-ttu-id="11f21-142">25 ago</span><span class="sxs-lookup"><span data-stu-id="11f21-142">25-Aug</span></span> | <span data-ttu-id="11f21-143">555.950039</span><span class="sxs-lookup"><span data-stu-id="11f21-143">555.950039</span></span> | <span data-ttu-id="11f21-144">410.17</span><span class="sxs-lookup"><span data-stu-id="11f21-144">410.17</span></span> | <span data-ttu-id="11f21-145">0.737782122900436</span><span class="sxs-lookup"><span data-stu-id="11f21-145">0.737782122900436</span></span> |

## <a name="next-steps"></a><span data-ttu-id="11f21-146">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="11f21-146">Next steps</span></span>

- [<span data-ttu-id="11f21-147">Faturação e impostos</span><span class="sxs-lookup"><span data-stu-id="11f21-147">Billing and taxes</span></span>](billing.md)
