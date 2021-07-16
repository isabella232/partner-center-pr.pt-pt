---
title: Experimente consultas de relatório API
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Utilize esta API para testar a sua consulta e validar os resultados em insights do Partner Center.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 13ad6fe385a4d31390b6806d863da3f647105b2c
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/16/2021
ms.locfileid: "114377181"
---
# <a name="try-report-queries-api"></a>Experimente consultas de relatório API

Esta API executa uma declaração de consulta de relatório. A API devolve apenas 100 registos que pode utilizar como parceiro para verificar se os dados são como esperava.

> [!IMPORTANT]
> Esta API tem um tempo de execução de consulta de 100 segundos. Se notar que a API está a demorar mais de 100 segundos, é muito provável que a consulta esteja sintaticamente correta ou então teria recebido um código de erro que não seja 200. A geração de relatórios efetivamente passará se a sintaxe de consulta estiver correta.

**Solicitar sintaxe**

|    Método    |    URI do pedido    |
|    ----    |    ----    |
|    GET    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries/testQueryResult?<exportQuery={query text}|queryId={queryId}>`    |
|        |        |

**Cabeçalho de pedido**

|    Cabeçalho    |    Tipo    |    Descrição    |
|    ----    |    ----    |    ----    |
|    Autorização    |    string    |    Obrigatório. O Azure Ative Directory (AAD) símbolo de acesso na forma`Bearer <token>`    |
|    Content-Type    |    string    |    `Application/JSON`    |
|        |        |        |

**Parâmetro do caminho**

Nenhuma

**Parâmetro de consulta**

|    Nome do Parâmetro    |    Tipo    |    Necessário    |    Descrição    |
|    ----    |    ----    |    ----    |    ----    |
|    exportaçãoQuery     |    cadeia (de carateres)    |    No    |    Cadeia de consulta de relatório que precisa ser executada     |
|    consultaD     |    cadeia (de carateres)    |    No    |    Um documento de consulta válido existente. Mutuamente exclusivo com cadeia de consulta especificada no parâmetro exportQuery    |
|    startTime     |    cadeia (de carateres)    |    No    |    Hora de início a partir da qual queremos os dados. Sobrepõe-se à timepan especificada na consulta    |
|    endTime     |    cadeia (de carateres)    |    No    |    Fim do tempo até que queremos os dados. Sobrepõe-se à timepan especificada na consulta    |
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
Top 100 rows of query execution 
{ 
  "Value": [ 
    { 
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
|    TotalCount     |    Número de conjuntos de dados na matriz de valor     |
|    Mensagem     |    Mensagem de estado da execução da API     |
|    Código de Estado     |    Código de resultados. Os valores possíveis são 200, 400, 401, 403, 500     |
|        |        |
