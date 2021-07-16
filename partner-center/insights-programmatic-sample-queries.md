---
title: Lista de consultas de amostra
description: Utilize as consultas de amostra para aceder programaticamente aos dados de análise de insights de parceiros.
ms.topic: reference
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: e25784585a1ac505db99e58265939a8851edcbad
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376939"
---
# <a name="sample-queries-for-partner-center-insights-report"></a><span data-ttu-id="94798-103">Consultas de amostra para relatório de insights do Partner Center</span><span class="sxs-lookup"><span data-stu-id="94798-103">Sample queries for Partner Center insights report</span></span>

<span data-ttu-id="94798-104">Este artigo fornece consultas de amostra para os relatórios Informações do Parceiro.</span><span class="sxs-lookup"><span data-stu-id="94798-104">This article provides sample queries for the Partner Insights reports.</span></span> <span data-ttu-id="94798-105">Pode utilizar estas consultas ligando para o ponto final da API de consulta de relatório create.</span><span class="sxs-lookup"><span data-stu-id="94798-105">You can use these queries by calling the Create Report Query API endpoint.</span></span> <span data-ttu-id="94798-106">Se necessário, a chamada [de API de Consulta de Relatório de Criação](insights-programmatic-access-paradigm.md#create-report-query-api) pode ser modificada para adicionar mais colunas, ajustar o período de cálculo e adicionar condições de filtro.</span><span class="sxs-lookup"><span data-stu-id="94798-106">If necessary, the [Create Report Query API](insights-programmatic-access-paradigm.md#create-report-query-api) call can be modified to add more columns, adjust the computation period, and add filter conditions.</span></span>

<span data-ttu-id="94798-107">Para obter mais informações sobre os nomes, atributos e descrições das colunas, consulte as [Definições de Dados](insights-data-definitions.md).</span><span class="sxs-lookup"><span data-stu-id="94798-107">For details about the column names, attributes, and descriptions, refer to the [Data Definitions](insights-data-definitions.md).</span></span>

## <a name="customer-details"></a><span data-ttu-id="94798-108">Detalhes do cliente</span><span class="sxs-lookup"><span data-stu-id="94798-108">Customer details</span></span>

<span data-ttu-id="94798-109">Estas consultas de amostra aplicam-se aos dados dos clientes:</span><span class="sxs-lookup"><span data-stu-id="94798-109">These sample queries apply to the customers details report:</span></span>

### <a name="by-geography"></a><span data-ttu-id="94798-110">Por geografia</span><span class="sxs-lookup"><span data-stu-id="94798-110">By geography</span></span>

<span data-ttu-id="94798-111">Lista de clientes de uma geografia específica no mês passado.</span><span class="sxs-lookup"><span data-stu-id="94798-111">List of customers from a specific geography in last month.</span></span>

```sql
SELECT CustomerName, CustomerTpid, Product 
FROM CustomersAndTenants 
WHERE CustomerMarket='United States' TIMESPAN LAST_MONTH
```

### <a name="by-sku-and-billed-revenue"></a><span data-ttu-id="94798-112">Por SKU e receitas faturadas</span><span class="sxs-lookup"><span data-stu-id="94798-112">By SKU and billed revenue</span></span>

<span data-ttu-id="94798-113">Lista de clientes que usam receitas específicas da SKU e billed é superior a 20.000 nos últimos 6 meses</span><span class="sxs-lookup"><span data-stu-id="94798-113">List of customers using specific SKU and Billed Revenue is more than 20,000 in the last 6 months</span></span>

```sql
SELECT CustomerName, CustomerTpid, SKU, Month, BilledRevenueUSD 
FROM CustomersAndTenants 
WHERE SKU='MICROSOFT 365 BUSINESS STANDARD' AND BilledRevenueUSD>20000 TIMESPAN LAST_6_MONTHS
```

### <a name="by-available-seats"></a><span data-ttu-id="94798-114">Por lugares disponíveis</span><span class="sxs-lookup"><span data-stu-id="94798-114">By available seats</span></span>

<span data-ttu-id="94798-115">Top 10 clientes com base em lugares disponíveis no mês passado</span><span class="sxs-lookup"><span data-stu-id="94798-115">Top 10 customers based on Available seats in last month</span></span>

```sql
SELECT CustomerName, CustomerTpid, Product, AvailableSeats 
FROM CustomersAndTenants ORDER BY AvailableSeats DESC LIMIT 10 TIMESPAN LAST_MONTH
```

## <a name="partner-profile"></a><span data-ttu-id="94798-116">Perfil do parceiro</span><span class="sxs-lookup"><span data-stu-id="94798-116">Partner Profile</span></span>

<span data-ttu-id="94798-117">Estas consultas de amostra aplicam-se ao relatório do perfil do parceiro:</span><span class="sxs-lookup"><span data-stu-id="94798-117">These sample queries apply to the partner profile report:</span></span>

### <a name="by-geography"></a><span data-ttu-id="94798-118">Por geografia</span><span class="sxs-lookup"><span data-stu-id="94798-118">By geography</span></span>

<span data-ttu-id="94798-119">Lista de parceiros de uma geografia específica.</span><span class="sxs-lookup"><span data-stu-id="94798-119">List of partners from a specific geography.</span></span>

```sql
SELECT MPNId, PartnerName 
FROM Profile 
WHERE Country='United States'
```

### <a name="by-mpn-partner"></a><span data-ttu-id="94798-120">Por parceiro MPN</span><span class="sxs-lookup"><span data-stu-id="94798-120">By MPN partner</span></span>

<span data-ttu-id="94798-121">Lista de sócios com o mesmo Parceiro MPN da PGA</span><span class="sxs-lookup"><span data-stu-id="94798-121">List of partners under same PGA MPN Partner</span></span>

```sql
SELECT MPNId, PartnerName, PGAMpnId 
FROM Profile 
WHERE PGAMpnId='1001xx'
```

## <a name="reseller-performance"></a><span data-ttu-id="94798-122">Desempenho do Revendedor</span><span class="sxs-lookup"><span data-stu-id="94798-122">Reseller Performance</span></span>

<span data-ttu-id="94798-123">Estas consultas de amostra aplicam-se ao relatório de desempenho do revendedor:</span><span class="sxs-lookup"><span data-stu-id="94798-123">These sample queries apply to the reseller performance report:</span></span>

### <a name="by-geography"></a><span data-ttu-id="94798-124">Por geografia</span><span class="sxs-lookup"><span data-stu-id="94798-124">By geography</span></span>

<span data-ttu-id="94798-125">Lista de revendedores de uma geografia específica no mês passado.</span><span class="sxs-lookup"><span data-stu-id="94798-125">List of resellers from a specific geography in last month.</span></span>

```sql
SELECT ResellerMpnId, ResellerName 
FROM ResellerPerformance 
WHERE ResellerMarket='US' TIMESPAN LAST_MONTH
```

### <a name="by-reseller"></a><span data-ttu-id="94798-126">Por revendedor</span><span class="sxs-lookup"><span data-stu-id="94798-126">By reseller</span></span>

<span data-ttu-id="94798-127">Contagem de clientes, contagem de assinaturas, total de lugares disponíveis, total de lugares atribuídos, receita total para um revendedor específico.</span><span class="sxs-lookup"><span data-stu-id="94798-127">Customer count, subscription count, total available seats, total assigned seats, total revenue for a specific reseller.</span></span>

```sql
SELECT ResellerMpnId, ResellerName, CustomerCount, SubscriptionCount, TotalAvailableSeats, TotalAssignedSeats, TotalRevenue 
FROM ResellerPerformance 
WHERE ResellerMpnId='1051xxx'
```

### <a name="top-10-by-revenue"></a><span data-ttu-id="94798-128">Top 10 por receitas</span><span class="sxs-lookup"><span data-stu-id="94798-128">Top 10 by revenue</span></span>

<span data-ttu-id="94798-129">Top 10 revendedores com base no total das receitas no mês passado.</span><span class="sxs-lookup"><span data-stu-id="94798-129">Top 10 resellers based on total revenue in last month.</span></span>

```sql
SELECT ResellerMpnId, ResellerName, TotalRevenue 
FROM ResellerPerformance 
ORDER BY TotalRevenue 
LIMIT 10 
TIMESPAN LAST_MONTH
```

## <a name="subscription-details"></a><span data-ttu-id="94798-130">Detalhes da subscrição</span><span class="sxs-lookup"><span data-stu-id="94798-130">Subscription Details</span></span>

<span data-ttu-id="94798-131">Estas consultas de amostra aplicam-se ao relatório de detalhes da subscrição:</span><span class="sxs-lookup"><span data-stu-id="94798-131">These sample queries apply to the subscription details report:</span></span>

### <a name="by-renewal-eligibility"></a><span data-ttu-id="94798-132">Por elegibilidade de renovação</span><span class="sxs-lookup"><span data-stu-id="94798-132">By renewal eligibility</span></span>

<span data-ttu-id="94798-133">Lista de assinaturas que não são elegíveis para renovação automática no mês passado.</span><span class="sxs-lookup"><span data-stu-id="94798-133">List of subscriptions who are not eligible for auto renewal in last month.</span></span>

```sql
SELECT SubscriptionId, SubscriptionEndDate, CustomerName, CustomerTpid, Product 
FROM SeatsSubscriptionsAndRevenue 
WHERE IsAutoRenew='N' TIMESPAN LAST_MONTH
```

### <a name="by-subscription-state"></a><span data-ttu-id="94798-134">Por estado de subscrição</span><span class="sxs-lookup"><span data-stu-id="94798-134">By subscription state</span></span>

<span data-ttu-id="94798-135">Lista de subscrições que estão em Estado de Desativação no mês passado.</span><span class="sxs-lookup"><span data-stu-id="94798-135">List of subscriptions who are in Disable state in last month.</span></span>

```sql
SELECT SubscriptionId, SubscriptionEndDate, CustomerName, CustomerTpid, Product 
FROM SeatsSubscriptionsAndRevenue 
WHERE SubscriptionState='Disabled' TIMESPAN LAST_MONTH
```

### <a name="counts-for-six-months"></a><span data-ttu-id="94798-136">Conta por seis meses</span><span class="sxs-lookup"><span data-stu-id="94798-136">Counts for six months</span></span>

<span data-ttu-id="94798-137">Contagem de assinaturas, total de lugares vendidos, contagem de clientes para um parceiro específico nos últimos seis meses.</span><span class="sxs-lookup"><span data-stu-id="94798-137">Subscription count, total sold seats, customer count for a specific partner in last six months.</span></span>

```sql
SELECT MPNId, SubscriptionCount, TotalSoldSeats, BilledRevenueUSD, CustomerCount 
FROM SeatsSubscriptionsAndRevenue 
WHERE MPNId=6096xxx TIMESPAN LAST_6_MONTHS
```

## <a name="azure-usage"></a><span data-ttu-id="94798-138">Utilização Azure</span><span class="sxs-lookup"><span data-stu-id="94798-138">Azure Usage</span></span>

<span data-ttu-id="94798-139">Estas consultas de amostras aplicam-se ao relatório de utilização do Azure:</span><span class="sxs-lookup"><span data-stu-id="94798-139">These sample queries apply to the Azure usage report:</span></span>

### <a name="by-meter-category"></a><span data-ttu-id="94798-140">Por categoria de medidor</span><span class="sxs-lookup"><span data-stu-id="94798-140">By meter category</span></span>

<span data-ttu-id="94798-141">Lista de subscrições de utilização Azure com unidades de utilização e ACR para a categoria de contador específico nos últimos seis meses.</span><span class="sxs-lookup"><span data-stu-id="94798-141">List of Azure usage subscriptions with usage units and ACR for specific meter category in last six months.</span></span>

```sql
SELECT SubscriptionId, CustomerName, Month, UsageUnits, UsageQuantity, TotalACR 
FROM AzureUsage 
WHERE MeterCategory='Azure DNS' 
TIMESPAN LAST_6_MONTHS
```

### <a name="by-total-acr"></a><span data-ttu-id="94798-142">Pelo total de ACR</span><span class="sxs-lookup"><span data-stu-id="94798-142">By total ACR</span></span>

<span data-ttu-id="94798-143">Lista de subscrições de utilização da Azure onde o total de ACR é superior a 20.000 nos últimos seis meses</span><span class="sxs-lookup"><span data-stu-id="94798-143">List of Azure usage subscriptions where total ACR is greater than 20,000 in last six months</span></span>

```sql
SELECT SubscriptionId, ServiceName, CustomerName, Month, UsageUnits, UsageQuantity, TotalACR 
FROM AzureUsage 
WHERE TotalACR>20000 TIMESPAN LAST_6_MONTHS
```

## <a name="next-steps"></a><span data-ttu-id="94798-144">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="94798-144">Next steps</span></span>

- [<span data-ttu-id="94798-145">APIs para aceder a dados de análise de insights de parceiros</span><span class="sxs-lookup"><span data-stu-id="94798-145">APIs for accessing partner insights analytics data</span></span>](insights-programmatic-analytics-available-api.md)