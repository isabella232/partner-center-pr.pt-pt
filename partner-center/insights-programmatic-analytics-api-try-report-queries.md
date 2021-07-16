---
title: Experimente consultas de relatório API
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Utilize esta API para testar a sua consulta e validar os resultados em insights do Partner Center.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 13ad6fe385a4d31390b6806d863da3f647105b2c
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/16/2021
ms.locfileid: "114377181"
---
# <a name="try-report-queries-api"></a><span data-ttu-id="822eb-103">Experimente consultas de relatório API</span><span class="sxs-lookup"><span data-stu-id="822eb-103">Try report queries API</span></span>

<span data-ttu-id="822eb-104">Esta API executa uma declaração de consulta de relatório.</span><span class="sxs-lookup"><span data-stu-id="822eb-104">This API executes a Report query statement.</span></span> <span data-ttu-id="822eb-105">A API devolve apenas 100 registos que pode utilizar como parceiro para verificar se os dados são como esperava.</span><span class="sxs-lookup"><span data-stu-id="822eb-105">The API returns only 100 records that you as a partner can use to verify if the data is as you expected.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="822eb-106">Esta API tem um tempo de execução de consulta de 100 segundos.</span><span class="sxs-lookup"><span data-stu-id="822eb-106">This API has a query execution timeout of 100 seconds.</span></span> <span data-ttu-id="822eb-107">Se notar que a API está a demorar mais de 100 segundos, é muito provável que a consulta esteja sintaticamente correta ou então teria recebido um código de erro que não seja 200.</span><span class="sxs-lookup"><span data-stu-id="822eb-107">If you notice the API is taking more than 100 seconds, it is highly likely that the query is syntactically correct or else you would have received an error code other than 200.</span></span> <span data-ttu-id="822eb-108">A geração de relatórios efetivamente passará se a sintaxe de consulta estiver correta.</span><span class="sxs-lookup"><span data-stu-id="822eb-108">The actual report generation will pass if the query syntax is correct.</span></span>

<span data-ttu-id="822eb-109">**Solicitar sintaxe**</span><span class="sxs-lookup"><span data-stu-id="822eb-109">**Request syntax**</span></span>

|    <span data-ttu-id="822eb-110">Método</span><span class="sxs-lookup"><span data-stu-id="822eb-110">Method</span></span>    |    <span data-ttu-id="822eb-111">URI do pedido</span><span class="sxs-lookup"><span data-stu-id="822eb-111">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="822eb-112">GET</span><span class="sxs-lookup"><span data-stu-id="822eb-112">GET</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries/testQueryResult?<exportQuery={query text}|queryId={queryId}>`    |
|        |        |

<span data-ttu-id="822eb-113">**Cabeçalho de pedido**</span><span class="sxs-lookup"><span data-stu-id="822eb-113">**Request header**</span></span>

|    <span data-ttu-id="822eb-114">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="822eb-114">Header</span></span>    |    <span data-ttu-id="822eb-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="822eb-115">Type</span></span>    |    <span data-ttu-id="822eb-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="822eb-116">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="822eb-117">Autorização</span><span class="sxs-lookup"><span data-stu-id="822eb-117">Authorization</span></span>    |    <span data-ttu-id="822eb-118">string</span><span class="sxs-lookup"><span data-stu-id="822eb-118">string</span></span>    |    <span data-ttu-id="822eb-119">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="822eb-119">Required.</span></span> <span data-ttu-id="822eb-120">O Azure Ative Directory (AAD) símbolo de acesso na forma`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="822eb-120">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="822eb-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="822eb-121">Content-Type</span></span>    |    <span data-ttu-id="822eb-122">string</span><span class="sxs-lookup"><span data-stu-id="822eb-122">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="822eb-123">**Parâmetro do caminho**</span><span class="sxs-lookup"><span data-stu-id="822eb-123">**Path parameter**</span></span>

<span data-ttu-id="822eb-124">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="822eb-124">None</span></span>

<span data-ttu-id="822eb-125">**Parâmetro de consulta**</span><span class="sxs-lookup"><span data-stu-id="822eb-125">**Query parameter**</span></span>

|    <span data-ttu-id="822eb-126">Nome do Parâmetro</span><span class="sxs-lookup"><span data-stu-id="822eb-126">Parameter Name</span></span>    |    <span data-ttu-id="822eb-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="822eb-127">Type</span></span>    |    <span data-ttu-id="822eb-128">Necessário</span><span class="sxs-lookup"><span data-stu-id="822eb-128">Required</span></span>    |    <span data-ttu-id="822eb-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="822eb-129">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="822eb-130">exportaçãoQuery</span><span class="sxs-lookup"><span data-stu-id="822eb-130">exportQuery</span></span>     |    <span data-ttu-id="822eb-131">cadeia (de carateres)</span><span class="sxs-lookup"><span data-stu-id="822eb-131">string</span></span>    |    <span data-ttu-id="822eb-132">No</span><span class="sxs-lookup"><span data-stu-id="822eb-132">No</span></span>    |    <span data-ttu-id="822eb-133">Cadeia de consulta de relatório que precisa ser executada</span><span class="sxs-lookup"><span data-stu-id="822eb-133">Report query string that needs to be executed</span></span>     |
|    <span data-ttu-id="822eb-134">consultaD</span><span class="sxs-lookup"><span data-stu-id="822eb-134">queryId</span></span>     |    <span data-ttu-id="822eb-135">cadeia (de carateres)</span><span class="sxs-lookup"><span data-stu-id="822eb-135">string</span></span>    |    <span data-ttu-id="822eb-136">No</span><span class="sxs-lookup"><span data-stu-id="822eb-136">No</span></span>    |    <span data-ttu-id="822eb-137">Um documento de consulta válido existente.</span><span class="sxs-lookup"><span data-stu-id="822eb-137">A valid existing query ID.</span></span> <span data-ttu-id="822eb-138">Mutuamente exclusivo com cadeia de consulta especificada no parâmetro exportQuery</span><span class="sxs-lookup"><span data-stu-id="822eb-138">Mutually exclusive with query string specified in exportQuery parameter</span></span>    |
|    <span data-ttu-id="822eb-139">startTime</span><span class="sxs-lookup"><span data-stu-id="822eb-139">startTime</span></span>     |    <span data-ttu-id="822eb-140">cadeia (de carateres)</span><span class="sxs-lookup"><span data-stu-id="822eb-140">string</span></span>    |    <span data-ttu-id="822eb-141">No</span><span class="sxs-lookup"><span data-stu-id="822eb-141">No</span></span>    |    <span data-ttu-id="822eb-142">Hora de início a partir da qual queremos os dados.</span><span class="sxs-lookup"><span data-stu-id="822eb-142">Start time from which we want the data.</span></span> <span data-ttu-id="822eb-143">Sobrepõe-se à timepan especificada na consulta</span><span class="sxs-lookup"><span data-stu-id="822eb-143">It overrides timespan specified in the query</span></span>    |
|    <span data-ttu-id="822eb-144">endTime</span><span class="sxs-lookup"><span data-stu-id="822eb-144">endTime</span></span>     |    <span data-ttu-id="822eb-145">cadeia (de carateres)</span><span class="sxs-lookup"><span data-stu-id="822eb-145">string</span></span>    |    <span data-ttu-id="822eb-146">No</span><span class="sxs-lookup"><span data-stu-id="822eb-146">No</span></span>    |    <span data-ttu-id="822eb-147">Fim do tempo até que queremos os dados.</span><span class="sxs-lookup"><span data-stu-id="822eb-147">End time till which we want the data.</span></span> <span data-ttu-id="822eb-148">Sobrepõe-se à timepan especificada na consulta</span><span class="sxs-lookup"><span data-stu-id="822eb-148">It overrides timespan specified in the query</span></span>    |
|        |        |        |        |

<span data-ttu-id="822eb-149">**Solicitar carga útil**</span><span class="sxs-lookup"><span data-stu-id="822eb-149">**Request payload**</span></span>

<span data-ttu-id="822eb-150">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="822eb-150">None</span></span>

<span data-ttu-id="822eb-151">**Glossário**</span><span class="sxs-lookup"><span data-stu-id="822eb-151">**Glossary**</span></span>

<span data-ttu-id="822eb-152">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="822eb-152">None</span></span>

<span data-ttu-id="822eb-153">**Response**</span><span class="sxs-lookup"><span data-stu-id="822eb-153">**Response**</span></span>

<span data-ttu-id="822eb-154">A carga útil de resposta é estruturada da seguinte forma:</span><span class="sxs-lookup"><span data-stu-id="822eb-154">The response payload is structured as follows:</span></span>

<span data-ttu-id="822eb-155">Código de resposta: 200, 400, 401, 403, 404,500</span><span class="sxs-lookup"><span data-stu-id="822eb-155">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="822eb-156">Exemplo de carga útil de resposta:</span><span class="sxs-lookup"><span data-stu-id="822eb-156">Response payload example:</span></span>

```json
Top 100 rows of query execution 
{ 
  "Value": [ 
    { 
    } 
  ], 
  "TotalCount": 0, 
  "Message": "string", 
  "StatusCode": 0, 
} 
```

<span data-ttu-id="822eb-157">**Glossário**</span><span class="sxs-lookup"><span data-stu-id="822eb-157">**Glossary**</span></span>

<span data-ttu-id="822eb-158">Esta tabela define os elementos-chave na resposta:</span><span class="sxs-lookup"><span data-stu-id="822eb-158">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="822eb-159">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="822eb-159">Parameter</span></span>    |    <span data-ttu-id="822eb-160">Descrição</span><span class="sxs-lookup"><span data-stu-id="822eb-160">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="822eb-161">TotalCount</span><span class="sxs-lookup"><span data-stu-id="822eb-161">TotalCount</span></span>     |    <span data-ttu-id="822eb-162">Número de conjuntos de dados na matriz de valor</span><span class="sxs-lookup"><span data-stu-id="822eb-162">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="822eb-163">Mensagem</span><span class="sxs-lookup"><span data-stu-id="822eb-163">Message</span></span>     |    <span data-ttu-id="822eb-164">Mensagem de estado da execução da API</span><span class="sxs-lookup"><span data-stu-id="822eb-164">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="822eb-165">Código de Estado</span><span class="sxs-lookup"><span data-stu-id="822eb-165">StatusCode</span></span>     |    <span data-ttu-id="822eb-166">Código de resultados.</span><span class="sxs-lookup"><span data-stu-id="822eb-166">Result Code.</span></span> <span data-ttu-id="822eb-167">Os valores possíveis são 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="822eb-167">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
