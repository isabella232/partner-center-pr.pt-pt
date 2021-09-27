---
title: Faça a sua primeira chamada de API para aceder a dados de análise de insights de parceiros
description: Exemplos para aprender a usar a API para aceder a dados de análise de insights de parceiros.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: 622cb3eb44b5d89b8721c223aac44635a1782ac7
ms.sourcegitcommit: d731813da1d31519dc2dc583d17899e5cf4ec1b2
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/27/2021
ms.locfileid: "129071862"
---
# <a name="make-your-first-api-call-to-access-partner-insights-analytics-data"></a>Faça a sua primeira chamada de API para aceder a dados de análise de insights de parceiros

Para obter uma lista das APIs para aceder a dados de análise de insights de parceiros, consulte [APIs para aceder a dados de análise de insights de parceiros](insights-programmatic-analytics-available-api.md). Antes de fazer a sua primeira chamada API, certifique-se de que cumpriu os [requisitos prévios](insights-programmatic-prerequisites.md) para aceder programáticamente ao Parceiro Informações dados de análise.

## <a name="token-generation"></a>Geração Token

Antes de ligar para qualquer um dos métodos, você deve primeiro obter um token de acesso Azure Ative Directory (AAD). Você precisa passar o token de acesso Azure para o cabeçalho de autorização de cada método na API. Depois de obter um token de acesso, tem 60 minutos para usá-lo antes de expirar. Após o fim do token, pode refrescar o token e pode continuar a usá-lo para mais chamadas para a API.

Consulte um pedido de amostra abaixo para gerar um token. Os três valores que são necessários para gerar o símbolo `clientId` `clientSecret` são, e `tenantId` . O parâmetro de recurso deve ser definido para `https://api.partnercenter.microsoft.com`

#### <a name="request-example"></a>Exemplo de pedido

```console
curl --location --request POST 'https://login.microsoftonline.com/<tenantId>/oauth2/token' \
--header 'return-client-request-id: true' \
--header 'Content-Type: application/x-www-form-urlencoded' \
--header 'Cookie: fpc=Ar2GMei7JwdKg4Y4onHrMpvxqd4FAQAAAEhU_tcOAAAA; stsservicecookie=estsfd; x-ms-gateway-slice=estsfd' \
--data-urlencode 'resource= https://api.partnercenter.microsoft.com' \
--data-urlencode 'client_id= ' \
--data-urlencode 'client_secret= ' \
--data-urlencode 'grant_type=password' \
--data-urlencode 'scope=openid' \
--data-urlencode 'username= ' \
--data-urlencode 'password= '
```

#### <a name="response-example"></a>Exemplo de resposta

```json
{
    "token_type": "Bearer",
    "expires_in": "3599",
    "ext_expires_in": "3599",
    "expires_on": "1612794445",
    "not_before": "1612790545",
    "resource": "https://api.partnercenter.microsoft.com",
    "access_token": {Token}
}
```

Para obter mais informações sobre como obter um token AD Azure para a sua aplicação, consulte [os dados de análise do Access através dos serviços da Loja.](/windows/uwp/monetize/access-analytics-data-using-windows-store-services#step-2-obtain-an-azure-ad-access-token)

## <a name="programmatic-api-call"></a>Chamada de API programática

Depois de obter o Token AAD como descrito na secção anterior, siga estes passos para criar o seu primeiro relatório de acesso programático.

Os dados podem ser descarregados a partir dos seguintes conjuntos de dados (datasetName):

- ClientesAndTenants
- AssentosSubscriçõesAndRevenue
- AzureUsage
- MSLearn
- OfficeUsage
- Perfil
- FormaçãoCompletions
- Dinâmica
- CompetênciaSSummaryHistória
- PowerBIUsage
- EMSUsage
- CompetênciaPeformanceRequirement
- RevendedorPerformance
- CLASAgreementRenewalsPropensity
- CLASAzurePropensity
- CLASD365Propensity
- CLASM365Propensity
- TeamsUsage3PApps
- TeamsUsageWorkload
- TeamsUsageMeetingsAndCalls

Na secção seguinte, veremos exemplos de como aceder programáticamente `SubscriptionId` a partir do conjunto de dados DynamicsUsage.

### <a name="step-1-make-a-rest-call-using-the-get-datasets-api"></a>Passo 1: Faça uma chamada DECONSE usando a API de conjuntos de dados

A resposta da API fornece o nome do conjunto de dados de onde pode descarregar o relatório. Para o conjunto de dados específico, a resposta API também fornece a lista de colunas selecionáveis que podem ser usadas para o seu modelo de relatório personalizado. Também pode consultar as [Definições de Dados](insights-data-definitions.md) para obter os nomes das colunas.

#### <a name="request-example"></a>Exemplo de pedido

```cli
curl 
--location 
--request GET 'https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledDataset'\
--header 'Authorization: Bearer <AADToken>'
```

#### <a name="response-example"></a>Exemplo de resposta

```json
{
  "value": [
    {
      "datasetName": "DynamicsUsage",
      "selectableColumns": [
        "PGAMpnId",
        "SubscriptionId",
        "SubscriptionStartDate",
        "SubscriptionEndDate",
        "SubscriptionStatus",
        "Month",
        "RevSumDivisionName",
        "RevSumCategoryName",
        "SKU",
        "SKUId",
        "FreeVsPaidSKU",
        "SalesModel",
        "DetailedSalesModel",
        "CustomerName",
        "CustomerTenantId",
        "CustomerTpid",
        "CustomerSegment",
        "CustomerMarket",
        "MPNId",
        "PartnerName",
        "PartnerLocation",
        "PartnerAttachType",
        "AvailableSeats",
        "AssignedSeats",
        "ActiveSeats",
        "DeploymentOpportunity",
        "ActiveUsagePercent"
      ],
      "availableMetrics": [
        "SubscriptionCount",
        "TotalAssignedSeats",
        "TotalSoldSeats",
        "TotalActiveSeats",
        "TotalRevenueAndACR",
        "CustomerCount",
        "CustomerTenantCount"
      ],
      "availableDateRanges": [
        "LAST_MONTH",
        "LAST_3_MONTHS",
        "LAST_6_MONTHS",
        "LAST_1_YEAR",
        "LIFETIME"
      ],
      "minimumRecurrenceInterval": 24
    }
  ],
  "nextLink": null,
  "totalCount": 1,
  "message": "Dataset fetched successfully",
  "statusCode": 200,
  "dataRedacted": false
}
```

### <a name="step-2-create-the-custom-query"></a>Passo 2: Criar a Consulta Personalizada

Neste passo, usaremos SubscriçãoId do conjunto de dados DynamicsUsage para criar uma consulta personalizada para o relatório que queremos. O período de tempo padrão se não for especificado na consulta é de 6 meses.

#### <a name="request-example"></a>Exemplo de pedido

```cli
curl 
--location 
--request POST 'https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries' \ 
--header ' Authorization: Bearer <AADToken>' \ 
--header 'Content-Type: application/json' \ 
--data-raw 
{
  "Name": "SubscriptionId Dynamics ",
  "Description": "List of Subscription Id from DynamicsUsage",
  "Query": "SELECT SubscriptionId from DynamicsUsage "
            }"
```

#### <a name="response-example"></a>Exemplo de resposta

```json
{
  "value": [
    {
      "queryId": "7d19305c-56db-4edc-b776-428340e3a9c8",
      "name": "SubscriptionId Dynamics",
      "description": "List of Subscription Id from DynamicsUsage",
      "query": "SELECT SubscriptionId from DynamicsUsage",
      "type": "userDefined",
      "user": "GAUser@PITEST2.ccsctp.net",
      "createdTime": "2021-03-31T07:28:37Z"
    }
 ],
  "nextLink": null,
  "totalCount": 1,
  "message": "Query created successfully",
  "statusCode": 200,
  "dataRedacted": false
}
```

Na execução bem sucedida da consulta, `queryId` gera-se um que precisa de ser utilizado para gerar o relatório.

### <a name="step-3-execute-test-query-api"></a>Passo 3: Executar consulta de teste API

Neste passo, vamos usar a consulta de teste API para obter as 100 melhores linhas para a consulta que foi criada.

#### <a name="request-example"></a>Exemplo de pedido

```cli
curl 
--location 
--request GET 'https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries/testQueryResult?queryId=7d19305c-56db-4edc-b776-428340e3a9c8' \
--header ' Authorization: Bearer <AADToken>'
```

#### <a name="response-example"></a>Exemplo de resposta

```json
{
  "value": [
    {
      "SubscriptionId": "251DE3D4-8868-4032-B518-F142DA50522F"
    },
    {
      "SubscriptionId": "758A0647-790C-435B-BEAA-652DF47E327C"
    },
    {
      "SubscriptionId": "ACE5A84B-9794-4480-82C5-AF9462DE2589"
    },
    {
      "SubscriptionId": "C75163EE-A0CA-4822-8275-E29E2490FF1C"
    },
    {
      "SubscriptionId": "082A8A18-0834-4376-A9A4-3AA4ECD02826"
    },
    .
    .
    .
    {
      "SubscriptionId": "5E10B817-7FCB-43CE-9F32-9CB60CF14658"
    },
    {
      "SubscriptionId": "7578872A-18C1-4E6B-8F51-469555337389"
    },
    {
      "SubscriptionId": "00601E10-4C05-4BA2-B977-6578F5C81D69"
    },
    {
      "SubscriptionId": "7EBFC3A9-D502-4EA2-87E7-C42971639E8C"
    },
    {
      "SubscriptionId": "2AC30AE1-5934-48FB-A0E5-EF6985761138"
    }
  ],
  "nextLink": null,
  "totalCount": 100,
  "message": null,
  "statusCode": 200,
  "dataRedacted": false
}
```

### <a name="step-4-create-the-report"></a>Passo 4: Criar o relatório

Neste passo, usaremos o QueryId anteriormente gerado para criar o relatório.

#### <a name="request-example"></a>Exemplo de pedido

```cli
curl 
--location 
--request POST 'https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport'\
--header ' Authorization: Bearer <AADToken>' \ 
--header 'Content-Type: application/json' \ 
--data-raw 
'{
  "ReportName": "DynamicsUsage Subscription ID Report",
  "Description": "Report for getting list of Subscription Id for Dynamics Usage",
  "QueryId": "7d19305c-56db-4edc-b776-428340e3a9c8",
  "StartTime": "2021-04-01T18:41:00Z",
  "ExecuteNow": false,
  "QueryStartTime": "2021-03-31T18:41:00Z",
  "QueryEndTime": "2021-06-30T18:41:00Z",
  "RecurrenceInterval": 48,
  "RecurrenceCount": 20,
  "Format": "csv",
  "CallbackUrl": "https://<SampleCallbackUrl>",
  "CallbackMethod": "GET"
}'
```

#### <a name="response-example"></a>Exemplo de resposta

```json
{
  "value": [
    {
      "reportId": "cdc61cfe-d028-4333-a215-a1df51ccbfd4",
      "reportName": "DynamicsUsage Subscription ID Report",
      "description": "Report for getting list of Subscription Id for Dynamics Usage",
      "queryId": "7d19305c-56db-4edc-b776-428340e3a9c8",
      "query": "SELECT SubscriptionId from DynamicsUsage",
      "user": "GAUser@PITEST2.ccsctp.net",
      "createdTime": "2021-03-31T08:15:15Z",
      "modifiedTime": null,
      "executeNow": false,
      "startTime": "2021-04-01T18:41:00Z",
      "reportStatus": "Active",
      "recurrenceInterval": 48,
      "recurrenceCount": 20,
      "callbackUrl": "https://<SampleCallbackUrl>",
      "CallbackMethod": "GET",
      "format": "csv"
    }
  ],
  "nextLink": null,
  "totalCount": 1,
  "message": "Report created successfully",
  "statusCode": 200,
  "dataRedacted": false
}
```

Na execução bem sucedida, é gerado um `reportId` que precisa ser usado para agendar um download do relatório.

### <a name="step-5-execute-report-executions-api"></a>Passo 5: Executar relatório execuções execuções API

Neste passo, usaremos a API de Execuções de Relatório para obter a localização segura (URL) do relatório.

#### <a name="request-example"></a>Exemplo de pedido

```cli
Curl
--location 
--request GET 'https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/execution/ cdc61cfe-d028-4333-a215-a1df51ccbfd4?getLatestExecution=true'\
--header ' Authorization: Bearer <AADToken>' \
```

#### <a name="response-example"></a>Exemplo de resposta

```json
{
  "value": [
    {
      "executionId": "315eb63e-e2b2-41a2-ad8e-790b040fdce3",
      "reportId": "cdc61cfe-d028-4333-a215-a1df51ccbfd4",
      "recurrenceInterval": 48,
      "recurrenceCount": 20,
      "callbackUrl": null,
      "CallbackMethod": null,
      "format": "csv",
      "executionStatus": "Pending",
      "reportLocation": null,
      "reportAccessSecureLink": null,
      "reportExpiryTime": null,
      "reportGeneratedTime": null
    }
  ],
  "nextLink": null,
  "totalCount": 1,
  "message": null,
  "statusCode": 200,
  "dataRedacted": false
}
```

## <a name="next-steps"></a>Passos seguintes

- Experimente as APIs através do [URL da API swagger](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html)