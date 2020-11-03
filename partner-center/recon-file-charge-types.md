---
title: Tipos de carga de ficheiros de reconciliação
ms.topic: article
ms.date: 06/05/2020
description: Descubra os tipos de encargos (tais como, baseados em licenças, baseados em uso e uma vez), créditos e descontos em ficheiros de reconciliação do Partner Center.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f65c4a6496082934e8c38fbd924b96ef969be95b
ms.sourcegitcommit: e7931fbe7ce16a62124e00b2802520a17d7285b8
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/31/2020
ms.locfileid: "92529388"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a><span data-ttu-id="56314-103">Compreenda os diferentes tipos de carga nos ficheiros de reconciliação do Partner Center</span><span class="sxs-lookup"><span data-stu-id="56314-103">Understand the different charge types in Partner Center reconciliation files</span></span>

<span data-ttu-id="56314-104">**Aplica-se a**</span><span class="sxs-lookup"><span data-stu-id="56314-104">**Applies to**</span></span>

- <span data-ttu-id="56314-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="56314-105">Partner Center</span></span>
- <span data-ttu-id="56314-106">Centro de Parceiros para Microsoft Cloud para governo dos EUA</span><span class="sxs-lookup"><span data-stu-id="56314-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="56314-107">**Funções adequadas**</span><span class="sxs-lookup"><span data-stu-id="56314-107">**Appropriate roles**</span></span>

- <span data-ttu-id="56314-108">Agente administrativo</span><span class="sxs-lookup"><span data-stu-id="56314-108">Admin agent</span></span>
- <span data-ttu-id="56314-109">Administrador de faturação</span><span class="sxs-lookup"><span data-stu-id="56314-109">Billing admin</span></span>
- <span data-ttu-id="56314-110">Administrador global</span><span class="sxs-lookup"><span data-stu-id="56314-110">Global admin</span></span>

<span data-ttu-id="56314-111">Este tópico descreve os mapeamentos entre uma secção de fatura e tipos de carga associados que podem estar no seu ficheiro de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="56314-111">This topic describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span></span> <span data-ttu-id="56314-112">A sua fatura fornece um resumo das taxas.</span><span class="sxs-lookup"><span data-stu-id="56314-112">Your invoice provides a summary of charges.</span></span> <span data-ttu-id="56314-113">O seu ficheiro de reconciliação fornece uma desagregação detalhada das transações de item de linha, incluindo tipos de carga.</span><span class="sxs-lookup"><span data-stu-id="56314-113">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span> <span data-ttu-id="56314-114">Para obter mais informações sobre ficheiros de reconciliação, [consulte como utilizar ficheiros de reconciliação](use-the-reconciliation-files.md).</span><span class="sxs-lookup"><span data-stu-id="56314-114">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span></span>

<span data-ttu-id="56314-115">Tanto os [ficheiros de reconciliação baseados na utilização](usage-based-recon-files.md) como [os ficheiros de reconciliação baseados em licenças](license-based-recon-files.md) apenas mostram transações e encargos relacionados com o uso (unidades consumidas e encargos relacionados).</span><span class="sxs-lookup"><span data-stu-id="56314-115">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span></span>

> [!NOTE]
> <span data-ttu-id="56314-116">Créditos pontuais, descontos ou reembolsos que apareçam na fatura, uma vez que os **ajustes** não constam do ficheiro de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="56314-116">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span></span>

## <a name="map-charge-types-to-invoice-charges"></a><span data-ttu-id="56314-117">Tipos de carga de mapa para cobrar faturas</span><span class="sxs-lookup"><span data-stu-id="56314-117">Map charge types to invoice charges</span></span>

<span data-ttu-id="56314-118">Para cruzar os valores de carga entre a sua fatura e o ficheiro de reconciliação, utilize as opções de filtro no Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="56314-118">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span></span> <span data-ttu-id="56314-119">Filtrar por tipos de carga no seu ficheiro de reconciliação para mapear os encargos da fatura para um conjunto de avarias de carga no ficheiro de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="56314-119">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span></span>

## <a name="license-based-charges"></a><span data-ttu-id="56314-120">Encargos baseados em licença</span><span class="sxs-lookup"><span data-stu-id="56314-120">License-based charges</span></span>

<span data-ttu-id="56314-121">Para mapear estes encargos baseados na licença para a sua fatura, em suma a coluna **Valor** a partir do ficheiro baseado em licença.</span><span class="sxs-lookup"><span data-stu-id="56314-121">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="56314-122">Descrição da carga (coluna ChargeType no ficheiro de reconciliação)</span><span class="sxs-lookup"><span data-stu-id="56314-122">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="56314-123">Explicação de cobrança</span><span class="sxs-lookup"><span data-stu-id="56314-123">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="56314-124">Taxa de ativação</span><span class="sxs-lookup"><span data-stu-id="56314-124">Activation fee</span></span> | <span data-ttu-id="56314-125">O valor cobrado ao cliente quando utiliza a subscrição após a compra.</span><span class="sxs-lookup"><span data-stu-id="56314-125">The amount charged to the customer when they use the subscription after purchase.</span></span> |
| <span data-ttu-id="56314-126">Taxa de cancelamento</span><span class="sxs-lookup"><span data-stu-id="56314-126">Cancel fee</span></span> | <span data-ttu-id="56314-127">Encargos procitados reembolsados ao cliente quando as licenças associadas são alteradas.</span><span class="sxs-lookup"><span data-stu-id="56314-127">Prorated charges refunded to the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="56314-128">Cancelar caso prorate</span><span class="sxs-lookup"><span data-stu-id="56314-128">Cancel instance prorate</span></span> | <span data-ttu-id="56314-129">Os encargos procitados cancelados quando o cliente com subscrição mensal tem subscrição suspensa e as licenças associadas alteradas no mesmo mês.</span><span class="sxs-lookup"><span data-stu-id="56314-129">Prorated charges canceled when customer with monthly subscription has subscription suspended and associated licenses changed within the same month.</span></span> |
| <span data-ttu-id="56314-130">Taxa de ciclo</span><span class="sxs-lookup"><span data-stu-id="56314-130">Cycle fee</span></span> | <span data-ttu-id="56314-131">Encargos periódicos para uma subscrição.</span><span class="sxs-lookup"><span data-stu-id="56314-131">Periodic charges for a subscription.</span></span> |
| <span data-ttu-id="56314-132">Prorate de instância de ciclo</span><span class="sxs-lookup"><span data-stu-id="56314-132">Cycle instance prorate</span></span> | <span data-ttu-id="56314-133">Encargos procitados avaliados pelo cliente quando as licenças associadas são alteradas.</span><span class="sxs-lookup"><span data-stu-id="56314-133">Prorated charges assessed from the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="56314-134">Taxas de prorate quando cancela</span><span class="sxs-lookup"><span data-stu-id="56314-134">Prorate fees when cancel</span></span> | <span data-ttu-id="56314-135">Reembolso prostimado para parte não utilizada do serviço após cancelamento.</span><span class="sxs-lookup"><span data-stu-id="56314-135">Prorated refund for unused portion of service upon cancellation.</span></span> |
| <span data-ttu-id="56314-136">Taxas de prorate quando convertidas fora da oferta atual</span><span class="sxs-lookup"><span data-stu-id="56314-136">Prorate fees when convert away from current offering</span></span> | <span data-ttu-id="56314-137">Taxas prostimadas após a conversão da subscrição mensal atual para uma subscrição anual.</span><span class="sxs-lookup"><span data-stu-id="56314-137">Prorated charges after converting away from the current monthly subscription to an annual subscription.</span></span> |
| <span data-ttu-id="56314-138">Taxas de prorate quando convertidas para uma nova oferta</span><span class="sxs-lookup"><span data-stu-id="56314-138">Prorate fees when convert to a new offering</span></span> | <span data-ttu-id="56314-139">Taxas prostimadas após converter uma subscrição mensal para uma nova subscrição anual.</span><span class="sxs-lookup"><span data-stu-id="56314-139">Prorated charges after converting a monthly subscription to a new annual subscription.</span></span> |
| <span data-ttu-id="56314-140">Taxas de prorate na compra</span><span class="sxs-lookup"><span data-stu-id="56314-140">Prorate fees when purchase</span></span> | <span data-ttu-id="56314-141">O tipo de cobrança de uma subscrição quando se utiliza faturação mensal ou anual.</span><span class="sxs-lookup"><span data-stu-id="56314-141">The charge type for a subscription when using both monthly or annual billing.</span></span> |
| <span data-ttu-id="56314-142">Taxa de prorate ao renovar</span><span class="sxs-lookup"><span data-stu-id="56314-142">Prorate fee when renew</span></span> | <span data-ttu-id="56314-143">Taxas prostimadas após a renovação da subscrição.</span><span class="sxs-lookup"><span data-stu-id="56314-143">Prorated fees upon subscription renewal.</span></span> |
| <span data-ttu-id="56314-144">Taxa de renovação</span><span class="sxs-lookup"><span data-stu-id="56314-144">Renew fee</span></span> | <span data-ttu-id="56314-145">Cobrança pela renovação de uma subscrição</span><span class="sxs-lookup"><span data-stu-id="56314-145">Charge for renewing a subscription</span></span> |
| <span data-ttu-id="56314-146">Taxas de prorate quando ativadas</span><span class="sxs-lookup"><span data-stu-id="56314-146">Prorate fees when activate</span></span> | <span data-ttu-id="56314-147">Taxas prostimadas desde a ativação até ao final do período de faturação.</span><span class="sxs-lookup"><span data-stu-id="56314-147">Prorated fees from activation until end of billing period.</span></span> |

## <a name="one-time-charges"></a><span data-ttu-id="56314-148">Encargos únicos</span><span class="sxs-lookup"><span data-stu-id="56314-148">One-time charges</span></span>

<span data-ttu-id="56314-149">Para mapear estes encargos únicos para a sua fatura, em suma a coluna **Valor** a partir do ficheiro baseado na licença.</span><span class="sxs-lookup"><span data-stu-id="56314-149">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="56314-150">Descrição da carga (coluna ChargeType no ficheiro de reconciliação)</span><span class="sxs-lookup"><span data-stu-id="56314-150">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="56314-151">Explicação de cobrança</span><span class="sxs-lookup"><span data-stu-id="56314-151">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="56314-152">Novo</span><span class="sxs-lookup"><span data-stu-id="56314-152">New</span></span> | <span data-ttu-id="56314-153">Usado quando uma nova compra é criada.</span><span class="sxs-lookup"><span data-stu-id="56314-153">Used when a new purchase is created.</span></span> |
| <span data-ttu-id="56314-154">adicionarQuantity</span><span class="sxs-lookup"><span data-stu-id="56314-154">addQuantity</span></span> | <span data-ttu-id="56314-155">Utilizado tanto no reembolso da compra original como na nova quantidade após um aumento.</span><span class="sxs-lookup"><span data-stu-id="56314-155">Used in both the refund of the original purchase and the new quantity after an increase.</span></span> |
| <span data-ttu-id="56314-156">removerQuantidade</span><span class="sxs-lookup"><span data-stu-id="56314-156">removeQuantity</span></span> | <span data-ttu-id="56314-157">Utilizado tanto no reembolso da compra original como na nova quantidade após uma diminuição.</span><span class="sxs-lookup"><span data-stu-id="56314-157">Used in both the refund of the original purchase and the new quantity after a decrease.</span></span> |
| <span data-ttu-id="56314-158">Cancelar</span><span class="sxs-lookup"><span data-stu-id="56314-158">Cancel</span></span> | <span data-ttu-id="56314-159">Usado quando uma subscrição é cancelada.</span><span class="sxs-lookup"><span data-stu-id="56314-159">Used when a subscription is canceled.</span></span> |
| <span data-ttu-id="56314-160">Converter</span><span class="sxs-lookup"><span data-stu-id="56314-160">Convert</span></span> | <span data-ttu-id="56314-161">Usado quando uma licença é atualizada, mas o número de licenças permanece inalterado.</span><span class="sxs-lookup"><span data-stu-id="56314-161">Used when a license is upgraded but the number of licenses remains unchanged.</span></span> |

## <a name="usage-charges"></a><span data-ttu-id="56314-162">Custos de utilização</span><span class="sxs-lookup"><span data-stu-id="56314-162">Usage charges</span></span>

<span data-ttu-id="56314-163">Para mapear estes custos de utilização na sua fatura, em suma a coluna **PretaxCharges** a partir do ficheiro baseado em utilização.</span><span class="sxs-lookup"><span data-stu-id="56314-163">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="56314-164">Descrição da carga (coluna ChargeType no ficheiro de reconciliação)</span><span class="sxs-lookup"><span data-stu-id="56314-164">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="56314-165">Explicação de cobrança</span><span class="sxs-lookup"><span data-stu-id="56314-165">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="56314-166">Avaliar a taxa de utilização ao cancelar</span><span class="sxs-lookup"><span data-stu-id="56314-166">Assess usage fee when cancel</span></span> | <span data-ttu-id="56314-167">Taxa de utilização de acesso após cancelamento de uso não pago durante o período de faturação atual.</span><span class="sxs-lookup"><span data-stu-id="56314-167">Access usage fee upon cancellation for unpaid usage during the current billing period.</span></span> |
| <span data-ttu-id="56314-168">Avaliar a taxa de utilização do ciclo atual</span><span class="sxs-lookup"><span data-stu-id="56314-168">Assess usage fee for current cycle</span></span> | <span data-ttu-id="56314-169">Taxa de utilização de acesso para o período de faturação atual.</span><span class="sxs-lookup"><span data-stu-id="56314-169">Access usage fee for the current billing period.</span></span> |

### <a name="credits"></a><span data-ttu-id="56314-170">Créditos</span><span class="sxs-lookup"><span data-stu-id="56314-170">Credits</span></span>

<span data-ttu-id="56314-171">Para mapear estes créditos na sua fatura:</span><span class="sxs-lookup"><span data-stu-id="56314-171">To map these credits to your invoice:</span></span>

- <span data-ttu-id="56314-172">Em suma, o **TotalForCustomer** do ficheiro baseado na licença.</span><span class="sxs-lookup"><span data-stu-id="56314-172">Sum the **TotalForCustomer** from the license-based file.</span></span>
- <span data-ttu-id="56314-173">Em suma, a coluna **PostTaxTotal** a partir do ficheiro baseado na utilização.</span><span class="sxs-lookup"><span data-stu-id="56314-173">Sum the **PostTaxTotal** column from the usage-based file.</span></span>

| <span data-ttu-id="56314-174">Descrição da carga (coluna ChargeType no ficheiro de reconciliação)</span><span class="sxs-lookup"><span data-stu-id="56314-174">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="56314-175">Explicação de cobrança</span><span class="sxs-lookup"><span data-stu-id="56314-175">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="56314-176">Compensar um item de linha</span><span class="sxs-lookup"><span data-stu-id="56314-176">Offset a line item</span></span> | <span data-ttu-id="56314-177">Reembolso parcial ou total a um item de linha, incluindo impostos.</span><span class="sxs-lookup"><span data-stu-id="56314-177">Partial or whole refund to a line item, including taxes.</span></span> |

### <a name="usage-based-discounts"></a><span data-ttu-id="56314-178">Descontos baseados na utilização</span><span class="sxs-lookup"><span data-stu-id="56314-178">Usage-based discounts</span></span>

<span data-ttu-id="56314-179">Para mapear estes descontos baseados na sua fatura, em suma a coluna **PretaxCharges** a partir do ficheiro baseado em utilização.</span><span class="sxs-lookup"><span data-stu-id="56314-179">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="56314-180">Descrição da carga (coluna ChargeType no ficheiro de reconciliação)</span><span class="sxs-lookup"><span data-stu-id="56314-180">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="56314-181">Explicação de cobrança</span><span class="sxs-lookup"><span data-stu-id="56314-181">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="56314-182">Desconto de ativação</span><span class="sxs-lookup"><span data-stu-id="56314-182">Activation discount</span></span> | <span data-ttu-id="56314-183">Desconto aplicado quando a subscrição é ativada.</span><span class="sxs-lookup"><span data-stu-id="56314-183">Discount applied when subscription activated.</span></span> |
| <span data-ttu-id="56314-184">Desconto de ciclo</span><span class="sxs-lookup"><span data-stu-id="56314-184">Cycle discount</span></span> | <span data-ttu-id="56314-185">Desconto aplicado em encargos periódicos.</span><span class="sxs-lookup"><span data-stu-id="56314-185">Discount applied on periodic charges.</span></span> |
| <span data-ttu-id="56314-186">Renovar desconto</span><span class="sxs-lookup"><span data-stu-id="56314-186">Renew discount</span></span> | <span data-ttu-id="56314-187">Desconto aplicado quando a subscrição renovada.</span><span class="sxs-lookup"><span data-stu-id="56314-187">Discount applied when subscription renewed.</span></span> |
| <span data-ttu-id="56314-188">Cancelar desconto</span><span class="sxs-lookup"><span data-stu-id="56314-188">Cancel discount</span></span> | <span data-ttu-id="56314-189">Encargos aplicados quando os descontos são cancelados.</span><span class="sxs-lookup"><span data-stu-id="56314-189">Charges applied when discounts are canceled.</span></span> |

### <a name="license-based-discounts"></a><span data-ttu-id="56314-190">Descontos baseados em licenças</span><span class="sxs-lookup"><span data-stu-id="56314-190">License-based discounts</span></span>

<span data-ttu-id="56314-191">Para mapear descontos baseados em licenças na sua fatura, em suma a coluna **TotalOtherDiscount** a partir do ficheiro baseado na licença.</span><span class="sxs-lookup"><span data-stu-id="56314-191">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span></span>

<span data-ttu-id="56314-192">*Os descontos baseados na licença podem ser aplicados a vários tipos de carga.*</span><span class="sxs-lookup"><span data-stu-id="56314-192">*License-based discounts may be applied to multiple charge types.*</span></span>
