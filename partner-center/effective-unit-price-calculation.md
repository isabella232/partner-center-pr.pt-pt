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
ms.openlocfilehash: 84beac77d41b8c11be9ac3cad87460eec9632ac4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147127"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a><span data-ttu-id="f5439-104">Cálculo efetivo dos preços unitários para o consumo do plano Azure</span><span class="sxs-lookup"><span data-stu-id="f5439-104">Effective unit price calculation for Azure plan consumption</span></span>

<span data-ttu-id="f5439-105">**Funções apropriadas**: Administrador de Faturação</span><span class="sxs-lookup"><span data-stu-id="f5439-105">**Appropriate roles**: Billing admin</span></span>

## <a name="the-effective-unit-price"></a><span data-ttu-id="f5439-106">O preço unitário efetivo</span><span class="sxs-lookup"><span data-stu-id="f5439-106">The effective unit price</span></span>

<span data-ttu-id="f5439-107">O preço unitário efetivo é calculado ao nível do contador (ao contrário do nível de recursos), e é ajustado diariamente de acordo com a utilização do medidor.</span><span class="sxs-lookup"><span data-stu-id="f5439-107">The effective unit price is calculated at the meter level (as opposed to the resource level), and is adjusted daily according to meter usage.</span></span>

<span data-ttu-id="f5439-108">Calculamos o preço unitário efetivo utilizando os seguintes três fatores:</span><span class="sxs-lookup"><span data-stu-id="f5439-108">We calculate the effective unit price using the following three factors:</span></span>

- <span data-ttu-id="f5439-109">Consumo, que é monitorizado diariamente ao longo do ciclo de faturação</span><span class="sxs-lookup"><span data-stu-id="f5439-109">Consumption, which is monitored daily throughout the billing cycle</span></span>
- <span data-ttu-id="f5439-110">Custo faturado para o contador</span><span class="sxs-lookup"><span data-stu-id="f5439-110">Billable cost for the meter</span></span>
- <span data-ttu-id="f5439-111">Tiering (se aplicável)</span><span class="sxs-lookup"><span data-stu-id="f5439-111">Tiering (if applicable)</span></span>

<span data-ttu-id="f5439-112">Como monitorizamos o consumo diariamente ao longo do ciclo de faturação, o preço unitário efetivo irá oscilar.</span><span class="sxs-lookup"><span data-stu-id="f5439-112">Because we monitor consumption daily throughout the billing cycle, the effective unit price will fluctuate.</span></span> <span data-ttu-id="f5439-113">O preço final de um determinado ciclo de faturação estará disponível depois de pararmos o cálculo do consumo e fecharmos o período de faturação.</span><span class="sxs-lookup"><span data-stu-id="f5439-113">The final price for a given billing cycle will be available after we stop the consumption calculation and close the billing period.</span></span> <span data-ttu-id="f5439-114">Verá a maioria das mudanças no consumo após a quarta ou quinta decimal.</span><span class="sxs-lookup"><span data-stu-id="f5439-114">You’ll see most changes in consumption after the fourth or fifth decimal place.</span></span>

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a><span data-ttu-id="f5439-115">Descubra se o seu contador utiliza preços hierárquicos</span><span class="sxs-lookup"><span data-stu-id="f5439-115">Find out whether your meter uses tiered pricing</span></span>

<span data-ttu-id="f5439-116">Se não sabe se o seu contador utiliza preços hierárquicos, use o procedimento abaixo para saber.</span><span class="sxs-lookup"><span data-stu-id="f5439-116">If you don’t know whether your meter uses tiered pricing, use the procedure below to find out.</span></span> 

1. <span data-ttu-id="f5439-117">Inicie sessão no [dashboard do Centro de Parceiros](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="f5439-117">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="f5439-118">Selecione **Vender,** **selecione Preços e ofertas**, e, em seguida, selecione **preços do plano Azure**.</span><span class="sxs-lookup"><span data-stu-id="f5439-118">Select **Sell**, select **Pricing and offers**, and then select **Azure plan pricing**.</span></span>
3. <span data-ttu-id="f5439-119">Localize o seu medidor por ID e, em seguida, descarregue os seus dados de preços.</span><span class="sxs-lookup"><span data-stu-id="f5439-119">Locate your meter by ID, and then download your pricing data.</span></span> 

## <a name="sample-calculation"></a><span data-ttu-id="f5439-120">Cálculo da amostra</span><span class="sxs-lookup"><span data-stu-id="f5439-120">Sample calculation</span></span>

<span data-ttu-id="f5439-121">O quadro abaixo dá um exemplo de como calculamos o preço unitário efetivo durante o período aberto.</span><span class="sxs-lookup"><span data-stu-id="f5439-121">The table below gives an example of how we calculate the effective unit price during the open period.</span></span>

<span data-ttu-id="f5439-122">Na tabela, aplicam-se os seguintes valores:</span><span class="sxs-lookup"><span data-stu-id="f5439-122">In the table, the following values apply:</span></span> 

- <span data-ttu-id="f5439-123">**UP** = Preço unitário do recurso/hora = 0,868</span><span class="sxs-lookup"><span data-stu-id="f5439-123">**UP** = Unit price of the resource/hour = 0.868</span></span>

- <span data-ttu-id="f5439-124">**BCU** = Unidade de consumo alusário para o contador</span><span class="sxs-lookup"><span data-stu-id="f5439-124">**BCU** = Billable consumption unit for the meter</span></span>

- <span data-ttu-id="f5439-125">**BC** = Custo billable para o medidor = BCU \* UP \* 0,85.</span><span class="sxs-lookup"><span data-stu-id="f5439-125">**BC** = Billable cost for the meter = BCU \* UP \* 0.85.</span></span> <span data-ttu-id="f5439-126">Isto reflete um ajustamento para o desconto de 15% do PEC.</span><span class="sxs-lookup"><span data-stu-id="f5439-126">This reflects an adjustment for the 15% PEC discount.</span></span> <span data-ttu-id="f5439-127">Em seguida, usamos o limite inferior da função para limitar o valor a dois dígitos após o ponto decimal, de modo a cobrar o valor mínimo.</span><span class="sxs-lookup"><span data-stu-id="f5439-127">We then use the lower limit of the function to limit the value to two digits after the decimal point, in order to charge the minimum amount.</span></span> 

- <span data-ttu-id="f5439-128">**Preço unitário efetivo** = BCU/BC</span><span class="sxs-lookup"><span data-stu-id="f5439-128">**Effective unit price** = BCU/BC</span></span>

>[!NOTE]

><span data-ttu-id="f5439-129">Nota: O medidor neste exemplo não tem níveis de preços ou outros descontos — os fatores de Preço Unitário Efetivo em percentagens de desconto e outros ajustes.</span><span class="sxs-lookup"><span data-stu-id="f5439-129">Note: The meter in this example does not have tiers in pricing or other discounts—the Effective Unit Price factors in discount percentages and other adjustments.</span></span>


| <span data-ttu-id="f5439-130">Data</span><span class="sxs-lookup"><span data-stu-id="f5439-130">Date</span></span> | <span data-ttu-id="f5439-131">BCU (unidade de consumo a cobrar)</span><span class="sxs-lookup"><span data-stu-id="f5439-131">BCU (Billable consumption unit)</span></span> | <span data-ttu-id="f5439-132">BC (Custo faturado)</span><span class="sxs-lookup"><span data-stu-id="f5439-132">BC (Billable cost)</span></span> | <span data-ttu-id="f5439-133">Preço unitário eficaz</span><span class="sxs-lookup"><span data-stu-id="f5439-133">Effective unit price</span></span> |
| ------ | ----------- | ----------- | ----------- |  
| <span data-ttu-id="f5439-134">3-Ago</span><span class="sxs-lookup"><span data-stu-id="f5439-134">3-Aug</span></span> | <span data-ttu-id="f5439-135">29</span><span class="sxs-lookup"><span data-stu-id="f5439-135">29</span></span> | <span data-ttu-id="f5439-136">21.39</span><span class="sxs-lookup"><span data-stu-id="f5439-136">21.39</span></span> | <span data-ttu-id="f5439-137">0.737586206896552</span><span class="sxs-lookup"><span data-stu-id="f5439-137">0.737586206896552</span></span> |
| <span data-ttu-id="f5439-138">10 ago</span><span class="sxs-lookup"><span data-stu-id="f5439-138">10-Aug</span></span> | <span data-ttu-id="f5439-139">210.950039</span><span class="sxs-lookup"><span data-stu-id="f5439-139">210.950039</span></span> | <span data-ttu-id="f5439-140">155.63</span><span class="sxs-lookup"><span data-stu-id="f5439-140">155.63</span></span> | <span data-ttu-id="f5439-141">0.737757626107858</span><span class="sxs-lookup"><span data-stu-id="f5439-141">0.737757626107858</span></span> |
| <span data-ttu-id="f5439-142">25 ago</span><span class="sxs-lookup"><span data-stu-id="f5439-142">25-Aug</span></span> | <span data-ttu-id="f5439-143">555.950039</span><span class="sxs-lookup"><span data-stu-id="f5439-143">555.950039</span></span> | <span data-ttu-id="f5439-144">410.17</span><span class="sxs-lookup"><span data-stu-id="f5439-144">410.17</span></span> | <span data-ttu-id="f5439-145">0.737782122900436</span><span class="sxs-lookup"><span data-stu-id="f5439-145">0.737782122900436</span></span> |

## <a name="next-steps"></a><span data-ttu-id="f5439-146">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="f5439-146">Next steps</span></span>

- [<span data-ttu-id="f5439-147">Faturação e impostos</span><span class="sxs-lookup"><span data-stu-id="f5439-147">Billing and taxes</span></span>](billing.md)
