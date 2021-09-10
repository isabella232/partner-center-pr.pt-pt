---
title: Obtenha consultas de relatório API - dados Informações
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: Utilize esta API para obter todas as consultas disponíveis para uso no relatório API.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 5f65784ce93350c92e0ffe38849ce505f045e0b0
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/09/2021
ms.locfileid: "123960909"
---
# <a name="get-report-queries-api"></a>Obtenha consultas de relatório API

O relatório Get consultas API obtém todas as consultas que estão disponíveis para uso em relatórios. Obtém todo o sistema e consultas definidas pelo utilizador por padrão.

**Solicitar sintaxe**

|    Método    |    URI do pedido    |
|    ----    |    ----    |
|    GET    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries?queryId={QueryID}&queryName={QueryName}&includeSystemQueries={include_system_queries}&includeOnlySystemQueries={include_only_system_queries}`     |
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
|    consultaD     |    cadeia (de carateres)     |    No    |    Filtrar para obter detalhes de apenas consultas com o ID dado no argumento     |
|    consultaName     |    cadeia (de carateres)     |    No    |    Filtrar para obter detalhes de apenas consultas com o nome dado no argumento     |
|    Incluir Sistemaqueries     |    boolean     |    No    |    Incluir consultas de sistema predefinidas na resposta     |
|    Incluir Apenas SistemasQueries     |    boolean     |    No    |    Incluir apenas consultas de sistema na resposta     |
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
      "QueryId": "string", 
      "Name": "string", 
      "Description": "string", 
      "Query": "string", 
      "Type": "string", 
      "User": "string", 
      "CreatedTime": "string", 
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
|    QueryId     |    UUID único da consulta     |
|    Name     |    Nome dado à consulta no momento da criação de consultas     |
|    Description     |    Descrição dada durante a criação da consulta     |
|    Consulta     |    Cadeia de consulta de relatório     |
|    Tipo     |    Conjunto para utilizadorDefined para consultas e sistema criados pelo utilizador para consultas de sistema predefinidos     |
|    Utilizador     |    ID do utilizador que criou a consulta     |
|    CreatedTime     |    Tempo de criação de consulta     |
|    TotalCount     |    Número de conjuntos de dados na matriz de valor     |
|    Mensagem     |    Mensagem de estado da execução da API     |
|    Código de Estado     |    Código de resultados. Os valores possíveis são 200, 400, 401, 403, 500     |
|        |        |
