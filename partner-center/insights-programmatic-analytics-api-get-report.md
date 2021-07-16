---
title: Obtenha relatório API - dados Informações
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Utilize esta API para obter toda a identificação de relatório disponível nos insights do Partner Center.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 174a2f60a36cb46b287b787b177dd32236cef4eb
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/16/2021
ms.locfileid: "114377204"
---
# <a name="get-report-api"></a><span data-ttu-id="c698a-103">Obtenha relatório API</span><span class="sxs-lookup"><span data-stu-id="c698a-103">Get report API</span></span>

<span data-ttu-id="c698a-104">Esta API recebe todos os relatórios que foram agendados.</span><span class="sxs-lookup"><span data-stu-id="c698a-104">This API gets all the reports that have been scheduled.</span></span>

<span data-ttu-id="c698a-105">**Solicitar sintaxe**</span><span class="sxs-lookup"><span data-stu-id="c698a-105">**Request syntax**</span></span>

|    <span data-ttu-id="c698a-106">Método</span><span class="sxs-lookup"><span data-stu-id="c698a-106">Method</span></span>    |    <span data-ttu-id="c698a-107">URI do pedido</span><span class="sxs-lookup"><span data-stu-id="c698a-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="c698a-108">GET</span><span class="sxs-lookup"><span data-stu-id="c698a-108">GET</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport?reportId={Report ID}&reportName={Report Name}&queryId={Query ID}` |
|        |        |

<span data-ttu-id="c698a-109">**Cabeçalho de pedido**</span><span class="sxs-lookup"><span data-stu-id="c698a-109">**Request header**</span></span>

|    <span data-ttu-id="c698a-110">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c698a-110">Header</span></span>    |    <span data-ttu-id="c698a-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="c698a-111">Type</span></span>    |    <span data-ttu-id="c698a-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="c698a-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="c698a-113">Autorização</span><span class="sxs-lookup"><span data-stu-id="c698a-113">Authorization</span></span>    |    <span data-ttu-id="c698a-114">string</span><span class="sxs-lookup"><span data-stu-id="c698a-114">string</span></span>    |    <span data-ttu-id="c698a-115">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c698a-115">Required.</span></span> <span data-ttu-id="c698a-116">O Azure Ative Directory (AAD) símbolo de acesso na forma`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="c698a-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="c698a-117">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c698a-117">Content-Type</span></span>    |    <span data-ttu-id="c698a-118">string</span><span class="sxs-lookup"><span data-stu-id="c698a-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="c698a-119">**Parâmetro do caminho**</span><span class="sxs-lookup"><span data-stu-id="c698a-119">**Path parameter**</span></span>

<span data-ttu-id="c698a-120">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="c698a-120">None</span></span>

<span data-ttu-id="c698a-121">**Parâmetro de consulta**</span><span class="sxs-lookup"><span data-stu-id="c698a-121">**Query parameter**</span></span>

|    <span data-ttu-id="c698a-122">Nome do Parâmetro</span><span class="sxs-lookup"><span data-stu-id="c698a-122">Parameter Name</span></span>    |    <span data-ttu-id="c698a-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="c698a-123">Type</span></span>    |    <span data-ttu-id="c698a-124">Necessário</span><span class="sxs-lookup"><span data-stu-id="c698a-124">Required</span></span>    |    <span data-ttu-id="c698a-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="c698a-125">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="c698a-126">reportId</span><span class="sxs-lookup"><span data-stu-id="c698a-126">reportId</span></span>     |    <span data-ttu-id="c698a-127">cadeia (de carateres)</span><span class="sxs-lookup"><span data-stu-id="c698a-127">string</span></span>    |    <span data-ttu-id="c698a-128">No</span><span class="sxs-lookup"><span data-stu-id="c698a-128">No</span></span>    |    <span data-ttu-id="c698a-129">Filtrar para obter detalhes de apenas relatórios com o reportId dado neste argumento</span><span class="sxs-lookup"><span data-stu-id="c698a-129">Filter to get details of only reports with the reportId given in this argument</span></span>     |
|    <span data-ttu-id="c698a-130">relatórioName</span><span class="sxs-lookup"><span data-stu-id="c698a-130">reportName</span></span>     |    <span data-ttu-id="c698a-131">cadeia (de carateres)</span><span class="sxs-lookup"><span data-stu-id="c698a-131">string</span></span>    |    <span data-ttu-id="c698a-132">No</span><span class="sxs-lookup"><span data-stu-id="c698a-132">No</span></span>    |    <span data-ttu-id="c698a-133">Filtrar para obter detalhes de apenas relatórios com o relatórioName dado neste argumento</span><span class="sxs-lookup"><span data-stu-id="c698a-133">Filter to get details of only reports with the reportName given in this argument</span></span>     |
|    <span data-ttu-id="c698a-134">consultaD</span><span class="sxs-lookup"><span data-stu-id="c698a-134">queryId</span></span>     |    <span data-ttu-id="c698a-135">cadeia (de carateres)</span><span class="sxs-lookup"><span data-stu-id="c698a-135">string</span></span>    |    <span data-ttu-id="c698a-136">No</span><span class="sxs-lookup"><span data-stu-id="c698a-136">No</span></span>    |    <span data-ttu-id="c698a-137">Filtrar para obter detalhes de apenas relatórios com a consulta dada neste argumento</span><span class="sxs-lookup"><span data-stu-id="c698a-137">Filter to get details of only reports with the queryId given in this argument</span></span>     |
|        |        |        |        |


<span data-ttu-id="c698a-138">**Solicitar carga útil**</span><span class="sxs-lookup"><span data-stu-id="c698a-138">**Request payload**</span></span>

<span data-ttu-id="c698a-139">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="c698a-139">None</span></span>

<span data-ttu-id="c698a-140">**Glossário**</span><span class="sxs-lookup"><span data-stu-id="c698a-140">**Glossary**</span></span>

<span data-ttu-id="c698a-141">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="c698a-141">None</span></span>

<span data-ttu-id="c698a-142">**Response**</span><span class="sxs-lookup"><span data-stu-id="c698a-142">**Response**</span></span>

<span data-ttu-id="c698a-143">A carga útil de resposta é estruturada da seguinte forma:</span><span class="sxs-lookup"><span data-stu-id="c698a-143">The response payload is structured as follows:</span></span>

<span data-ttu-id="c698a-144">Código de resposta: 200, 400, 401, 403, 404,500</span><span class="sxs-lookup"><span data-stu-id="c698a-144">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="c698a-145">Exemplo de carga útil de resposta:</span><span class="sxs-lookup"><span data-stu-id="c698a-145">Response payload example:</span></span>

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
      "executeNow": true, 
      "StartTime": "string", 
      "ReportStatus": "string", 
      "RecurrenceInterval": 0, 
      " RecurrenceCount": 0, 
      "CallbackUrl": "string",
      "CallbackMethod": null,
      "Format": "string" 
    } 
  ], 
  "TotalCount": 0, 
  "Message": "string", 
  "StatusCode": 0 
}
```

<span data-ttu-id="c698a-146">**Glossário**</span><span class="sxs-lookup"><span data-stu-id="c698a-146">**Glossary**</span></span>

<span data-ttu-id="c698a-147">Esta tabela define os elementos-chave na resposta:</span><span class="sxs-lookup"><span data-stu-id="c698a-147">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="c698a-148">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="c698a-148">Parameter</span></span>    |    <span data-ttu-id="c698a-149">Descrição</span><span class="sxs-lookup"><span data-stu-id="c698a-149">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="c698a-150">ReportId</span><span class="sxs-lookup"><span data-stu-id="c698a-150">ReportId</span></span>     |    <span data-ttu-id="c698a-151">UUID único do relatório que foi criado</span><span class="sxs-lookup"><span data-stu-id="c698a-151">Unique UUID of the report that was created</span></span>     |
|    <span data-ttu-id="c698a-152">Nome do relatório</span><span class="sxs-lookup"><span data-stu-id="c698a-152">ReportName</span></span>     |    <span data-ttu-id="c698a-153">Nome dado ao relatório na carga útil do pedido</span><span class="sxs-lookup"><span data-stu-id="c698a-153">Name given to the report in the request payload</span></span>     |
|    <span data-ttu-id="c698a-154">Descrição</span><span class="sxs-lookup"><span data-stu-id="c698a-154">Description</span></span>     |    <span data-ttu-id="c698a-155">Descrição dada quando o relatório foi criado</span><span class="sxs-lookup"><span data-stu-id="c698a-155">Description given when the report was created</span></span>     |
|    <span data-ttu-id="c698a-156">QueryId</span><span class="sxs-lookup"><span data-stu-id="c698a-156">QueryId</span></span>     |    <span data-ttu-id="c698a-157">Consulta ID passou no momento em que o relatório foi criado</span><span class="sxs-lookup"><span data-stu-id="c698a-157">Query ID passed at the time the report was created</span></span>     |
|    <span data-ttu-id="c698a-158">Consulta</span><span class="sxs-lookup"><span data-stu-id="c698a-158">Query</span></span>     |    <span data-ttu-id="c698a-159">Texto de consulta que será executado para este relatório</span><span class="sxs-lookup"><span data-stu-id="c698a-159">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="c698a-160">Utilizador</span><span class="sxs-lookup"><span data-stu-id="c698a-160">User</span></span>     |    <span data-ttu-id="c698a-161">ID do utilizador usado para criar o relatório</span><span class="sxs-lookup"><span data-stu-id="c698a-161">User ID used to create the report</span></span>     |
|    <span data-ttu-id="c698a-162">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="c698a-162">CreatedTime</span></span>     |    <span data-ttu-id="c698a-163">Hora de criar o relatório.</span><span class="sxs-lookup"><span data-stu-id="c698a-163">Time the report was created.</span></span> <span data-ttu-id="c698a-164">O formato de tempo é yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="c698a-164">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="c698a-165">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="c698a-165">ModifiedTime</span></span>     |    <span data-ttu-id="c698a-166">Foi a última vez que o relatório foi modificado.</span><span class="sxs-lookup"><span data-stu-id="c698a-166">Time the report was last modified.</span></span> <span data-ttu-id="c698a-167">O formato de tempo é yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="c698a-167">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="c698a-168">executarNow</span><span class="sxs-lookup"><span data-stu-id="c698a-168">executeNow</span></span>     |    <span data-ttu-id="c698a-169">ExecuteNow bandeira definida no momento em que o relatório foi criado</span><span class="sxs-lookup"><span data-stu-id="c698a-169">ExecuteNow flag set at the time the report was created</span></span>    |
|    <span data-ttu-id="c698a-170">StartTime</span><span class="sxs-lookup"><span data-stu-id="c698a-170">StartTime</span></span>     |    <span data-ttu-id="c698a-171">A execução do tempo começará.</span><span class="sxs-lookup"><span data-stu-id="c698a-171">Time execution will begin.</span></span> <span data-ttu-id="c698a-172">O formato de tempo é yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="c698a-172">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="c698a-173">Relatório Estatísticas</span><span class="sxs-lookup"><span data-stu-id="c698a-173">ReportStatus</span></span>     |    <span data-ttu-id="c698a-174">Estado da execução do relatório.</span><span class="sxs-lookup"><span data-stu-id="c698a-174">Status of the report execution.</span></span> <span data-ttu-id="c698a-175">Os valores possíveis são Pausados, Ativos e Inativos.</span><span class="sxs-lookup"><span data-stu-id="c698a-175">The possible values are Paused, Active, and Inactive.</span></span>     |
|    <span data-ttu-id="c698a-176">RecorrenceInterval</span><span class="sxs-lookup"><span data-stu-id="c698a-176">RecurrenceInterval</span></span>     |    <span data-ttu-id="c698a-177">Intervalo de recorrência fornecido durante a criação do relatório</span><span class="sxs-lookup"><span data-stu-id="c698a-177">Recurrence interval provided during report creation</span></span>     |
|    <span data-ttu-id="c698a-178">RecorrenceCount</span><span class="sxs-lookup"><span data-stu-id="c698a-178">RecurrenceCount</span></span>     |    <span data-ttu-id="c698a-179">Contagem de recorrência fornecida durante a criação do relatório</span><span class="sxs-lookup"><span data-stu-id="c698a-179">Recurrence count provided during report creation</span></span>     |
|    <span data-ttu-id="c698a-180">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="c698a-180">CallbackUrl</span></span>     |    <span data-ttu-id="c698a-181">URL de retorno fornecido no pedido</span><span class="sxs-lookup"><span data-stu-id="c698a-181">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="c698a-182">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="c698a-182">CallbackMethod</span></span>    |    <span data-ttu-id="c698a-183">Método de retorno fornecido no pedido</span><span class="sxs-lookup"><span data-stu-id="c698a-183">Callback method provided in the request</span></span>    |
|    <span data-ttu-id="c698a-184">Formato</span><span class="sxs-lookup"><span data-stu-id="c698a-184">Format</span></span>     |    <span data-ttu-id="c698a-185">Formato dos ficheiros de relatório</span><span class="sxs-lookup"><span data-stu-id="c698a-185">Format of the report files</span></span>     |
|    <span data-ttu-id="c698a-186">TotalCount</span><span class="sxs-lookup"><span data-stu-id="c698a-186">TotalCount</span></span>     |    <span data-ttu-id="c698a-187">Número de conjuntos de dados na matriz de valor</span><span class="sxs-lookup"><span data-stu-id="c698a-187">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="c698a-188">Mensagem</span><span class="sxs-lookup"><span data-stu-id="c698a-188">Message</span></span>     |    <span data-ttu-id="c698a-189">Mensagem de estado da execução da API</span><span class="sxs-lookup"><span data-stu-id="c698a-189">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="c698a-190">Código de Estado</span><span class="sxs-lookup"><span data-stu-id="c698a-190">StatusCode</span></span>     |    <span data-ttu-id="c698a-191">Código de resultados.</span><span class="sxs-lookup"><span data-stu-id="c698a-191">Result Code.</span></span> <span data-ttu-id="c698a-192">Os valores possíveis são 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="c698a-192">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |