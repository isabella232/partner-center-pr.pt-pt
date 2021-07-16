---
title: Relatório de pausa execução API - dados Informações
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Utilize esta API para interromper a execução de qualquer relatório nos insights do Partner Center.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 1e490a6d5120d729f0ea4979a201e9a80ba2991c
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/16/2021
ms.locfileid: "114377199"
---
# <a name="pause-report-executions-api"></a><span data-ttu-id="c781c-103">Pausa relatório execuções API</span><span class="sxs-lookup"><span data-stu-id="c781c-103">Pause report executions API</span></span>

<span data-ttu-id="c781c-104">Na execução, esta API interrompe a execução programada de relatórios.</span><span class="sxs-lookup"><span data-stu-id="c781c-104">On execution, this API pauses the scheduled execution of reports.</span></span>

<span data-ttu-id="c781c-105">**Solicitar sintaxe**</span><span class="sxs-lookup"><span data-stu-id="c781c-105">**Request syntax**</span></span>

|    <span data-ttu-id="c781c-106">Método</span><span class="sxs-lookup"><span data-stu-id="c781c-106">Method</span></span>    |    <span data-ttu-id="c781c-107">URI do pedido</span><span class="sxs-lookup"><span data-stu-id="c781c-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="c781c-108">PUT</span><span class="sxs-lookup"><span data-stu-id="c781c-108">PUT</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/pause/{ReportID}`    |
|        |        |

<span data-ttu-id="c781c-109">**Cabeçalho de pedido**</span><span class="sxs-lookup"><span data-stu-id="c781c-109">**Request header**</span></span>

|    <span data-ttu-id="c781c-110">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c781c-110">Header</span></span>    |    <span data-ttu-id="c781c-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="c781c-111">Type</span></span>    |    <span data-ttu-id="c781c-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="c781c-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="c781c-113">Autorização</span><span class="sxs-lookup"><span data-stu-id="c781c-113">Authorization</span></span>    |    <span data-ttu-id="c781c-114">string</span><span class="sxs-lookup"><span data-stu-id="c781c-114">string</span></span>    |    <span data-ttu-id="c781c-115">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c781c-115">Required.</span></span> <span data-ttu-id="c781c-116">O Azure Ative Directory (AAD) símbolo de acesso na forma`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="c781c-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="c781c-117">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c781c-117">Content-Type</span></span>    |    <span data-ttu-id="c781c-118">string</span><span class="sxs-lookup"><span data-stu-id="c781c-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="c781c-119">**Parâmetro do caminho**</span><span class="sxs-lookup"><span data-stu-id="c781c-119">**Path parameter**</span></span>

|    <span data-ttu-id="c781c-120">Nome do Parâmetro</span><span class="sxs-lookup"><span data-stu-id="c781c-120">Parameter Name</span></span>    |    <span data-ttu-id="c781c-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="c781c-121">Type</span></span>    |    <span data-ttu-id="c781c-122">Necessário</span><span class="sxs-lookup"><span data-stu-id="c781c-122">Required</span></span>    |    <span data-ttu-id="c781c-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="c781c-123">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="c781c-124">reportId</span><span class="sxs-lookup"><span data-stu-id="c781c-124">reportId</span></span>     |    <span data-ttu-id="c781c-125">cadeia (de carateres)</span><span class="sxs-lookup"><span data-stu-id="c781c-125">string</span></span>    |    <span data-ttu-id="c781c-126">No</span><span class="sxs-lookup"><span data-stu-id="c781c-126">No</span></span>    |    <span data-ttu-id="c781c-127">ID do relatório a ser modificado</span><span class="sxs-lookup"><span data-stu-id="c781c-127">ID of the report being modified</span></span>     |
|        |        |        |        |

<span data-ttu-id="c781c-128">**Parâmetro de consulta**</span><span class="sxs-lookup"><span data-stu-id="c781c-128">**Query parameter**</span></span>

<span data-ttu-id="c781c-129">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="c781c-129">None</span></span>

<span data-ttu-id="c781c-130">**Solicitar carga útil**</span><span class="sxs-lookup"><span data-stu-id="c781c-130">**Request payload**</span></span>

<span data-ttu-id="c781c-131">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="c781c-131">None</span></span>

<span data-ttu-id="c781c-132">**Glossário**</span><span class="sxs-lookup"><span data-stu-id="c781c-132">**Glossary**</span></span>

<span data-ttu-id="c781c-133">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="c781c-133">None</span></span>

<span data-ttu-id="c781c-134">**Response**</span><span class="sxs-lookup"><span data-stu-id="c781c-134">**Response**</span></span>

<span data-ttu-id="c781c-135">A carga útil de resposta é estruturada da seguinte forma:</span><span class="sxs-lookup"><span data-stu-id="c781c-135">The response payload is structured as follows:</span></span>

<span data-ttu-id="c781c-136">Código de resposta: 200, 400, 401, 403, 404,500</span><span class="sxs-lookup"><span data-stu-id="c781c-136">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="c781c-137">Exemplo de carga útil de resposta:</span><span class="sxs-lookup"><span data-stu-id="c781c-137">Response payload example:</span></span>

```json
{ 
  "Value": [ 
    { 
      "ReportId": "string", 
      "ReportName": "string", 
      "Description": "string", 
      "QueryId": "string", 
      "Query": "string", 
      "User": "string", 
      "CreatedTime": "string", 
      "ModifiedTime": "string", 
      "ExecuteNow": true, 
      "StartTime": "string", 
      "ReportStatus": "string", 
      "RecurrenceInterval": 0, 
      "RecurrenceCount": 0, 
      "CallbackUrl": "string", 
      "CallbackMethod": "string", 
      "Format": "string" 
    } 
  ], 
  "TotalCount": 0, 
  "Message": "string", 
  "StatusCode": 0, 
} 
```

<span data-ttu-id="c781c-138">**Glossário**</span><span class="sxs-lookup"><span data-stu-id="c781c-138">**Glossary**</span></span>

<span data-ttu-id="c781c-139">Esta tabela define os elementos-chave na resposta:</span><span class="sxs-lookup"><span data-stu-id="c781c-139">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="c781c-140">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="c781c-140">Parameter</span></span>    |    <span data-ttu-id="c781c-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="c781c-141">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="c781c-142">ReportId</span><span class="sxs-lookup"><span data-stu-id="c781c-142">ReportId</span></span>     |    <span data-ttu-id="c781c-143">Identificador universalmente único (UUID) do relatório pausado</span><span class="sxs-lookup"><span data-stu-id="c781c-143">Universally unique identifier (UUID) of the paused report</span></span>     |
|    <span data-ttu-id="c781c-144">Nome do relatório</span><span class="sxs-lookup"><span data-stu-id="c781c-144">ReportName</span></span>     |    <span data-ttu-id="c781c-145">Nome dado ao relatório durante a criação</span><span class="sxs-lookup"><span data-stu-id="c781c-145">Name given to the report during creation</span></span>     |
|    <span data-ttu-id="c781c-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="c781c-146">Description</span></span>     |    <span data-ttu-id="c781c-147">Descrição dada durante a criação do relatório</span><span class="sxs-lookup"><span data-stu-id="c781c-147">Description given during creation of the report</span></span>     |
|    <span data-ttu-id="c781c-148">QueryId</span><span class="sxs-lookup"><span data-stu-id="c781c-148">QueryId</span></span>     |    <span data-ttu-id="c781c-149">Consulta ID passou no momento em que o relatório foi criado</span><span class="sxs-lookup"><span data-stu-id="c781c-149">Query ID passed at the time the report was created</span></span>     |
|    <span data-ttu-id="c781c-150">Consulta</span><span class="sxs-lookup"><span data-stu-id="c781c-150">Query</span></span>     |    <span data-ttu-id="c781c-151">Texto de consulta que será executado para este relatório</span><span class="sxs-lookup"><span data-stu-id="c781c-151">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="c781c-152">Utilizador</span><span class="sxs-lookup"><span data-stu-id="c781c-152">User</span></span>     |    <span data-ttu-id="c781c-153">ID do utilizador usado para criar o relatório</span><span class="sxs-lookup"><span data-stu-id="c781c-153">User ID used to create the report</span></span>     |
|    <span data-ttu-id="c781c-154">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="c781c-154">CreatedTime</span></span>     |    <span data-ttu-id="c781c-155">Hora de criar o relatório.</span><span class="sxs-lookup"><span data-stu-id="c781c-155">Time the report was created.</span></span> <span data-ttu-id="c781c-156">O formato de tempo é yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="c781c-156">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="c781c-157">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="c781c-157">ModifiedTime</span></span>     |    <span data-ttu-id="c781c-158">Foi a última vez que o relatório foi modificado.</span><span class="sxs-lookup"><span data-stu-id="c781c-158">Time the report was last modified.</span></span> <span data-ttu-id="c781c-159">O formato de tempo é yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="c781c-159">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="c781c-160">Executar Agora</span><span class="sxs-lookup"><span data-stu-id="c781c-160">ExecuteNow</span></span>     |    <span data-ttu-id="c781c-161">ExecuteNow bandeira definida no momento em que o relatório foi criado</span><span class="sxs-lookup"><span data-stu-id="c781c-161">ExecuteNow flag set at the time the report was created</span></span>     |
|    <span data-ttu-id="c781c-162">StartTime</span><span class="sxs-lookup"><span data-stu-id="c781c-162">StartTime</span></span>     |    <span data-ttu-id="c781c-163">Quando começar a execução do relatório.</span><span class="sxs-lookup"><span data-stu-id="c781c-163">Time the report execution will begin.</span></span> <span data-ttu-id="c781c-164">O formato de tempo é yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="c781c-164">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="c781c-165">Relatório Estatísticas</span><span class="sxs-lookup"><span data-stu-id="c781c-165">ReportStatus</span></span>     |    <span data-ttu-id="c781c-166">Estado da execução do relatório.</span><span class="sxs-lookup"><span data-stu-id="c781c-166">Status of the report execution.</span></span> <span data-ttu-id="c781c-167">Os valores possíveis são Pausados, Ativos e Inativos.</span><span class="sxs-lookup"><span data-stu-id="c781c-167">The possible values are Paused, Active, and Inactive.</span></span>     |
|    <span data-ttu-id="c781c-168">RecorrenceInterval</span><span class="sxs-lookup"><span data-stu-id="c781c-168">RecurrenceInterval</span></span>     |    <span data-ttu-id="c781c-169">Intervalo de recorrência fornecido durante a criação do relatório</span><span class="sxs-lookup"><span data-stu-id="c781c-169">Recurrence interval provided during report creation</span></span>     |
|    <span data-ttu-id="c781c-170">RecorrenceCount</span><span class="sxs-lookup"><span data-stu-id="c781c-170">RecurrenceCount</span></span>     |    <span data-ttu-id="c781c-171">Contagem de recorrência fornecida durante a criação do relatório</span><span class="sxs-lookup"><span data-stu-id="c781c-171">Recurrence count provided during report creation</span></span>     |
|    <span data-ttu-id="c781c-172">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="c781c-172">CallbackUrl</span></span>     |    <span data-ttu-id="c781c-173">URL de retorno fornecido no pedido</span><span class="sxs-lookup"><span data-stu-id="c781c-173">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="c781c-174">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="c781c-174">CallbackMethod</span></span>    |    <span data-ttu-id="c781c-175">Método de retorno fornecido no pedido</span><span class="sxs-lookup"><span data-stu-id="c781c-175">Callback method provided in the request</span></span>    |
|    <span data-ttu-id="c781c-176">Formato</span><span class="sxs-lookup"><span data-stu-id="c781c-176">Format</span></span>     |    <span data-ttu-id="c781c-177">Formato dos ficheiros de relatório</span><span class="sxs-lookup"><span data-stu-id="c781c-177">Format of the report files</span></span>     |
|    <span data-ttu-id="c781c-178">TotalCount</span><span class="sxs-lookup"><span data-stu-id="c781c-178">TotalCount</span></span>     |    <span data-ttu-id="c781c-179">Número de conjuntos de dados na matriz de valor</span><span class="sxs-lookup"><span data-stu-id="c781c-179">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="c781c-180">Mensagem</span><span class="sxs-lookup"><span data-stu-id="c781c-180">Message</span></span>     |    <span data-ttu-id="c781c-181">Mensagem de estado da execução da API</span><span class="sxs-lookup"><span data-stu-id="c781c-181">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="c781c-182">Código de Estado</span><span class="sxs-lookup"><span data-stu-id="c781c-182">StatusCode</span></span>     |    <span data-ttu-id="c781c-183">Código de resultados.</span><span class="sxs-lookup"><span data-stu-id="c781c-183">Result Code.</span></span> <span data-ttu-id="c781c-184">Os valores possíveis são 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="c781c-184">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
