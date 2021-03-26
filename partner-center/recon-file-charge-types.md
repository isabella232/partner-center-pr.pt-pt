---
title: Tipos de encargos de ficheiro de reconciliação
ms.topic: article
ms.date: 06/05/2020
description: Descubra os tipos de encargos (tais como, baseados em licenças, baseados em uso e uma vez), créditos e descontos em ficheiros de reconciliação do Partner Center.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: ba42ac5beb28a3cf819c54a86385fb79853cdcd0
ms.sourcegitcommit: 700150044ea4f1a0b96cb4caeb97d7197da29ef6
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/25/2021
ms.locfileid: "105549231"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a><span data-ttu-id="9b292-103">Compreenda os diferentes tipos de carga nos ficheiros de reconciliação do Partner Center</span><span class="sxs-lookup"><span data-stu-id="9b292-103">Understand the different charge types in Partner Center reconciliation files</span></span>

<span data-ttu-id="9b292-104">**Aplica-se a**</span><span class="sxs-lookup"><span data-stu-id="9b292-104">**Applies to**</span></span>

- <span data-ttu-id="9b292-105">Centro de Parceiros para a nuvem do Governo da Microsoft</span><span class="sxs-lookup"><span data-stu-id="9b292-105">Partner Center for Microsoft Government cloud</span></span>

<span data-ttu-id="9b292-106">**Funções adequadas**</span><span class="sxs-lookup"><span data-stu-id="9b292-106">**Appropriate roles**</span></span>

- <span data-ttu-id="9b292-107">Agente administrativo</span><span class="sxs-lookup"><span data-stu-id="9b292-107">Admin agent</span></span>
- <span data-ttu-id="9b292-108">Administrador de faturação</span><span class="sxs-lookup"><span data-stu-id="9b292-108">Billing admin</span></span>
- <span data-ttu-id="9b292-109">Administrador global</span><span class="sxs-lookup"><span data-stu-id="9b292-109">Global admin</span></span>

<span data-ttu-id="9b292-110">Este artigo descreve os mapeamentos entre uma secção de fatura e tipos de carga associados que podem estar no seu ficheiro de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="9b292-110">This article describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span></span> <span data-ttu-id="9b292-111">A sua fatura fornece um resumo das taxas.</span><span class="sxs-lookup"><span data-stu-id="9b292-111">Your invoice provides a summary of charges.</span></span> <span data-ttu-id="9b292-112">O seu ficheiro de reconciliação fornece uma desagregação detalhada das transações de item de linha, incluindo tipos de carga.</span><span class="sxs-lookup"><span data-stu-id="9b292-112">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span> <span data-ttu-id="9b292-113">Para obter mais informações sobre ficheiros de reconciliação, [consulte como utilizar ficheiros de reconciliação](use-the-reconciliation-files.md).</span><span class="sxs-lookup"><span data-stu-id="9b292-113">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span></span>

<span data-ttu-id="9b292-114">Tanto os [ficheiros de reconciliação baseados na utilização](usage-based-recon-files.md) como [os ficheiros de reconciliação baseados em licenças](license-based-recon-files.md) apenas mostram transações e encargos relacionados com o uso (unidades consumidas e encargos relacionados).</span><span class="sxs-lookup"><span data-stu-id="9b292-114">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span></span>

> [!NOTE]
> <span data-ttu-id="9b292-115">Créditos pontuais, descontos ou reembolsos que apareçam na fatura, uma vez que os **ajustes** não constam do ficheiro de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="9b292-115">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span></span>

## <a name="map-charge-types-to-invoice-charges"></a><span data-ttu-id="9b292-116">Tipos de carga de mapa para cobrar faturas</span><span class="sxs-lookup"><span data-stu-id="9b292-116">Map charge types to invoice charges</span></span>

<span data-ttu-id="9b292-117">Para cruzar os valores de carga entre a sua fatura e o ficheiro de reconciliação, utilize as opções de filtro no Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="9b292-117">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span></span> <span data-ttu-id="9b292-118">Filtrar por tipos de carga no seu ficheiro de reconciliação para mapear os encargos da fatura para um conjunto de avarias de carga no ficheiro de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="9b292-118">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span></span>

## <a name="license-based-charges"></a><span data-ttu-id="9b292-119">Encargos baseados em licença</span><span class="sxs-lookup"><span data-stu-id="9b292-119">License-based charges</span></span>

<span data-ttu-id="9b292-120">Para mapear estes encargos baseados na licença para a sua fatura, em suma a coluna **Valor** a partir do ficheiro baseado em licença.</span><span class="sxs-lookup"><span data-stu-id="9b292-120">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="9b292-121">Descrição da carga (coluna ChargeType no ficheiro de reconciliação)</span><span class="sxs-lookup"><span data-stu-id="9b292-121">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="9b292-122">Explicação de cobrança</span><span class="sxs-lookup"><span data-stu-id="9b292-122">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="9b292-123">Taxa de ativação</span><span class="sxs-lookup"><span data-stu-id="9b292-123">Activation fee</span></span> | <span data-ttu-id="9b292-124">O valor cobrado ao cliente quando utiliza a subscrição após a compra.</span><span class="sxs-lookup"><span data-stu-id="9b292-124">The amount charged to the customer when they use the subscription after purchase.</span></span> |
| <span data-ttu-id="9b292-125">Taxa de cancelamento</span><span class="sxs-lookup"><span data-stu-id="9b292-125">Cancel fee</span></span> | <span data-ttu-id="9b292-126">Encargos procitados reembolsados ao cliente quando as licenças associadas são alteradas.</span><span class="sxs-lookup"><span data-stu-id="9b292-126">Prorated charges refunded to the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="9b292-127">Cancelar caso prorate</span><span class="sxs-lookup"><span data-stu-id="9b292-127">Cancel instance prorate</span></span> | <span data-ttu-id="9b292-128">Os encargos procitados cancelados quando o cliente com subscrição mensal tem subscrição suspensa e as licenças associadas alteradas no mesmo mês.</span><span class="sxs-lookup"><span data-stu-id="9b292-128">Prorated charges canceled when customer with monthly subscription has subscription suspended and associated licenses changed within the same month.</span></span> |
| <span data-ttu-id="9b292-129">Taxa de ciclo</span><span class="sxs-lookup"><span data-stu-id="9b292-129">Cycle fee</span></span> | <span data-ttu-id="9b292-130">Encargos periódicos para uma subscrição.</span><span class="sxs-lookup"><span data-stu-id="9b292-130">Periodic charges for a subscription.</span></span> |
| <span data-ttu-id="9b292-131">Prorate de instância de ciclo</span><span class="sxs-lookup"><span data-stu-id="9b292-131">Cycle instance prorate</span></span> | <span data-ttu-id="9b292-132">Encargos procitados avaliados pelo cliente quando as licenças associadas são alteradas.</span><span class="sxs-lookup"><span data-stu-id="9b292-132">Prorated charges assessed from the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="9b292-133">Taxas de prorate quando cancela</span><span class="sxs-lookup"><span data-stu-id="9b292-133">Prorate fees when cancel</span></span> | <span data-ttu-id="9b292-134">Reembolso prostimado para parte não utilizada do serviço após cancelamento.</span><span class="sxs-lookup"><span data-stu-id="9b292-134">Prorated refund for unused portion of service upon cancellation.</span></span> |
| <span data-ttu-id="9b292-135">Taxas de prorate quando convertidas fora da oferta atual</span><span class="sxs-lookup"><span data-stu-id="9b292-135">Prorate fees when convert away from current offering</span></span> | <span data-ttu-id="9b292-136">Taxas prostimadas após a conversão da subscrição mensal atual para uma subscrição anual.</span><span class="sxs-lookup"><span data-stu-id="9b292-136">Prorated charges after converting away from the current monthly subscription to an annual subscription.</span></span> |
| <span data-ttu-id="9b292-137">Taxas de prorate quando convertidas para uma nova oferta</span><span class="sxs-lookup"><span data-stu-id="9b292-137">Prorate fees when convert to a new offering</span></span> | <span data-ttu-id="9b292-138">Taxas prostimadas após converter uma subscrição mensal para uma nova subscrição anual.</span><span class="sxs-lookup"><span data-stu-id="9b292-138">Prorated charges after converting a monthly subscription to a new annual subscription.</span></span> |
| <span data-ttu-id="9b292-139">Taxas de prorate na compra</span><span class="sxs-lookup"><span data-stu-id="9b292-139">Prorate fees when purchase</span></span> | <span data-ttu-id="9b292-140">O tipo de cobrança de uma subscrição quando se utiliza faturação mensal ou anual.</span><span class="sxs-lookup"><span data-stu-id="9b292-140">The charge type for a subscription when using both monthly or annual billing.</span></span> |
| <span data-ttu-id="9b292-141">Taxa de prorate ao renovar</span><span class="sxs-lookup"><span data-stu-id="9b292-141">Prorate fee when renew</span></span> | <span data-ttu-id="9b292-142">Taxas prostimadas após a renovação da subscrição.</span><span class="sxs-lookup"><span data-stu-id="9b292-142">Prorated fees upon subscription renewal.</span></span> |
| <span data-ttu-id="9b292-143">Taxa de renovação</span><span class="sxs-lookup"><span data-stu-id="9b292-143">Renew fee</span></span> | <span data-ttu-id="9b292-144">Cobrança pela renovação de uma subscrição</span><span class="sxs-lookup"><span data-stu-id="9b292-144">Charge for renewing a subscription</span></span> |
| <span data-ttu-id="9b292-145">Taxas de prorate quando ativadas</span><span class="sxs-lookup"><span data-stu-id="9b292-145">Prorate fees when activate</span></span> | <span data-ttu-id="9b292-146">Taxas prostimadas desde a ativação até ao final do período de faturação.</span><span class="sxs-lookup"><span data-stu-id="9b292-146">Prorated fees from activation until end of billing period.</span></span> |

## <a name="one-time-charges"></a><span data-ttu-id="9b292-147">Encargos únicos</span><span class="sxs-lookup"><span data-stu-id="9b292-147">One-time charges</span></span>

<span data-ttu-id="9b292-148">Para mapear estes encargos únicos para a sua fatura, em suma a coluna **Valor** a partir do ficheiro baseado na licença.</span><span class="sxs-lookup"><span data-stu-id="9b292-148">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="9b292-149">Descrição da carga (coluna ChargeType no ficheiro de reconciliação)</span><span class="sxs-lookup"><span data-stu-id="9b292-149">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="9b292-150">Explicação de cobrança</span><span class="sxs-lookup"><span data-stu-id="9b292-150">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="9b292-151">Novo</span><span class="sxs-lookup"><span data-stu-id="9b292-151">New</span></span> | <span data-ttu-id="9b292-152">Usado quando uma nova compra é criada.</span><span class="sxs-lookup"><span data-stu-id="9b292-152">Used when a new purchase is created.</span></span> |
| <span data-ttu-id="9b292-153">adicionarQuantity</span><span class="sxs-lookup"><span data-stu-id="9b292-153">addQuantity</span></span> | <span data-ttu-id="9b292-154">Utilizado tanto no reembolso da compra original como na nova quantidade após um aumento.</span><span class="sxs-lookup"><span data-stu-id="9b292-154">Used in both the refund of the original purchase and the new quantity after an increase.</span></span> |
| <span data-ttu-id="9b292-155">removerQuantidade</span><span class="sxs-lookup"><span data-stu-id="9b292-155">removeQuantity</span></span> | <span data-ttu-id="9b292-156">Utilizado tanto no reembolso da compra original como na nova quantidade após uma diminuição.</span><span class="sxs-lookup"><span data-stu-id="9b292-156">Used in both the refund of the original purchase and the new quantity after a decrease.</span></span> |
| <span data-ttu-id="9b292-157">Cancelar</span><span class="sxs-lookup"><span data-stu-id="9b292-157">Cancel</span></span> | <span data-ttu-id="9b292-158">Usado quando uma subscrição é cancelada.</span><span class="sxs-lookup"><span data-stu-id="9b292-158">Used when a subscription is canceled.</span></span> |
| <span data-ttu-id="9b292-159">Converter</span><span class="sxs-lookup"><span data-stu-id="9b292-159">Convert</span></span> | <span data-ttu-id="9b292-160">Usado quando uma licença é atualizada, mas o número de licenças permanece inalterado.</span><span class="sxs-lookup"><span data-stu-id="9b292-160">Used when a license is upgraded but the number of licenses remains unchanged.</span></span> |

## <a name="usage-charges"></a><span data-ttu-id="9b292-161">Custos de utilização</span><span class="sxs-lookup"><span data-stu-id="9b292-161">Usage charges</span></span>

<span data-ttu-id="9b292-162">Para mapear estes custos de utilização na sua fatura, em suma a coluna **PretaxCharges** a partir do ficheiro baseado em utilização.</span><span class="sxs-lookup"><span data-stu-id="9b292-162">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="9b292-163">Descrição da carga (coluna ChargeType no ficheiro de reconciliação)</span><span class="sxs-lookup"><span data-stu-id="9b292-163">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="9b292-164">Explicação de cobrança</span><span class="sxs-lookup"><span data-stu-id="9b292-164">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="9b292-165">Avaliar a taxa de utilização ao cancelar</span><span class="sxs-lookup"><span data-stu-id="9b292-165">Assess usage fee when cancel</span></span> | <span data-ttu-id="9b292-166">Taxa de utilização de acesso após cancelamento de uso não pago durante o período de faturação atual.</span><span class="sxs-lookup"><span data-stu-id="9b292-166">Access usage fee upon cancellation for unpaid usage during the current billing period.</span></span> |
| <span data-ttu-id="9b292-167">Avaliar a taxa de utilização do ciclo atual</span><span class="sxs-lookup"><span data-stu-id="9b292-167">Assess usage fee for current cycle</span></span> | <span data-ttu-id="9b292-168">Taxa de utilização de acesso para o período de faturação atual.</span><span class="sxs-lookup"><span data-stu-id="9b292-168">Access usage fee for the current billing period.</span></span> |

### <a name="credits"></a><span data-ttu-id="9b292-169">Créditos</span><span class="sxs-lookup"><span data-stu-id="9b292-169">Credits</span></span>

<span data-ttu-id="9b292-170">Para mapear estes créditos na sua fatura:</span><span class="sxs-lookup"><span data-stu-id="9b292-170">To map these credits to your invoice:</span></span>

- <span data-ttu-id="9b292-171">Em suma, o **TotalForCustomer** do ficheiro baseado na licença.</span><span class="sxs-lookup"><span data-stu-id="9b292-171">Sum the **TotalForCustomer** from the license-based file.</span></span>
- <span data-ttu-id="9b292-172">Em suma, a coluna **PostTaxTotal** a partir do ficheiro baseado na utilização.</span><span class="sxs-lookup"><span data-stu-id="9b292-172">Sum the **PostTaxTotal** column from the usage-based file.</span></span>

| <span data-ttu-id="9b292-173">Descrição da carga (coluna ChargeType no ficheiro de reconciliação)</span><span class="sxs-lookup"><span data-stu-id="9b292-173">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="9b292-174">Explicação de cobrança</span><span class="sxs-lookup"><span data-stu-id="9b292-174">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="9b292-175">Compensar um item de linha</span><span class="sxs-lookup"><span data-stu-id="9b292-175">Offset a line item</span></span> | <span data-ttu-id="9b292-176">Reembolso parcial ou total a um item de linha, incluindo impostos.</span><span class="sxs-lookup"><span data-stu-id="9b292-176">Partial or whole refund to a line item, including taxes.</span></span> |

### <a name="usage-based-discounts"></a><span data-ttu-id="9b292-177">Descontos baseados na utilização</span><span class="sxs-lookup"><span data-stu-id="9b292-177">Usage-based discounts</span></span>

<span data-ttu-id="9b292-178">Para mapear estes descontos baseados na sua fatura, em suma a coluna **PretaxCharges** a partir do ficheiro baseado em utilização.</span><span class="sxs-lookup"><span data-stu-id="9b292-178">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="9b292-179">Descrição da carga (coluna ChargeType no ficheiro de reconciliação)</span><span class="sxs-lookup"><span data-stu-id="9b292-179">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="9b292-180">Explicação de cobrança</span><span class="sxs-lookup"><span data-stu-id="9b292-180">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="9b292-181">Desconto de ativação</span><span class="sxs-lookup"><span data-stu-id="9b292-181">Activation discount</span></span> | <span data-ttu-id="9b292-182">Desconto aplicado quando a subscrição é ativada.</span><span class="sxs-lookup"><span data-stu-id="9b292-182">Discount applied when subscription activated.</span></span> |
| <span data-ttu-id="9b292-183">Desconto de ciclo</span><span class="sxs-lookup"><span data-stu-id="9b292-183">Cycle discount</span></span> | <span data-ttu-id="9b292-184">Desconto aplicado em encargos periódicos.</span><span class="sxs-lookup"><span data-stu-id="9b292-184">Discount applied on periodic charges.</span></span> |
| <span data-ttu-id="9b292-185">Renovar desconto</span><span class="sxs-lookup"><span data-stu-id="9b292-185">Renew discount</span></span> | <span data-ttu-id="9b292-186">Desconto aplicado quando a subscrição renovada.</span><span class="sxs-lookup"><span data-stu-id="9b292-186">Discount applied when subscription renewed.</span></span> |
| <span data-ttu-id="9b292-187">Cancelar desconto</span><span class="sxs-lookup"><span data-stu-id="9b292-187">Cancel discount</span></span> | <span data-ttu-id="9b292-188">Encargos aplicados quando os descontos são cancelados.</span><span class="sxs-lookup"><span data-stu-id="9b292-188">Charges applied when discounts are canceled.</span></span> |

### <a name="license-based-discounts"></a><span data-ttu-id="9b292-189">Descontos baseados em licenças</span><span class="sxs-lookup"><span data-stu-id="9b292-189">License-based discounts</span></span>

<span data-ttu-id="9b292-190">Para mapear descontos baseados em licenças na sua fatura, em suma a coluna **TotalOtherDiscount** a partir do ficheiro baseado na licença.</span><span class="sxs-lookup"><span data-stu-id="9b292-190">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span></span>

<span data-ttu-id="9b292-191">*Os descontos baseados na licença podem ser aplicados a vários tipos de carga.*</span><span class="sxs-lookup"><span data-stu-id="9b292-191">*License-based discounts may be applied to multiple charge types.*</span></span>
