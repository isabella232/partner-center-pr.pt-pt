---
title: Obtenha consultas de relatório API - dados Informações
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Utilize esta API para obter todas as consultas disponíveis para uso no relatório API.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 3bf140576a19439990405cfef23190045e0a98be
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/16/2021
ms.locfileid: "114377205"
---
# <a name="get-report-queries-api"></a><span data-ttu-id="6a3fb-103">Obtenha consultas de relatório API</span><span class="sxs-lookup"><span data-stu-id="6a3fb-103">Get report queries API</span></span>

<span data-ttu-id="6a3fb-104">O relatório Get consultas API obtém todas as consultas que estão disponíveis para uso em relatórios.</span><span class="sxs-lookup"><span data-stu-id="6a3fb-104">The Get report queries API gets all the queries that are available for use in reports.</span></span> <span data-ttu-id="6a3fb-105">Obtém todo o sistema e consultas definidas pelo utilizador por padrão.</span><span class="sxs-lookup"><span data-stu-id="6a3fb-105">It gets all the system and user-defined queries by default.</span></span>

<span data-ttu-id="6a3fb-106">**Solicitar sintaxe**</span><span class="sxs-lookup"><span data-stu-id="6a3fb-106">**Request syntax**</span></span>

|    <span data-ttu-id="6a3fb-107">Método</span><span class="sxs-lookup"><span data-stu-id="6a3fb-107">Method</span></span>    |    <span data-ttu-id="6a3fb-108">URI do pedido</span><span class="sxs-lookup"><span data-stu-id="6a3fb-108">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="6a3fb-109">GET</span><span class="sxs-lookup"><span data-stu-id="6a3fb-109">GET</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries?queryId={QueryID}&queryName={QueryName}&includeSystemQueries={include_system_queries}&includeOnlySystemQueries={include_only_system_queries}`     |
|        |        |

<span data-ttu-id="6a3fb-110">**Cabeçalho de pedido**</span><span class="sxs-lookup"><span data-stu-id="6a3fb-110">**Request header**</span></span>

|    <span data-ttu-id="6a3fb-111">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6a3fb-111">Header</span></span>    |    <span data-ttu-id="6a3fb-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="6a3fb-112">Type</span></span>    |    <span data-ttu-id="6a3fb-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a3fb-113">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="6a3fb-114">Autorização</span><span class="sxs-lookup"><span data-stu-id="6a3fb-114">Authorization</span></span>    |    <span data-ttu-id="6a3fb-115">string</span><span class="sxs-lookup"><span data-stu-id="6a3fb-115">string</span></span>    |    <span data-ttu-id="6a3fb-116">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6a3fb-116">Required.</span></span> <span data-ttu-id="6a3fb-117">O Azure Ative Directory (AAD) símbolo de acesso na forma`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="6a3fb-117">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="6a3fb-118">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6a3fb-118">Content-Type</span></span>    |    <span data-ttu-id="6a3fb-119">string</span><span class="sxs-lookup"><span data-stu-id="6a3fb-119">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="6a3fb-120">**Parâmetro do caminho**</span><span class="sxs-lookup"><span data-stu-id="6a3fb-120">**Path parameter**</span></span>

<span data-ttu-id="6a3fb-121">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="6a3fb-121">None</span></span>

<span data-ttu-id="6a3fb-122">**Parâmetro de consulta**</span><span class="sxs-lookup"><span data-stu-id="6a3fb-122">**Query parameter**</span></span>

|    <span data-ttu-id="6a3fb-123">Nome do Parâmetro</span><span class="sxs-lookup"><span data-stu-id="6a3fb-123">Parameter Name</span></span>    |    <span data-ttu-id="6a3fb-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="6a3fb-124">Type</span></span>    |    <span data-ttu-id="6a3fb-125">Necessário</span><span class="sxs-lookup"><span data-stu-id="6a3fb-125">Required</span></span>    |    <span data-ttu-id="6a3fb-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a3fb-126">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="6a3fb-127">consultaD</span><span class="sxs-lookup"><span data-stu-id="6a3fb-127">queryId</span></span>     |    <span data-ttu-id="6a3fb-128">cadeia (de carateres)</span><span class="sxs-lookup"><span data-stu-id="6a3fb-128">string</span></span>     |    <span data-ttu-id="6a3fb-129">No</span><span class="sxs-lookup"><span data-stu-id="6a3fb-129">No</span></span>    |    <span data-ttu-id="6a3fb-130">Filtrar para obter detalhes de apenas consultas com o ID dado no argumento</span><span class="sxs-lookup"><span data-stu-id="6a3fb-130">Filter to get details of only queries with the ID given in the argument</span></span>     |
|    <span data-ttu-id="6a3fb-131">consultaName</span><span class="sxs-lookup"><span data-stu-id="6a3fb-131">queryName</span></span>     |    <span data-ttu-id="6a3fb-132">cadeia (de carateres)</span><span class="sxs-lookup"><span data-stu-id="6a3fb-132">string</span></span>     |    <span data-ttu-id="6a3fb-133">No</span><span class="sxs-lookup"><span data-stu-id="6a3fb-133">No</span></span>    |    <span data-ttu-id="6a3fb-134">Filtrar para obter detalhes de apenas consultas com o nome dado no argumento</span><span class="sxs-lookup"><span data-stu-id="6a3fb-134">Filter to get details of only queries with the name given in the argument</span></span>     |
|    <span data-ttu-id="6a3fb-135">Incluir Sistemaqueries</span><span class="sxs-lookup"><span data-stu-id="6a3fb-135">IncludeSystemQueries</span></span>     |    <span data-ttu-id="6a3fb-136">boolean</span><span class="sxs-lookup"><span data-stu-id="6a3fb-136">boolean</span></span>     |    <span data-ttu-id="6a3fb-137">No</span><span class="sxs-lookup"><span data-stu-id="6a3fb-137">No</span></span>    |    <span data-ttu-id="6a3fb-138">Incluir consultas de sistema predefinidas na resposta</span><span class="sxs-lookup"><span data-stu-id="6a3fb-138">Include predefined system queries in the response</span></span>     |
|    <span data-ttu-id="6a3fb-139">Incluir Apenas SistemasQueries</span><span class="sxs-lookup"><span data-stu-id="6a3fb-139">IncludeOnlySystemQueries</span></span>     |    <span data-ttu-id="6a3fb-140">boolean</span><span class="sxs-lookup"><span data-stu-id="6a3fb-140">boolean</span></span>     |    <span data-ttu-id="6a3fb-141">No</span><span class="sxs-lookup"><span data-stu-id="6a3fb-141">No</span></span>    |    <span data-ttu-id="6a3fb-142">Incluir apenas consultas de sistema na resposta</span><span class="sxs-lookup"><span data-stu-id="6a3fb-142">Include only system queries in the response</span></span>     |
|        |        |        |        |


<span data-ttu-id="6a3fb-143">**Solicitar carga útil**</span><span class="sxs-lookup"><span data-stu-id="6a3fb-143">**Request payload**</span></span>

<span data-ttu-id="6a3fb-144">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="6a3fb-144">None</span></span>

<span data-ttu-id="6a3fb-145">**Glossário**</span><span class="sxs-lookup"><span data-stu-id="6a3fb-145">**Glossary**</span></span>

<span data-ttu-id="6a3fb-146">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="6a3fb-146">None</span></span>

<span data-ttu-id="6a3fb-147">**Response**</span><span class="sxs-lookup"><span data-stu-id="6a3fb-147">**Response**</span></span>

<span data-ttu-id="6a3fb-148">A carga útil de resposta é estruturada da seguinte forma:</span><span class="sxs-lookup"><span data-stu-id="6a3fb-148">The response payload is structured as follows:</span></span>

<span data-ttu-id="6a3fb-149">Código de resposta: 200, 400, 401, 403, 404,500</span><span class="sxs-lookup"><span data-stu-id="6a3fb-149">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="6a3fb-150">Exemplo de carga útil de resposta:</span><span class="sxs-lookup"><span data-stu-id="6a3fb-150">Response payload example:</span></span>

```json
{ 
  "Value": [ 
    { 
      "QueryId": "string", 
      "Name": "string", 
      "Description": "string", 
      "Query": "string", 
      "Type": "string", 
      "User": "string", 
      "CreatedTime": "string", 
    } 
  ], 
  "TotalCount": 0, 
  "Message": "string", 
  "StatusCode": 0, 
} 
```

<span data-ttu-id="6a3fb-151">**Glossário**</span><span class="sxs-lookup"><span data-stu-id="6a3fb-151">**Glossary**</span></span>

<span data-ttu-id="6a3fb-152">Esta tabela define os elementos-chave na resposta:</span><span class="sxs-lookup"><span data-stu-id="6a3fb-152">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="6a3fb-153">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="6a3fb-153">Parameter</span></span>    |    <span data-ttu-id="6a3fb-154">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a3fb-154">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="6a3fb-155">QueryId</span><span class="sxs-lookup"><span data-stu-id="6a3fb-155">QueryId</span></span>     |    <span data-ttu-id="6a3fb-156">UUID único da consulta</span><span class="sxs-lookup"><span data-stu-id="6a3fb-156">Unique UUID of the query</span></span>     |
|    <span data-ttu-id="6a3fb-157">Name</span><span class="sxs-lookup"><span data-stu-id="6a3fb-157">Name</span></span>     |    <span data-ttu-id="6a3fb-158">Nome dado à consulta no momento da criação de consultas</span><span class="sxs-lookup"><span data-stu-id="6a3fb-158">Name given to the query at the time of query creation</span></span>     |
|    <span data-ttu-id="6a3fb-159">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a3fb-159">Description</span></span>     |    <span data-ttu-id="6a3fb-160">Descrição dada durante a criação da consulta</span><span class="sxs-lookup"><span data-stu-id="6a3fb-160">Description given during creation of the query</span></span>     |
|    <span data-ttu-id="6a3fb-161">Consulta</span><span class="sxs-lookup"><span data-stu-id="6a3fb-161">Query</span></span>     |    <span data-ttu-id="6a3fb-162">Cadeia de consulta de relatório</span><span class="sxs-lookup"><span data-stu-id="6a3fb-162">Report query string</span></span>     |
|    <span data-ttu-id="6a3fb-163">Tipo</span><span class="sxs-lookup"><span data-stu-id="6a3fb-163">Type</span></span>     |    <span data-ttu-id="6a3fb-164">Conjunto para utilizadorDefined para consultas e sistema criados pelo utilizador para consultas de sistema predefinidos</span><span class="sxs-lookup"><span data-stu-id="6a3fb-164">Set to userDefined for user created queries and system for predefined system queries</span></span>     |
|    <span data-ttu-id="6a3fb-165">Utilizador</span><span class="sxs-lookup"><span data-stu-id="6a3fb-165">User</span></span>     |    <span data-ttu-id="6a3fb-166">ID do utilizador que criou a consulta</span><span class="sxs-lookup"><span data-stu-id="6a3fb-166">User ID who created the query</span></span>     |
|    <span data-ttu-id="6a3fb-167">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="6a3fb-167">CreatedTime</span></span>     |    <span data-ttu-id="6a3fb-168">Tempo de criação de consulta</span><span class="sxs-lookup"><span data-stu-id="6a3fb-168">Time of creation of query</span></span>     |
|    <span data-ttu-id="6a3fb-169">TotalCount</span><span class="sxs-lookup"><span data-stu-id="6a3fb-169">TotalCount</span></span>     |    <span data-ttu-id="6a3fb-170">Número de conjuntos de dados na matriz de valor</span><span class="sxs-lookup"><span data-stu-id="6a3fb-170">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="6a3fb-171">Mensagem</span><span class="sxs-lookup"><span data-stu-id="6a3fb-171">Message</span></span>     |    <span data-ttu-id="6a3fb-172">Mensagem de estado da execução da API</span><span class="sxs-lookup"><span data-stu-id="6a3fb-172">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="6a3fb-173">Código de Estado</span><span class="sxs-lookup"><span data-stu-id="6a3fb-173">StatusCode</span></span>     |    <span data-ttu-id="6a3fb-174">Código de resultados.</span><span class="sxs-lookup"><span data-stu-id="6a3fb-174">Result Code.</span></span> <span data-ttu-id="6a3fb-175">Os valores possíveis são 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="6a3fb-175">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
