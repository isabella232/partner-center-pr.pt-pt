---
title: Eliminar relatório API - dados de Informações
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Utilize esta API para eliminar qualquer relatório nos insights do Partner Center.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: e060104f8f09f69c213ab1b22d4be08d58babced
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/16/2021
ms.locfileid: "114377216"
---
# <a name="delete-report-api"></a><span data-ttu-id="4312e-103">Apagar relatório API</span><span class="sxs-lookup"><span data-stu-id="4312e-103">Delete report API</span></span>

<span data-ttu-id="4312e-104">Na execução, esta API elimina todos os registos de execução do relatório e reporta os registos de execução.</span><span class="sxs-lookup"><span data-stu-id="4312e-104">On execution, this API deletes all of the report and report execution records.</span></span>

<span data-ttu-id="4312e-105">**Solicitar sintaxe**</span><span class="sxs-lookup"><span data-stu-id="4312e-105">**Request syntax**</span></span>

|    <span data-ttu-id="4312e-106">Método</span><span class="sxs-lookup"><span data-stu-id="4312e-106">Method</span></span>    |    <span data-ttu-id="4312e-107">URI do pedido</span><span class="sxs-lookup"><span data-stu-id="4312e-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="4312e-108">DELETE</span><span class="sxs-lookup"><span data-stu-id="4312e-108">DELETE</span></span>    |    ` https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/{Report ID}`    |
|        |        |

<span data-ttu-id="4312e-109">**Cabeçalho de pedido**</span><span class="sxs-lookup"><span data-stu-id="4312e-109">**Request header**</span></span>

|    <span data-ttu-id="4312e-110">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4312e-110">Header</span></span>    |    <span data-ttu-id="4312e-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="4312e-111">Type</span></span>    |    <span data-ttu-id="4312e-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="4312e-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="4312e-113">Autorização</span><span class="sxs-lookup"><span data-stu-id="4312e-113">Authorization</span></span>    |    <span data-ttu-id="4312e-114">string</span><span class="sxs-lookup"><span data-stu-id="4312e-114">string</span></span>    |    <span data-ttu-id="4312e-115">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4312e-115">Required.</span></span> <span data-ttu-id="4312e-116">O Azure Ative Directory (AAD) símbolo de acesso na forma`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="4312e-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="4312e-117">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4312e-117">Content-Type</span></span>    |    <span data-ttu-id="4312e-118">string</span><span class="sxs-lookup"><span data-stu-id="4312e-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="4312e-119">**Parâmetro do caminho**</span><span class="sxs-lookup"><span data-stu-id="4312e-119">**Path parameter**</span></span>

|    <span data-ttu-id="4312e-120">Nome do Parâmetro</span><span class="sxs-lookup"><span data-stu-id="4312e-120">Parameter Name</span></span>    |    <span data-ttu-id="4312e-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="4312e-121">Type</span></span>    |    <span data-ttu-id="4312e-122">Necessário</span><span class="sxs-lookup"><span data-stu-id="4312e-122">Required</span></span>    |    <span data-ttu-id="4312e-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="4312e-123">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="4312e-124">reportId</span><span class="sxs-lookup"><span data-stu-id="4312e-124">reportId</span></span>     |    <span data-ttu-id="4312e-125">cadeia (de carateres)</span><span class="sxs-lookup"><span data-stu-id="4312e-125">string</span></span>    |    <span data-ttu-id="4312e-126">No</span><span class="sxs-lookup"><span data-stu-id="4312e-126">No</span></span>    |    <span data-ttu-id="4312e-127">ID do relatório a ser apagado</span><span class="sxs-lookup"><span data-stu-id="4312e-127">ID of the report being deleted</span></span>    |
|        |        |        |        |

<span data-ttu-id="4312e-128">**Parâmetro de consulta**</span><span class="sxs-lookup"><span data-stu-id="4312e-128">**Query parameter**</span></span>

<span data-ttu-id="4312e-129">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="4312e-129">None</span></span>

<span data-ttu-id="4312e-130">**Solicitar carga útil**</span><span class="sxs-lookup"><span data-stu-id="4312e-130">**Request payload**</span></span>

<span data-ttu-id="4312e-131">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="4312e-131">None</span></span>

<span data-ttu-id="4312e-132">**Glossário**</span><span class="sxs-lookup"><span data-stu-id="4312e-132">**Glossary**</span></span>

<span data-ttu-id="4312e-133">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="4312e-133">None</span></span>

<span data-ttu-id="4312e-134">**Response**</span><span class="sxs-lookup"><span data-stu-id="4312e-134">**Response**</span></span>

<span data-ttu-id="4312e-135">A carga útil de resposta é estruturada da seguinte forma:</span><span class="sxs-lookup"><span data-stu-id="4312e-135">The response payload is structured as follows:</span></span>

<span data-ttu-id="4312e-136">Código de resposta: 200, 400, 401, 403, 404,500</span><span class="sxs-lookup"><span data-stu-id="4312e-136">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="4312e-137">Exemplo de carga útil de resposta:</span><span class="sxs-lookup"><span data-stu-id="4312e-137">Response payload example:</span></span>

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

<span data-ttu-id="4312e-138">**Glossário**</span><span class="sxs-lookup"><span data-stu-id="4312e-138">**Glossary**</span></span>

<span data-ttu-id="4312e-139">Esta tabela define os elementos-chave na resposta:</span><span class="sxs-lookup"><span data-stu-id="4312e-139">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="4312e-140">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="4312e-140">Parameter</span></span>    |    <span data-ttu-id="4312e-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="4312e-141">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="4312e-142">ReportId</span><span class="sxs-lookup"><span data-stu-id="4312e-142">ReportId</span></span>     |    <span data-ttu-id="4312e-143">Identificador universalmente único (UUID) do relatório eliminado</span><span class="sxs-lookup"><span data-stu-id="4312e-143">Universally unique identifier (UUID) of the deleted report</span></span>     |
|    <span data-ttu-id="4312e-144">Nome do relatório</span><span class="sxs-lookup"><span data-stu-id="4312e-144">ReportName</span></span>     |    <span data-ttu-id="4312e-145">Nome dado ao relatório durante a criação</span><span class="sxs-lookup"><span data-stu-id="4312e-145">Name given to the report during creation</span></span>     |
|    <span data-ttu-id="4312e-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="4312e-146">Description</span></span>     |    <span data-ttu-id="4312e-147">Descrição dada durante a criação do relatório</span><span class="sxs-lookup"><span data-stu-id="4312e-147">Description given during creation of the report</span></span>     |
|    <span data-ttu-id="4312e-148">QueryId</span><span class="sxs-lookup"><span data-stu-id="4312e-148">QueryId</span></span>     |    <span data-ttu-id="4312e-149">Consulta ID passou no momento em que o relatório foi criado</span><span class="sxs-lookup"><span data-stu-id="4312e-149">Query ID passed at the time the report was created</span></span>     |
|    <span data-ttu-id="4312e-150">Consulta</span><span class="sxs-lookup"><span data-stu-id="4312e-150">Query</span></span>     |    <span data-ttu-id="4312e-151">Texto de consulta que será executado para este relatório</span><span class="sxs-lookup"><span data-stu-id="4312e-151">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="4312e-152">Utilizador</span><span class="sxs-lookup"><span data-stu-id="4312e-152">User</span></span>     |    <span data-ttu-id="4312e-153">ID do utilizador usado para criar o relatório</span><span class="sxs-lookup"><span data-stu-id="4312e-153">User ID used to create the report</span></span>     |
|    <span data-ttu-id="4312e-154">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="4312e-154">CreatedTime</span></span>     |    <span data-ttu-id="4312e-155">Hora de criar o relatório.</span><span class="sxs-lookup"><span data-stu-id="4312e-155">Time the report was created.</span></span> <span data-ttu-id="4312e-156">O formato de tempo é yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="4312e-156">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="4312e-157">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="4312e-157">ModifiedTime</span></span>     |    <span data-ttu-id="4312e-158">Foi a última vez que o relatório foi modificado.</span><span class="sxs-lookup"><span data-stu-id="4312e-158">Time the report was last modified.</span></span> <span data-ttu-id="4312e-159">O formato de tempo é yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="4312e-159">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="4312e-160">Executar Agora</span><span class="sxs-lookup"><span data-stu-id="4312e-160">ExecuteNow</span></span>     |    <span data-ttu-id="4312e-161">ExecuteNow bandeira definida no momento em que o relatório foi criado</span><span class="sxs-lookup"><span data-stu-id="4312e-161">ExecuteNow flag set at the time the report was created</span></span>     |
|    <span data-ttu-id="4312e-162">StartTime</span><span class="sxs-lookup"><span data-stu-id="4312e-162">StartTime</span></span>     |    <span data-ttu-id="4312e-163">Quando começar a execução do relatório.</span><span class="sxs-lookup"><span data-stu-id="4312e-163">Time the report execution will begin.</span></span> <span data-ttu-id="4312e-164">O formato de tempo é yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="4312e-164">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="4312e-165">Relatório Estatísticas</span><span class="sxs-lookup"><span data-stu-id="4312e-165">ReportStatus</span></span>     |    <span data-ttu-id="4312e-166">Estado da execução do relatório.</span><span class="sxs-lookup"><span data-stu-id="4312e-166">Status of the report execution.</span></span> <span data-ttu-id="4312e-167">Os valores possíveis são Pausados, Ativos e Inativos.</span><span class="sxs-lookup"><span data-stu-id="4312e-167">The possible values are Paused, Active, and Inactive.</span></span>     |
|    <span data-ttu-id="4312e-168">RecorrenceInterval</span><span class="sxs-lookup"><span data-stu-id="4312e-168">RecurrenceInterval</span></span>     |    <span data-ttu-id="4312e-169">Intervalo de recorrência fornecido durante a criação do relatório</span><span class="sxs-lookup"><span data-stu-id="4312e-169">Recurrence interval provided during report creation</span></span>     |
|    <span data-ttu-id="4312e-170">RecorrenceCount</span><span class="sxs-lookup"><span data-stu-id="4312e-170">RecurrenceCount</span></span>     |    <span data-ttu-id="4312e-171">Contagem de recorrência fornecida durante a criação do relatório</span><span class="sxs-lookup"><span data-stu-id="4312e-171">Recurrence count provided during report creation</span></span>     |
|    <span data-ttu-id="4312e-172">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="4312e-172">CallbackUrl</span></span>     |    <span data-ttu-id="4312e-173">URL de retorno fornecido no pedido</span><span class="sxs-lookup"><span data-stu-id="4312e-173">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="4312e-174">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="4312e-174">CallbackMethod</span></span>    |    <span data-ttu-id="4312e-175">Método de retorno fornecido no pedido</span><span class="sxs-lookup"><span data-stu-id="4312e-175">Callback method provided in the request</span></span>    |
|    <span data-ttu-id="4312e-176">Formato</span><span class="sxs-lookup"><span data-stu-id="4312e-176">Format</span></span>     |    <span data-ttu-id="4312e-177">Formato dos ficheiros de relatório</span><span class="sxs-lookup"><span data-stu-id="4312e-177">Format of the report files</span></span>     |
|    <span data-ttu-id="4312e-178">TotalCount</span><span class="sxs-lookup"><span data-stu-id="4312e-178">TotalCount</span></span>     |    <span data-ttu-id="4312e-179">Número de conjuntos de dados na matriz de valor</span><span class="sxs-lookup"><span data-stu-id="4312e-179">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="4312e-180">Mensagem</span><span class="sxs-lookup"><span data-stu-id="4312e-180">Message</span></span>     |    <span data-ttu-id="4312e-181">Mensagem de estado da execução da API</span><span class="sxs-lookup"><span data-stu-id="4312e-181">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="4312e-182">Código de Estado</span><span class="sxs-lookup"><span data-stu-id="4312e-182">StatusCode</span></span>     |    <span data-ttu-id="4312e-183">Código de resultados.</span><span class="sxs-lookup"><span data-stu-id="4312e-183">Result Code.</span></span> <span data-ttu-id="4312e-184">Os valores possíveis são 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="4312e-184">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
