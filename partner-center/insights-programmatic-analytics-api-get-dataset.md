---
title: Obtenha todos os conjuntos de dados API - Informações dados
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: Utilize esta API para obter detalhes de todos os conjuntos de dados disponíveis em insights do Partner Center.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 8f4e69c8759c16bc38e64a361c8c077989447d3e
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/29/2021
ms.locfileid: "114843804"
---
# <a name="get-all-datasets-api"></a>Obtenha todos os conjuntos de dados API

A API obtém todos os conjuntos de dados que a API obtém todos os conjuntos de dados disponíveis. Os conjuntos de dados listam as tabelas, colunas, métricas e intervalos de tempo.

**Solicitar sintaxe**

|    Método    |    URI do pedido    |
|    ----    |    ----    |
|    GET    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledDataset?datasetName={Dataset Name}`     |
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
|    datasetName    |    cadeia (de carateres)    |    No    |    Filtrar para obter detalhes de apenas um conjunto de dados    |
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
   "Value":[ 
      { 
         "DatasetName ":"string", 
         "SelectableColumns":[ 
            "string" 
         ], 
         "AvailableMetrics":[ 
            "string" 
         ], 
         "AvailableDateRanges":[ 
            "string" 
         ], 
         "minimumRecurrenceInterval":0 
      } 
   ], 
   "TotalCount":0, 
   "Message":"<Error Message>", 
   "StatusCode": 0, 
} 
```

**Glossário**

Esta tabela define os elementos-chave na resposta:

|    Parâmetro    |    Descrição    |
|    ----    |    ----    |
|    DatasetName     |    Nome do conjunto de dados que este objeto de matriz define     |
|    Universidades selecionadas     |    Colunas em bruto que podem ser especificadas nas colunas selecionadas     |
|    Métrica Disponível     |    Nomes de colunas agregação/métrica que podem ser especificados nas colunas selecionadas     |
|    DisponíveisDateRanges     |    Intervalo de datas que pode ser usado em consultas de relatório para o conjunto de dados     |
|    mínimoRecurrenceInterval     |    Valor mínimo do Intervalo de Recorrência     |
|    TotalCount     |    Número de conjuntos de dados na matriz de valor     |
|    Mensagem     |    Mensagem de estado da execução da API     |
|    Código de Estado     |    Código de resultados. Os valores possíveis são 200, 400, 401, 403, 500     |
|        |        |
