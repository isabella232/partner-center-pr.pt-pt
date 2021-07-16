---
title: Obtenha todos os conjuntos de dados API - Informações dados
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Utilize esta API para obter detalhes de todos os conjuntos de dados disponíveis em insights do Partner Center.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 42ff7cc1f097e2423be5f1f7f9a7f62214d64949
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376957"
---
# <a name="get-all-datasets-api"></a><span data-ttu-id="659f8-103">Obtenha todos os conjuntos de dados API</span><span class="sxs-lookup"><span data-stu-id="659f8-103">Get all datasets API</span></span>

<span data-ttu-id="659f8-104">A API obtém todos os conjuntos de dados que a API obtém todos os conjuntos de dados disponíveis.</span><span class="sxs-lookup"><span data-stu-id="659f8-104">The Get all datasets API gets all the available datasets.</span></span> <span data-ttu-id="659f8-105">Os conjuntos de dados listam as tabelas, colunas, métricas e intervalos de tempo.</span><span class="sxs-lookup"><span data-stu-id="659f8-105">Datasets list the tables, columns, metrics, and time ranges.</span></span>

<span data-ttu-id="659f8-106">**Solicitar sintaxe**</span><span class="sxs-lookup"><span data-stu-id="659f8-106">**Request syntax**</span></span>

|    <span data-ttu-id="659f8-107">Método</span><span class="sxs-lookup"><span data-stu-id="659f8-107">Method</span></span>    |    <span data-ttu-id="659f8-108">URI do pedido</span><span class="sxs-lookup"><span data-stu-id="659f8-108">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="659f8-109">GET</span><span class="sxs-lookup"><span data-stu-id="659f8-109">GET</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledDataset?datasetName={Dataset Name}`     |
|        |        |

<span data-ttu-id="659f8-110">**Cabeçalho de pedido**</span><span class="sxs-lookup"><span data-stu-id="659f8-110">**Request header**</span></span>

|    <span data-ttu-id="659f8-111">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="659f8-111">Header</span></span>    |    <span data-ttu-id="659f8-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="659f8-112">Type</span></span>    |    <span data-ttu-id="659f8-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="659f8-113">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="659f8-114">Autorização</span><span class="sxs-lookup"><span data-stu-id="659f8-114">Authorization</span></span>    |    <span data-ttu-id="659f8-115">string</span><span class="sxs-lookup"><span data-stu-id="659f8-115">string</span></span>    |    <span data-ttu-id="659f8-116">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="659f8-116">Required.</span></span> <span data-ttu-id="659f8-117">O Azure Ative Directory (AAD) símbolo de acesso na forma`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="659f8-117">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="659f8-118">Content-Type</span><span class="sxs-lookup"><span data-stu-id="659f8-118">Content-Type</span></span>    |    <span data-ttu-id="659f8-119">string</span><span class="sxs-lookup"><span data-stu-id="659f8-119">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="659f8-120">**Parâmetro do caminho**</span><span class="sxs-lookup"><span data-stu-id="659f8-120">**Path parameter**</span></span>

<span data-ttu-id="659f8-121">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="659f8-121">None</span></span>

<span data-ttu-id="659f8-122">**Parâmetro de consulta**</span><span class="sxs-lookup"><span data-stu-id="659f8-122">**Query parameter**</span></span>

|    <span data-ttu-id="659f8-123">Nome do Parâmetro</span><span class="sxs-lookup"><span data-stu-id="659f8-123">Parameter Name</span></span>    |    <span data-ttu-id="659f8-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="659f8-124">Type</span></span>    |    <span data-ttu-id="659f8-125">Necessário</span><span class="sxs-lookup"><span data-stu-id="659f8-125">Required</span></span>    |    <span data-ttu-id="659f8-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="659f8-126">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="659f8-127">datasetName</span><span class="sxs-lookup"><span data-stu-id="659f8-127">datasetName</span></span>    |    <span data-ttu-id="659f8-128">cadeia (de carateres)</span><span class="sxs-lookup"><span data-stu-id="659f8-128">string</span></span>    |    <span data-ttu-id="659f8-129">No</span><span class="sxs-lookup"><span data-stu-id="659f8-129">No</span></span>    |    <span data-ttu-id="659f8-130">Filtrar para obter detalhes de apenas um conjunto de dados</span><span class="sxs-lookup"><span data-stu-id="659f8-130">Filter to get details of only one dataset</span></span>    |
|        |        |        |        |

<span data-ttu-id="659f8-131">**Solicitar carga útil**</span><span class="sxs-lookup"><span data-stu-id="659f8-131">**Request payload**</span></span>

<span data-ttu-id="659f8-132">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="659f8-132">None</span></span>

<span data-ttu-id="659f8-133">**Glossário**</span><span class="sxs-lookup"><span data-stu-id="659f8-133">**Glossary**</span></span>

<span data-ttu-id="659f8-134">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="659f8-134">None</span></span>

<span data-ttu-id="659f8-135">**Response**</span><span class="sxs-lookup"><span data-stu-id="659f8-135">**Response**</span></span>

<span data-ttu-id="659f8-136">A carga útil de resposta é estruturada da seguinte forma:</span><span class="sxs-lookup"><span data-stu-id="659f8-136">The response payload is structured as follows:</span></span>

<span data-ttu-id="659f8-137">Código de resposta: 200, 400, 401, 403, 404,500</span><span class="sxs-lookup"><span data-stu-id="659f8-137">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="659f8-138">Exemplo de carga útil de resposta:</span><span class="sxs-lookup"><span data-stu-id="659f8-138">Response payload example:</span></span>

```json
{ 
   "Value":[ 
      { 
         "DatasetName ":"string", 
         "SelectableColumns":[ 
            "string" 
         ], 
         "AvailableMetrics":[ 
            "string" 
         ], 
         "AvailableDateRanges":[ 
            "string" 
         ], 
         "minimumRecurrenceInterval":0 
      } 
   ], 
   "TotalCount":0, 
   "Message":"<Error Message>", 
   "StatusCode": 0, 
} 
```

<span data-ttu-id="659f8-139">**Glossário**</span><span class="sxs-lookup"><span data-stu-id="659f8-139">**Glossary**</span></span>

<span data-ttu-id="659f8-140">Esta tabela define os elementos-chave na resposta:</span><span class="sxs-lookup"><span data-stu-id="659f8-140">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="659f8-141">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="659f8-141">Parameter</span></span>    |    <span data-ttu-id="659f8-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="659f8-142">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="659f8-143">DatasetName</span><span class="sxs-lookup"><span data-stu-id="659f8-143">DatasetName</span></span>     |    <span data-ttu-id="659f8-144">Nome do conjunto de dados que este objeto de matriz define</span><span class="sxs-lookup"><span data-stu-id="659f8-144">Name of the dataset that this array object defines</span></span>     |
|    <span data-ttu-id="659f8-145">Universidades selecionadas</span><span class="sxs-lookup"><span data-stu-id="659f8-145">SelectableColumns</span></span>     |    <span data-ttu-id="659f8-146">Colunas em bruto que podem ser especificadas nas colunas selecionadas</span><span class="sxs-lookup"><span data-stu-id="659f8-146">Raw columns that can be specified in the select columns</span></span>     |
|    <span data-ttu-id="659f8-147">Métrica Disponível</span><span class="sxs-lookup"><span data-stu-id="659f8-147">AvailableMetrics</span></span>     |    <span data-ttu-id="659f8-148">Nomes de colunas agregação/métrica que podem ser especificados nas colunas selecionadas</span><span class="sxs-lookup"><span data-stu-id="659f8-148">Aggregation/metric column names that can be specified in the select columns</span></span>     |
|    <span data-ttu-id="659f8-149">DisponíveisDateRanges</span><span class="sxs-lookup"><span data-stu-id="659f8-149">AvailableDateRanges</span></span>     |    <span data-ttu-id="659f8-150">Intervalo de datas que pode ser usado em consultas de relatório para o conjunto de dados</span><span class="sxs-lookup"><span data-stu-id="659f8-150">Date range that can be used in report queries for the dataset</span></span>     |
|    <span data-ttu-id="659f8-151">mínimoRecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="659f8-151">minimumRecurrenceInterval</span></span>     |    <span data-ttu-id="659f8-152">Valor mínimo do Intervalo de Recorrência</span><span class="sxs-lookup"><span data-stu-id="659f8-152">Minimum value of Recurrence Interval</span></span>     |
|    <span data-ttu-id="659f8-153">TotalCount</span><span class="sxs-lookup"><span data-stu-id="659f8-153">TotalCount</span></span>     |    <span data-ttu-id="659f8-154">Número de conjuntos de dados na matriz de valor</span><span class="sxs-lookup"><span data-stu-id="659f8-154">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="659f8-155">Mensagem</span><span class="sxs-lookup"><span data-stu-id="659f8-155">Message</span></span>     |    <span data-ttu-id="659f8-156">Mensagem de estado da execução da API</span><span class="sxs-lookup"><span data-stu-id="659f8-156">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="659f8-157">Código de Estado</span><span class="sxs-lookup"><span data-stu-id="659f8-157">StatusCode</span></span>     |    <span data-ttu-id="659f8-158">Código de resultados.</span><span class="sxs-lookup"><span data-stu-id="659f8-158">Result Code.</span></span> <span data-ttu-id="659f8-159">Os valores possíveis são 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="659f8-159">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
