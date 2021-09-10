---
title: Eliminar relatório API - dados de Informações
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: Utilize esta API para eliminar qualquer relatório nos insights do Partner Center.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: a8a94fc1a6e69bab0a7671bd27949e271a77dbbe
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/09/2021
ms.locfileid: "123960889"
---
# <a name="delete-report-api"></a>Apagar relatório API

Na execução, esta API elimina todos os registos de execução do relatório e reporta os registos de execução.

**Solicitar sintaxe**

|    Método    |    URI do pedido    |
|    ----    |    ----    |
|    DELETE    |    ` https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/{Report ID}`    |
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
|    reportId     |    cadeia (de carateres)    |    No    |    ID do relatório a ser apagado    |
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
|    ReportId     |    Identificador universalmente único (UUID) do relatório eliminado     |
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
