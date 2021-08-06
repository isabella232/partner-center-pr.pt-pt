---
title: Relatório de pausa execução API - dados Informações
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: Utilize esta API para interromper a execução de qualquer relatório nos insights do Partner Center.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 01bb70e46e5a80c039bfc90b2ac0a034aa73b1163f485af8b98676d756b73e18
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/06/2021
ms.locfileid: "115697164"
---
# <a name="pause-report-executions-api"></a>Pausa relatório execuções API

Na execução, esta API interrompe a execução programada de relatórios.

**Solicitar sintaxe**

|    Método    |    URI do pedido    |
|    ----    |    ----    |
|    PUT    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/pause/{ReportID}`    |
|        |        |

**Cabeçalho de pedido**

|    Cabeçalho    |    Tipo    |    Description    |
|    ----    |    ----    |    ----    |
|    Autorização    |    string    |    Obrigatório. O Azure Ative Directory (AAD) símbolo de acesso na forma`Bearer <token>`    |
|    Content-Type    |    string    |    `Application/JSON`    |
|        |        |        |

**Parâmetro do caminho**

|    Nome do Parâmetro    |    Tipo    |    Necessário    |    Descrição    |
|    ----    |    ----    |    ----    |    ----    |
|    reportId     |    cadeia (de carateres)    |    No    |    ID do relatório a ser modificado     |
|        |        |        |        |

**Parâmetro de consulta**

Nenhuma

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

**Glossário**

Esta tabela define os elementos-chave na resposta:

|    Parâmetro    |    Descrição    |
|    ----    |    ----    |
|    ReportId     |    Identificador universalmente único (UUID) do relatório pausado     |
|    Nome do relatório     |    Nome dado ao relatório durante a criação     |
|    Description     |    Descrição dada durante a criação do relatório     |
|    QueryId     |    Consulta ID passou no momento em que o relatório foi criado     |
|    Consulta     |    Texto de consulta que será executado para este relatório     |
|    Utilizador     |    ID do utilizador usado para criar o relatório     |
|    CreatedTime     |    Hora de criar o relatório. O formato de tempo é yyyy-MM-ddTHH:mm:ssZ     |
|    ModifiedTime     |    Foi a última vez que o relatório foi modificado. O formato de tempo é yyyy-MM-ddTHH:mm:ssZ     |
|    Executar Agora     |    ExecuteNow bandeira definida no momento em que o relatório foi criado     |
|    StartTime     |    Quando começar a execução do relatório. O formato de tempo é yyyy-MM-ddTHH:mm:ssZ     |
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
