---
title: Especificação de consulta personalizada
description: Saiba como criar consultas personalizadas para extrair dados de tabelas de análise.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: 8749e9c65a232514028e0842a020267d0df7fcadcd9f36ac9dd9ba165377f401
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/06/2021
ms.locfileid: "115696921"
---
# <a name="custom-query-specification"></a>Especificação de consulta personalizada

Os parceiros podem usar esta especificação de consulta para formular facilmente consultas personalizadas para extrair dados de tabelas de análise. As consultas podem ser usadas para selecionar apenas as colunas e métricas desejadas que correspondam a um determinado critério. No centro da especificação linguística está a definição de conjunto de dados na qual uma consulta personalizada pode ser escrita.

## <a name="datasets"></a>Conjuntos de dados

Da mesma forma que algumas consultas são executadas contra uma base de dados que tem tabelas e colunas, uma consulta personalizada funciona em Datasets que têm colunas e métricas. A lista completa dos conjuntos de dados disponíveis para formular uma consulta pode ser obtida utilizando a API dos conjuntos de dados.

Este é um exemplo de um conjunto de dados mostrado como um JSON:

```json
{ 
      "datasetName": "OfficeUsage", 
      "selectableColumns": [ 
        "CustomerTenantId", 
        "CustomerTpid", 
        "WorkloadName", 
        "Month", 
        "PaidAvailableUnits", 
        "MonthlyActiveUsers", 
        "CustomerName", 
        "CustomerMarket", 
        "CustomerSegment",  
        "MPNId", 
        "PartnerName", 
        "PartnerLocation", 
        "PartnerAttributionType", 
        "IsDuplicateRowForPGA" 
      ], 
      "availableMetrics": [ 
        "CustomerCount", 
        "CustomerTenantCount", 
        "TotalPaidAvailableUnits", 
        "TotalMonthlyActiveUsers" 
      ], 
      "availableDateRanges": [ 
        "LAST_MONTH", 
        "LAST_3_MONTHS", 
        "LAST_6_MONTHS", 
        "LAST_1_YEAR", 
        "LIFETIME" 
      ], 
      "minimumRecurrenceInterval": 24 
    },
```

## <a name="parts-of-a-dataset"></a>Partes de um conjunto de dados

- Um nome de conjunto de dados é como um nome de tabela de base de dados. Por exemplo, OfficeUsage. Um conjunto de dados tem uma lista de colunas que podem ser selecionadas, como o CustomerTenantId.
- Um conjunto de dados também tem métricas, que são como funções de agregação numa base de dados. Por exemplo, TotalMonthlyActiveUsers.
- Existem períodos de tempo fixos sobre os quais os dados podem ser exportados.

## <a name="formulating-a-query-on-a-dataset"></a>Formular uma consulta num conjunto de dados

Estas são algumas consultas de amostra que mostram como extrair vários tipos de dados.

|Consulta|    Description    |
|----|    ----    |
|**SELECIONE** CustomerTenantId, Unidades Disponíveis Pagas **DE** <br>OfficeUsage **TIMESPAN** LAST_MONTH|    Esta consulta receberá todos os CusotmerTenantID e as respetivas Unidades Pagas Disponíveis no último 1 mês.    |
|**SELECIONE** CustomerTenantId, Unidades Disponíveis Pagas **DE** <br>Ordem de **ServiçoSUsage** BY PayAvailableUns **LIMIT** 10|    Esta consulta irá obter os 10 melhores inquilinos clientes em ordem decrescente do número de unidades disponíveis pagas.     |
|**SELECIONE** CustomerTenantId, PayAvailableUnits, MonthlyActiveUsers **FROM** OfficeUsage **WHERE** MonthlyActiveUsers > 100000 **ORDER BY** MonthlyActiveUsers **TIMESPAN** LAST_6_MONTHS |    Esta consulta receberá os Serviços PayAvailableUnits e MensaisActiveUsers de todos os Clientes que tenham MensalmenteActiveUsers superiores a 100.000.     |
|**SELECIONE** CustomerTenantId, Mês, MensalActiveUsers **FROM** <br>OfficeUsage **WHERE** CustomerTpId IN ('2a31c234-1f4e-4c60-909e-76d234f93161', '80780748-3f9a-11eb-b378-0242ac130002') |    Esta consulta irá obter o CustomerTenantId e os utilizadores ativos mensais por cada mês pelos dois valores Do ClienteTpIde: '2a31c234-1f4e-4c60-909e-76d234f93161' e '80780748-3f9a-11eb-b378-0242ac130002'.     |
|        |        |

## <a name="query-specification"></a>Especificação de consulta

Esta secção descreve a definição e estrutura da consulta.

## <a name="grammar-reference"></a>Referência gramatical

Esta tabela descreve os símbolos usados nas consultas.

|    Consulta    |    Description    |
|    ----    |    ----    |
|    `?`    |    Opcional    |
|    `*`    |    Zero ou mais    |
|    `+`    |    Um ou mais    |
|    `\|`    |    Ou / Uma das listas    |
|        |        |

## <a name="query-definition"></a>Definição de consulta

A declaração de consulta tem as seguintes cláusulas: SelectClause, FromClause, WhereClause, OrderClause, LimitClause e TimeSpan.

- **SelectClause:**`SELECT ColumOrMetricName (, ColumOrMetricName)*`
    - **Nome ColumOrMetricName**: Colunas e Métricas definidas no Conjunto de Dados
- **FromClause:**`FROM DatasetName`
    - **DatasetName**: Nome do conjunto de dados definido no Conjunto de Dados
- **Onde aClause:**`WHERE FilterCondition (AND FilterCondition)`
    - **FiltragemCondição**: Valor do operador columormétrico
        - **Operador:**`=` | `>` | `<` | `>=` | `<=` | `!=` | `LIKE` | `NOT LIKE` | `IN` | `NOT IN`
        - **Valor**: Número | | De CordasLiteral | MultiNumberList MultiStringList
            - **Número:**`-? [0-9]+ (. [0-9] [0-9]*)?`
            - **StringLiteral:**`' [a-zA-Z0-9_]*'`
            - **MultiNumberList:**`(Number (,Number)*)`
            - **MultiStringList:**`(StringLiteral (,StringLiteral)*)`
- **OrdemClause:**`ORDER BY OrderCondition (,OrderCondition)`
    - **Ordem:**`ColumOrMetricName (ASC | DESC)*`
- **LimitClause:**`LIMIT [0-9]+`
- **Intervalo temporal:**`TIMESPAN ( TODAY | YESTERDAY | LAST_7_DAYS | LAST_14_DAYS |LAST_30_DAYS | LAST_90_DAYS | LAST_180_DAYS | LAST_365_DAYS |LAST_MONTH | LAST_3_MONTHS | LAST_6_MONTHS | LAST_1_YEAR | LIFETIME)`

## <a name="query-structure"></a>Estrutura de Consulta

Uma consulta de relatório é composta por várias partes:
- `SELECT`
- `FROM`
- `WHERE`
- `ORDER BY`
- `LIMIT`
- `TIMESPAN`

Cada parte é descrita abaixo.

### `SELECT`

Esta parte da consulta especifica as colunas que serão exportadas. As colunas que podem ser selecionadas são os campos listados em *coalunos selecionáveis* e secções *métricas disponíveis* de um conjunto de dados.

Opcionalmente, `DISTINCT` a palavra-chave pode ser especificada depois `SELECT` . Se `DISTINCT` for especificado, as linhas exportadas finais contêm sempre valores distintos das colunas selecionadas. As métricas serão calculadas para cada combinação distinta das colunas selecionadas, pelo que `DISTINCT` a palavra-chave não é necessária quando uma coluna métrica é incluída na lista de colunas selecionadas.

**Exemplo:**

```sql
SELECT CustomerTenantId, PaidAvailableUnits; 
SELECT DISTINCT CustomerTenantId
```

### `FROM`

Esta parte da consulta indica o conjunto de dados a partir do qual os dados devem ser exportados. O nome do conjunto de dados aqui dado precisa de ser um nome de conjunto de dados válido devolvido pela API dos conjuntos de dados.

**Exemplo:**

- `FROM  OfficeUsage`
- `FROM  AzureUsage`

### `WHERE`

Esta parte da consulta é utilizada para especificar as condições do filtro no conjunto de dados. Apenas as linhas correspondentes a todas as condições enumeradas nesta cláusula estarão presentes no ficheiro final exportado. A condição do filtro pode estar em qualquer uma das colunas listadas em *coalunos selecionados* e *disponíveisMetricagens*. Os valores especificados na condição do filtro podem ser uma lista de números ou uma lista de cordas apenas quando o operador estiver `IN` ou `NOT IN` . Os valores podem sempre ser dados como uma corda literal e serão convertidos para os tipos nativos de colunas. As várias condições do filtro devem ser separadas com uma operação E.

**Exemplo:**

- `CustomerTenantId= '868368da-957d-4959-8992-3c12dc7e6260'`
- `CustomerName LIKE '%Contoso%'`
- `CustomerId NOT IN (1000, 1001, 1002)`
- `OrderQuantity=100`
- `CustomerTenantId='7b487ac0-ce12-b732-dcd6-91a1e4e74a50' AND CustomerTpId=' 0f8b7fa0-eb83-a183-1225-ca153ef807aa'`

### `ORDER BY`

Esta parte da consulta especifica os critérios de encomenda das linhas exportadas. As colunas sobre as quais a encomenda pode ser definida devem ser provenientes dos *alunos selecionados* e *disponíveisMetricagens* do conjunto de dados. Se não houver uma direção de encomenda especificada, será incumprida para o DESC na coluna. A encomenda pode ser definida em várias colunas separando os critérios com uma vírgula.

**Exemplo:**

- `ORDER BY  MonthlyActiveUsers ASC,  Month DESC`
- `ORDER BY CustomerName ASC,  Month`

### `LIMIT`

Esta parte da consulta especifica o número de linhas que serão exportadas. O número que especifica tem de ser um número não-número positivo.

### `TIMESPAN`

Esta parte da consulta especifica a duração para a qual os dados devem ser exportados. Os valores possíveis devem ser do campo *DisponíveisDateRanges* na definição de conjunto de dados.

### <a name="case-sensitivity-in-query-specification"></a>Sensibilidade do caso na especificação de consulta

A especificação é completamente insensível. Palavras-chave predefinidas, nomes de colunas e valores podem ser especificados utilizando maiúsão ou minúscula.

## <a name="next-steps"></a>Passos seguintes

- [Lista de consultas de sistema](insights-programmatic-system-queries.md)
- [Lista de consultas de amostra](insights-programmatic-sample-queries.md)