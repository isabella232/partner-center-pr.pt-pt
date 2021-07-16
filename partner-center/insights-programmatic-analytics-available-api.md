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
# <a name="available-apis-for-partner-insights-analytics"></a>APIs disponíveis para análise de insights de parceiros

Segue-se a lista de APIs para análise de insights de parceiros e as suas funcionalidades associadas.

## <a name="dataset-pull-apis"></a>ApIs de recolha de conjunto de dados

***Quadro 1: Dataset puxa APIs***

| **API** | **Funcionalidade** |
| --- | --- |
| [Obtenha todos os conjuntos de dados](insights-programmatic-analytics-api-get-dataset.md) | Obtém todos os conjuntos de dados disponíveis. Os conjuntos de dados listam as tabelas, colunas, métricas e intervalos de tempo. |
|||

## <a name="query-management-apis"></a>APIs de gestão de consultas

***Quadro 2: APIs de gestão de consultas***

| **API** | **Funcionalidade** |
| --- | --- |
| [Criar Consulta de Relatório](insights-programmatic-access-paradigm.md#create-report-query-api) | Cria consultas personalizadas que definem o conjunto de dados a partir do qual as colunas e métricas precisam de ser exportadas. |
| [GET Report Consulta](insights-programmatic-analytics-api-get-report-queries.md) | Obtém todas as consultas disponíveis para uso em relatórios. Obtém todo o sistema e consultas definidas pelo utilizador por padrão. |
| [Consulta de relatórios DELETE](insights-programmatic-analytics-api-delete-report-queries.md) | Elimina consultas definidas pelo utilizador. |
|||

## <a name="report-management-apis"></a>APIs de gestão de relatórios

***Quadro 3: ApIs de gestão de relatórios***

| **API** | **Funcionalidade** |
| --- | --- |
| [Criar Relatório](insights-programmatic-access-paradigm.md#create-report-api) | Agenda uma consulta a ser executada em intervalos regulares. |
| [CONSULTA DE RELATÓRIO DE TRY](insights-programmatic-analytics-api-try-report-queries.md) | Executa uma declaração de consulta de relatório. Devolve apenas 10 registos que um parceiro pode usar para verificar se os dados são como esperado. |
| [Get Report](insights-programmatic-analytics-api-get-report.md) | Receba todos os relatórios que foram agendados. |
| [Relatório de Atualização](insights-programmatic-analytics-api-update-report.md) | Modifique um parâmetro de relatório. |
| [Excluir Relatório](insights-programmatic-analytics-api-delete-report.md) | Elimina todos os registos de execução do relatório e reporta os registos de execução. |
| [Execuções do Relatório de Pausa](insights-programmatic-analytics-api-pause-report-executions.md) | Pausa na execução programada de relatórios. |
| [Retomar execuções de relatório](insights-programmatic-analytics-api-resume-report-executions.md) | Retoma a execução programada de um relatório pausado. |
|||

## <a name="report-execution-pull-apis"></a>Relatório de execução puxa APIs

***Quadro 4: Relatório de execução puxa APIs***

| **API** | **Funcionalidade** |
| --- | --- |
| [Obter Execuções de Relatório](insights-programmatic-access-paradigm.md#get-report-execution-api) | Pegue todas as execuções que aconteceram para um dado relatório. |
|||

## <a name="next-steps"></a>Passos seguintes

- Pode experimentar as APIs através do [URL da API swagger.](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html)