---
title: Questões comuns para o acesso programático de insights de parceiros
description: Obtenha respostas a perguntas comumente feitas sobre o acesso a dados de insights de parceiros através da API.
ms.topic: troubleshooting
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: 418af23ae50e1f8d9086b2eb6247ba964e4c1516
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/09/2021
ms.locfileid: "123961399"
---
# <a name="programmatic-access-of-analytics-data-common-questions"></a>Perguntas comuns sobre o acesso programático dos dados de análise

Este artigo aborda perguntas comumente sobre como aceder programáticamente aos dados de insights de parceiros no Partner Center.

## <a name="api-responses"></a>Respostas da API

Quais são os diferentes cenários em que posso receber uma resposta da API que não seja 200 (Sucesso)?

Esta tabela descreve as respostas da API e o que fazer se as receber.

|    Descrição do erro     |    Código de erro     |    Resolução de problemas     |
|    ----    |    ----    |    ----    |
|    Não autorizado     |    401     |    Esta é uma exceção de autenticação. Verifique a correção do token Azure Ative Directory (AAD). O token AAD é válido por 60 minutos, após o qual você precisaria regenerar o token AAD.     |
|    Nome de mesa inválido     |    400     |    O nome do conjunto de dados está errado. Recheck o nome do conjunto de dados chamando a API "Get All Datasets".     |
|    Nome da coluna incorreta     |    400     |    O nome da coluna na consulta está incorreto. Recheck o nome da coluna chamando a API "Obter todos os conjuntos de dados" ou consulte os nomes das colunas nas Definições de Dados    |
|    Valor nulo ou em falta     |    400     |    Pode estar a faltar parâmetros obrigatórios como parte da carga útil do pedido da API.     |
|    Parâmetros de relatório inválidos     |    400     |    Certifique-se de que os parâmetros do relatório estão corretos. Por exemplo, pode estar a dar um valor inferior a 4 para o parâmetro RecorrenceInterval.     |
|    Intervalo de recorrência deve ser entre 4 e 2160     |    400     |    Certifique-se de que o valor do parâmetro de pedido RecorrenceInterval está entre 4 e 2160.     |
|    Querid inválido     |    400     |    Rever a Consulta gerada.     |
|    Parâmetros de relatório inválidos para a criação - A hora de início do relatório deve ser pelo menos 4 horas a partir do tempo atual utc     |    400     |    O parâmetro tempo de início como parte da carga útil do pedido não deve ser no passado. A hora de início do relatório deve ser de, pelo menos, 4 horas a partir da hora atual da UTC.     |
|    Valor solicitado 'string' não encontrado     |    400     |    Verifique se atualizou os parâmetros ou formato do `callbackurl` pedido.     |
|    Nenhum item encontrado com filtros dados.     |    404     |    Verifique o parâmetro reportID utilizado na API get executões de relatório.     |
|    Não há execuções que tenham ocorrido para as condições de filtro dadas. Verifique duas vezes o relatórioId ou execuçãoId e volte a julgar a API após o tempo de execução programado do relatório     |    404     |    Certifique-se de que o relatórioid está correto. Recandidutar a API após o tempo de execução programado do relatório, conforme especificado na carga útil do pedido.     |
|    Erro interno encontrado durante a criação de relatório. ID de correlação <>     |    500     |    Certifique-se de que o formato de data para os campos *StartTime,* *QueryStartTime* e *QueryEndTime* estão corretos.     |
|    Serviço indisponível    |    500     |    Se receber continuamente um serviço indisponível (erro 5xx), abra um bilhete de apoio.    |
|        |        |        |

## <a name="no-records"></a>Sem registos.

Recebo resposta da API 200 quando descarrego o relatório do local seguro. Porque é que não estou a receber registos?
Verifique se o fio na consulta tem um dos valores admissíveis para o cabeçalho da coluna. Por exemplo, esta consulta devolverá zero resultados:

```sql
SELECT CustomerTenantId, CustomerTpId, WorkloadName, Month, MonthlyActiveUsers 
FROM OfficeUsage 
WHERE IsDuplicateRowForPGA = 'False' 
ORDER BY CustomerTenantId DESC
```

Neste exemplo, os valores admissíveis `IsDuplicateRowForPGA` são 0 ou 1. Consulte as [Definições de Dados](insights-data-definitions.md) para todos os valores possíveis para as várias colunas.
