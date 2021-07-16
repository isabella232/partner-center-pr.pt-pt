---
title: Paradigma de acesso programático para dados Informações
description: Compreenda o fluxo de alto nível do padrão de chamada da API para análise programática. As APIs para aceder a relatórios de análise de insights de parceiros também são abrangidas.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: dcdd54fcc744fdb1683259203188c309a3949eff
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376981"
---
# <a name="programmatic-access-paradigm"></a>Paradigma de acesso programático

Este diagrama mostra o padrão de chamada da API usado para criar um novo modelo de relatório, agendar o relatório personalizado e recuperar dados de falha.

:::image type="content" source="images/insights/prog-acc-paradigm.png" alt-text="Fluxo de alto nível":::
***Figura 1: Fluxo de alto nível do padrão de chamada API***

Esta lista fornece mais detalhes sobre a Figura 1.

1. A Aplicação do Cliente pode definir o esquema/modelo de relatório personalizado, chamando a [API de Consulta de Relatório de Criação](#create-report-query-api). Alternadamente, pode escolher um modelo de relatório (QueryId) a partir das amostras da biblioteca do modelo de relatório listadas [aqui.](insights-programmatic-system-queries.md)
2. No sucesso, a API de Consulta de Relatório de Criação devolve o QueryId.
3. A aplicação do cliente precisa então de ligar para a [API do Relatório de Criação](#create-report-api) utilizando o QueryId juntamente com a data de início do relatório, Repeat Interval, Recorrence e um URI de retorno opcional.
4. Sobre o Sucesso, a [API do Relatório de Criação](#create-report-api) devolve o ReportId.
5. A aplicação do cliente é notificada no URL de retorno assim que os dados do relatório estiverem prontos para download.
6. A aplicação do cliente utiliza então a [API get report execuções](#get-report-execution-api) para consultar o estado do relatório com o ID do relatório e o intervalo de data.
7. Com o sucesso, o link de descarregamento do relatório é devolvido e a aplicação pode iniciar o download dos dados.

## <a name="report-query-language-specification"></a>Especificação da linguagem de consulta de relatório

Enquanto fornecemos [consultas de sistema](insights-programmatic-system-queries.md) que pode usar para criar relatórios, também pode criar as suas próprias consultas com base nas necessidades do seu negócio. Para saber mais sobre consultas personalizadas, consulte [Especificação de Consulta Personalizada.](insights-programmatic-custom-query.md)

## <a name="create-report-query-api"></a>Criar consulta de relatório API

A API ajuda a criar consultas personalizadas que definem o conjunto de dados a partir do qual as colunas e métricas precisam de ser exportadas. A API fornece a flexibilidade para criar um novo modelo de reporte baseado nas necessidades do seu negócio.  

Também pode utilizar as [consultas do sistema](insights-programmatic-system-queries.md) que fornecemos. Quando não forem necessários modelos de relatórios personalizados, pode ligar para [a API do Relatório de Criar](#create-report-api) diretamente utilizando as Consultas das consultas do sistema fornecidas.  

O exemplo a seguir mostra como criar uma consulta personalizada para obter os 10 melhores clientes por receitas do mês passado.

### <a name="request-syntax"></a>Solicitar sintaxe

|    Método     |    URI do pedido     |
|----- | -----|
|    POST     |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries`|
|||

### <a name="request-header"></a>Cabeçalho do pedido

|    Cabeçalho     |    Tipo     |    Descrição     |
|-------|-----|------|
|    Autorização     |    string |Obrigatório. O Azure Ative Directory (Azure AD) de acesso. O formato é  `Bearer <token>` .|
|    Content-Type     |string |`Application/JSON` |
||||

### <a name="path-parameter"></a>Parâmetro do caminho

Nenhuma

### <a name="query-parameter"></a>Parâmetro de consulta

Nenhuma

### <a name="sample-request-payload"></a>Carga útil do pedido de amostra

```json
{ 
  "Name": "CustomersRevenueQuery", 
  "Description": "Query to get top 10 customers by revenue for last month", 
  "Query": "SELECT CustomerName, Product, BilledRevenueUSD FROM CustomersAndTenants ORDER BY BilledRevenueUSD LIMIT 10 TIMESPAN LAST_MONTH" 
}
```

### <a name="glossary"></a>Glossário

Esta tabela fornece as definições-chave dos elementos na carga útil do pedido.

|Parâmetro|    Obrigatório     |    Descrição     |    Valores Permitidos     |
|-----|    -----    |    -----    |    -----    |
|Name |    Yes     |    Nome amigável da consulta     |    string     |
|    Descrição     |    Não     |    Descrição do que a consulta retorna     |    string     |
|    Consulta     |    Yes     |    Cadeia de consulta de relatório     |    Tipo de dados: cadeia <br> [Consulta personalizada](insights-programmatic-custom-query.md) baseada na necessidade de negócio |
|        |        |        |        |

> [!Note]
> Para amostras de consulta personalizada, consulte [exemplos de consultas de amostras.](insights-programmatic-sample-queries.md)

### <a name="sample-response"></a>Resposta de amostra

A carga útil de resposta é estruturada da seguinte forma:

Códigos de Resposta: 200, 400, 401, 403, 500

Exemplo de carga útil de resposta:

```json
{ 
  "value": [ 
    { 
      "queryId": "ec8366a4-d96e-4194-8c37-d5dbc0639033",
      "name": "CustomersRevenueQuery",
      "description": "Query to get top 10 customers by revenue for last month",
      "query": "SELECT CustomerName, Product, BilledRevenueUSD FROM CustomersAndTenants ORDER BY BilledRevenueUSD LIMIT 10 TIMESPAN LAST_MONTH",
      "type": "userDefined",
      "user": "GAUser@PITEST2.ccsctp.net", 
      "createdTime": "2021-03-30T12:52:39Z" 
    }
  ], 
  "nextLink": null,
  "totalCount": 1,
  "message": "Query created successfully",
  "statusCode": 200,
  "dataRedacted": false
} 
```

### <a name="glossary"></a>Glossário

Esta tabela fornece as definições-chave dos elementos na carga útil do pedido.

|    Parâmetro     |    Descrição     |
|    ----    |    ----    |
|    QueryId     |    Identificador universalmente único (UUID) da consulta que criou     |
|    Name     |    Nome amigável dado à consulta na carga útil do pedido     |
|    Descrição     |    Descrição dada durante a criação da consulta     |
|    Consulta     |    Consulta de relatório passada como entrada durante a criação de consulta     |
|    Tipo     |    Definir para `userDefined`     |
|    Utilizador     |    ID do utilizador usado para criar a consulta     |
|    CreatedTime     |    TEMPO UTC A consulta foi criada neste formato: yyyy-MM-ddTHH:mm:ssZ     |
|    TotalCount     |    Número de conjuntos de dados na matriz de valor     |
|    Código de Estado     |    Código do Resultado <br> Os valores possíveis são 200, 400, 401, 403, 500     |
|    message     |    Mensagem de estado da execução da API     |
|        |        |

## <a name="create-report-api"></a>Criar relatório API

Ao criar um modelo de relatório personalizado com sucesso e receber o QueryID como parte da resposta [Create Report Query,](#create-report-query-api) esta API pode ser chamada para agendar uma consulta a ser executada a intervalos regulares. Pode definir uma frequência e um horário para que o relatório seja entregue.
Para consultas de sistema que fornecemos, a API do Relatório de Criação também pode ser chamada com [Consulta.](insights-programmatic-system-queries.md)

### <a name="callback-url"></a>URL de chamada de retorno

A API do relatório de criação aceita um URL de retorno. Esta URL será chamada assim que a geração do relatório for bem sucedida. O URL de retorno deve ser acessível publicamente. Além do URL, um método de retorno também pode ser dado. O método de retorno só pode ser "GET" ou "POST". O método padrão se nenhum valor for passado será "POST". O reportId que completou a geração será sempre reensibar durante a chamada.

POST callback: Se o URL passou foi `https://www.contosso.com/callback` , então o URL chamado de volta será `https://www.contosso.com/callback/<reportID>` 

GET callback: Se o URL passou foi `https://www.contosso.com/callback` , então o URL chamado de volta será `https://www.contosso.com/callback?reportId=<reportID>` 

### <a name="executenow-reports"></a>Executar Relatórios DeNow

Existe uma disposição para gerar um relatório sem agendamento. O relatório que cria a carga útil da API pode aceitar um parâmetro `ExecuteNow` , que irá encarregar o relatório a ser gerado assim que a API for chamada. Quando `ExecuteNow` é definido como verdadeiro, os campos: , são `StartTime` `RecurrenceCount` `RecurrenceInterval` ignorados porque estes relatórios não estão agendados.

Dois campos adicionais podem ser passados quando `ExecuteNow` é verdade, `QueryStartTime` e `QueryEndTime` . Estes dois campos vão sobrepor-se `TIMESPAN` ao campo na consulta. Estes campos não são aplicáveis aos relatórios agendados, uma vez que os dados serão gerados continuamente por um período de tempo fixo que não se altere.

### <a name="request-syntax"></a>Solicitar sintaxe

|    Método     |    URI do pedido     |
|----- | -----|
|    POST     |`https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport` |

### <a name="request-header"></a>Cabeçalho do pedido

|    Cabeçalho     |    Tipo     |    Descrição     |
|-------|-----|------|
|    Autorização     |    string |Obrigatório. O Azure Ative Directory (Azure AD) de acesso. O formato é  `Bearer <token>` .|
|    Content-Type     |string |`Application/JSON` |

### <a name="path-parameter"></a>Parâmetro do caminho

Nenhuma

### <a name="query-parameter"></a>Parâmetro de consulta

Nenhuma

### <a name="sample-request-payload"></a>Carga útil do pedido de amostra

```json
{
  "ReportName": "Top10_CustomersReport",
  "Description": "Top 10 customers by revenue for last month",
  "QueryId": "ec8366a4-d96e-4194-8c37-d5dbc0639033",
  "StartTime": "2021-03-31T18:41:00Z",
  "ExecuteNow": false,
  "QueryStartTime": null,
  "QueryEndTime": null,
  "RecurrenceInterval": 24,
  "RecurrenceCount": 100,
  "Format": "CSV",
  "CallbackUrl": "https://<SampleCallbackUrl>",
  "CallbackMethod": "GET"
}
```

### <a name="glossary"></a>Glossário

As definições-chave dos elementos na carga útil do pedido são articuladas abaixo:

|    Parâmetro     |    Obrigatório     |    Descrição     |    Valores Permitidos     |
|    ----    |    ----    |    ----    |    ----    |
|    Nome do relatório     |    Yes     |    Nome a atribuir ao relatório     |    string     |
|    Descrição     |    Não     |    Descrição do relatório criado     |    string     |
|    QueryId     |    Yes     |    ID de consulta de relatório     |    string     |
|    StartTime     |    Yes     |    Utc Timestamp em que a geração do relatório começará. <br> O formato deve ser: yyy-MM-ddTHH:mm:ssZ       |    string     |
|    Executar Agora     |    No     |    Este parâmetro deve ser usado para criar um relatório que será executado apenas uma vez. `StartTime`, `RecurrenceInterval` e `RecurrenceCount` são ignorados se isto for verdade. O relatório é executado imediatamente de forma assíncronea     |    verdadeiro/falso     |
|    Horário de ConsultaStart     |    No     |    Opcionalmente especifica a hora de início para a consulta extração dos dados. Este parâmetro é aplicável apenas por um relatório de execução de tempo que `ExecuteNow` se definiu como verdadeiro. Definir este parâmetro sobrepõe-se a perguntas dadas `TIMESPAN` na consulta. O formato deve ser yyy-MM-ddTHH:mm:ssZ     |    Tempotam como corda     |
|    ConsultaEndTime     |    No     |    Opcionalmente especifica o tempo final para a consulta extração dos dados. Este parâmetro é aplicável apenas por um relatório de execução de tempo que `ExecuteNow` se definiu como verdadeiro. Definir este parâmetro sobrepõe-se a perguntas dadas `TIMESPAN` na consulta. O formato deve ser yyy-MM-ddTHH:mm:ssZ     |    Tempotam como corda     |
|    RecorrenceInterval     |    Yes     |    Frequência em horas em que o relatório deve ser gerado. <br> O valor mínimo é 4 e o valor máximo é 2160.      |    número inteiro     |
|    RecorrenceCount     |    No     |    Número de relatórios a serem gerados.     |    número inteiro     |
|    Formato     |    No     |    Formato de ficheiro do ficheiro exportado. <br> O padrão é CSV.    |    "CSV"/"TSV"     |
|    CallbackUrl     |    No     |    URL acessível publicamente que pode ser configurado opcionalmente como destino de retorno     |    String (http URL)     |
|    CallbackMethod     |    No     |    O método a ser usado para o retorno     |    GET/POST     |
|        |        |        |        |

### <a name="sample-response"></a>Resposta de amostra

A carga útil de resposta é estruturada da seguinte forma:

Códigos de Resposta: 200, 400, 401, 403, 404,500

Exemplo de carga útil de resposta:

```json
{ 
  "value": [
    { 
      "reportId": "d9548477-16d4-492a-bf9c-0cf91a9f69bf", 
      "reportName": "Top10_CustomersReport", 
      "description": "Top 10 customers by revenue for last month", 
      "queryId": "ec8366a4-d96e-4194-8c37-d5dbc0639033", 
      "query": "SELECT CustomerName, Product, BilledRevenueUSD FROM CustomersAndTenants ORDER BY BilledRevenueUSD LIMIT 10 TIMESPAN LAST_MONTH", 
      "user": "GAUser@PITEST2.ccsctp.net", 
      "createdTime": "2021-03-30T13:11:58Z", 
      "modifiedTime": null, 
      "executeNow": false, 
      "startTime": "2021-03-31T18:41:00Z", 
      "reportStatus": "Active", 
      "recurrenceInterval": 24, 
      "recurrenceCount": 100, 
      "callbackUrl": "https://<SampleCallbackUrl>", 
      "callbackMethod": "GET", 
      "format": "csv"
    } 
  ], 
  "nextLink": null, 
  "totalCount": 1, 
  "message": "Report created successfully", 
  "statusCode": 200, 
  "dataRedacted": false 
}
```

### <a name="glossary"></a>Glossário

As definições-chave dos elementos na resposta são articuladas abaixo:

|    Parâmetro     |    Descrição     |
|    ----    |    ----    |
|    ReportId     |    Identificador universalmente único (UUID) do relatório que criou     |
|    Nome do relatório     |    Nome dado ao relatório na carga útil do pedido     |
|    Descrição     |    Descrição dada durante a criação do relatório     |
|    QueryId     |    Consulta ID passou no momento em que criou o relatório     |
|    Consulta     |    Texto de consulta que será executado para este relatório     |
|    Utilizador     |    ID do utilizador usado para criar o relatório     |
|    CreatedTime     |    TEMPO UTC O relatório foi criado neste formato: yyyy-MM-ddTHH:mm:ssZ     |
|    ModifiedTime     |    UTC Tempo o relatório foi modificado pela última vez neste formato: yyyy-MM-ddTHH:mm:ssZ     |
|    Executar Agora     |    `ExecuteNow` bandeira definida no momento em que o relatório foi criado     |
|    StartTime     |    UTC Tempo a execução do relatório começará neste formato: yyyy-MM-ddTHH:mm:ssZ     |
|    Relatório Estatísticas     |    Estado da execução do relatório. Os valores possíveis `Paused` `Active` são, e `Inactive`     |
|    RecorrenceInterval     |    Intervalo de recorrência fornecido durante a criação do relatório     |
|    RecorrenceCount     |    Contagem de recorrência fornecida durante a criação do relatório.      |
|    CallbackUrl     |    URL de retorno fornecido no pedido     |
|    CallbackMethod     |    Método de retorno fornecido no pedido     |
|    Formato     |    Formato dos ficheiros do relatório. Os valores possíveis são `CSV` ou `TSV` .     |
|    TotalCount     |    Número de registos na matriz de valor     |
|    Código de Estado     |    Código do Resultado     |
|    message     |    Os valores possíveis são 200, 400, 401, 403, 500. Mensagem de estado da execução da API     |
|        |        |

## <a name="get-report-execution-api"></a>Obtenha relatório execução API

Pode utilizar este método para consultar o estado de execução de um relatório utilizando o RelatórioId recebido da API do [Relatório de Criação](#create-report-api). O método devolve o link de descarregamento do relatório se o relatório estiver pronto para download. Caso contrário, o método devolve o estado. Você também pode usar esta API para obter todas as execuções que aconteceram para um dado relatório.  

>[!IMPORTANT]
>Esta API tem parâmetros de consulta predefinidos definidos para `executionStatus=Completed` e `getLatestExecution=true` . Por isso, chamar a API antes da primeira execução bem sucedida do relatório devolverá 404. Execuções pendentes podem ser obtidas por definição `executionStatus=Pending` .

### <a name="request-syntax"></a>Solicitar sintaxe

|    Método     |    URI do pedido     |
|----- | -----|
|    GET    |`https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/execution/{reportId}?executionId={executionId}&executionStatus={executionStatus}&getLatestExecution={getLatestExecution}`  |

### <a name="request-header"></a>Cabeçalho do pedido

|    Cabeçalho     |    Tipo     |    Descrição     |
|-------|-----|------|
|    Autorização     |    string |Obrigatório. O Azure Ative Directory (Azure AD) de acesso. O formato é  `Bearer <token>` .|
|    Content-Type     |string |`Application/JSON` |

### <a name="path-parameter"></a>Parâmetro do caminho

|    Nome do Parâmetro    |    Necessário    |    Tipo    |    Descrição    |
|    ----    |    ----    |    ----    |    ----    |
|    reportId    |    Yes    |    string    |    Filtrar para obter detalhes de execução de apenas relatórios com o relatório Dado neste argumento. Vários reportIds podem ser especificados separando-os com um ponto e vírgula ";".    |
|        |        |        |        |

### <a name="query-parameter"></a>Parâmetro de consulta

|    Nome do Parâmetro    |    Necessário    |    Tipo    |    Descrição    |
|    ----    |    ----    |    ----    |    ----    |
|    execuçãoId    |    No    |    string    |    Filtre para obter detalhes de apenas relatórios com a execuçãoId dado neste argumento. Execuções múltiplas podem ser especificadas separando-as com um ponto e vírgula ";".    |
|    execuçãoStatus    |    No    |    Corda/enum    |    Filtre para obter detalhes de apenas relatórios com a execuçãoStatus dada neste argumento. <br> Os valores válidos são: `Pending` `Running` `Paused` `Completed` e. <br> O valor predefinido é `Completed`. <br> Vários estados podem ser especificados separando-os com um ponto e vírgula ";".    |
|    obterExecução de Pré-executivos    |    No    |    boolean    |    A API devolverá detalhes da última execução. Por padrão, este parâmetro é definido como verdadeiro.<br> Se optar por passar o valor deste parâmetro como falso, então a API devolverá os últimos 90 dias de execução.    |
|        |        |        |        |

### <a name="sample-request-payload"></a>Carga de pedido de amostra

Nenhuma

### <a name="sample-response"></a>Resposta de Amostra

A carga útil de resposta é estruturada da seguinte forma:

Códigos de Resposta: 200, 400, 401, 403, 404,500

Exemplo de carga útil de resposta:

```json
{
  "value": [
    {
      "executionId": "906931dc-4f2f-4195-bbb2-d7295c7550d3",
      "reportId": "d9548477-16d4-492a-bf9c-0cf91a9f69bf",
      "recurrenceInterval": 24,
      "recurrenceCount": 100,
      "callbackUrl": null,
      "callbackMethod": null,
      "format": "csv",
      "executionStatus": "Completed",
      "reportLocation": null,
      "reportAccessSecureLink": "https://<path to report for download>",
      "reportExpiryTime": null,
      "reportGeneratedTime": "2021-03-31T18:41:00Z"
    }
  ],
  "nextLink": null,
  "totalCount": 1,
  "message": null,
  "statusCode": 200,
  "dataRedacted": false
}
```

Uma vez concluída a execução do relatório, o estado de execução `Completed` é mostrado. Pode descarregar o relatório selecionando o URL no `reportAccessSecureLink` .

### <a name="glossary"></a>Glossário

Definições-chave de elementos na resposta.

|    Parâmetro    |    Descrição    |
|    ----    |    ----    |
|    ExecuçãoId    |    Identificador universalmente único (UUID) da instância de execução    |
|    ReportId    |    ID do relatório associado à instância de execução    |
|    RecorrenceInterval    |    Intervalo de recorrência fornecido durante a criação do relatório    |
|    RecorrenceCount    |    Contagem de recorrência fornecida durante a criação do relatório    |
|    CallbackUrl    |    URL de retorno associado à instância de execução    |
|    CallbackMethod    |    Método de retorno associado à instância de execução    |
|    Formato    |    Formato do ficheiro gerado no final da execução    |
|    ExecuçãoStatus    |    Estado da instância de execução do relatório. <br> Valores válidos são: `Pending` `Running` , e `Paused``Completed`    |
|    ReportAccessSecureLink    |Link através do qual o relatório pode ser acedido de forma segura        |
|    ReportExpiryTime    |    Tempo UTC após o qual a ligação de relatório expirará neste formato: yyyy-MM-ddTHH:mm:ssZ    |
|    ReportGeneratedTime    |    Tempo UTC em que o relatório foi gerado neste formato: yyyy-MM-ddTHH:mm:ssZ    |
|    TotalCount    |    Número de conjuntos de dados na matriz de valor    |
|    Código de Estado    |    Código do Resultado <br> Os valores possíveis são 200, 400, 401, 403, 404 e 500    |
|    message    |    Mensagem de estado da execução da API    |
|        |        |

## <a name="next-steps"></a>Passos seguintes

- Experimente as APIs através do [URL da API](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html)
- [Faça a sua primeira chamada API](insights-programmatic-first-api-call.md)