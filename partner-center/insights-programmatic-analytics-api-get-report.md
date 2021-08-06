---
title: Obtenha relatório API - dados Informações
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: Utilize esta API para obter toda a identificação de relatório disponível nos insights do Partner Center.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 9c6930d8be430f6a9219e7b3d11b2e64ed2af5253b81581581ad6254a2a1d8d3
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/06/2021
ms.locfileid: "115697147"
---
# <a name="get-report-api"></a>Obtenha relatório API

Esta API recebe todos os relatórios que foram agendados.

**Solicitar sintaxe**

|    Método    |    URI do pedido    |
|    ----    |    ----    |
|    GET    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport?reportId={Report ID}&reportName={Report Name}&queryId={Query ID}` |
|        |        |

**Cabeçalho de pedido**

|    Cabeçalho    |    Tipo    |    Description    |
|    ----    |    ----    |    ----    |
|    Autorização    |    string    |    Obrigatório. O Azure Ative Directory (AAD) símbolo de acesso na forma`Bearer <token>`    |
|    Content-Type    |    string    |    `Application/JSON`    |
|        |        |        |

**Parâmetro do caminho**

Nenhuma

**Parâmetro de consulta**

|    Nome do Parâmetro    |    Tipo    |    Necessário    |    Descrição    |
|    ----    |    ----    |    ----    |    ----    |
|    reportId     |    cadeia (de carateres)    |    No    |    Filtrar para obter detalhes de apenas relatórios com o reportId dado neste argumento     |
|    relatórioName     |    cadeia (de carateres)    |    No    |    Filtrar para obter detalhes de apenas relatórios com o relatórioName dado neste argumento     |
|    consultaD     |    cadeia (de carateres)    |    No    |    Filtrar para obter detalhes de apenas relatórios com a consulta dada neste argumento     |
|        |        |        |        |


**Solicitar carga útil**

Nenhuma

**Glossário**

Nenhuma

**Response**

A carga útil de resposta é estruturada da seguinte forma:

Código de resposta: 200, 400, 401, 403, 404,500

Exemplo de carga útil de resposta:

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

**Glossário**

Esta tabela define os elementos-chave na resposta:

|    Parâmetro    |    Descrição    |
|    ----    |    ----    |
|    ReportId     |    UUID único do relatório que foi criado     |
|    Nome do relatório     |    Nome dado ao relatório na carga útil do pedido     |
|    Description     |    Descrição dada quando o relatório foi criado     |
|    QueryId     |    Consulta ID passou no momento em que o relatório foi criado     |
|    Consulta     |    Texto de consulta que será executado para este relatório     |
|    Utilizador     |    ID do utilizador usado para criar o relatório     |
|    CreatedTime     |    Hora de criar o relatório. O formato de tempo é yyyy-MM-ddTHH:mm:ssZ     |
|    ModifiedTime     |    Foi a última vez que o relatório foi modificado. O formato de tempo é yyyy-MM-ddTHH:mm:ssZ     |
|    executarNow     |    ExecuteNow bandeira definida no momento em que o relatório foi criado    |
|    StartTime     |    A execução do tempo começará. O formato de tempo é yyyy-MM-ddTHH:mm:ssZ     |
|    Relatório Estatísticas     |    Estado da execução do relatório. Os valores possíveis são Pausados, Ativos e Inativos.     |
|    RecorrenceInterval     |    Intervalo de recorrência fornecido durante a criação do relatório     |
|    RecorrenceCount     |    Contagem de recorrência fornecida durante a criação do relatório     |
|    CallbackUrl     |    URL de retorno fornecido no pedido     |
|    CallbackMethod    |    Método de retorno fornecido no pedido    |
|    Formato     |    Formato dos ficheiros de relatório     |
|    TotalCount     |    Número de conjuntos de dados na matriz de valor     |
|    Mensagem     |    Mensagem de estado da execução da API     |
|    Código de Estado     |    Código de resultados. Os valores possíveis são 200, 400, 401, 403, 500     |
|        |        |