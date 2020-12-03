---
title: Cálculo efetivo do preço por unidade
ms.topic: how-to
ms.date: 11/10/2020
description: Saiba mais sobre o preço unitário eficaz e como é calculado. Este artigo também inclui um cálculo de amostra.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 6ca6e9bf6a49e695314a3e33e36d2d1d5d4d2a25
ms.sourcegitcommit: 147813ba322653c989df5afe0b3bf0c252523a92
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/03/2020
ms.locfileid: "96556332"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a><span data-ttu-id="22b53-104">Cálculo efetivo dos preços unitários para o consumo do plano Azure</span><span class="sxs-lookup"><span data-stu-id="22b53-104">Effective unit price calculation for Azure plan consumption</span></span>

## <a name="the-effective-unit-price"></a><span data-ttu-id="22b53-105">O preço unitário efetivo</span><span class="sxs-lookup"><span data-stu-id="22b53-105">The effective unit price</span></span>

<span data-ttu-id="22b53-106">O preço unitário efetivo é calculado ao nível do contador (ao contrário do nível de recursos), e é ajustado diariamente de acordo com a utilização do medidor.</span><span class="sxs-lookup"><span data-stu-id="22b53-106">The effective unit price is calculated at the meter level (as opposed to the resource level), and is adjusted daily according to meter usage.</span></span>

<span data-ttu-id="22b53-107">Calculamos o preço unitário efetivo utilizando os seguintes três fatores:</span><span class="sxs-lookup"><span data-stu-id="22b53-107">We calculate the effective unit price using the following three factors:</span></span>

- <span data-ttu-id="22b53-108">Consumo, que é monitorizado diariamente ao longo do ciclo de faturação</span><span class="sxs-lookup"><span data-stu-id="22b53-108">Consumption, which is monitored daily throughout the billing cycle</span></span>
- <span data-ttu-id="22b53-109">Custo faturado para o contador</span><span class="sxs-lookup"><span data-stu-id="22b53-109">Billable cost for the meter</span></span>
- <span data-ttu-id="22b53-110">Tiering (se aplicável)</span><span class="sxs-lookup"><span data-stu-id="22b53-110">Tiering (if applicable)</span></span>

<span data-ttu-id="22b53-111">Como monitorizamos o consumo diariamente ao longo do ciclo de faturação, o preço unitário efetivo irá oscilar.</span><span class="sxs-lookup"><span data-stu-id="22b53-111">Because we monitor consumption daily throughout the billing cycle, the effective unit price will fluctuate.</span></span> <span data-ttu-id="22b53-112">O preço final de um determinado ciclo de faturação estará disponível depois de pararmos o cálculo do consumo e fecharmos o período de faturação.</span><span class="sxs-lookup"><span data-stu-id="22b53-112">The final price for a given billing cycle will be available after we stop the consumption calculation and close the billing period.</span></span> <span data-ttu-id="22b53-113">Verá a maioria das mudanças no consumo após a quarta ou quinta decimal.</span><span class="sxs-lookup"><span data-stu-id="22b53-113">You’ll see most changes in consumption after the fourth or fifth decimal place.</span></span>

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a><span data-ttu-id="22b53-114">Descubra se o seu contador utiliza preços hierárquicos</span><span class="sxs-lookup"><span data-stu-id="22b53-114">Find out whether your meter uses tiered pricing</span></span>

<span data-ttu-id="22b53-115">Se não sabe se o seu contador utiliza preços hierárquicos, use o procedimento abaixo para saber.</span><span class="sxs-lookup"><span data-stu-id="22b53-115">If you don’t know whether your meter uses tiered pricing, use the procedure below to find out.</span></span> 

1. <span data-ttu-id="22b53-116">Inicie sessão no [dashboard do Centro de Parceiros](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="22b53-116">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="22b53-117">Selecione **Vender,** **selecione Preços e ofertas**, e, em seguida, selecione **preços do plano Azure**.</span><span class="sxs-lookup"><span data-stu-id="22b53-117">Select **Sell**, select **Pricing and offers**, and then select **Azure plan pricing**.</span></span>
3. <span data-ttu-id="22b53-118">Localize o seu medidor por ID e, em seguida, descarregue os seus dados de preços.</span><span class="sxs-lookup"><span data-stu-id="22b53-118">Locate your meter by ID, and then download your pricing data.</span></span> 

## <a name="sample-calculation"></a><span data-ttu-id="22b53-119">Cálculo da amostra</span><span class="sxs-lookup"><span data-stu-id="22b53-119">Sample calculation</span></span>

<span data-ttu-id="22b53-120">O quadro abaixo dá um exemplo de como calculamos o preço unitário efetivo durante o período aberto.</span><span class="sxs-lookup"><span data-stu-id="22b53-120">The table below gives an example of how we calculate the effective unit price during the open period.</span></span>

<span data-ttu-id="22b53-121">Na tabela, aplicam-se os seguintes valores:</span><span class="sxs-lookup"><span data-stu-id="22b53-121">In the table, the following values apply:</span></span> 

- <span data-ttu-id="22b53-122">**UP** = Preço unitário do recurso/hora = 0,868</span><span class="sxs-lookup"><span data-stu-id="22b53-122">**UP** = Unit price of the resource/hour = 0.868</span></span>

- <span data-ttu-id="22b53-123">**BCU** = Unidade de consumo alusário para o contador</span><span class="sxs-lookup"><span data-stu-id="22b53-123">**BCU** = Billable consumption unit for the meter</span></span>

- <span data-ttu-id="22b53-124">**BC** = Custo billable para o medidor = BCU \* UP \* 0,85.</span><span class="sxs-lookup"><span data-stu-id="22b53-124">**BC** = Billable cost for the meter = BCU \* UP \* 0.85.</span></span> <span data-ttu-id="22b53-125">Isto reflete um ajustamento para o desconto de 15% do PEC.</span><span class="sxs-lookup"><span data-stu-id="22b53-125">This reflects an adjustment for the 15% PEC discount.</span></span> <span data-ttu-id="22b53-126">Em seguida, usamos o limite inferior da função para limitar o valor a dois dígitos após o ponto decimal, de modo a cobrar o valor mínimo.</span><span class="sxs-lookup"><span data-stu-id="22b53-126">We then use the lower limit of the function to limit the value to two digits after the decimal point, in order to charge the minimum amount.</span></span> 

- <span data-ttu-id="22b53-127">**Preço unitário efetivo** = BCU/BC</span><span class="sxs-lookup"><span data-stu-id="22b53-127">**Effective unit price** = BCU/BC</span></span>

>[!NOTE]
><span data-ttu-id="22b53-128">Nota: O medidor neste exemplo não tem níveis de preços.</span><span class="sxs-lookup"><span data-stu-id="22b53-128">Note: The meter in this example does not have tiers in pricing.</span></span>

| <span data-ttu-id="22b53-129">Data</span><span class="sxs-lookup"><span data-stu-id="22b53-129">Date</span></span> | <span data-ttu-id="22b53-130">BCU (unidade de consumo a cobrar)</span><span class="sxs-lookup"><span data-stu-id="22b53-130">BCU (Billable consumption unit)</span></span> | <span data-ttu-id="22b53-131">BC (Custo faturado)</span><span class="sxs-lookup"><span data-stu-id="22b53-131">BC (Billable cost)</span></span> | <span data-ttu-id="22b53-132">Preço unitário eficaz</span><span class="sxs-lookup"><span data-stu-id="22b53-132">Effective unit price</span></span> |
| ------ | ----------- | ----------- | ----------- |  
| <span data-ttu-id="22b53-133">3-Ago</span><span class="sxs-lookup"><span data-stu-id="22b53-133">3-Aug</span></span> | <span data-ttu-id="22b53-134">29</span><span class="sxs-lookup"><span data-stu-id="22b53-134">29</span></span> | <span data-ttu-id="22b53-135">21.39</span><span class="sxs-lookup"><span data-stu-id="22b53-135">21.39</span></span> | <span data-ttu-id="22b53-136">0.737586206896552</span><span class="sxs-lookup"><span data-stu-id="22b53-136">0.737586206896552</span></span> |
| <span data-ttu-id="22b53-137">10 ago</span><span class="sxs-lookup"><span data-stu-id="22b53-137">10-Aug</span></span> | <span data-ttu-id="22b53-138">210.950039</span><span class="sxs-lookup"><span data-stu-id="22b53-138">210.950039</span></span> | <span data-ttu-id="22b53-139">155.63</span><span class="sxs-lookup"><span data-stu-id="22b53-139">155.63</span></span> | <span data-ttu-id="22b53-140">0.737757626107858</span><span class="sxs-lookup"><span data-stu-id="22b53-140">0.737757626107858</span></span> |
| <span data-ttu-id="22b53-141">25 ago</span><span class="sxs-lookup"><span data-stu-id="22b53-141">25-Aug</span></span> | <span data-ttu-id="22b53-142">555.950039</span><span class="sxs-lookup"><span data-stu-id="22b53-142">555.950039</span></span> | <span data-ttu-id="22b53-143">410.17</span><span class="sxs-lookup"><span data-stu-id="22b53-143">410.17</span></span> | <span data-ttu-id="22b53-144">0.737782122900436</span><span class="sxs-lookup"><span data-stu-id="22b53-144">0.737782122900436</span></span> |

## <a name="next-steps"></a><span data-ttu-id="22b53-145">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="22b53-145">Next steps</span></span>

- [<span data-ttu-id="22b53-146">Faturação e impostos</span><span class="sxs-lookup"><span data-stu-id="22b53-146">Billing and taxes</span></span>](billing.md)
