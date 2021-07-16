---
title: Relatório de atualização API
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Utilize esta API para atualizar os parâmetros do relatório nos insights do Partner Center.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: c5ab1059e9be9b42918d268da6a6c1a3cbfe52af
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/16/2021
ms.locfileid: "114377180"
---
# <a name="update-report-api"></a><span data-ttu-id="519c4-103">Relatório de atualização API</span><span class="sxs-lookup"><span data-stu-id="519c4-103">Update report API</span></span>

<span data-ttu-id="519c4-104">Esta API ajuda-o a modificar um parâmetro de relatório.</span><span class="sxs-lookup"><span data-stu-id="519c4-104">This API helps you modify a report parameter.</span></span>

<span data-ttu-id="519c4-105">**Solicitar sintaxe**</span><span class="sxs-lookup"><span data-stu-id="519c4-105">**Request syntax**</span></span>

|    <span data-ttu-id="519c4-106">Método</span><span class="sxs-lookup"><span data-stu-id="519c4-106">Method</span></span>    |    <span data-ttu-id="519c4-107">URI do pedido</span><span class="sxs-lookup"><span data-stu-id="519c4-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="519c4-108">PUT</span><span class="sxs-lookup"><span data-stu-id="519c4-108">PUT</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/{Report ID}`    |
|        |        |

<span data-ttu-id="519c4-109">**Cabeçalho de pedido**</span><span class="sxs-lookup"><span data-stu-id="519c4-109">**Request header**</span></span>

|    <span data-ttu-id="519c4-110">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="519c4-110">Header</span></span>    |    <span data-ttu-id="519c4-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="519c4-111">Type</span></span>    |    <span data-ttu-id="519c4-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="519c4-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="519c4-113">Autorização</span><span class="sxs-lookup"><span data-stu-id="519c4-113">Authorization</span></span>    |    <span data-ttu-id="519c4-114">string</span><span class="sxs-lookup"><span data-stu-id="519c4-114">string</span></span>    |    <span data-ttu-id="519c4-115">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="519c4-115">Required.</span></span> <span data-ttu-id="519c4-116">O Azure Ative Directory (AAD) símbolo de acesso na forma`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="519c4-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="519c4-117">Content-Type</span><span class="sxs-lookup"><span data-stu-id="519c4-117">Content-Type</span></span>    |    <span data-ttu-id="519c4-118">string</span><span class="sxs-lookup"><span data-stu-id="519c4-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="519c4-119">**Parâmetro do caminho**</span><span class="sxs-lookup"><span data-stu-id="519c4-119">**Path parameter**</span></span>

|    <span data-ttu-id="519c4-120">Nome do Parâmetro</span><span class="sxs-lookup"><span data-stu-id="519c4-120">Parameter Name</span></span>    |    <span data-ttu-id="519c4-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="519c4-121">Type</span></span>    |    <span data-ttu-id="519c4-122">Necessário</span><span class="sxs-lookup"><span data-stu-id="519c4-122">Required</span></span>    |    <span data-ttu-id="519c4-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="519c4-123">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="519c4-124">reportId</span><span class="sxs-lookup"><span data-stu-id="519c4-124">reportId</span></span>     |    <span data-ttu-id="519c4-125">cadeia (de carateres)</span><span class="sxs-lookup"><span data-stu-id="519c4-125">string</span></span>    |    <span data-ttu-id="519c4-126">No</span><span class="sxs-lookup"><span data-stu-id="519c4-126">No</span></span>    |    <span data-ttu-id="519c4-127">ID do relatório a ser modificado</span><span class="sxs-lookup"><span data-stu-id="519c4-127">ID of the report being modified</span></span>     |
|        |        |        |        |

<span data-ttu-id="519c4-128">**Parâmetro de consulta**</span><span class="sxs-lookup"><span data-stu-id="519c4-128">**Query parameter**</span></span>

<span data-ttu-id="519c4-129">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="519c4-129">None</span></span>

<span data-ttu-id="519c4-130">**Solicitar carga útil**</span><span class="sxs-lookup"><span data-stu-id="519c4-130">**Request payload**</span></span>

```json
{ 
  "ReportName": "string", 
  "Description": "string", 
  "StartTime": "string", 
  "RecurrenceInterval": 0, 
  "RecurrenceCount": 0, 
  "Format": "string", 
  "CallbackUrl": "string",
 "CallbackMethod": "string"
}
```

<span data-ttu-id="519c4-131">**Glossário**</span><span class="sxs-lookup"><span data-stu-id="519c4-131">**Glossary**</span></span>

<span data-ttu-id="519c4-132">Esta tabela lista as definições-chave dos elementos na resposta.</span><span class="sxs-lookup"><span data-stu-id="519c4-132">This table lists the key definitions of elements in the response.</span></span>

|    <span data-ttu-id="519c4-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="519c4-133">Parameter</span></span>    |    <span data-ttu-id="519c4-134">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="519c4-134">Required</span></span>    |    <span data-ttu-id="519c4-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="519c4-135">Description</span></span>    |    <span data-ttu-id="519c4-136">Valores Permitidos</span><span class="sxs-lookup"><span data-stu-id="519c4-136">Allowed Values</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="519c4-137">Nome do relatório</span><span class="sxs-lookup"><span data-stu-id="519c4-137">ReportName</span></span>     |    <span data-ttu-id="519c4-138">Yes</span><span class="sxs-lookup"><span data-stu-id="519c4-138">Yes</span></span>     |    <span data-ttu-id="519c4-139">Nome a atribuir ao relatório</span><span class="sxs-lookup"><span data-stu-id="519c4-139">Name to be assigned to the report</span></span>     |    <span data-ttu-id="519c4-140">String</span><span class="sxs-lookup"><span data-stu-id="519c4-140">String</span></span>     |
|    <span data-ttu-id="519c4-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="519c4-141">Description</span></span>     |    <span data-ttu-id="519c4-142">Não</span><span class="sxs-lookup"><span data-stu-id="519c4-142">No</span></span>     |    <span data-ttu-id="519c4-143">Descrição do relatório criado</span><span class="sxs-lookup"><span data-stu-id="519c4-143">Description of the created report</span></span>     |    <span data-ttu-id="519c4-144">String</span><span class="sxs-lookup"><span data-stu-id="519c4-144">String</span></span>     |
|    <span data-ttu-id="519c4-145">StartTime</span><span class="sxs-lookup"><span data-stu-id="519c4-145">StartTime</span></span>     |    <span data-ttu-id="519c4-146">Yes</span><span class="sxs-lookup"><span data-stu-id="519c4-146">Yes</span></span>    |    <span data-ttu-id="519c4-147">Timetamp após o qual a geração do relatório vai começar</span><span class="sxs-lookup"><span data-stu-id="519c4-147">Timestamp after which the report generation will begin</span></span>     |    <span data-ttu-id="519c4-148">String</span><span class="sxs-lookup"><span data-stu-id="519c4-148">String</span></span>     |
|    <span data-ttu-id="519c4-149">RecorrenceInterval</span><span class="sxs-lookup"><span data-stu-id="519c4-149">RecurrenceInterval</span></span>     |    <span data-ttu-id="519c4-150">No</span><span class="sxs-lookup"><span data-stu-id="519c4-150">No</span></span>     |    <span data-ttu-id="519c4-151">Frequência na qual o relatório deve ser gerado em horas.</span><span class="sxs-lookup"><span data-stu-id="519c4-151">Frequency at which the report should be generated in hours.</span></span> <span data-ttu-id="519c4-152">Valor mínimo é 4</span><span class="sxs-lookup"><span data-stu-id="519c4-152">Minimum value is 4</span></span>     |    <span data-ttu-id="519c4-153">Número inteiro</span><span class="sxs-lookup"><span data-stu-id="519c4-153">Integer</span></span>     |
|    <span data-ttu-id="519c4-154">RecorrenceCount</span><span class="sxs-lookup"><span data-stu-id="519c4-154">RecurrenceCount</span></span>     |    <span data-ttu-id="519c4-155">No</span><span class="sxs-lookup"><span data-stu-id="519c4-155">No</span></span>     |    <span data-ttu-id="519c4-156">Número de relatórios a serem gerados.</span><span class="sxs-lookup"><span data-stu-id="519c4-156">Numbers of report to be generated.</span></span> <span data-ttu-id="519c4-157">O padrão é indefinido.</span><span class="sxs-lookup"><span data-stu-id="519c4-157">Default is indefinite.</span></span>     |    <span data-ttu-id="519c4-158">Número inteiro</span><span class="sxs-lookup"><span data-stu-id="519c4-158">Integer</span></span>     |
|    <span data-ttu-id="519c4-159">Formato</span><span class="sxs-lookup"><span data-stu-id="519c4-159">Format</span></span>     |    <span data-ttu-id="519c4-160">No</span><span class="sxs-lookup"><span data-stu-id="519c4-160">No</span></span>    |    <span data-ttu-id="519c4-161">Formato de ficheiro do ficheiro exportado.</span><span class="sxs-lookup"><span data-stu-id="519c4-161">File format of the exported file.</span></span> <span data-ttu-id="519c4-162">O padrão é CSV</span><span class="sxs-lookup"><span data-stu-id="519c4-162">Default is CSV</span></span>     |    <span data-ttu-id="519c4-163">CSV/TSV</span><span class="sxs-lookup"><span data-stu-id="519c4-163">CSV/TSV</span></span>     |
|    <span data-ttu-id="519c4-164">CallbackURL</span><span class="sxs-lookup"><span data-stu-id="519c4-164">CallbackURL</span></span>     |    <span data-ttu-id="519c4-165">No</span><span class="sxs-lookup"><span data-stu-id="519c4-165">No</span></span>     |    <span data-ttu-id="519c4-166">URL de retorno https a ser chamado na geração de relatório</span><span class="sxs-lookup"><span data-stu-id="519c4-166">https callback URL to be called on report generation</span></span>     |    <span data-ttu-id="519c4-167">String</span><span class="sxs-lookup"><span data-stu-id="519c4-167">String</span></span>     |
|    <span data-ttu-id="519c4-168">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="519c4-168">CallbackMethod</span></span>    |    <span data-ttu-id="519c4-169">No</span><span class="sxs-lookup"><span data-stu-id="519c4-169">No</span></span>    |    <span data-ttu-id="519c4-170">Método http a ser usado para retorno</span><span class="sxs-lookup"><span data-stu-id="519c4-170">Http method to be used for callback</span></span>    |    <span data-ttu-id="519c4-171">GET/POST</span><span class="sxs-lookup"><span data-stu-id="519c4-171">GET/POST</span></span>    |
|        |        |        |        |


<span data-ttu-id="519c4-172">**Response**</span><span class="sxs-lookup"><span data-stu-id="519c4-172">**Response**</span></span>

<span data-ttu-id="519c4-173">A carga útil de resposta é estruturada da seguinte forma:</span><span class="sxs-lookup"><span data-stu-id="519c4-173">The response payload is structured as follows:</span></span>

<span data-ttu-id="519c4-174">Código de resposta: 200, 400, 401, 403, 404,500</span><span class="sxs-lookup"><span data-stu-id="519c4-174">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="519c4-175">Exemplo de carga útil de resposta:</span><span class="sxs-lookup"><span data-stu-id="519c4-175">Response payload example:</span></span>

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

<span data-ttu-id="519c4-176">**Glossário**</span><span class="sxs-lookup"><span data-stu-id="519c4-176">**Glossary**</span></span>

<span data-ttu-id="519c4-177">Esta tabela define os elementos-chave na resposta:</span><span class="sxs-lookup"><span data-stu-id="519c4-177">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="519c4-178">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="519c4-178">Parameter</span></span>    |    <span data-ttu-id="519c4-179">Descrição</span><span class="sxs-lookup"><span data-stu-id="519c4-179">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="519c4-180">ReportId</span><span class="sxs-lookup"><span data-stu-id="519c4-180">ReportId</span></span>     |    <span data-ttu-id="519c4-181">Identificador universalmente único (UUID) do relatório que está a ser atualizado</span><span class="sxs-lookup"><span data-stu-id="519c4-181">Universally unique identifier (UUID) of the report being updated</span></span>     |
|    <span data-ttu-id="519c4-182">Nome do relatório</span><span class="sxs-lookup"><span data-stu-id="519c4-182">ReportName</span></span>     |    <span data-ttu-id="519c4-183">Nome dado ao relatório na carga útil do pedido</span><span class="sxs-lookup"><span data-stu-id="519c4-183">Name given to the report in the request payload</span></span>     |
|    <span data-ttu-id="519c4-184">Descrição</span><span class="sxs-lookup"><span data-stu-id="519c4-184">Description</span></span>     |    <span data-ttu-id="519c4-185">Descrição dada ao relatório na carga útil do pedido</span><span class="sxs-lookup"><span data-stu-id="519c4-185">Description given to the report in the request payload</span></span>     |
|    <span data-ttu-id="519c4-186">QueryId</span><span class="sxs-lookup"><span data-stu-id="519c4-186">QueryId</span></span>     |    <span data-ttu-id="519c4-187">Consulta ID passou no momento em que o relatório foi criado</span><span class="sxs-lookup"><span data-stu-id="519c4-187">Query ID passed at the time the report was created</span></span>     |
|    <span data-ttu-id="519c4-188">Consulta</span><span class="sxs-lookup"><span data-stu-id="519c4-188">Query</span></span>     |    <span data-ttu-id="519c4-189">Texto de consulta que será executado para este relatório</span><span class="sxs-lookup"><span data-stu-id="519c4-189">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="519c4-190">Utilizador</span><span class="sxs-lookup"><span data-stu-id="519c4-190">User</span></span>     |    <span data-ttu-id="519c4-191">ID do utilizador usado para criar o relatório</span><span class="sxs-lookup"><span data-stu-id="519c4-191">User ID used to create the report</span></span>     |
|    <span data-ttu-id="519c4-192">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="519c4-192">CreatedTime</span></span>     |    <span data-ttu-id="519c4-193">Hora de criar o relatório.</span><span class="sxs-lookup"><span data-stu-id="519c4-193">Time the report was created.</span></span> <span data-ttu-id="519c4-194">O formato de tempo é yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="519c4-194">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="519c4-195">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="519c4-195">ModifiedTime</span></span>     |    <span data-ttu-id="519c4-196">Foi a última vez que o relatório foi modificado.</span><span class="sxs-lookup"><span data-stu-id="519c4-196">Time the report was last modified.</span></span> <span data-ttu-id="519c4-197">O formato de tempo é yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="519c4-197">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="519c4-198">Executar Agora</span><span class="sxs-lookup"><span data-stu-id="519c4-198">ExecuteNow</span></span>     |    <span data-ttu-id="519c4-199">ExecuteNow bandeira definida no momento em que o relatório foi criado</span><span class="sxs-lookup"><span data-stu-id="519c4-199">ExecuteNow flag set at the time the report was created</span></span>    |
|    <span data-ttu-id="519c4-200">StartTime</span><span class="sxs-lookup"><span data-stu-id="519c4-200">StartTime</span></span>     |    <span data-ttu-id="519c4-201">Quando começar a execução do relatório.</span><span class="sxs-lookup"><span data-stu-id="519c4-201">Time the report execution will begin.</span></span> <span data-ttu-id="519c4-202">O formato de tempo é yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="519c4-202">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="519c4-203">Relatório Estatísticas</span><span class="sxs-lookup"><span data-stu-id="519c4-203">ReportStatus</span></span>     |    <span data-ttu-id="519c4-204">Estado da execução do relatório.</span><span class="sxs-lookup"><span data-stu-id="519c4-204">Status of the report execution.</span></span> <span data-ttu-id="519c4-205">Os valores possíveis são Pausados, Ativos e Inativos.</span><span class="sxs-lookup"><span data-stu-id="519c4-205">The possible values are Paused, Active, and Inactive.</span></span>     |
|    <span data-ttu-id="519c4-206">RecorrenceInterval</span><span class="sxs-lookup"><span data-stu-id="519c4-206">RecurrenceInterval</span></span>     |    <span data-ttu-id="519c4-207">Intervalo de recorrência fornecido na carga útil do pedido</span><span class="sxs-lookup"><span data-stu-id="519c4-207">Recurrence interval provided in the request payload</span></span>     |
|    <span data-ttu-id="519c4-208">RecorrenceCount</span><span class="sxs-lookup"><span data-stu-id="519c4-208">RecurrenceCount</span></span>     |    <span data-ttu-id="519c4-209">Contagem de recorrência fornecida na carga útil do pedido</span><span class="sxs-lookup"><span data-stu-id="519c4-209">Recurrence count provided in the request payload</span></span>     |
|    <span data-ttu-id="519c4-210">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="519c4-210">CallbackUrl</span></span>     |    <span data-ttu-id="519c4-211">URL de retorno fornecido no pedido</span><span class="sxs-lookup"><span data-stu-id="519c4-211">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="519c4-212">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="519c4-212">CallbackMethod</span></span>    |    <span data-ttu-id="519c4-213">Método de retorno fornecido no pedido</span><span class="sxs-lookup"><span data-stu-id="519c4-213">Callback method provided in the request</span></span>    |
|    <span data-ttu-id="519c4-214">Formato</span><span class="sxs-lookup"><span data-stu-id="519c4-214">Format</span></span>     |    <span data-ttu-id="519c4-215">Formato dos ficheiros de relatório</span><span class="sxs-lookup"><span data-stu-id="519c4-215">Format of the report files</span></span>     |
|    <span data-ttu-id="519c4-216">TotalCount</span><span class="sxs-lookup"><span data-stu-id="519c4-216">TotalCount</span></span>     |    <span data-ttu-id="519c4-217">Número de conjuntos de dados na matriz de valor</span><span class="sxs-lookup"><span data-stu-id="519c4-217">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="519c4-218">Mensagem</span><span class="sxs-lookup"><span data-stu-id="519c4-218">Message</span></span>     |    <span data-ttu-id="519c4-219">Mensagem de estado da execução da API</span><span class="sxs-lookup"><span data-stu-id="519c4-219">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="519c4-220">Código de Estado</span><span class="sxs-lookup"><span data-stu-id="519c4-220">StatusCode</span></span>     |    <span data-ttu-id="519c4-221">Código de resultados.</span><span class="sxs-lookup"><span data-stu-id="519c4-221">Result Code.</span></span> <span data-ttu-id="519c4-222">Os valores possíveis são 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="519c4-222">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |