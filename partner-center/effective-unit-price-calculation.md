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
ms.openlocfilehash: 1473b3c0b90cca1152b4dab0b8efec86dbc3d22d
ms.sourcegitcommit: f8fd51e1acdbfafdde86d6490bade66c63033ebd
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/28/2021
ms.locfileid: "108172222"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a><span data-ttu-id="27a94-104">Cálculo efetivo dos preços unitários para o consumo do plano Azure</span><span class="sxs-lookup"><span data-stu-id="27a94-104">Effective unit price calculation for Azure plan consumption</span></span>

<span data-ttu-id="27a94-105">**Funções adequadas**</span><span class="sxs-lookup"><span data-stu-id="27a94-105">**Appropriate roles**</span></span>

- <span data-ttu-id="27a94-106">Administrador de faturação</span><span class="sxs-lookup"><span data-stu-id="27a94-106">Billing admin</span></span>

## <a name="the-effective-unit-price"></a><span data-ttu-id="27a94-107">O preço unitário efetivo</span><span class="sxs-lookup"><span data-stu-id="27a94-107">The effective unit price</span></span>

<span data-ttu-id="27a94-108">O preço unitário efetivo é calculado ao nível do contador (ao contrário do nível de recursos), e é ajustado diariamente de acordo com a utilização do medidor.</span><span class="sxs-lookup"><span data-stu-id="27a94-108">The effective unit price is calculated at the meter level (as opposed to the resource level), and is adjusted daily according to meter usage.</span></span>

<span data-ttu-id="27a94-109">Calculamos o preço unitário efetivo utilizando os seguintes três fatores:</span><span class="sxs-lookup"><span data-stu-id="27a94-109">We calculate the effective unit price using the following three factors:</span></span>

- <span data-ttu-id="27a94-110">Consumo, que é monitorizado diariamente ao longo do ciclo de faturação</span><span class="sxs-lookup"><span data-stu-id="27a94-110">Consumption, which is monitored daily throughout the billing cycle</span></span>
- <span data-ttu-id="27a94-111">Custo faturado para o contador</span><span class="sxs-lookup"><span data-stu-id="27a94-111">Billable cost for the meter</span></span>
- <span data-ttu-id="27a94-112">Tiering (se aplicável)</span><span class="sxs-lookup"><span data-stu-id="27a94-112">Tiering (if applicable)</span></span>

<span data-ttu-id="27a94-113">Como monitorizamos o consumo diariamente ao longo do ciclo de faturação, o preço unitário efetivo irá oscilar.</span><span class="sxs-lookup"><span data-stu-id="27a94-113">Because we monitor consumption daily throughout the billing cycle, the effective unit price will fluctuate.</span></span> <span data-ttu-id="27a94-114">O preço final de um determinado ciclo de faturação estará disponível depois de pararmos o cálculo do consumo e fecharmos o período de faturação.</span><span class="sxs-lookup"><span data-stu-id="27a94-114">The final price for a given billing cycle will be available after we stop the consumption calculation and close the billing period.</span></span> <span data-ttu-id="27a94-115">Verá a maioria das mudanças no consumo após a quarta ou quinta decimal.</span><span class="sxs-lookup"><span data-stu-id="27a94-115">You’ll see most changes in consumption after the fourth or fifth decimal place.</span></span>

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a><span data-ttu-id="27a94-116">Descubra se o seu contador utiliza preços hierárquicos</span><span class="sxs-lookup"><span data-stu-id="27a94-116">Find out whether your meter uses tiered pricing</span></span>

<span data-ttu-id="27a94-117">Se não sabe se o seu contador utiliza preços hierárquicos, use o procedimento abaixo para saber.</span><span class="sxs-lookup"><span data-stu-id="27a94-117">If you don’t know whether your meter uses tiered pricing, use the procedure below to find out.</span></span> 

1. <span data-ttu-id="27a94-118">Inicie sessão no [dashboard do Centro de Parceiros](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="27a94-118">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="27a94-119">Selecione **Vender,** **selecione Preços e ofertas**, e, em seguida, selecione **preços do plano Azure**.</span><span class="sxs-lookup"><span data-stu-id="27a94-119">Select **Sell**, select **Pricing and offers**, and then select **Azure plan pricing**.</span></span>
3. <span data-ttu-id="27a94-120">Localize o seu medidor por ID e, em seguida, descarregue os seus dados de preços.</span><span class="sxs-lookup"><span data-stu-id="27a94-120">Locate your meter by ID, and then download your pricing data.</span></span> 

## <a name="sample-calculation"></a><span data-ttu-id="27a94-121">Cálculo da amostra</span><span class="sxs-lookup"><span data-stu-id="27a94-121">Sample calculation</span></span>

<span data-ttu-id="27a94-122">O quadro abaixo dá um exemplo de como calculamos o preço unitário efetivo durante o período aberto.</span><span class="sxs-lookup"><span data-stu-id="27a94-122">The table below gives an example of how we calculate the effective unit price during the open period.</span></span>

<span data-ttu-id="27a94-123">Na tabela, aplicam-se os seguintes valores:</span><span class="sxs-lookup"><span data-stu-id="27a94-123">In the table, the following values apply:</span></span> 

- <span data-ttu-id="27a94-124">**UP** = Preço unitário do recurso/hora = 0,868</span><span class="sxs-lookup"><span data-stu-id="27a94-124">**UP** = Unit price of the resource/hour = 0.868</span></span>

- <span data-ttu-id="27a94-125">**BCU** = Unidade de consumo alusário para o contador</span><span class="sxs-lookup"><span data-stu-id="27a94-125">**BCU** = Billable consumption unit for the meter</span></span>

- <span data-ttu-id="27a94-126">**BC** = Custo billable para o medidor = BCU \* UP \* 0,85.</span><span class="sxs-lookup"><span data-stu-id="27a94-126">**BC** = Billable cost for the meter = BCU \* UP \* 0.85.</span></span> <span data-ttu-id="27a94-127">Isto reflete um ajustamento para o desconto de 15% do PEC.</span><span class="sxs-lookup"><span data-stu-id="27a94-127">This reflects an adjustment for the 15% PEC discount.</span></span> <span data-ttu-id="27a94-128">Em seguida, usamos o limite inferior da função para limitar o valor a dois dígitos após o ponto decimal, de modo a cobrar o valor mínimo.</span><span class="sxs-lookup"><span data-stu-id="27a94-128">We then use the lower limit of the function to limit the value to two digits after the decimal point, in order to charge the minimum amount.</span></span> 

- <span data-ttu-id="27a94-129">**Preço unitário efetivo** = BCU/BC</span><span class="sxs-lookup"><span data-stu-id="27a94-129">**Effective unit price** = BCU/BC</span></span>

>[!NOTE]

><span data-ttu-id="27a94-130">Nota: O medidor neste exemplo não tem níveis de preços ou outros descontos — os fatores de Preço Unitário Efetivo em percentagens de desconto e outros ajustes.</span><span class="sxs-lookup"><span data-stu-id="27a94-130">Note: The meter in this example does not have tiers in pricing or other discounts—the Effective Unit Price factors in discount percentages and other adjustments.</span></span>


| <span data-ttu-id="27a94-131">Data</span><span class="sxs-lookup"><span data-stu-id="27a94-131">Date</span></span> | <span data-ttu-id="27a94-132">BCU (unidade de consumo a cobrar)</span><span class="sxs-lookup"><span data-stu-id="27a94-132">BCU (Billable consumption unit)</span></span> | <span data-ttu-id="27a94-133">BC (Custo faturado)</span><span class="sxs-lookup"><span data-stu-id="27a94-133">BC (Billable cost)</span></span> | <span data-ttu-id="27a94-134">Preço unitário eficaz</span><span class="sxs-lookup"><span data-stu-id="27a94-134">Effective unit price</span></span> |
| ------ | ----------- | ----------- | ----------- |  
| <span data-ttu-id="27a94-135">3-Ago</span><span class="sxs-lookup"><span data-stu-id="27a94-135">3-Aug</span></span> | <span data-ttu-id="27a94-136">29</span><span class="sxs-lookup"><span data-stu-id="27a94-136">29</span></span> | <span data-ttu-id="27a94-137">21.39</span><span class="sxs-lookup"><span data-stu-id="27a94-137">21.39</span></span> | <span data-ttu-id="27a94-138">0.737586206896552</span><span class="sxs-lookup"><span data-stu-id="27a94-138">0.737586206896552</span></span> |
| <span data-ttu-id="27a94-139">10 ago</span><span class="sxs-lookup"><span data-stu-id="27a94-139">10-Aug</span></span> | <span data-ttu-id="27a94-140">210.950039</span><span class="sxs-lookup"><span data-stu-id="27a94-140">210.950039</span></span> | <span data-ttu-id="27a94-141">155.63</span><span class="sxs-lookup"><span data-stu-id="27a94-141">155.63</span></span> | <span data-ttu-id="27a94-142">0.737757626107858</span><span class="sxs-lookup"><span data-stu-id="27a94-142">0.737757626107858</span></span> |
| <span data-ttu-id="27a94-143">25 ago</span><span class="sxs-lookup"><span data-stu-id="27a94-143">25-Aug</span></span> | <span data-ttu-id="27a94-144">555.950039</span><span class="sxs-lookup"><span data-stu-id="27a94-144">555.950039</span></span> | <span data-ttu-id="27a94-145">410.17</span><span class="sxs-lookup"><span data-stu-id="27a94-145">410.17</span></span> | <span data-ttu-id="27a94-146">0.737782122900436</span><span class="sxs-lookup"><span data-stu-id="27a94-146">0.737782122900436</span></span> |

## <a name="next-steps"></a><span data-ttu-id="27a94-147">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="27a94-147">Next steps</span></span>

- [<span data-ttu-id="27a94-148">Faturação e impostos</span><span class="sxs-lookup"><span data-stu-id="27a94-148">Billing and taxes</span></span>](billing.md)
