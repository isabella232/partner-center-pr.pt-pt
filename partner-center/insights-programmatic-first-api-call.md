---
title: Faça a sua primeira chamada de API para aceder a dados de análise de insights de parceiros
description: Exemplos para aprender a usar a API para aceder a dados de análise de insights de parceiros.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: d2252ccfb601ae22ce106d87fb06b67bf0927df5
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376956"
---
# <a name="make-your-first-api-call-to-access-partner-insights-analytics-data"></a><span data-ttu-id="8ea05-103">Faça a sua primeira chamada de API para aceder a dados de análise de insights de parceiros</span><span class="sxs-lookup"><span data-stu-id="8ea05-103">Make your first API call to access partner insights analytics data</span></span>

<span data-ttu-id="8ea05-104">Para obter uma lista das APIs para aceder a dados de análise de insights de parceiros, consulte [APIs para aceder aos dados de análise de insights de parceiros](insights-programmatic-analytics-available-api.md).</span><span class="sxs-lookup"><span data-stu-id="8ea05-104">For a list of the APIs for accessing partner insights analytics data, see [APIs for accessing partner insights analytics data](insights-programmatic-analytics-available-api.md).</span></span> <span data-ttu-id="8ea05-105">Antes de fazer a sua primeira chamada API, certifique-se de que cumpriu os [requisitos necessários](insights-programmatic-prerequisites.md) para aceder programaticamente ao Parceiro Informações dados de análise.</span><span class="sxs-lookup"><span data-stu-id="8ea05-105">Before you make your first API call, make sure that you met the [pre-requisites](insights-programmatic-prerequisites.md) to programmatically access Partner Insights analytics data.</span></span>

## <a name="token-generation"></a><span data-ttu-id="8ea05-106">Geração Token</span><span class="sxs-lookup"><span data-stu-id="8ea05-106">Token generation</span></span>

<span data-ttu-id="8ea05-107">Antes de ligar para qualquer um dos métodos, você deve primeiro obter um token de acesso Azure Ative Directory (AAD).</span><span class="sxs-lookup"><span data-stu-id="8ea05-107">Before calling any of the methods, you must first obtain an Azure Active Directory (AAD) access token.</span></span> <span data-ttu-id="8ea05-108">Você precisa passar o token de acesso Azure para o cabeçalho de autorização de cada método na API.</span><span class="sxs-lookup"><span data-stu-id="8ea05-108">You need to pass the Azure AD access token to the Authorization header of each method in the API.</span></span> <span data-ttu-id="8ea05-109">Depois de obter um token de acesso, tem 60 minutos para usá-lo antes de expirar.</span><span class="sxs-lookup"><span data-stu-id="8ea05-109">After obtaining an access token, you have 60 minutes to use it before it expires.</span></span> <span data-ttu-id="8ea05-110">Após o fim do token, pode refrescar o token e pode continuar a usá-lo para mais chamadas para a API.</span><span class="sxs-lookup"><span data-stu-id="8ea05-110">After the token expires, you can refresh the token and can continue to use it for further calls to the API.</span></span>

<span data-ttu-id="8ea05-111">Consulte um pedido de amostra abaixo para gerar um token.</span><span class="sxs-lookup"><span data-stu-id="8ea05-111">Refer to a sample request below for generating a token.</span></span> <span data-ttu-id="8ea05-112">Os três valores que são necessários para gerar o símbolo `clientId` `clientSecret` são, e `tenantId` .</span><span class="sxs-lookup"><span data-stu-id="8ea05-112">The three values that are required to generate the token are `clientId`, `clientSecret`, and `tenantId`.</span></span> <span data-ttu-id="8ea05-113">O parâmetro de recurso deve ser definido para `https://api.partnercenter.microsoft.com`</span><span class="sxs-lookup"><span data-stu-id="8ea05-113">The resource parameter should be set to `https://api.partnercenter.microsoft.com`</span></span>

#### <a name="request-example"></a><span data-ttu-id="8ea05-114">Exemplo de pedido</span><span class="sxs-lookup"><span data-stu-id="8ea05-114">Request example</span></span>

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

#### <a name="response-example"></a><span data-ttu-id="8ea05-115">Exemplo de resposta</span><span class="sxs-lookup"><span data-stu-id="8ea05-115">Response example</span></span>

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

<span data-ttu-id="8ea05-116">Para obter mais informações sobre como obter um token AD Azure para a sua aplicação, consulte [os dados de análise do Access através dos serviços da Loja.](/windows/uwp/monetize/access-analytics-data-using-windows-store-services#step-2-obtain-an-azure-ad-access-token)</span><span class="sxs-lookup"><span data-stu-id="8ea05-116">For more information about how to obtain an Azure AD token for your application, see [Access analytics data using Store services.](/windows/uwp/monetize/access-analytics-data-using-windows-store-services#step-2-obtain-an-azure-ad-access-token)</span></span>

## <a name="programmatic-api-call"></a><span data-ttu-id="8ea05-117">Chamada de API programática</span><span class="sxs-lookup"><span data-stu-id="8ea05-117">Programmatic API call</span></span>

<span data-ttu-id="8ea05-118">Depois de obter o Token AAD como descrito na secção anterior, siga estes passos para criar o seu primeiro relatório de acesso programático.</span><span class="sxs-lookup"><span data-stu-id="8ea05-118">After you obtain the AAD Token as described in the previous section, follow these steps to create your first programmatic access report.</span></span>

<span data-ttu-id="8ea05-119">Os dados podem ser descarregados a partir dos seguintes conjuntos de dados (datasetName):</span><span class="sxs-lookup"><span data-stu-id="8ea05-119">Data can be downloaded from the following datasets (datasetName):</span></span>

- <span data-ttu-id="8ea05-120">ClientesTenants</span><span class="sxs-lookup"><span data-stu-id="8ea05-120">CustomersAndTenants</span></span>
- <span data-ttu-id="8ea05-121">AssentosSubscriçõesAndRevenue</span><span class="sxs-lookup"><span data-stu-id="8ea05-121">SeatsSubscriptionsAndRevenue</span></span>
- <span data-ttu-id="8ea05-122">AzureUsage</span><span class="sxs-lookup"><span data-stu-id="8ea05-122">AzureUsage</span></span>
- <span data-ttu-id="8ea05-123">MSLearn</span><span class="sxs-lookup"><span data-stu-id="8ea05-123">MSLearn</span></span>
- <span data-ttu-id="8ea05-124">OfficeUsage</span><span class="sxs-lookup"><span data-stu-id="8ea05-124">OfficeUsage</span></span>
- <span data-ttu-id="8ea05-125">Perfil</span><span class="sxs-lookup"><span data-stu-id="8ea05-125">Profile</span></span>
- <span data-ttu-id="8ea05-126">FormaçãoCompletions</span><span class="sxs-lookup"><span data-stu-id="8ea05-126">TrainingCompletions</span></span>
- <span data-ttu-id="8ea05-127">Dinâmica</span><span class="sxs-lookup"><span data-stu-id="8ea05-127">DynamicsUsage</span></span>
- <span data-ttu-id="8ea05-128">CompetênciaSSummaryHistória</span><span class="sxs-lookup"><span data-stu-id="8ea05-128">CompetencySummaryHistory</span></span>
- <span data-ttu-id="8ea05-129">PowerBIUsage</span><span class="sxs-lookup"><span data-stu-id="8ea05-129">PowerBIUsage</span></span>
- <span data-ttu-id="8ea05-130">EMSUsage</span><span class="sxs-lookup"><span data-stu-id="8ea05-130">EMSUsage</span></span>
- <span data-ttu-id="8ea05-131">CompetênciaPeformanceRequirement</span><span class="sxs-lookup"><span data-stu-id="8ea05-131">CompetencyPeformanceRequirement</span></span>
- <span data-ttu-id="8ea05-132">RevendedorPerformance</span><span class="sxs-lookup"><span data-stu-id="8ea05-132">ResellerPerformance</span></span>
- <span data-ttu-id="8ea05-133">CLASAgreementRenewalsPropensity</span><span class="sxs-lookup"><span data-stu-id="8ea05-133">CLASAgreementRenewalsPropensity</span></span>
- <span data-ttu-id="8ea05-134">CLASAzurePropensity</span><span class="sxs-lookup"><span data-stu-id="8ea05-134">CLASAzurePropensity</span></span>
- <span data-ttu-id="8ea05-135">CLASD365Propensity</span><span class="sxs-lookup"><span data-stu-id="8ea05-135">CLASD365Propensity</span></span>
- <span data-ttu-id="8ea05-136">CLASM365Propensity</span><span class="sxs-lookup"><span data-stu-id="8ea05-136">CLASM365Propensity</span></span>
- <span data-ttu-id="8ea05-137">TeamsUsage3PApps</span><span class="sxs-lookup"><span data-stu-id="8ea05-137">TeamsUsage3PApps</span></span>
- <span data-ttu-id="8ea05-138">TeamsUsageWorkload</span><span class="sxs-lookup"><span data-stu-id="8ea05-138">TeamsUsageWorkload</span></span>
- <span data-ttu-id="8ea05-139">TeamsUsageMeetingsAndCalls</span><span class="sxs-lookup"><span data-stu-id="8ea05-139">TeamsUsageMeetingsAndCalls</span></span>

<span data-ttu-id="8ea05-140">Na secção seguinte, veremos exemplos de como aceder programáticamente `SubscriptionId` a partir do conjunto de dados DynamicsUsage.</span><span class="sxs-lookup"><span data-stu-id="8ea05-140">In the following section, we will see examples of how to programmatically access `SubscriptionId` from the DynamicsUsage dataset.</span></span>

### <a name="step-1-make-a-rest-call-using-the-get-datasets-api"></a><span data-ttu-id="8ea05-141">Passo 1: Faça uma chamada REST utilizando a API de conjuntos de dados</span><span class="sxs-lookup"><span data-stu-id="8ea05-141">Step 1: Make a REST call using the get datasets API</span></span>

<span data-ttu-id="8ea05-142">A resposta da API fornece o nome do conjunto de dados de onde pode descarregar o relatório.</span><span class="sxs-lookup"><span data-stu-id="8ea05-142">The API response provides the dataset name from where you can download the report.</span></span> <span data-ttu-id="8ea05-143">Para o conjunto de dados específico, a resposta API também fornece a lista de colunas selecionáveis que podem ser usadas para o seu modelo de relatório personalizado.</span><span class="sxs-lookup"><span data-stu-id="8ea05-143">For the specific dataset, the API response also provides the list of selectable columns that can be used for your custom report template.</span></span> <span data-ttu-id="8ea05-144">Também pode consultar as [Definições de Dados](insights-data-definitions.md) para obter os nomes das colunas.</span><span class="sxs-lookup"><span data-stu-id="8ea05-144">You can also refer to the [Data Definitions](insights-data-definitions.md) to get the names of the columns.</span></span>

#### <a name="request-example"></a><span data-ttu-id="8ea05-145">Exemplo de pedido</span><span class="sxs-lookup"><span data-stu-id="8ea05-145">Request example</span></span>

```cli
curl 
--location 
--request GET 'https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledDataset'\
--header 'Authorization: Bearer <AADToken>'
```

#### <a name="response-example"></a><span data-ttu-id="8ea05-146">Exemplo de resposta</span><span class="sxs-lookup"><span data-stu-id="8ea05-146">Response example</span></span>

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

### <a name="step-2-create-the-custom-query"></a><span data-ttu-id="8ea05-147">Passo 2: Criar a Consulta Personalizada</span><span class="sxs-lookup"><span data-stu-id="8ea05-147">Step 2: Create the Custom Query</span></span>

<span data-ttu-id="8ea05-148">Neste passo, usaremos SubscriçãoId do conjunto de dados DynamicsUsage para criar uma consulta personalizada para o relatório que queremos.</span><span class="sxs-lookup"><span data-stu-id="8ea05-148">In this step, we will use SubscriptionId from the DynamicsUsage dataset to create a custom query for the report we want.</span></span> <span data-ttu-id="8ea05-149">O período de tempo padrão se não for especificado na consulta é de 6 meses.</span><span class="sxs-lookup"><span data-stu-id="8ea05-149">The default timespan if not specified in the query is 6 months.</span></span>

#### <a name="request-example"></a><span data-ttu-id="8ea05-150">Exemplo de pedido</span><span class="sxs-lookup"><span data-stu-id="8ea05-150">Request example</span></span>

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

#### <a name="response-example"></a><span data-ttu-id="8ea05-151">Exemplo de resposta</span><span class="sxs-lookup"><span data-stu-id="8ea05-151">Response example</span></span>

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

<span data-ttu-id="8ea05-152">Na execução bem sucedida da consulta, é gerada uma `queryId` que precisa de ser usada para gerar o relatório.</span><span class="sxs-lookup"><span data-stu-id="8ea05-152">On successful execution of the query, a `queryId` is generated that needs to be used to generate the report.</span></span>

### <a name="step-3-execute-test-query-api"></a><span data-ttu-id="8ea05-153">Passo 3: Executar consulta de teste API</span><span class="sxs-lookup"><span data-stu-id="8ea05-153">Step 3: Execute test query API</span></span>

<span data-ttu-id="8ea05-154">Neste passo, vamos usar a consulta de teste API para obter as 100 melhores linhas para a consulta que foi criada.</span><span class="sxs-lookup"><span data-stu-id="8ea05-154">In this step, we will use the test query API to get the top 100 rows for the query that was created.</span></span>

#### <a name="request-example"></a><span data-ttu-id="8ea05-155">Exemplo de pedido</span><span class="sxs-lookup"><span data-stu-id="8ea05-155">Request example</span></span>

```cli
curl 
--location 
--request GET 'https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries/testQueryResult?queryId=7d19305c-56db-4edc-b776-428340e3a9c8' \
--header ' Authorization: Bearer <AADToken>'
```

#### <a name="response-example"></a><span data-ttu-id="8ea05-156">Exemplo de resposta</span><span class="sxs-lookup"><span data-stu-id="8ea05-156">Response example</span></span>

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

### <a name="step-4-create-the-report"></a><span data-ttu-id="8ea05-157">Passo 4: Criar o relatório</span><span class="sxs-lookup"><span data-stu-id="8ea05-157">Step 4: Create the report</span></span>

<span data-ttu-id="8ea05-158">Neste passo, usaremos a Consulta anteriormente gerada para criar o relatório.</span><span class="sxs-lookup"><span data-stu-id="8ea05-158">In this step, we will use the previously generated QueryId to create the report.</span></span>

#### <a name="request-example"></a><span data-ttu-id="8ea05-159">Exemplo de pedido</span><span class="sxs-lookup"><span data-stu-id="8ea05-159">Request example</span></span>

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

#### <a name="response-example"></a><span data-ttu-id="8ea05-160">Exemplo de resposta</span><span class="sxs-lookup"><span data-stu-id="8ea05-160">Response example</span></span>

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

<span data-ttu-id="8ea05-161">Na execução bem sucedida, é gerado um `reportId` que precisa ser usado para agendar um download do relatório.</span><span class="sxs-lookup"><span data-stu-id="8ea05-161">On successful execution, a `reportId` is generated that needs to be used to schedule a download of the report.</span></span>

### <a name="step-5-execute-report-executions-api"></a><span data-ttu-id="8ea05-162">Passo 5: Executar relatório execuções execuções API</span><span class="sxs-lookup"><span data-stu-id="8ea05-162">Step 5: Execute Report Executions API</span></span>

<span data-ttu-id="8ea05-163">Neste passo, usaremos a API de Execuções de Relatório para obter a localização segura (URL) do relatório.</span><span class="sxs-lookup"><span data-stu-id="8ea05-163">In this step, we will use the Report Executions API to get the secure location (URL) of the report.</span></span>

#### <a name="request-example"></a><span data-ttu-id="8ea05-164">Exemplo de pedido</span><span class="sxs-lookup"><span data-stu-id="8ea05-164">Request example</span></span>

```cli
Curl
--location 
--request GET 'https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/execution/ cdc61cfe-d028-4333-a215-a1df51ccbfd4?getLatestExecution=true'\
--header ' Authorization: Bearer <AADToken>' \
```

#### <a name="response-example"></a><span data-ttu-id="8ea05-165">Exemplo de resposta</span><span class="sxs-lookup"><span data-stu-id="8ea05-165">Response example</span></span>

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

## <a name="next-steps"></a><span data-ttu-id="8ea05-166">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="8ea05-166">Next steps</span></span>

- <span data-ttu-id="8ea05-167">Experimente as APIs através do [URL da API](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html)</span><span class="sxs-lookup"><span data-stu-id="8ea05-167">Try out the APIs through the [swagger API URL](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html)</span></span>