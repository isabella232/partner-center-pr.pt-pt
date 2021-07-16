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
# <a name="update-report-api"></a>Relatório de atualização API

Esta API ajuda-o a modificar um parâmetro de relatório.

**Solicitar sintaxe**

|    Método    |    URI do pedido    |
|    ----    |    ----    |
|    PUT    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/{Report ID}`    |
|        |        |

**Cabeçalho de pedido**

|    Cabeçalho    |    Tipo    |    Descrição    |
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

**Glossário**

Esta tabela lista as definições-chave dos elementos na resposta.

|    Parâmetro    |    Obrigatório    |    Descrição    |    Valores Permitidos    |
|    ----    |    ----    |    ----    |    ----    |
|    Nome do relatório     |    Yes     |    Nome a atribuir ao relatório     |    String     |
|    Descrição     |    Não     |    Descrição do relatório criado     |    String     |
|    StartTime     |    Yes    |    Timetamp após o qual a geração do relatório vai começar     |    String     |
|    RecorrenceInterval     |    No     |    Frequência na qual o relatório deve ser gerado em horas. Valor mínimo é 4     |    Número inteiro     |
|    RecorrenceCount     |    No     |    Número de relatórios a serem gerados. O padrão é indefinido.     |    Número inteiro     |
|    Formato     |    No    |    Formato de ficheiro do ficheiro exportado. O padrão é CSV     |    CSV/TSV     |
|    CallbackURL     |    No     |    URL de retorno https a ser chamado na geração de relatório     |    String     |
|    CallbackMethod    |    No    |    Método http a ser usado para retorno    |    GET/POST    |
|        |        |        |        |


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
|    ReportId     |    Identificador universalmente único (UUID) do relatório que está a ser atualizado     |
|    Nome do relatório     |    Nome dado ao relatório na carga útil do pedido     |
|    Descrição     |    Descrição dada ao relatório na carga útil do pedido     |
|    QueryId     |    Consulta ID passou no momento em que o relatório foi criado     |
|    Consulta     |    Texto de consulta que será executado para este relatório     |
|    Utilizador     |    ID do utilizador usado para criar o relatório     |
|    CreatedTime     |    Hora de criar o relatório. O formato de tempo é yyyy-MM-ddTHH:mm:ssZ     |
|    ModifiedTime     |    Foi a última vez que o relatório foi modificado. O formato de tempo é yyyy-MM-ddTHH:mm:ssZ     |
|    Executar Agora     |    ExecuteNow bandeira definida no momento em que o relatório foi criado    |
|    StartTime     |    Quando começar a execução do relatório. O formato de tempo é yyyy-MM-ddTHH:mm:ssZ     |
|    Relatório Estatísticas     |    Estado da execução do relatório. Os valores possíveis são Pausados, Ativos e Inativos.     |
|    RecorrenceInterval     |    Intervalo de recorrência fornecido na carga útil do pedido     |
|    RecorrenceCount     |    Contagem de recorrência fornecida na carga útil do pedido     |
|    CallbackUrl     |    URL de retorno fornecido no pedido     |
|    CallbackMethod    |    Método de retorno fornecido no pedido    |
|    Formato     |    Formato dos ficheiros de relatório     |
|    TotalCount     |    Número de conjuntos de dados na matriz de valor     |
|    Mensagem     |    Mensagem de estado da execução da API     |
|    Código de Estado     |    Código de resultados. Os valores possíveis são 200, 400, 401, 403, 500     |
|        |        |