---
title: Lista de API para aceder a dados de insights de parceiros
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lista de API para aceder a dados de insights de parceiros.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 71d04b6927e27b1d7a8d72bbdaa56b41cb113625
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/16/2021
ms.locfileid: "114377169"
---
# <a name="available-apis-for-partner-insights-analytics"></a><span data-ttu-id="b0a3e-103">APIs disponíveis para análise de insights de parceiros</span><span class="sxs-lookup"><span data-stu-id="b0a3e-103">Available APIs for partner insights analytics</span></span>

<span data-ttu-id="b0a3e-104">Segue-se a lista de APIs para análise de insights de parceiros e as suas funcionalidades associadas.</span><span class="sxs-lookup"><span data-stu-id="b0a3e-104">Following are the list of APIs for partner insights analytics and their associated functionalities.</span></span>

## <a name="dataset-pull-apis"></a><span data-ttu-id="b0a3e-105">ApIs de recolha de conjunto de dados</span><span class="sxs-lookup"><span data-stu-id="b0a3e-105">Dataset pull APIs</span></span>

<span data-ttu-id="b0a3e-106">***Quadro 1: Dataset puxa APIs***</span><span class="sxs-lookup"><span data-stu-id="b0a3e-106">***Table 1: Dataset pull APIs***</span></span>

| <span data-ttu-id="b0a3e-107">**API**</span><span class="sxs-lookup"><span data-stu-id="b0a3e-107">**API**</span></span> | <span data-ttu-id="b0a3e-108">**Funcionalidade**</span><span class="sxs-lookup"><span data-stu-id="b0a3e-108">**Functionality**</span></span> |
| --- | --- |
| [<span data-ttu-id="b0a3e-109">Obtenha todos os conjuntos de dados</span><span class="sxs-lookup"><span data-stu-id="b0a3e-109">Get all datasets</span></span>](insights-programmatic-analytics-api-get-dataset.md) | <span data-ttu-id="b0a3e-110">Obtém todos os conjuntos de dados disponíveis.</span><span class="sxs-lookup"><span data-stu-id="b0a3e-110">Gets all the available datasets.</span></span> <span data-ttu-id="b0a3e-111">Os conjuntos de dados listam as tabelas, colunas, métricas e intervalos de tempo.</span><span class="sxs-lookup"><span data-stu-id="b0a3e-111">Datasets list the tables, columns, metrics, and time ranges.</span></span> |
|||

## <a name="query-management-apis"></a><span data-ttu-id="b0a3e-112">APIs de gestão de consultas</span><span class="sxs-lookup"><span data-stu-id="b0a3e-112">Query management APIs</span></span>

<span data-ttu-id="b0a3e-113">***Quadro 2: APIs de gestão de consultas***</span><span class="sxs-lookup"><span data-stu-id="b0a3e-113">***Table 2: Query management APIs***</span></span>

| <span data-ttu-id="b0a3e-114">**API**</span><span class="sxs-lookup"><span data-stu-id="b0a3e-114">**API**</span></span> | <span data-ttu-id="b0a3e-115">**Funcionalidade**</span><span class="sxs-lookup"><span data-stu-id="b0a3e-115">**Functionality**</span></span> |
| --- | --- |
| [<span data-ttu-id="b0a3e-116">Criar Consulta de Relatório</span><span class="sxs-lookup"><span data-stu-id="b0a3e-116">Create Report Query</span></span>](insights-programmatic-access-paradigm.md#create-report-query-api) | <span data-ttu-id="b0a3e-117">Cria consultas personalizadas que definem o conjunto de dados a partir do qual as colunas e métricas precisam de ser exportadas.</span><span class="sxs-lookup"><span data-stu-id="b0a3e-117">Creates custom queries that define the dataset from which columns and metrics need to be exported.</span></span> |
| [<span data-ttu-id="b0a3e-118">GET Report Consulta</span><span class="sxs-lookup"><span data-stu-id="b0a3e-118">GET Report Query</span></span>](insights-programmatic-analytics-api-get-report-queries.md) | <span data-ttu-id="b0a3e-119">Obtém todas as consultas disponíveis para uso em relatórios.</span><span class="sxs-lookup"><span data-stu-id="b0a3e-119">Gets all the queries available for use in reports.</span></span> <span data-ttu-id="b0a3e-120">Obtém todo o sistema e consultas definidas pelo utilizador por padrão.</span><span class="sxs-lookup"><span data-stu-id="b0a3e-120">Gets all the system and user-defined queries by default.</span></span> |
| [<span data-ttu-id="b0a3e-121">Consulta de relatórios DELETE</span><span class="sxs-lookup"><span data-stu-id="b0a3e-121">DELETE Report Query</span></span>](insights-programmatic-analytics-api-delete-report-queries.md) | <span data-ttu-id="b0a3e-122">Elimina consultas definidas pelo utilizador.</span><span class="sxs-lookup"><span data-stu-id="b0a3e-122">Deletes user-defined queries.</span></span> |
|||

## <a name="report-management-apis"></a><span data-ttu-id="b0a3e-123">APIs de gestão de relatórios</span><span class="sxs-lookup"><span data-stu-id="b0a3e-123">Report management APIs</span></span>

<span data-ttu-id="b0a3e-124">***Quadro 3: ApIs de gestão de relatórios***</span><span class="sxs-lookup"><span data-stu-id="b0a3e-124">***Table 3: Report management APIs***</span></span>

| <span data-ttu-id="b0a3e-125">**API**</span><span class="sxs-lookup"><span data-stu-id="b0a3e-125">**API**</span></span> | <span data-ttu-id="b0a3e-126">**Funcionalidade**</span><span class="sxs-lookup"><span data-stu-id="b0a3e-126">**Functionality**</span></span> |
| --- | --- |
| [<span data-ttu-id="b0a3e-127">Criar Relatório</span><span class="sxs-lookup"><span data-stu-id="b0a3e-127">Create Report</span></span>](insights-programmatic-access-paradigm.md#create-report-api) | <span data-ttu-id="b0a3e-128">Agenda uma consulta a ser executada em intervalos regulares.</span><span class="sxs-lookup"><span data-stu-id="b0a3e-128">Schedules a query to be executed at regular intervals.</span></span> |
| [<span data-ttu-id="b0a3e-129">CONSULTA DE RELATÓRIO DE TRY</span><span class="sxs-lookup"><span data-stu-id="b0a3e-129">TRY Report Query</span></span>](insights-programmatic-analytics-api-try-report-queries.md) | <span data-ttu-id="b0a3e-130">Executa uma declaração de consulta de relatório.</span><span class="sxs-lookup"><span data-stu-id="b0a3e-130">Executes a Report query statement.</span></span> <span data-ttu-id="b0a3e-131">Devolve apenas 10 registos que um parceiro pode usar para verificar se os dados são como esperado.</span><span class="sxs-lookup"><span data-stu-id="b0a3e-131">Returns only 10 records that a partner can use to verify if the data is as expected.</span></span> |
| [<span data-ttu-id="b0a3e-132">Get Report</span><span class="sxs-lookup"><span data-stu-id="b0a3e-132">Get Report</span></span>](insights-programmatic-analytics-api-get-report.md) | <span data-ttu-id="b0a3e-133">Receba todos os relatórios que foram agendados.</span><span class="sxs-lookup"><span data-stu-id="b0a3e-133">Get all the reports that have been scheduled.</span></span> |
| [<span data-ttu-id="b0a3e-134">Relatório de Atualização</span><span class="sxs-lookup"><span data-stu-id="b0a3e-134">Update Report</span></span>](insights-programmatic-analytics-api-update-report.md) | <span data-ttu-id="b0a3e-135">Modifique um parâmetro de relatório.</span><span class="sxs-lookup"><span data-stu-id="b0a3e-135">Modify a report parameter.</span></span> |
| [<span data-ttu-id="b0a3e-136">Excluir Relatório</span><span class="sxs-lookup"><span data-stu-id="b0a3e-136">Delete Report</span></span>](insights-programmatic-analytics-api-delete-report.md) | <span data-ttu-id="b0a3e-137">Elimina todos os registos de execução do relatório e reporta os registos de execução.</span><span class="sxs-lookup"><span data-stu-id="b0a3e-137">Deletes all the report and report execution records.</span></span> |
| [<span data-ttu-id="b0a3e-138">Execuções do Relatório de Pausa</span><span class="sxs-lookup"><span data-stu-id="b0a3e-138">Pause Report Executions</span></span>](insights-programmatic-analytics-api-pause-report-executions.md) | <span data-ttu-id="b0a3e-139">Pausa na execução programada de relatórios.</span><span class="sxs-lookup"><span data-stu-id="b0a3e-139">Pauses the scheduled execution of reports.</span></span> |
| [<span data-ttu-id="b0a3e-140">Retomar execuções de relatório</span><span class="sxs-lookup"><span data-stu-id="b0a3e-140">Resume Report Executions</span></span>](insights-programmatic-analytics-api-resume-report-executions.md) | <span data-ttu-id="b0a3e-141">Retoma a execução programada de um relatório pausado.</span><span class="sxs-lookup"><span data-stu-id="b0a3e-141">Resumes the scheduled execution of a paused report.</span></span> |
|||

## <a name="report-execution-pull-apis"></a><span data-ttu-id="b0a3e-142">Relatório de execução puxa APIs</span><span class="sxs-lookup"><span data-stu-id="b0a3e-142">Report execution pull APIs</span></span>

<span data-ttu-id="b0a3e-143">***Quadro 4: Relatório de execução puxa APIs***</span><span class="sxs-lookup"><span data-stu-id="b0a3e-143">***Table 4: Report execution pull APIs***</span></span>

| <span data-ttu-id="b0a3e-144">**API**</span><span class="sxs-lookup"><span data-stu-id="b0a3e-144">**API**</span></span> | <span data-ttu-id="b0a3e-145">**Funcionalidade**</span><span class="sxs-lookup"><span data-stu-id="b0a3e-145">**Functionality**</span></span> |
| --- | --- |
| [<span data-ttu-id="b0a3e-146">Obter Execuções de Relatório</span><span class="sxs-lookup"><span data-stu-id="b0a3e-146">Get Report Executions</span></span>](insights-programmatic-access-paradigm.md#get-report-execution-api) | <span data-ttu-id="b0a3e-147">Pegue todas as execuções que aconteceram para um dado relatório.</span><span class="sxs-lookup"><span data-stu-id="b0a3e-147">Get all the executions that have happened for a given report.</span></span> |
|||

## <a name="next-steps"></a><span data-ttu-id="b0a3e-148">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="b0a3e-148">Next steps</span></span>

- <span data-ttu-id="b0a3e-149">Pode experimentar as APIs através do [URL da API swagger.](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html)</span><span class="sxs-lookup"><span data-stu-id="b0a3e-149">You can try out the APIs through the [Swagger API URL](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html).</span></span>