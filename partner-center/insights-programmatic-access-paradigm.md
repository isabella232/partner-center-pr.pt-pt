---
title: Paradigma de acesso programático para dados Informações
description: Compreenda o fluxo de alto nível do padrão de chamada da API para análise programática. As APIs para aceder a relatórios de análise de insights de parceiros também são abrangidas.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: dcdd54fcc744fdb1683259203188c309a3949eff
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376981"
---
# <a name="programmatic-access-paradigm"></a><span data-ttu-id="3079a-104">Paradigma de acesso programático</span><span class="sxs-lookup"><span data-stu-id="3079a-104">Programmatic access paradigm</span></span>

<span data-ttu-id="3079a-105">Este diagrama mostra o padrão de chamada da API usado para criar um novo modelo de relatório, agendar o relatório personalizado e recuperar dados de falha.</span><span class="sxs-lookup"><span data-stu-id="3079a-105">This diagram shows the API call pattern used to create a new report template, schedule the custom report and retrieve failure data.</span></span>

:::image type="content" source="images/insights/prog-acc-paradigm.png" alt-text="Fluxo de alto nível":::
<span data-ttu-id="3079a-107">***Figura 1: Fluxo de alto nível do padrão de chamada API***</span><span class="sxs-lookup"><span data-stu-id="3079a-107">***Figure 1: High level flow of the API call pattern***</span></span>

<span data-ttu-id="3079a-108">Esta lista fornece mais detalhes sobre a Figura 1.</span><span class="sxs-lookup"><span data-stu-id="3079a-108">This list provides more details about Figure 1.</span></span>

1. <span data-ttu-id="3079a-109">A Aplicação do Cliente pode definir o esquema/modelo de relatório personalizado, chamando a [API de Consulta de Relatório de Criação](#create-report-query-api).</span><span class="sxs-lookup"><span data-stu-id="3079a-109">The Client Application can define the custom report schema/template by calling the [Create Report Query API](#create-report-query-api).</span></span> <span data-ttu-id="3079a-110">Alternadamente, pode escolher um modelo de relatório (QueryId) a partir das amostras da biblioteca do modelo de relatório listadas [aqui.](insights-programmatic-system-queries.md)</span><span class="sxs-lookup"><span data-stu-id="3079a-110">Alternately, you can pick a report template (QueryId) from the report template library samples listed [here.](insights-programmatic-system-queries.md)</span></span>
2. <span data-ttu-id="3079a-111">No sucesso, a API de Consulta de Relatório de Criação devolve o QueryId.</span><span class="sxs-lookup"><span data-stu-id="3079a-111">On success, the Create Report Query API returns the QueryId.</span></span>
3. <span data-ttu-id="3079a-112">A aplicação do cliente precisa então de ligar para a [API do Relatório de Criação](#create-report-api) utilizando o QueryId juntamente com a data de início do relatório, Repeat Interval, Recorrence e um URI de retorno opcional.</span><span class="sxs-lookup"><span data-stu-id="3079a-112">The client application then needs to call the [Create Report API](#create-report-api) using the QueryId along with the report start date, Repeat Interval, Recurrence, and an optional Callback URI.</span></span>
4. <span data-ttu-id="3079a-113">Sobre o Sucesso, a [API do Relatório de Criação](#create-report-api) devolve o ReportId.</span><span class="sxs-lookup"><span data-stu-id="3079a-113">On Success, the [Create Report API](#create-report-api) returns the ReportId.</span></span>
5. <span data-ttu-id="3079a-114">A aplicação do cliente é notificada no URL de retorno assim que os dados do relatório estiverem prontos para download.</span><span class="sxs-lookup"><span data-stu-id="3079a-114">The client application gets notified at the callback URL as soon as the report data is ready for download.</span></span>
6. <span data-ttu-id="3079a-115">A aplicação do cliente utiliza então a [API get report execuções](#get-report-execution-api) para consultar o estado do relatório com o ID do relatório e o intervalo de data.</span><span class="sxs-lookup"><span data-stu-id="3079a-115">The client application then uses the [Get Report Executions API](#get-report-execution-api) to query the status of the report with the Report ID and date range.</span></span>
7. <span data-ttu-id="3079a-116">Com o sucesso, o link de descarregamento do relatório é devolvido e a aplicação pode iniciar o download dos dados.</span><span class="sxs-lookup"><span data-stu-id="3079a-116">On success, the report download link is returned and the application can initiate download of the data.</span></span>

## <a name="report-query-language-specification"></a><span data-ttu-id="3079a-117">Especificação da linguagem de consulta de relatório</span><span class="sxs-lookup"><span data-stu-id="3079a-117">Report query language specification</span></span>

<span data-ttu-id="3079a-118">Enquanto fornecemos [consultas de sistema](insights-programmatic-system-queries.md) que pode usar para criar relatórios, também pode criar as suas próprias consultas com base nas necessidades do seu negócio.</span><span class="sxs-lookup"><span data-stu-id="3079a-118">While we do provide [system queries](insights-programmatic-system-queries.md) you can use to create reports, you can also create your own queries based on your business needs.</span></span> <span data-ttu-id="3079a-119">Para saber mais sobre consultas personalizadas, consulte [Especificação de Consulta Personalizada.](insights-programmatic-custom-query.md)</span><span class="sxs-lookup"><span data-stu-id="3079a-119">To learn more about custom queries, see [Custom Query Specification](insights-programmatic-custom-query.md).</span></span>

## <a name="create-report-query-api"></a><span data-ttu-id="3079a-120">Criar consulta de relatório API</span><span class="sxs-lookup"><span data-stu-id="3079a-120">Create report query API</span></span>

<span data-ttu-id="3079a-121">A API ajuda a criar consultas personalizadas que definem o conjunto de dados a partir do qual as colunas e métricas precisam de ser exportadas.</span><span class="sxs-lookup"><span data-stu-id="3079a-121">The API helps to create custom queries that define the dataset from which columns and metrics need to be exported.</span></span> <span data-ttu-id="3079a-122">A API fornece a flexibilidade para criar um novo modelo de reporte baseado nas necessidades do seu negócio.</span><span class="sxs-lookup"><span data-stu-id="3079a-122">The API provides the flexibility to create a new reporting template based on your business needs.</span></span>  

<span data-ttu-id="3079a-123">Também pode utilizar as [consultas do sistema](insights-programmatic-system-queries.md) que fornecemos.</span><span class="sxs-lookup"><span data-stu-id="3079a-123">You can also use the [system queries](insights-programmatic-system-queries.md) we provide.</span></span> <span data-ttu-id="3079a-124">Quando não forem necessários modelos de relatórios personalizados, pode ligar para [a API do Relatório de Criar](#create-report-api) diretamente utilizando as Consultas das consultas do sistema fornecidas.</span><span class="sxs-lookup"><span data-stu-id="3079a-124">When custom report templates are not needed, you can call [Create Report API](#create-report-api) directly using the QueryIds of the system queries that are provided.</span></span>  

<span data-ttu-id="3079a-125">O exemplo a seguir mostra como criar uma consulta personalizada para obter os 10 melhores clientes por receitas do mês passado.</span><span class="sxs-lookup"><span data-stu-id="3079a-125">The following example shows how to create a custom query to get top 10 customers by revenue for last month.</span></span>

### <a name="request-syntax"></a><span data-ttu-id="3079a-126">Solicitar sintaxe</span><span class="sxs-lookup"><span data-stu-id="3079a-126">Request syntax</span></span>

|    <span data-ttu-id="3079a-127">Método</span><span class="sxs-lookup"><span data-stu-id="3079a-127">Method</span></span>     |    <span data-ttu-id="3079a-128">URI do pedido</span><span class="sxs-lookup"><span data-stu-id="3079a-128">Request URI</span></span>     |
|----- | -----|
|    <span data-ttu-id="3079a-129">POST</span><span class="sxs-lookup"><span data-stu-id="3079a-129">POST</span></span>     |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries`|
|||

### <a name="request-header"></a><span data-ttu-id="3079a-130">Cabeçalho do pedido</span><span class="sxs-lookup"><span data-stu-id="3079a-130">Request header</span></span>

|    <span data-ttu-id="3079a-131">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3079a-131">Header</span></span>     |    <span data-ttu-id="3079a-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="3079a-132">Type</span></span>     |    <span data-ttu-id="3079a-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="3079a-133">Description</span></span>     |
|-------|-----|------|
|    <span data-ttu-id="3079a-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="3079a-134">Authorization</span></span>     |    <span data-ttu-id="3079a-135">string</span><span class="sxs-lookup"><span data-stu-id="3079a-135">string</span></span> |<span data-ttu-id="3079a-136">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3079a-136">Required.</span></span> <span data-ttu-id="3079a-137">O Azure Ative Directory (Azure AD) de acesso.</span><span class="sxs-lookup"><span data-stu-id="3079a-137">The Azure Active Directory (Azure AD) access token.</span></span> <span data-ttu-id="3079a-138">O formato é  `Bearer <token>` .</span><span class="sxs-lookup"><span data-stu-id="3079a-138">The format is `Bearer <token>`.</span></span>|
|    <span data-ttu-id="3079a-139">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3079a-139">Content-Type</span></span>     |<span data-ttu-id="3079a-140">string</span><span class="sxs-lookup"><span data-stu-id="3079a-140">string</span></span> |`Application/JSON` |
||||

### <a name="path-parameter"></a><span data-ttu-id="3079a-141">Parâmetro do caminho</span><span class="sxs-lookup"><span data-stu-id="3079a-141">Path parameter</span></span>

<span data-ttu-id="3079a-142">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="3079a-142">None</span></span>

### <a name="query-parameter"></a><span data-ttu-id="3079a-143">Parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="3079a-143">Query parameter</span></span>

<span data-ttu-id="3079a-144">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="3079a-144">None</span></span>

### <a name="sample-request-payload"></a><span data-ttu-id="3079a-145">Carga útil do pedido de amostra</span><span class="sxs-lookup"><span data-stu-id="3079a-145">Sample request payload</span></span>

```json
{ 
  "Name": "CustomersRevenueQuery", 
  "Description": "Query to get top 10 customers by revenue for last month", 
  "Query": "SELECT CustomerName, Product, BilledRevenueUSD FROM CustomersAndTenants ORDER BY BilledRevenueUSD LIMIT 10 TIMESPAN LAST_MONTH" 
}
```

### <a name="glossary"></a><span data-ttu-id="3079a-146">Glossário</span><span class="sxs-lookup"><span data-stu-id="3079a-146">Glossary</span></span>

<span data-ttu-id="3079a-147">Esta tabela fornece as definições-chave dos elementos na carga útil do pedido.</span><span class="sxs-lookup"><span data-stu-id="3079a-147">This table provides the key definitions of elements in the request payload.</span></span>

|<span data-ttu-id="3079a-148">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="3079a-148">Parameter</span></span>|    <span data-ttu-id="3079a-149">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="3079a-149">Required</span></span>     |    <span data-ttu-id="3079a-150">Descrição</span><span class="sxs-lookup"><span data-stu-id="3079a-150">Description</span></span>     |    <span data-ttu-id="3079a-151">Valores Permitidos</span><span class="sxs-lookup"><span data-stu-id="3079a-151">Allowed Values</span></span>     |
|-----|    -----    |    -----    |    -----    |
|<span data-ttu-id="3079a-152">Name</span><span class="sxs-lookup"><span data-stu-id="3079a-152">Name</span></span> |    <span data-ttu-id="3079a-153">Yes</span><span class="sxs-lookup"><span data-stu-id="3079a-153">Yes</span></span>     |    <span data-ttu-id="3079a-154">Nome amigável da consulta</span><span class="sxs-lookup"><span data-stu-id="3079a-154">Friendly name of the query</span></span>     |    <span data-ttu-id="3079a-155">string</span><span class="sxs-lookup"><span data-stu-id="3079a-155">string</span></span>     |
|    <span data-ttu-id="3079a-156">Descrição</span><span class="sxs-lookup"><span data-stu-id="3079a-156">Description</span></span>     |    <span data-ttu-id="3079a-157">Não</span><span class="sxs-lookup"><span data-stu-id="3079a-157">No</span></span>     |    <span data-ttu-id="3079a-158">Descrição do que a consulta retorna</span><span class="sxs-lookup"><span data-stu-id="3079a-158">Description of what the query returns</span></span>     |    <span data-ttu-id="3079a-159">string</span><span class="sxs-lookup"><span data-stu-id="3079a-159">string</span></span>     |
|    <span data-ttu-id="3079a-160">Consulta</span><span class="sxs-lookup"><span data-stu-id="3079a-160">Query</span></span>     |    <span data-ttu-id="3079a-161">Yes</span><span class="sxs-lookup"><span data-stu-id="3079a-161">Yes</span></span>     |    <span data-ttu-id="3079a-162">Cadeia de consulta de relatório</span><span class="sxs-lookup"><span data-stu-id="3079a-162">Report query string</span></span>     |    <span data-ttu-id="3079a-163">Tipo de dados: cadeia</span><span class="sxs-lookup"><span data-stu-id="3079a-163">Data type: string</span></span> <br> <span data-ttu-id="3079a-164">[Consulta personalizada](insights-programmatic-custom-query.md) baseada na necessidade de negócio</span><span class="sxs-lookup"><span data-stu-id="3079a-164">[Custom query](insights-programmatic-custom-query.md) based on business need</span></span> |
|        |        |        |        |

> [!Note]
> <span data-ttu-id="3079a-165">Para amostras de consulta personalizada, consulte [exemplos de consultas de amostras.](insights-programmatic-sample-queries.md)</span><span class="sxs-lookup"><span data-stu-id="3079a-165">For custom query samples, see [Examples of sample queries.](insights-programmatic-sample-queries.md)</span></span>

### <a name="sample-response"></a><span data-ttu-id="3079a-166">Resposta de amostra</span><span class="sxs-lookup"><span data-stu-id="3079a-166">Sample response</span></span>

<span data-ttu-id="3079a-167">A carga útil de resposta é estruturada da seguinte forma:</span><span class="sxs-lookup"><span data-stu-id="3079a-167">The response payload is structured as follows:</span></span>

<span data-ttu-id="3079a-168">Códigos de Resposta: 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="3079a-168">Response Codes: 200, 400, 401, 403, 500</span></span>

<span data-ttu-id="3079a-169">Exemplo de carga útil de resposta:</span><span class="sxs-lookup"><span data-stu-id="3079a-169">Response payload example:</span></span>

```json
{ 
  "value": [ 
    { 
      "queryId": "ec8366a4-d96e-4194-8c37-d5dbc0639033",
      "name": "CustomersRevenueQuery",
      "description": "Query to get top 10 customers by revenue for last month",
      "query": "SELECT CustomerName, Product, BilledRevenueUSD FROM CustomersAndTenants ORDER BY BilledRevenueUSD LIMIT 10 TIMESPAN LAST_MONTH",
      "type": "userDefined",
      "user": "GAUser@PITEST2.ccsctp.net", 
      "createdTime": "2021-03-30T12:52:39Z" 
    }
  ], 
  "nextLink": null,
  "totalCount": 1,
  "message": "Query created successfully",
  "statusCode": 200,
  "dataRedacted": false
} 
```

### <a name="glossary"></a><span data-ttu-id="3079a-170">Glossário</span><span class="sxs-lookup"><span data-stu-id="3079a-170">Glossary</span></span>

<span data-ttu-id="3079a-171">Esta tabela fornece as definições-chave dos elementos na carga útil do pedido.</span><span class="sxs-lookup"><span data-stu-id="3079a-171">This table provides the key definitions of elements in the request payload.</span></span>

|    <span data-ttu-id="3079a-172">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="3079a-172">Parameter</span></span>     |    <span data-ttu-id="3079a-173">Descrição</span><span class="sxs-lookup"><span data-stu-id="3079a-173">Description</span></span>     |
|    ----    |    ----    |
|    <span data-ttu-id="3079a-174">QueryId</span><span class="sxs-lookup"><span data-stu-id="3079a-174">QueryId</span></span>     |    <span data-ttu-id="3079a-175">Identificador universalmente único (UUID) da consulta que criou</span><span class="sxs-lookup"><span data-stu-id="3079a-175">Universally unique identifier (UUID) of the query you created</span></span>     |
|    <span data-ttu-id="3079a-176">Name</span><span class="sxs-lookup"><span data-stu-id="3079a-176">Name</span></span>     |    <span data-ttu-id="3079a-177">Nome amigável dado à consulta na carga útil do pedido</span><span class="sxs-lookup"><span data-stu-id="3079a-177">Friendly name given to the query in the request payload</span></span>     |
|    <span data-ttu-id="3079a-178">Descrição</span><span class="sxs-lookup"><span data-stu-id="3079a-178">Description</span></span>     |    <span data-ttu-id="3079a-179">Descrição dada durante a criação da consulta</span><span class="sxs-lookup"><span data-stu-id="3079a-179">Description given during creation of the query</span></span>     |
|    <span data-ttu-id="3079a-180">Consulta</span><span class="sxs-lookup"><span data-stu-id="3079a-180">Query</span></span>     |    <span data-ttu-id="3079a-181">Consulta de relatório passada como entrada durante a criação de consulta</span><span class="sxs-lookup"><span data-stu-id="3079a-181">Report query passed as input during query creation</span></span>     |
|    <span data-ttu-id="3079a-182">Tipo</span><span class="sxs-lookup"><span data-stu-id="3079a-182">Type</span></span>     |    <span data-ttu-id="3079a-183">Definir para `userDefined`</span><span class="sxs-lookup"><span data-stu-id="3079a-183">Set to `userDefined`</span></span>     |
|    <span data-ttu-id="3079a-184">Utilizador</span><span class="sxs-lookup"><span data-stu-id="3079a-184">User</span></span>     |    <span data-ttu-id="3079a-185">ID do utilizador usado para criar a consulta</span><span class="sxs-lookup"><span data-stu-id="3079a-185">User ID used to create of the query</span></span>     |
|    <span data-ttu-id="3079a-186">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="3079a-186">CreatedTime</span></span>     |    <span data-ttu-id="3079a-187">TEMPO UTC A consulta foi criada neste formato: yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="3079a-187">UTC Time the query was created in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="3079a-188">TotalCount</span><span class="sxs-lookup"><span data-stu-id="3079a-188">TotalCount</span></span>     |    <span data-ttu-id="3079a-189">Número de conjuntos de dados na matriz de valor</span><span class="sxs-lookup"><span data-stu-id="3079a-189">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="3079a-190">Código de Estado</span><span class="sxs-lookup"><span data-stu-id="3079a-190">StatusCode</span></span>     |    <span data-ttu-id="3079a-191">Código do Resultado</span><span class="sxs-lookup"><span data-stu-id="3079a-191">Result Code</span></span> <br> <span data-ttu-id="3079a-192">Os valores possíveis são 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="3079a-192">The possible values are 200, 400, 401, 403, 500</span></span>     |
|    <span data-ttu-id="3079a-193">message</span><span class="sxs-lookup"><span data-stu-id="3079a-193">message</span></span>     |    <span data-ttu-id="3079a-194">Mensagem de estado da execução da API</span><span class="sxs-lookup"><span data-stu-id="3079a-194">Status message from the execution of the API</span></span>     |
|        |        |

## <a name="create-report-api"></a><span data-ttu-id="3079a-195">Criar relatório API</span><span class="sxs-lookup"><span data-stu-id="3079a-195">Create report API</span></span>

<span data-ttu-id="3079a-196">Ao criar um modelo de relatório personalizado com sucesso e receber o QueryID como parte da resposta [Create Report Query,](#create-report-query-api) esta API pode ser chamada para agendar uma consulta a ser executada a intervalos regulares.</span><span class="sxs-lookup"><span data-stu-id="3079a-196">On creating a custom report template successfully and receiving the QueryID as part of [Create Report Query](#create-report-query-api) response, this API can be called to schedule a query to be executed at regular intervals.</span></span> <span data-ttu-id="3079a-197">Pode definir uma frequência e um horário para que o relatório seja entregue.</span><span class="sxs-lookup"><span data-stu-id="3079a-197">You can set a frequency and schedule for the report to be delivered.</span></span>
<span data-ttu-id="3079a-198">Para consultas de sistema que fornecemos, a API do Relatório de Criação também pode ser chamada com [Consulta.](insights-programmatic-system-queries.md)</span><span class="sxs-lookup"><span data-stu-id="3079a-198">For system queries we provide, the Create Report API can also be called with [QueryId](insights-programmatic-system-queries.md).</span></span>

### <a name="callback-url"></a><span data-ttu-id="3079a-199">URL de chamada de retorno</span><span class="sxs-lookup"><span data-stu-id="3079a-199">Callback URL</span></span>

<span data-ttu-id="3079a-200">A API do relatório de criação aceita um URL de retorno.</span><span class="sxs-lookup"><span data-stu-id="3079a-200">The create report API accepts a callback URL.</span></span> <span data-ttu-id="3079a-201">Esta URL será chamada assim que a geração do relatório for bem sucedida.</span><span class="sxs-lookup"><span data-stu-id="3079a-201">This URL will be called once the report generation is successful.</span></span> <span data-ttu-id="3079a-202">O URL de retorno deve ser acessível publicamente.</span><span class="sxs-lookup"><span data-stu-id="3079a-202">The callback URL should be publicly reachable.</span></span> <span data-ttu-id="3079a-203">Além do URL, um método de retorno também pode ser dado.</span><span class="sxs-lookup"><span data-stu-id="3079a-203">In addition to the URL a callback method can also be given.</span></span> <span data-ttu-id="3079a-204">O método de retorno só pode ser "GET" ou "POST".</span><span class="sxs-lookup"><span data-stu-id="3079a-204">The callback method can only be "GET" or "POST".</span></span> <span data-ttu-id="3079a-205">O método padrão se nenhum valor for passado será "POST".</span><span class="sxs-lookup"><span data-stu-id="3079a-205">The default method if no value is passed will be "POST".</span></span> <span data-ttu-id="3079a-206">O reportId que completou a geração será sempre reensibar durante a chamada.</span><span class="sxs-lookup"><span data-stu-id="3079a-206">The reportId that has completed generation will always be passed back during the callback.</span></span>

<span data-ttu-id="3079a-207">POST callback: Se o URL passou foi `https://www.contosso.com/callback` , então o URL chamado de volta será `https://www.contosso.com/callback/<reportID>`</span><span class="sxs-lookup"><span data-stu-id="3079a-207">POST callback: If the URL passed was `https://www.contosso.com/callback`, then the called back URL will be `https://www.contosso.com/callback/<reportID>`</span></span> 

<span data-ttu-id="3079a-208">GET callback: Se o URL passou foi `https://www.contosso.com/callback` , então o URL chamado de volta será `https://www.contosso.com/callback?reportId=<reportID>`</span><span class="sxs-lookup"><span data-stu-id="3079a-208">GET callback: If the URL passed was `https://www.contosso.com/callback`, then the called back URL will be `https://www.contosso.com/callback?reportId=<reportID>`</span></span> 

### <a name="executenow-reports"></a><span data-ttu-id="3079a-209">Executar Relatórios DeNow</span><span class="sxs-lookup"><span data-stu-id="3079a-209">ExecuteNow reports</span></span>

<span data-ttu-id="3079a-210">Existe uma disposição para gerar um relatório sem agendamento.</span><span class="sxs-lookup"><span data-stu-id="3079a-210">There is a provision to generate a report without scheduling.</span></span> <span data-ttu-id="3079a-211">O relatório que cria a carga útil da API pode aceitar um parâmetro `ExecuteNow` , que irá encarregar o relatório a ser gerado assim que a API for chamada.</span><span class="sxs-lookup"><span data-stu-id="3079a-211">The report create API payload can accept a parameter `ExecuteNow`, which will enqueue the report to be generated as soon as the API is called.</span></span> <span data-ttu-id="3079a-212">Quando `ExecuteNow` é definido como verdadeiro, os campos: , são `StartTime` `RecurrenceCount` `RecurrenceInterval` ignorados porque estes relatórios não estão agendados.</span><span class="sxs-lookup"><span data-stu-id="3079a-212">When `ExecuteNow` is set to true, the fields: `StartTime`, `RecurrenceCount`, `RecurrenceInterval` are ignored as these reports are not scheduled.</span></span>

<span data-ttu-id="3079a-213">Dois campos adicionais podem ser passados quando `ExecuteNow` é verdade, `QueryStartTime` e `QueryEndTime` .</span><span class="sxs-lookup"><span data-stu-id="3079a-213">Two additional fields can be passed when `ExecuteNow` is true, `QueryStartTime` and `QueryEndTime`.</span></span> <span data-ttu-id="3079a-214">Estes dois campos vão sobrepor-se `TIMESPAN` ao campo na consulta.</span><span class="sxs-lookup"><span data-stu-id="3079a-214">These two fields will override the `TIMESPAN` field in the query.</span></span> <span data-ttu-id="3079a-215">Estes campos não são aplicáveis aos relatórios agendados, uma vez que os dados serão gerados continuamente por um período de tempo fixo que não se altere.</span><span class="sxs-lookup"><span data-stu-id="3079a-215">These fields are not applicable for scheduled reports as data will get continuously generated for a fixed time period that does not change.</span></span>

### <a name="request-syntax"></a><span data-ttu-id="3079a-216">Solicitar sintaxe</span><span class="sxs-lookup"><span data-stu-id="3079a-216">Request syntax</span></span>

|    <span data-ttu-id="3079a-217">Método</span><span class="sxs-lookup"><span data-stu-id="3079a-217">Method</span></span>     |    <span data-ttu-id="3079a-218">URI do pedido</span><span class="sxs-lookup"><span data-stu-id="3079a-218">Request URI</span></span>     |
|----- | -----|
|    <span data-ttu-id="3079a-219">POST</span><span class="sxs-lookup"><span data-stu-id="3079a-219">POST</span></span>     |`https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport` |

### <a name="request-header"></a><span data-ttu-id="3079a-220">Cabeçalho do pedido</span><span class="sxs-lookup"><span data-stu-id="3079a-220">Request header</span></span>

|    <span data-ttu-id="3079a-221">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3079a-221">Header</span></span>     |    <span data-ttu-id="3079a-222">Tipo</span><span class="sxs-lookup"><span data-stu-id="3079a-222">Type</span></span>     |    <span data-ttu-id="3079a-223">Descrição</span><span class="sxs-lookup"><span data-stu-id="3079a-223">Description</span></span>     |
|-------|-----|------|
|    <span data-ttu-id="3079a-224">Autorização</span><span class="sxs-lookup"><span data-stu-id="3079a-224">Authorization</span></span>     |    <span data-ttu-id="3079a-225">string</span><span class="sxs-lookup"><span data-stu-id="3079a-225">string</span></span> |<span data-ttu-id="3079a-226">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3079a-226">Required.</span></span> <span data-ttu-id="3079a-227">O Azure Ative Directory (Azure AD) de acesso.</span><span class="sxs-lookup"><span data-stu-id="3079a-227">The Azure Active Directory (Azure AD) access token.</span></span> <span data-ttu-id="3079a-228">O formato é  `Bearer <token>` .</span><span class="sxs-lookup"><span data-stu-id="3079a-228">The format is `Bearer <token>`.</span></span>|
|    <span data-ttu-id="3079a-229">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3079a-229">Content-Type</span></span>     |<span data-ttu-id="3079a-230">string</span><span class="sxs-lookup"><span data-stu-id="3079a-230">string</span></span> |`Application/JSON` |

### <a name="path-parameter"></a><span data-ttu-id="3079a-231">Parâmetro do caminho</span><span class="sxs-lookup"><span data-stu-id="3079a-231">Path Parameter</span></span>

<span data-ttu-id="3079a-232">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="3079a-232">None</span></span>

### <a name="query-parameter"></a><span data-ttu-id="3079a-233">Parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="3079a-233">Query Parameter</span></span>

<span data-ttu-id="3079a-234">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="3079a-234">None</span></span>

### <a name="sample-request-payload"></a><span data-ttu-id="3079a-235">Carga útil do pedido de amostra</span><span class="sxs-lookup"><span data-stu-id="3079a-235">Sample request payload</span></span>

```json
{
  "ReportName": "Top10_CustomersReport",
  "Description": "Top 10 customers by revenue for last month",
  "QueryId": "ec8366a4-d96e-4194-8c37-d5dbc0639033",
  "StartTime": "2021-03-31T18:41:00Z",
  "ExecuteNow": false,
  "QueryStartTime": null,
  "QueryEndTime": null,
  "RecurrenceInterval": 24,
  "RecurrenceCount": 100,
  "Format": "CSV",
  "CallbackUrl": "https://<SampleCallbackUrl>",
  "CallbackMethod": "GET"
}
```

### <a name="glossary"></a><span data-ttu-id="3079a-236">Glossário</span><span class="sxs-lookup"><span data-stu-id="3079a-236">Glossary</span></span>

<span data-ttu-id="3079a-237">As definições-chave dos elementos na carga útil do pedido são articuladas abaixo:</span><span class="sxs-lookup"><span data-stu-id="3079a-237">Key definitions of elements in the request payload are articulated below:</span></span>

|    <span data-ttu-id="3079a-238">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="3079a-238">Parameter</span></span>     |    <span data-ttu-id="3079a-239">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="3079a-239">Required</span></span>     |    <span data-ttu-id="3079a-240">Descrição</span><span class="sxs-lookup"><span data-stu-id="3079a-240">Description</span></span>     |    <span data-ttu-id="3079a-241">Valores Permitidos</span><span class="sxs-lookup"><span data-stu-id="3079a-241">Allowed Values</span></span>     |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="3079a-242">Nome do relatório</span><span class="sxs-lookup"><span data-stu-id="3079a-242">ReportName</span></span>     |    <span data-ttu-id="3079a-243">Yes</span><span class="sxs-lookup"><span data-stu-id="3079a-243">Yes</span></span>     |    <span data-ttu-id="3079a-244">Nome a atribuir ao relatório</span><span class="sxs-lookup"><span data-stu-id="3079a-244">Name to be assigned to the report</span></span>     |    <span data-ttu-id="3079a-245">string</span><span class="sxs-lookup"><span data-stu-id="3079a-245">string</span></span>     |
|    <span data-ttu-id="3079a-246">Descrição</span><span class="sxs-lookup"><span data-stu-id="3079a-246">Description</span></span>     |    <span data-ttu-id="3079a-247">Não</span><span class="sxs-lookup"><span data-stu-id="3079a-247">No</span></span>     |    <span data-ttu-id="3079a-248">Descrição do relatório criado</span><span class="sxs-lookup"><span data-stu-id="3079a-248">Description of the created report</span></span>     |    <span data-ttu-id="3079a-249">string</span><span class="sxs-lookup"><span data-stu-id="3079a-249">string</span></span>     |
|    <span data-ttu-id="3079a-250">QueryId</span><span class="sxs-lookup"><span data-stu-id="3079a-250">QueryId</span></span>     |    <span data-ttu-id="3079a-251">Yes</span><span class="sxs-lookup"><span data-stu-id="3079a-251">Yes</span></span>     |    <span data-ttu-id="3079a-252">ID de consulta de relatório</span><span class="sxs-lookup"><span data-stu-id="3079a-252">Report query ID</span></span>     |    <span data-ttu-id="3079a-253">string</span><span class="sxs-lookup"><span data-stu-id="3079a-253">string</span></span>     |
|    <span data-ttu-id="3079a-254">StartTime</span><span class="sxs-lookup"><span data-stu-id="3079a-254">StartTime</span></span>     |    <span data-ttu-id="3079a-255">Yes</span><span class="sxs-lookup"><span data-stu-id="3079a-255">Yes</span></span>     |    <span data-ttu-id="3079a-256">Utc Timestamp em que a geração do relatório começará.</span><span class="sxs-lookup"><span data-stu-id="3079a-256">UTC Timestamp at which the report generation will begin.</span></span> <br> <span data-ttu-id="3079a-257">O formato deve ser: yyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="3079a-257">The format should be: yyyy-MM-ddTHH:mm:ssZ</span></span>       |    <span data-ttu-id="3079a-258">string</span><span class="sxs-lookup"><span data-stu-id="3079a-258">string</span></span>     |
|    <span data-ttu-id="3079a-259">Executar Agora</span><span class="sxs-lookup"><span data-stu-id="3079a-259">ExecuteNow</span></span>     |    <span data-ttu-id="3079a-260">No</span><span class="sxs-lookup"><span data-stu-id="3079a-260">No</span></span>     |    <span data-ttu-id="3079a-261">Este parâmetro deve ser usado para criar um relatório que será executado apenas uma vez.</span><span class="sxs-lookup"><span data-stu-id="3079a-261">This parameter should be used to create a report that will be executed only once.</span></span> <span data-ttu-id="3079a-262">`StartTime`, `RecurrenceInterval` e `RecurrenceCount` são ignorados se isto for verdade.</span><span class="sxs-lookup"><span data-stu-id="3079a-262">`StartTime`, `RecurrenceInterval` and `RecurrenceCount` are ignored if this is set to true.</span></span> <span data-ttu-id="3079a-263">O relatório é executado imediatamente de forma assíncronea</span><span class="sxs-lookup"><span data-stu-id="3079a-263">The report is executed immediately in an asynchronous fashion</span></span>     |    <span data-ttu-id="3079a-264">verdadeiro/falso</span><span class="sxs-lookup"><span data-stu-id="3079a-264">true/false</span></span>     |
|    <span data-ttu-id="3079a-265">Horário de ConsultaStart</span><span class="sxs-lookup"><span data-stu-id="3079a-265">QueryStartTime</span></span>     |    <span data-ttu-id="3079a-266">No</span><span class="sxs-lookup"><span data-stu-id="3079a-266">No</span></span>     |    <span data-ttu-id="3079a-267">Opcionalmente especifica a hora de início para a consulta extração dos dados.</span><span class="sxs-lookup"><span data-stu-id="3079a-267">Optionally specifies the start time for the query extracting the data.</span></span> <span data-ttu-id="3079a-268">Este parâmetro é aplicável apenas por um relatório de execução de tempo que `ExecuteNow` se definiu como verdadeiro.</span><span class="sxs-lookup"><span data-stu-id="3079a-268">This parameter is applicable only for one time execution report that have `ExecuteNow` set to true.</span></span> <span data-ttu-id="3079a-269">Definir este parâmetro sobrepõe-se a perguntas dadas `TIMESPAN` na consulta.</span><span class="sxs-lookup"><span data-stu-id="3079a-269">Setting this parameter overrides `TIMESPAN` given in the query.</span></span> <span data-ttu-id="3079a-270">O formato deve ser yyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="3079a-270">The format should be yyyy-MM-ddTHH:mm:ssZ</span></span>     |    <span data-ttu-id="3079a-271">Tempotam como corda</span><span class="sxs-lookup"><span data-stu-id="3079a-271">Timestamp as string</span></span>     |
|    <span data-ttu-id="3079a-272">ConsultaEndTime</span><span class="sxs-lookup"><span data-stu-id="3079a-272">QueryEndTime</span></span>     |    <span data-ttu-id="3079a-273">No</span><span class="sxs-lookup"><span data-stu-id="3079a-273">No</span></span>     |    <span data-ttu-id="3079a-274">Opcionalmente especifica o tempo final para a consulta extração dos dados.</span><span class="sxs-lookup"><span data-stu-id="3079a-274">Optionally specifies the end time for the query extracting the data.</span></span> <span data-ttu-id="3079a-275">Este parâmetro é aplicável apenas por um relatório de execução de tempo que `ExecuteNow` se definiu como verdadeiro.</span><span class="sxs-lookup"><span data-stu-id="3079a-275">This parameter is applicable only for one time execution report that have `ExecuteNow` set to true.</span></span> <span data-ttu-id="3079a-276">Definir este parâmetro sobrepõe-se a perguntas dadas `TIMESPAN` na consulta.</span><span class="sxs-lookup"><span data-stu-id="3079a-276">Setting this parameter overrides `TIMESPAN` given in the query.</span></span> <span data-ttu-id="3079a-277">O formato deve ser yyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="3079a-277">The format should be yyyy-MM-ddTHH:mm:ssZ</span></span>     |    <span data-ttu-id="3079a-278">Tempotam como corda</span><span class="sxs-lookup"><span data-stu-id="3079a-278">Timestamp as string</span></span>     |
|    <span data-ttu-id="3079a-279">RecorrenceInterval</span><span class="sxs-lookup"><span data-stu-id="3079a-279">RecurrenceInterval</span></span>     |    <span data-ttu-id="3079a-280">Yes</span><span class="sxs-lookup"><span data-stu-id="3079a-280">Yes</span></span>     |    <span data-ttu-id="3079a-281">Frequência em horas em que o relatório deve ser gerado.</span><span class="sxs-lookup"><span data-stu-id="3079a-281">Frequency in hours at which the report should be generated.</span></span> <br> <span data-ttu-id="3079a-282">O valor mínimo é 4 e o valor máximo é 2160.</span><span class="sxs-lookup"><span data-stu-id="3079a-282">Minimum value is 4 and Maximum value is 2160.</span></span>      |    <span data-ttu-id="3079a-283">número inteiro</span><span class="sxs-lookup"><span data-stu-id="3079a-283">integer</span></span>     |
|    <span data-ttu-id="3079a-284">RecorrenceCount</span><span class="sxs-lookup"><span data-stu-id="3079a-284">RecurrenceCount</span></span>     |    <span data-ttu-id="3079a-285">No</span><span class="sxs-lookup"><span data-stu-id="3079a-285">No</span></span>     |    <span data-ttu-id="3079a-286">Número de relatórios a serem gerados.</span><span class="sxs-lookup"><span data-stu-id="3079a-286">Number of reports to be generated.</span></span>     |    <span data-ttu-id="3079a-287">número inteiro</span><span class="sxs-lookup"><span data-stu-id="3079a-287">integer</span></span>     |
|    <span data-ttu-id="3079a-288">Formato</span><span class="sxs-lookup"><span data-stu-id="3079a-288">Format</span></span>     |    <span data-ttu-id="3079a-289">No</span><span class="sxs-lookup"><span data-stu-id="3079a-289">No</span></span>     |    <span data-ttu-id="3079a-290">Formato de ficheiro do ficheiro exportado.</span><span class="sxs-lookup"><span data-stu-id="3079a-290">File format of the exported file.</span></span> <br> <span data-ttu-id="3079a-291">O padrão é CSV.</span><span class="sxs-lookup"><span data-stu-id="3079a-291">Default is CSV.</span></span>    |    <span data-ttu-id="3079a-292">"CSV"/"TSV"</span><span class="sxs-lookup"><span data-stu-id="3079a-292">"CSV"/"TSV"</span></span>     |
|    <span data-ttu-id="3079a-293">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="3079a-293">CallbackUrl</span></span>     |    <span data-ttu-id="3079a-294">No</span><span class="sxs-lookup"><span data-stu-id="3079a-294">No</span></span>     |    <span data-ttu-id="3079a-295">URL acessível publicamente que pode ser configurado opcionalmente como destino de retorno</span><span class="sxs-lookup"><span data-stu-id="3079a-295">Publicly reachable URL that can be optionally configured as callback destination</span></span>     |    <span data-ttu-id="3079a-296">String (http URL)</span><span class="sxs-lookup"><span data-stu-id="3079a-296">String (http URL)</span></span>     |
|    <span data-ttu-id="3079a-297">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="3079a-297">CallbackMethod</span></span>     |    <span data-ttu-id="3079a-298">No</span><span class="sxs-lookup"><span data-stu-id="3079a-298">No</span></span>     |    <span data-ttu-id="3079a-299">O método a ser usado para o retorno</span><span class="sxs-lookup"><span data-stu-id="3079a-299">The method to be used for callback</span></span>     |    <span data-ttu-id="3079a-300">GET/POST</span><span class="sxs-lookup"><span data-stu-id="3079a-300">GET/POST</span></span>     |
|        |        |        |        |

### <a name="sample-response"></a><span data-ttu-id="3079a-301">Resposta de amostra</span><span class="sxs-lookup"><span data-stu-id="3079a-301">Sample response</span></span>

<span data-ttu-id="3079a-302">A carga útil de resposta é estruturada da seguinte forma:</span><span class="sxs-lookup"><span data-stu-id="3079a-302">The response payload is structured as follows:</span></span>

<span data-ttu-id="3079a-303">Códigos de Resposta: 200, 400, 401, 403, 404,500</span><span class="sxs-lookup"><span data-stu-id="3079a-303">Response Codes: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="3079a-304">Exemplo de carga útil de resposta:</span><span class="sxs-lookup"><span data-stu-id="3079a-304">Response payload example:</span></span>

```json
{ 
  "value": [
    { 
      "reportId": "d9548477-16d4-492a-bf9c-0cf91a9f69bf", 
      "reportName": "Top10_CustomersReport", 
      "description": "Top 10 customers by revenue for last month", 
      "queryId": "ec8366a4-d96e-4194-8c37-d5dbc0639033", 
      "query": "SELECT CustomerName, Product, BilledRevenueUSD FROM CustomersAndTenants ORDER BY BilledRevenueUSD LIMIT 10 TIMESPAN LAST_MONTH", 
      "user": "GAUser@PITEST2.ccsctp.net", 
      "createdTime": "2021-03-30T13:11:58Z", 
      "modifiedTime": null, 
      "executeNow": false, 
      "startTime": "2021-03-31T18:41:00Z", 
      "reportStatus": "Active", 
      "recurrenceInterval": 24, 
      "recurrenceCount": 100, 
      "callbackUrl": "https://<SampleCallbackUrl>", 
      "callbackMethod": "GET", 
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

### <a name="glossary"></a><span data-ttu-id="3079a-305">Glossário</span><span class="sxs-lookup"><span data-stu-id="3079a-305">Glossary</span></span>

<span data-ttu-id="3079a-306">As definições-chave dos elementos na resposta são articuladas abaixo:</span><span class="sxs-lookup"><span data-stu-id="3079a-306">Key definitions of elements in the response are articulated below:</span></span>

|    <span data-ttu-id="3079a-307">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="3079a-307">Parameter</span></span>     |    <span data-ttu-id="3079a-308">Descrição</span><span class="sxs-lookup"><span data-stu-id="3079a-308">Description</span></span>     |
|    ----    |    ----    |
|    <span data-ttu-id="3079a-309">ReportId</span><span class="sxs-lookup"><span data-stu-id="3079a-309">ReportId</span></span>     |    <span data-ttu-id="3079a-310">Identificador universalmente único (UUID) do relatório que criou</span><span class="sxs-lookup"><span data-stu-id="3079a-310">Universally unique identifier (UUID) of the report you created</span></span>     |
|    <span data-ttu-id="3079a-311">Nome do relatório</span><span class="sxs-lookup"><span data-stu-id="3079a-311">ReportName</span></span>     |    <span data-ttu-id="3079a-312">Nome dado ao relatório na carga útil do pedido</span><span class="sxs-lookup"><span data-stu-id="3079a-312">Name given to the report in the request payload</span></span>     |
|    <span data-ttu-id="3079a-313">Descrição</span><span class="sxs-lookup"><span data-stu-id="3079a-313">Description</span></span>     |    <span data-ttu-id="3079a-314">Descrição dada durante a criação do relatório</span><span class="sxs-lookup"><span data-stu-id="3079a-314">Description given during creation of the report</span></span>     |
|    <span data-ttu-id="3079a-315">QueryId</span><span class="sxs-lookup"><span data-stu-id="3079a-315">QueryId</span></span>     |    <span data-ttu-id="3079a-316">Consulta ID passou no momento em que criou o relatório</span><span class="sxs-lookup"><span data-stu-id="3079a-316">Query ID passed at the time you created the report</span></span>     |
|    <span data-ttu-id="3079a-317">Consulta</span><span class="sxs-lookup"><span data-stu-id="3079a-317">Query</span></span>     |    <span data-ttu-id="3079a-318">Texto de consulta que será executado para este relatório</span><span class="sxs-lookup"><span data-stu-id="3079a-318">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="3079a-319">Utilizador</span><span class="sxs-lookup"><span data-stu-id="3079a-319">User</span></span>     |    <span data-ttu-id="3079a-320">ID do utilizador usado para criar o relatório</span><span class="sxs-lookup"><span data-stu-id="3079a-320">User ID used to create the report</span></span>     |
|    <span data-ttu-id="3079a-321">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="3079a-321">CreatedTime</span></span>     |    <span data-ttu-id="3079a-322">TEMPO UTC O relatório foi criado neste formato: yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="3079a-322">UTC Time the report was created in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="3079a-323">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="3079a-323">ModifiedTime</span></span>     |    <span data-ttu-id="3079a-324">UTC Tempo o relatório foi modificado pela última vez neste formato: yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="3079a-324">UTC Time the report was last modified in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="3079a-325">Executar Agora</span><span class="sxs-lookup"><span data-stu-id="3079a-325">ExecuteNow</span></span>     |    <span data-ttu-id="3079a-326">`ExecuteNow` bandeira definida no momento em que o relatório foi criado</span><span class="sxs-lookup"><span data-stu-id="3079a-326">`ExecuteNow` flag set at the time the report was created</span></span>     |
|    <span data-ttu-id="3079a-327">StartTime</span><span class="sxs-lookup"><span data-stu-id="3079a-327">StartTime</span></span>     |    <span data-ttu-id="3079a-328">UTC Tempo a execução do relatório começará neste formato: yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="3079a-328">UTC Time the report execution will begin in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="3079a-329">Relatório Estatísticas</span><span class="sxs-lookup"><span data-stu-id="3079a-329">ReportStatus</span></span>     |    <span data-ttu-id="3079a-330">Estado da execução do relatório.</span><span class="sxs-lookup"><span data-stu-id="3079a-330">Status of the report execution.</span></span> <span data-ttu-id="3079a-331">Os valores possíveis `Paused` `Active` são, e `Inactive`</span><span class="sxs-lookup"><span data-stu-id="3079a-331">The possible values are `Paused`, `Active`, and `Inactive`</span></span>     |
|    <span data-ttu-id="3079a-332">RecorrenceInterval</span><span class="sxs-lookup"><span data-stu-id="3079a-332">RecurrenceInterval</span></span>     |    <span data-ttu-id="3079a-333">Intervalo de recorrência fornecido durante a criação do relatório</span><span class="sxs-lookup"><span data-stu-id="3079a-333">Recurrence interval provided during report creation</span></span>     |
|    <span data-ttu-id="3079a-334">RecorrenceCount</span><span class="sxs-lookup"><span data-stu-id="3079a-334">RecurrenceCount</span></span>     |    <span data-ttu-id="3079a-335">Contagem de recorrência fornecida durante a criação do relatório.</span><span class="sxs-lookup"><span data-stu-id="3079a-335">Recurrence count provided during report creation.</span></span>      |
|    <span data-ttu-id="3079a-336">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="3079a-336">CallbackUrl</span></span>     |    <span data-ttu-id="3079a-337">URL de retorno fornecido no pedido</span><span class="sxs-lookup"><span data-stu-id="3079a-337">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="3079a-338">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="3079a-338">CallbackMethod</span></span>     |    <span data-ttu-id="3079a-339">Método de retorno fornecido no pedido</span><span class="sxs-lookup"><span data-stu-id="3079a-339">Callback method provided in the request</span></span>     |
|    <span data-ttu-id="3079a-340">Formato</span><span class="sxs-lookup"><span data-stu-id="3079a-340">Format</span></span>     |    <span data-ttu-id="3079a-341">Formato dos ficheiros do relatório.</span><span class="sxs-lookup"><span data-stu-id="3079a-341">Format of the report files.</span></span> <span data-ttu-id="3079a-342">Os valores possíveis são `CSV` ou `TSV` .</span><span class="sxs-lookup"><span data-stu-id="3079a-342">The possible values are `CSV` or `TSV`.</span></span>     |
|    <span data-ttu-id="3079a-343">TotalCount</span><span class="sxs-lookup"><span data-stu-id="3079a-343">TotalCount</span></span>     |    <span data-ttu-id="3079a-344">Número de registos na matriz de valor</span><span class="sxs-lookup"><span data-stu-id="3079a-344">Number of records in the Value array</span></span>     |
|    <span data-ttu-id="3079a-345">Código de Estado</span><span class="sxs-lookup"><span data-stu-id="3079a-345">StatusCode</span></span>     |    <span data-ttu-id="3079a-346">Código do Resultado</span><span class="sxs-lookup"><span data-stu-id="3079a-346">Result Code</span></span>     |
|    <span data-ttu-id="3079a-347">message</span><span class="sxs-lookup"><span data-stu-id="3079a-347">message</span></span>     |    <span data-ttu-id="3079a-348">Os valores possíveis são 200, 400, 401, 403, 500.</span><span class="sxs-lookup"><span data-stu-id="3079a-348">The possible values are 200, 400, 401, 403, 500.</span></span> <span data-ttu-id="3079a-349">Mensagem de estado da execução da API</span><span class="sxs-lookup"><span data-stu-id="3079a-349">Status message from the execution of the API</span></span>     |
|        |        |

## <a name="get-report-execution-api"></a><span data-ttu-id="3079a-350">Obtenha relatório execução API</span><span class="sxs-lookup"><span data-stu-id="3079a-350">Get report execution API</span></span>

<span data-ttu-id="3079a-351">Pode utilizar este método para consultar o estado de execução de um relatório utilizando o RelatórioId recebido da API do [Relatório de Criação](#create-report-api).</span><span class="sxs-lookup"><span data-stu-id="3079a-351">You can use this method to query the status of a report execution using the ReportId received from [Create Report API](#create-report-api).</span></span> <span data-ttu-id="3079a-352">O método devolve o link de descarregamento do relatório se o relatório estiver pronto para download.</span><span class="sxs-lookup"><span data-stu-id="3079a-352">The method returns the report download link if the report is ready for download.</span></span> <span data-ttu-id="3079a-353">Caso contrário, o método devolve o estado.</span><span class="sxs-lookup"><span data-stu-id="3079a-353">Otherwise, the method returns the status.</span></span> <span data-ttu-id="3079a-354">Você também pode usar esta API para obter todas as execuções que aconteceram para um dado relatório.</span><span class="sxs-lookup"><span data-stu-id="3079a-354">You can also use this API to get all the executions that have happened for a given report.</span></span>  

>[!IMPORTANT]
><span data-ttu-id="3079a-355">Esta API tem parâmetros de consulta predefinidos definidos para `executionStatus=Completed` e `getLatestExecution=true` .</span><span class="sxs-lookup"><span data-stu-id="3079a-355">This API has default query parameters set for `executionStatus=Completed` and `getLatestExecution=true`.</span></span> <span data-ttu-id="3079a-356">Por isso, chamar a API antes da primeira execução bem sucedida do relatório devolverá 404.</span><span class="sxs-lookup"><span data-stu-id="3079a-356">Hence, calling the API before the first successful execution of the report will return 404.</span></span> <span data-ttu-id="3079a-357">Execuções pendentes podem ser obtidas por definição `executionStatus=Pending` .</span><span class="sxs-lookup"><span data-stu-id="3079a-357">Pending executions can be obtained by setting `executionStatus=Pending`.</span></span>

### <a name="request-syntax"></a><span data-ttu-id="3079a-358">Solicitar sintaxe</span><span class="sxs-lookup"><span data-stu-id="3079a-358">Request syntax</span></span>

|    <span data-ttu-id="3079a-359">Método</span><span class="sxs-lookup"><span data-stu-id="3079a-359">Method</span></span>     |    <span data-ttu-id="3079a-360">URI do pedido</span><span class="sxs-lookup"><span data-stu-id="3079a-360">Request URI</span></span>     |
|----- | -----|
|    <span data-ttu-id="3079a-361">GET</span><span class="sxs-lookup"><span data-stu-id="3079a-361">GET</span></span>    |`https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/execution/{reportId}?executionId={executionId}&executionStatus={executionStatus}&getLatestExecution={getLatestExecution}`  |

### <a name="request-header"></a><span data-ttu-id="3079a-362">Cabeçalho do pedido</span><span class="sxs-lookup"><span data-stu-id="3079a-362">Request header</span></span>

|    <span data-ttu-id="3079a-363">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3079a-363">Header</span></span>     |    <span data-ttu-id="3079a-364">Tipo</span><span class="sxs-lookup"><span data-stu-id="3079a-364">Type</span></span>     |    <span data-ttu-id="3079a-365">Descrição</span><span class="sxs-lookup"><span data-stu-id="3079a-365">Description</span></span>     |
|-------|-----|------|
|    <span data-ttu-id="3079a-366">Autorização</span><span class="sxs-lookup"><span data-stu-id="3079a-366">Authorization</span></span>     |    <span data-ttu-id="3079a-367">string</span><span class="sxs-lookup"><span data-stu-id="3079a-367">string</span></span> |<span data-ttu-id="3079a-368">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3079a-368">Required.</span></span> <span data-ttu-id="3079a-369">O Azure Ative Directory (Azure AD) de acesso.</span><span class="sxs-lookup"><span data-stu-id="3079a-369">The Azure Active Directory (Azure AD) access token.</span></span> <span data-ttu-id="3079a-370">O formato é  `Bearer <token>` .</span><span class="sxs-lookup"><span data-stu-id="3079a-370">The format is `Bearer <token>`.</span></span>|
|    <span data-ttu-id="3079a-371">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3079a-371">Content-Type</span></span>     |<span data-ttu-id="3079a-372">string</span><span class="sxs-lookup"><span data-stu-id="3079a-372">string</span></span> |`Application/JSON` |

### <a name="path-parameter"></a><span data-ttu-id="3079a-373">Parâmetro do caminho</span><span class="sxs-lookup"><span data-stu-id="3079a-373">Path parameter</span></span>

|    <span data-ttu-id="3079a-374">Nome do Parâmetro</span><span class="sxs-lookup"><span data-stu-id="3079a-374">Parameter Name</span></span>    |    <span data-ttu-id="3079a-375">Necessário</span><span class="sxs-lookup"><span data-stu-id="3079a-375">Required</span></span>    |    <span data-ttu-id="3079a-376">Tipo</span><span class="sxs-lookup"><span data-stu-id="3079a-376">Type</span></span>    |    <span data-ttu-id="3079a-377">Descrição</span><span class="sxs-lookup"><span data-stu-id="3079a-377">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="3079a-378">reportId</span><span class="sxs-lookup"><span data-stu-id="3079a-378">reportId</span></span>    |    <span data-ttu-id="3079a-379">Yes</span><span class="sxs-lookup"><span data-stu-id="3079a-379">Yes</span></span>    |    <span data-ttu-id="3079a-380">string</span><span class="sxs-lookup"><span data-stu-id="3079a-380">string</span></span>    |    <span data-ttu-id="3079a-381">Filtrar para obter detalhes de execução de apenas relatórios com o relatório Dado neste argumento.</span><span class="sxs-lookup"><span data-stu-id="3079a-381">Filter to get execution details of only reports with the reportId given in this argument.</span></span> <span data-ttu-id="3079a-382">Vários reportIds podem ser especificados separando-os com um ponto e vírgula ";".</span><span class="sxs-lookup"><span data-stu-id="3079a-382">Multiple reportIds can be specified by separating them with a semicolon ";".</span></span>    |
|        |        |        |        |

### <a name="query-parameter"></a><span data-ttu-id="3079a-383">Parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="3079a-383">Query parameter</span></span>

|    <span data-ttu-id="3079a-384">Nome do Parâmetro</span><span class="sxs-lookup"><span data-stu-id="3079a-384">Parameter Name</span></span>    |    <span data-ttu-id="3079a-385">Necessário</span><span class="sxs-lookup"><span data-stu-id="3079a-385">Required</span></span>    |    <span data-ttu-id="3079a-386">Tipo</span><span class="sxs-lookup"><span data-stu-id="3079a-386">Type</span></span>    |    <span data-ttu-id="3079a-387">Descrição</span><span class="sxs-lookup"><span data-stu-id="3079a-387">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="3079a-388">execuçãoId</span><span class="sxs-lookup"><span data-stu-id="3079a-388">executionId</span></span>    |    <span data-ttu-id="3079a-389">No</span><span class="sxs-lookup"><span data-stu-id="3079a-389">No</span></span>    |    <span data-ttu-id="3079a-390">string</span><span class="sxs-lookup"><span data-stu-id="3079a-390">string</span></span>    |    <span data-ttu-id="3079a-391">Filtre para obter detalhes de apenas relatórios com a execuçãoId dado neste argumento.</span><span class="sxs-lookup"><span data-stu-id="3079a-391">Filter to get details of only reports with the executionId given in this argument.</span></span> <span data-ttu-id="3079a-392">Execuções múltiplas podem ser especificadas separando-as com um ponto e vírgula ";".</span><span class="sxs-lookup"><span data-stu-id="3079a-392">Multiple executionIds can be specified by separating them with a semicolon ";".</span></span>    |
|    <span data-ttu-id="3079a-393">execuçãoStatus</span><span class="sxs-lookup"><span data-stu-id="3079a-393">executionStatus</span></span>    |    <span data-ttu-id="3079a-394">No</span><span class="sxs-lookup"><span data-stu-id="3079a-394">No</span></span>    |    <span data-ttu-id="3079a-395">Corda/enum</span><span class="sxs-lookup"><span data-stu-id="3079a-395">String/enum</span></span>    |    <span data-ttu-id="3079a-396">Filtre para obter detalhes de apenas relatórios com a execuçãoStatus dada neste argumento.</span><span class="sxs-lookup"><span data-stu-id="3079a-396">Filter to get details of only reports with the executionStatus given in this argument.</span></span> <br> <span data-ttu-id="3079a-397">Os valores válidos são: `Pending` `Running` `Paused` `Completed` e.</span><span class="sxs-lookup"><span data-stu-id="3079a-397">Valid values are: `Pending`, `Running`, `Paused` and `Completed`.</span></span> <br> <span data-ttu-id="3079a-398">O valor predefinido é `Completed`.</span><span class="sxs-lookup"><span data-stu-id="3079a-398">The default value is `Completed`.</span></span> <br> <span data-ttu-id="3079a-399">Vários estados podem ser especificados separando-os com um ponto e vírgula ";".</span><span class="sxs-lookup"><span data-stu-id="3079a-399">Multiple statuses can be specified by separating them with a semicolon ";".</span></span>    |
|    <span data-ttu-id="3079a-400">obterExecução de Pré-executivos</span><span class="sxs-lookup"><span data-stu-id="3079a-400">getLatestExecution</span></span>    |    <span data-ttu-id="3079a-401">No</span><span class="sxs-lookup"><span data-stu-id="3079a-401">No</span></span>    |    <span data-ttu-id="3079a-402">boolean</span><span class="sxs-lookup"><span data-stu-id="3079a-402">boolean</span></span>    |    <span data-ttu-id="3079a-403">A API devolverá detalhes da última execução.</span><span class="sxs-lookup"><span data-stu-id="3079a-403">The API will return details of the latest execution.</span></span> <span data-ttu-id="3079a-404">Por padrão, este parâmetro é definido como verdadeiro.</span><span class="sxs-lookup"><span data-stu-id="3079a-404">By default, this parameter is set to true.</span></span><br> <span data-ttu-id="3079a-405">Se optar por passar o valor deste parâmetro como falso, então a API devolverá os últimos 90 dias de execução.</span><span class="sxs-lookup"><span data-stu-id="3079a-405">If you choose to pass the value of this parameter as false, then the API will return the last 90 days execution instances.</span></span>    |
|        |        |        |        |

### <a name="sample-request-payload"></a><span data-ttu-id="3079a-406">Carga de pedido de amostra</span><span class="sxs-lookup"><span data-stu-id="3079a-406">Sample Request Payload</span></span>

<span data-ttu-id="3079a-407">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="3079a-407">None</span></span>

### <a name="sample-response"></a><span data-ttu-id="3079a-408">Resposta de Amostra</span><span class="sxs-lookup"><span data-stu-id="3079a-408">Sample Response</span></span>

<span data-ttu-id="3079a-409">A carga útil de resposta é estruturada da seguinte forma:</span><span class="sxs-lookup"><span data-stu-id="3079a-409">The response payload is structured as follows:</span></span>

<span data-ttu-id="3079a-410">Códigos de Resposta: 200, 400, 401, 403, 404,500</span><span class="sxs-lookup"><span data-stu-id="3079a-410">Response Codes: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="3079a-411">Exemplo de carga útil de resposta:</span><span class="sxs-lookup"><span data-stu-id="3079a-411">Response payload example:</span></span>

```json
{
  "value": [
    {
      "executionId": "906931dc-4f2f-4195-bbb2-d7295c7550d3",
      "reportId": "d9548477-16d4-492a-bf9c-0cf91a9f69bf",
      "recurrenceInterval": 24,
      "recurrenceCount": 100,
      "callbackUrl": null,
      "callbackMethod": null,
      "format": "csv",
      "executionStatus": "Completed",
      "reportLocation": null,
      "reportAccessSecureLink": "https://<path to report for download>",
      "reportExpiryTime": null,
      "reportGeneratedTime": "2021-03-31T18:41:00Z"
    }
  ],
  "nextLink": null,
  "totalCount": 1,
  "message": null,
  "statusCode": 200,
  "dataRedacted": false
}
```

<span data-ttu-id="3079a-412">Uma vez concluída a execução do relatório, o estado de execução `Completed` é mostrado.</span><span class="sxs-lookup"><span data-stu-id="3079a-412">Once report execution is complete, the execution status `Completed` is shown.</span></span> <span data-ttu-id="3079a-413">Pode descarregar o relatório selecionando o URL no `reportAccessSecureLink` .</span><span class="sxs-lookup"><span data-stu-id="3079a-413">You can download the report by selecting the URL in the `reportAccessSecureLink`.</span></span>

### <a name="glossary"></a><span data-ttu-id="3079a-414">Glossário</span><span class="sxs-lookup"><span data-stu-id="3079a-414">Glossary</span></span>

<span data-ttu-id="3079a-415">Definições-chave de elementos na resposta.</span><span class="sxs-lookup"><span data-stu-id="3079a-415">Key definitions of elements in the response.</span></span>

|    <span data-ttu-id="3079a-416">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="3079a-416">Parameter</span></span>    |    <span data-ttu-id="3079a-417">Descrição</span><span class="sxs-lookup"><span data-stu-id="3079a-417">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="3079a-418">ExecuçãoId</span><span class="sxs-lookup"><span data-stu-id="3079a-418">ExecutionId</span></span>    |    <span data-ttu-id="3079a-419">Identificador universalmente único (UUID) da instância de execução</span><span class="sxs-lookup"><span data-stu-id="3079a-419">Universally unique identifier (UUID) of the execution instance</span></span>    |
|    <span data-ttu-id="3079a-420">ReportId</span><span class="sxs-lookup"><span data-stu-id="3079a-420">ReportId</span></span>    |    <span data-ttu-id="3079a-421">ID do relatório associado à instância de execução</span><span class="sxs-lookup"><span data-stu-id="3079a-421">Report ID associated with the execution instance</span></span>    |
|    <span data-ttu-id="3079a-422">RecorrenceInterval</span><span class="sxs-lookup"><span data-stu-id="3079a-422">RecurrenceInterval</span></span>    |    <span data-ttu-id="3079a-423">Intervalo de recorrência fornecido durante a criação do relatório</span><span class="sxs-lookup"><span data-stu-id="3079a-423">Recurrence interval provided during report creation</span></span>    |
|    <span data-ttu-id="3079a-424">RecorrenceCount</span><span class="sxs-lookup"><span data-stu-id="3079a-424">RecurrenceCount</span></span>    |    <span data-ttu-id="3079a-425">Contagem de recorrência fornecida durante a criação do relatório</span><span class="sxs-lookup"><span data-stu-id="3079a-425">Recurrence count provided during report creation</span></span>    |
|    <span data-ttu-id="3079a-426">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="3079a-426">CallbackUrl</span></span>    |    <span data-ttu-id="3079a-427">URL de retorno associado à instância de execução</span><span class="sxs-lookup"><span data-stu-id="3079a-427">Callback URL associated with the execution instance</span></span>    |
|    <span data-ttu-id="3079a-428">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="3079a-428">CallbackMethod</span></span>    |    <span data-ttu-id="3079a-429">Método de retorno associado à instância de execução</span><span class="sxs-lookup"><span data-stu-id="3079a-429">Callback method associated with the execution instance</span></span>    |
|    <span data-ttu-id="3079a-430">Formato</span><span class="sxs-lookup"><span data-stu-id="3079a-430">Format</span></span>    |    <span data-ttu-id="3079a-431">Formato do ficheiro gerado no final da execução</span><span class="sxs-lookup"><span data-stu-id="3079a-431">Format of the generated file at the end of execution</span></span>    |
|    <span data-ttu-id="3079a-432">ExecuçãoStatus</span><span class="sxs-lookup"><span data-stu-id="3079a-432">ExecutionStatus</span></span>    |    <span data-ttu-id="3079a-433">Estado da instância de execução do relatório.</span><span class="sxs-lookup"><span data-stu-id="3079a-433">Status of the report execution instance.</span></span> <br> <span data-ttu-id="3079a-434">Valores válidos são: `Pending` `Running` , e `Paused``Completed`</span><span class="sxs-lookup"><span data-stu-id="3079a-434">Valid values are: `Pending`, `Running`, `Paused`, and `Completed`</span></span>    |
|    <span data-ttu-id="3079a-435">ReportAccessSecureLink</span><span class="sxs-lookup"><span data-stu-id="3079a-435">ReportAccessSecureLink</span></span>    |<span data-ttu-id="3079a-436">Link através do qual o relatório pode ser acedido de forma segura</span><span class="sxs-lookup"><span data-stu-id="3079a-436">Link through which the report can be accessed securely</span></span>        |
|    <span data-ttu-id="3079a-437">ReportExpiryTime</span><span class="sxs-lookup"><span data-stu-id="3079a-437">ReportExpiryTime</span></span>    |    <span data-ttu-id="3079a-438">Tempo UTC após o qual a ligação de relatório expirará neste formato: yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="3079a-438">UTC Time after which the report link will expire in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>    |
|    <span data-ttu-id="3079a-439">ReportGeneratedTime</span><span class="sxs-lookup"><span data-stu-id="3079a-439">ReportGeneratedTime</span></span>    |    <span data-ttu-id="3079a-440">Tempo UTC em que o relatório foi gerado neste formato: yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="3079a-440">UTC Time at which the report was generated in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>    |
|    <span data-ttu-id="3079a-441">TotalCount</span><span class="sxs-lookup"><span data-stu-id="3079a-441">TotalCount</span></span>    |    <span data-ttu-id="3079a-442">Número de conjuntos de dados na matriz de valor</span><span class="sxs-lookup"><span data-stu-id="3079a-442">Number of datasets in the Value array</span></span>    |
|    <span data-ttu-id="3079a-443">Código de Estado</span><span class="sxs-lookup"><span data-stu-id="3079a-443">StatusCode</span></span>    |    <span data-ttu-id="3079a-444">Código do Resultado</span><span class="sxs-lookup"><span data-stu-id="3079a-444">Result Code</span></span> <br> <span data-ttu-id="3079a-445">Os valores possíveis são 200, 400, 401, 403, 404 e 500</span><span class="sxs-lookup"><span data-stu-id="3079a-445">The possible values are 200, 400, 401, 403, 404 and 500</span></span>    |
|    <span data-ttu-id="3079a-446">message</span><span class="sxs-lookup"><span data-stu-id="3079a-446">message</span></span>    |    <span data-ttu-id="3079a-447">Mensagem de estado da execução da API</span><span class="sxs-lookup"><span data-stu-id="3079a-447">Status message from the execution of the API</span></span>    |
|        |        |

## <a name="next-steps"></a><span data-ttu-id="3079a-448">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="3079a-448">Next steps</span></span>

- <span data-ttu-id="3079a-449">Experimente as APIs através do [URL da API](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html)</span><span class="sxs-lookup"><span data-stu-id="3079a-449">Try out the APIs through the [swagger API URL](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html)</span></span>
- [<span data-ttu-id="3079a-450">Faça a sua primeira chamada API</span><span class="sxs-lookup"><span data-stu-id="3079a-450">Make your first API call</span></span>](insights-programmatic-first-api-call.md)