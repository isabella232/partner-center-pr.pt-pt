---
title: Eliminar consultas de relatório API - Informações dados
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Utilize esta API para eliminar a consulta definida pelo utilizador nos insights do Partner Center.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: e608068613edad1fca277ba5886c9c4bc962ffd2
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376980"
---
# <a name="delete-report-queries-api"></a><span data-ttu-id="6f7c7-103">Eliminar consultas de relatório API</span><span class="sxs-lookup"><span data-stu-id="6f7c7-103">Delete report queries API</span></span>

<span data-ttu-id="6f7c7-104">Esta API elimina consultas definidas pelo utilizador.</span><span class="sxs-lookup"><span data-stu-id="6f7c7-104">This API deletes user-defined queries.</span></span>

<span data-ttu-id="6f7c7-105">**Solicitar sintaxe**</span><span class="sxs-lookup"><span data-stu-id="6f7c7-105">**Request syntax**</span></span>

|    <span data-ttu-id="6f7c7-106">Método</span><span class="sxs-lookup"><span data-stu-id="6f7c7-106">Method</span></span>    |    <span data-ttu-id="6f7c7-107">URI do pedido</span><span class="sxs-lookup"><span data-stu-id="6f7c7-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="6f7c7-108">DELETE</span><span class="sxs-lookup"><span data-stu-id="6f7c7-108">DELETE</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries/{queryId}` |
|        |        |

<span data-ttu-id="6f7c7-109">**Cabeçalho de pedido**</span><span class="sxs-lookup"><span data-stu-id="6f7c7-109">**Request header**</span></span>

|    <span data-ttu-id="6f7c7-110">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6f7c7-110">Header</span></span>    |    <span data-ttu-id="6f7c7-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="6f7c7-111">Type</span></span>    |    <span data-ttu-id="6f7c7-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f7c7-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="6f7c7-113">Autorização</span><span class="sxs-lookup"><span data-stu-id="6f7c7-113">Authorization</span></span>    |    <span data-ttu-id="6f7c7-114">string</span><span class="sxs-lookup"><span data-stu-id="6f7c7-114">string</span></span>    |    <span data-ttu-id="6f7c7-115">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6f7c7-115">Required.</span></span> <span data-ttu-id="6f7c7-116">O Azure Ative Directory (AAD) símbolo de acesso na forma`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="6f7c7-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="6f7c7-117">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6f7c7-117">Content-Type</span></span>    |    <span data-ttu-id="6f7c7-118">string</span><span class="sxs-lookup"><span data-stu-id="6f7c7-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="6f7c7-119">**Parâmetro do caminho**</span><span class="sxs-lookup"><span data-stu-id="6f7c7-119">**Path parameter**</span></span>

|    <span data-ttu-id="6f7c7-120">Nome do Parâmetro</span><span class="sxs-lookup"><span data-stu-id="6f7c7-120">Parameter Name</span></span>    |    <span data-ttu-id="6f7c7-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="6f7c7-121">Type</span></span>    |    <span data-ttu-id="6f7c7-122">Necessário</span><span class="sxs-lookup"><span data-stu-id="6f7c7-122">Required</span></span>    |    <span data-ttu-id="6f7c7-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f7c7-123">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="6f7c7-124">consultaD</span><span class="sxs-lookup"><span data-stu-id="6f7c7-124">queryId</span></span>     |    <span data-ttu-id="6f7c7-125">cadeia (de carateres)</span><span class="sxs-lookup"><span data-stu-id="6f7c7-125">string</span></span>     |    <span data-ttu-id="6f7c7-126">No</span><span class="sxs-lookup"><span data-stu-id="6f7c7-126">No</span></span>    |    <span data-ttu-id="6f7c7-127">Filtrar para obter detalhes de apenas consultas com o ID dado no argumento</span><span class="sxs-lookup"><span data-stu-id="6f7c7-127">Filter to get details of only queries with the ID given in the argument</span></span>     |
|        |        |        |        |

<span data-ttu-id="6f7c7-128">**Parâmetro de consulta**</span><span class="sxs-lookup"><span data-stu-id="6f7c7-128">**Query parameter**</span></span>

<span data-ttu-id="6f7c7-129">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="6f7c7-129">None</span></span>

<span data-ttu-id="6f7c7-130">**Solicitar carga útil**</span><span class="sxs-lookup"><span data-stu-id="6f7c7-130">**Request payload**</span></span>

<span data-ttu-id="6f7c7-131">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="6f7c7-131">None</span></span>

<span data-ttu-id="6f7c7-132">**Glossário**</span><span class="sxs-lookup"><span data-stu-id="6f7c7-132">**Glossary**</span></span>

<span data-ttu-id="6f7c7-133">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="6f7c7-133">None</span></span>

<span data-ttu-id="6f7c7-134">**Response**</span><span class="sxs-lookup"><span data-stu-id="6f7c7-134">**Response**</span></span>

<span data-ttu-id="6f7c7-135">A carga útil de resposta é estruturada da seguinte forma:</span><span class="sxs-lookup"><span data-stu-id="6f7c7-135">The response payload is structured as follows:</span></span>

<span data-ttu-id="6f7c7-136">Código de resposta: 200, 400, 401, 403, 404,500</span><span class="sxs-lookup"><span data-stu-id="6f7c7-136">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="6f7c7-137">Exemplo de carga útil de resposta:</span><span class="sxs-lookup"><span data-stu-id="6f7c7-137">Response payload example:</span></span>

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

<span data-ttu-id="6f7c7-138">**Glossário**</span><span class="sxs-lookup"><span data-stu-id="6f7c7-138">**Glossary**</span></span>

<span data-ttu-id="6f7c7-139">Esta tabela define os elementos-chave na resposta:</span><span class="sxs-lookup"><span data-stu-id="6f7c7-139">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="6f7c7-140">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="6f7c7-140">Parameter</span></span>    |    <span data-ttu-id="6f7c7-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f7c7-141">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="6f7c7-142">QueryId</span><span class="sxs-lookup"><span data-stu-id="6f7c7-142">QueryId</span></span>     |    <span data-ttu-id="6f7c7-143">UUID único da consulta que foi eliminada</span><span class="sxs-lookup"><span data-stu-id="6f7c7-143">Unique UUID of the query that was deleted</span></span>    |
|    <span data-ttu-id="6f7c7-144">Name</span><span class="sxs-lookup"><span data-stu-id="6f7c7-144">Name</span></span>     |    <span data-ttu-id="6f7c7-145">Nome da consulta que foi eliminada</span><span class="sxs-lookup"><span data-stu-id="6f7c7-145">Name of the query that was deleted</span></span>    |
|    <span data-ttu-id="6f7c7-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f7c7-146">Description</span></span>     |    <span data-ttu-id="6f7c7-147">Descrição da consulta eliminada</span><span class="sxs-lookup"><span data-stu-id="6f7c7-147">Description of the deleted query</span></span>     |
|    <span data-ttu-id="6f7c7-148">Consulta</span><span class="sxs-lookup"><span data-stu-id="6f7c7-148">Query</span></span>     |    <span data-ttu-id="6f7c7-149">Cadeia de consulta de relatório da consulta eliminada</span><span class="sxs-lookup"><span data-stu-id="6f7c7-149">Report query string of the deleted query</span></span>    |
|    <span data-ttu-id="6f7c7-150">Tipo</span><span class="sxs-lookup"><span data-stu-id="6f7c7-150">Type</span></span>     |    <span data-ttu-id="6f7c7-151">Definir para utilizadorDefined para consultas criadas pelo utilizador</span><span class="sxs-lookup"><span data-stu-id="6f7c7-151">Set to userDefined for user created queries</span></span>     |
|    <span data-ttu-id="6f7c7-152">Utilizador</span><span class="sxs-lookup"><span data-stu-id="6f7c7-152">User</span></span>     |    <span data-ttu-id="6f7c7-153">ID do utilizador que criou a consulta</span><span class="sxs-lookup"><span data-stu-id="6f7c7-153">User ID who created the query</span></span>     |
|    <span data-ttu-id="6f7c7-154">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="6f7c7-154">CreatedTime</span></span>     |    <span data-ttu-id="6f7c7-155">Tempo de criação de consulta</span><span class="sxs-lookup"><span data-stu-id="6f7c7-155">Time of creation of query</span></span>     |
|    <span data-ttu-id="6f7c7-156">TotalCount</span><span class="sxs-lookup"><span data-stu-id="6f7c7-156">TotalCount</span></span>     |    <span data-ttu-id="6f7c7-157">Número de conjuntos de dados na matriz de valor</span><span class="sxs-lookup"><span data-stu-id="6f7c7-157">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="6f7c7-158">Mensagem</span><span class="sxs-lookup"><span data-stu-id="6f7c7-158">Message</span></span>     |    <span data-ttu-id="6f7c7-159">Mensagem de estado da execução da API</span><span class="sxs-lookup"><span data-stu-id="6f7c7-159">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="6f7c7-160">Código de Estado</span><span class="sxs-lookup"><span data-stu-id="6f7c7-160">StatusCode</span></span>     |    <span data-ttu-id="6f7c7-161">Código de resultados.</span><span class="sxs-lookup"><span data-stu-id="6f7c7-161">Result Code.</span></span> <span data-ttu-id="6f7c7-162">Os valores possíveis são 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="6f7c7-162">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
