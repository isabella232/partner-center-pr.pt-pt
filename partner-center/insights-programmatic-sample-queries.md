---
title: Lista de consultas de amostra
description: Utilize as consultas de amostra para aceder programaticamente aos dados de análise de insights de parceiros.
ms.topic: reference
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: 36da8a59548142bf09daf42dbc936fba15d46d1e
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/29/2021
ms.locfileid: "114844688"
---
# <a name="sample-queries-for-partner-center-insights-report"></a>Consultas de amostra para relatório de insights do Partner Center

Este artigo fornece consultas de amostra para os relatórios Informações do Parceiro. Pode utilizar estas consultas ligando para o ponto final da API de consulta de relatório create. Se necessário, a chamada [de API de Consulta de Relatório de Criação](insights-programmatic-access-paradigm.md#create-report-query-api) pode ser modificada para adicionar mais colunas, ajustar o período de cálculo e adicionar condições de filtro.

Para obter mais informações sobre os nomes, atributos e descrições das colunas, consulte as [Definições de Dados](insights-data-definitions.md).

## <a name="customer-details"></a>Detalhes do cliente

Estas consultas de amostra aplicam-se aos dados dos clientes:

### <a name="by-geography"></a>Por geografia

Lista de clientes de uma geografia específica no mês passado.

```sql
SELECT CustomerName, CustomerTpid, Product 
FROM CustomersAndTenants 
WHERE CustomerMarket='United States' TIMESPAN LAST_MONTH
```

### <a name="by-sku-and-billed-revenue"></a>Por SKU e receitas faturadas

Lista de clientes que usam receitas específicas da SKU e billed é superior a 20.000 nos últimos 6 meses

```sql
SELECT CustomerName, CustomerTpid, SKU, Month, BilledRevenueUSD 
FROM CustomersAndTenants 
WHERE SKU='MICROSOFT 365 BUSINESS STANDARD' AND BilledRevenueUSD>20000 TIMESPAN LAST_6_MONTHS
```

### <a name="by-available-seats"></a>Por lugares disponíveis

Top 10 clientes com base em lugares disponíveis no mês passado

```sql
SELECT CustomerName, CustomerTpid, Product, AvailableSeats 
FROM CustomersAndTenants ORDER BY AvailableSeats DESC LIMIT 10 TIMESPAN LAST_MONTH
```

## <a name="partner-profile"></a>Perfil do parceiro

Estas consultas de amostra aplicam-se ao relatório do perfil do parceiro:

### <a name="by-geography"></a>Por geografia

Lista de parceiros de uma geografia específica.

```sql
SELECT MPNId, PartnerName 
FROM Profile 
WHERE Country='United States'
```

### <a name="by-mpn-partner"></a>Por parceiro MPN

Lista de sócios com o mesmo Parceiro MPN da PGA

```sql
SELECT MPNId, PartnerName, PGAMpnId 
FROM Profile 
WHERE PGAMpnId='1001xx'
```

## <a name="reseller-performance"></a>Desempenho do Revendedor

Estas consultas de amostra aplicam-se ao relatório de desempenho do revendedor:

### <a name="by-geography"></a>Por geografia

Lista de revendedores de uma geografia específica no mês passado.

```sql
SELECT ResellerMpnId, ResellerName 
FROM ResellerPerformance 
WHERE ResellerMarket='US' TIMESPAN LAST_MONTH
```

### <a name="by-reseller"></a>Por revendedor

Contagem de clientes, contagem de assinaturas, total de lugares disponíveis, total de lugares atribuídos, receita total para um revendedor específico.

```sql
SELECT ResellerMpnId, ResellerName, CustomerCount, SubscriptionCount, TotalAvailableSeats, TotalAssignedSeats, TotalRevenue 
FROM ResellerPerformance 
WHERE ResellerMpnId='1051xxx'
```

### <a name="top-10-by-revenue"></a>Top 10 por receitas

Top 10 revendedores com base no total das receitas no mês passado.

```sql
SELECT ResellerMpnId, ResellerName, TotalRevenue 
FROM ResellerPerformance 
ORDER BY TotalRevenue 
LIMIT 10 
TIMESPAN LAST_MONTH
```

## <a name="subscription-details"></a>Detalhes da subscrição

Estas consultas de amostra aplicam-se ao relatório de detalhes da subscrição:

### <a name="by-renewal-eligibility"></a>Por elegibilidade de renovação

Lista de assinaturas que não são elegíveis para renovação automática no mês passado.

```sql
SELECT SubscriptionId, SubscriptionEndDate, CustomerName, CustomerTpid, Product 
FROM SeatsSubscriptionsAndRevenue 
WHERE IsAutoRenew='N' TIMESPAN LAST_MONTH
```

### <a name="by-subscription-state"></a>Por estado de subscrição

Lista de subscrições que estão em Estado de Desativação no mês passado.

```sql
SELECT SubscriptionId, SubscriptionEndDate, CustomerName, CustomerTpid, Product 
FROM SeatsSubscriptionsAndRevenue 
WHERE SubscriptionState='Disabled' TIMESPAN LAST_MONTH
```

### <a name="counts-for-six-months"></a>Conta por seis meses

Contagem de assinaturas, total de lugares vendidos, contagem de clientes para um parceiro específico nos últimos seis meses.

```sql
SELECT MPNId, SubscriptionCount, TotalSoldSeats, BilledRevenueUSD, CustomerCount 
FROM SeatsSubscriptionsAndRevenue 
WHERE MPNId=6096xxx TIMESPAN LAST_6_MONTHS
```

## <a name="azure-usage"></a>Utilização Azure

Estas consultas de amostras aplicam-se ao relatório de utilização do Azure:

### <a name="by-meter-category"></a>Por categoria de medidor

Lista de subscrições de utilização Azure com unidades de utilização e ACR para a categoria de contador específico nos últimos seis meses.

```sql
SELECT SubscriptionId, CustomerName, Month, UsageUnits, UsageQuantity, TotalACR 
FROM AzureUsage 
WHERE MeterCategory='Azure DNS' 
TIMESPAN LAST_6_MONTHS
```

### <a name="by-total-acr"></a>Pelo total de ACR

Lista de subscrições de utilização da Azure onde o total de ACR é superior a 20.000 nos últimos seis meses

```sql
SELECT SubscriptionId, ServiceName, CustomerName, Month, UsageUnits, UsageQuantity, TotalACR 
FROM AzureUsage 
WHERE TotalACR>20000 TIMESPAN LAST_6_MONTHS
```

## <a name="next-steps"></a>Passos seguintes

- [APIs para aceder a dados de análise de insights de parceiros](insights-programmatic-analytics-available-api.md)