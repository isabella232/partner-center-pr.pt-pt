---
title: Eliminar consultas de relatório API - Informações dados
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: Utilize esta API para eliminar a consulta definida pelo utilizador nos insights do Partner Center.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: f755bc13ff4e0c4bc3a2c6ceda123c6a2bc47dc5
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/29/2021
ms.locfileid: "114836392"
---
# <a name="delete-report-queries-api"></a>Eliminar consultas de relatório API

Esta API elimina consultas definidas pelo utilizador.

**Solicitar sintaxe**

|    Método    |    URI do pedido    |
|    ----    |    ----    |
|    DELETE    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries/{queryId}` |
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
|    consultaD     |    cadeia (de carateres)     |    No    |    Filtrar para obter detalhes de apenas consultas com o ID dado no argumento     |
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
|    QueryId     |    UUID único da consulta que foi eliminada    |
|    Name     |    Nome da consulta que foi eliminada    |
|    Descrição     |    Descrição da consulta eliminada     |
|    Consulta     |    Cadeia de consulta de relatório da consulta eliminada    |
|    Tipo     |    Definir para utilizadorDefined para consultas criadas pelo utilizador     |
|    Utilizador     |    ID do utilizador que criou a consulta     |
|    CreatedTime     |    Tempo de criação de consulta     |
|    TotalCount     |    Número de conjuntos de dados na matriz de valor     |
|    Mensagem     |    Mensagem de estado da execução da API     |
|    Código de Estado     |    Código de resultados. Os valores possíveis são 200, 400, 401, 403, 500     |
|        |        |
