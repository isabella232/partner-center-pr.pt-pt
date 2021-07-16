---
title: Relatório de subscrições de Informações do Partner Center
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Veja o que está a fazer bem e onde pode melhorar no que diz respeito às subscrições em nuvem que vende ou gere para os seus clientes.
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a1ce0e75817376b5cf1996a56f416acc4bcbd0f3
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/16/2021
ms.locfileid: "114377028"
---
# <a name="product-subscriptions-report-available-from-the-partner-center-insights-dashboard"></a>Relatório de subscrições de produtos disponível no painel de Informações do Partner Center

**Funções adequadas**: Administração global | Agente administrativo | Relatório | do espectador Espectador de relatório executivo

O relatório de Subscrições de Produtos apresenta análises sobre subscrições em nuvem que vendeu ou que gere para os seus clientes. Este é um relatório específico do produto que inclui o desempenho de subscrições associadas a produtos na nuvem como Office 365, Azure, Dynamics, entre outros.

Pode ver as seguintes secções do relatório de Subscrições de Produtos.

- Resumo
- Spread geográfico das assinaturas
- Tendência de adicionar/churn de subscrições
- Distribuição de assinaturas por localizações de parceiros, canal de vendas, SKUs, tipo de anexação de parceiros, segmento
- Tendência por estados de subscrição
- Tendência dos produtos

 > [!NOTE]
 > Este relatório está disponível no painel de instrumentos Informações. Para visualizar este relatório, deve ser-lhe atribuído um papel específico no Partner Center, como administração global, administração de contas, espectador de relatório ou visualizador de relatórios executivos. Para mais informações, consulte a administração Global da sua empresa. Os tipos específicos de dados deste relatório também podem estar disponíveis apenas para utilizadores com privilégios de visualização de relatório executivo.

## <a name="summary"></a>Resumo

A secção de resumo apresenta uma visão instantânea dos principais indicadores de desempenho (KPI's) relacionados com subscrições vendidas ou geridas por si para os seus clientes.  

:::image type="content" source="images/insights/sub-report-summary.png" alt-text="subscrições reportam resumo.":::

Para obter mais informações sobre cada secção do resumo, consulte abaixo:

- Subscrições:
  - Contagem atual das subscrições de produtos em nuvem vendidas ou geridas por si.
  - Crescimento percentual ou declínio das subscrições durante o intervalo de datas selecionados.
  - O Micro chart apresenta uma tendência mensal de contagem de assinaturas durante a sua gama de datas selecionadas.

- Assinaturas ativas:
  - Contagem atual de subscrições de produtos em nuvem com utilização ativa medida com base na telemetria do produto. Isto exclui todas as subscrições de teste para subscrições Azure.
  - Crescimento percentual ou declínio de subscrições ativas durante o período de tempo selecionado.
  - O Micro chart apresenta uma tendência mensal de subscrições ativas durante a sua gama de datas selecionadas.

- Assinaturas adicionadas:
  - Total de subscrições de clientes adicionadas (vendidas ou geridas) por si durante o intervalo de datas selecionadas. As novas subscrições com estado **ativo** ou **renovado** são contadas à medida que as Assinaturas são adicionadas.
  - Crescimento percentual ou declínio das subscrições adicionadas no último mês completo em comparação com o primeiro mês completo.
  - O Micro chart apresenta uma tendência mensal de subscrições adicionadas durante a sua gama de datas selecionadas.

- Assinaturas agitadas:
  - Total de assinaturas de clientes agitadas durante o intervalo de datas selecionados. As assinaturas com estado **Deprovisionado** ou **Suspenso** nesse mês são contadas como uma subscrição chuçada.  
  - Percentagem de subscrições agitadas durante o intervalo de datas selecionadas.
  - O Micro chart apresenta uma tendência mensal de subscrições agitadas ao longo da gama de datas selecionadas.

- Subscrições por produtos: Repartição da contagem atual de subscrição por produtos na nuvem.

## <a name="geographical-spread-of-subscriptions"></a>Spread geográfico das assinaturas

As **subscrições por visualização de geografia** mostram a distribuição geográfica do total de subscrições pelos mercados de clientes. O valor total da subscrição inclui assinaturas vendidas e subscrições ativas.

O **número de países/tabela de região** apresenta o total de países/regiões onde tem subscrições e o valor por país de subscrições totais e ativas.

Pode pesquisar e selecionar um país na grelha para ampliar a localização no mapa. Pressione a opção **Home** no mapa para reverter para a vista original. Paire no mapa para ver todas as subscrições e subscrições ativas por país. Ambos os campos na grelha são ordenados.

:::image type="content" source="images/insights/sub-report-sub-by-geography.png" alt-text="subscrições por geografia.":::

## <a name="subscription-addschurns"></a>Adds/churns de assinatura

Esta visão apresenta uma tendência de subscrições. Estes são divididos em diferentes categorias (Novo, Existente, Churned) para a gama de datas selecionadas. O eixo X representa meses do intervalo de datas selecionados. O eixo Y representa a contagem de assinaturas. As assinaturas chuçadas são representadas na escala negativa do eixo Y. 

O gráfico de colunas empilhado apresenta uma desagregação de novas subscrições existentes e chumidas para o mês. Pode reconstruir o gráfico da coluna, dividido com itens de pilha específicos. Para tal, selecione os itens específicos na lenda. Também pode utilizar o slider no topo da tabela para ampliar para um período específico.

:::image type="content" source="images/insights/sub-report-sub-adds-churns.png" alt-text="subscrição adiciona e churns.":::

## <a name="subscription-distribution"></a>Distribuição de assinaturas

Esta visão apresenta uma desagregação das suas subscrições atuais pelas localizações da Microsoft Partner Network (MPN), segmentos de clientes, modelo de preços de canal de vendas/Azure e o tipo de atribuição. Selecione os respetivos separadores para ver a avaria por estas categorias. Para construir o gráfico de tortas com uma desagregação de categorias específicas de itens, selecione as categorias de itens na legenda.

:::image type="content" source="images/insights/sub-report-distribution.png" alt-text="distribuição de assinaturas.":::

## <a name="subscription-state-distribution"></a>Distribuição do estado de subscrição

Esta vista mostra a distribuição das suas subscrições atuais do cliente por estado ou estado de subscrição. Isto inclui os seguintes estados de subscrição: **Ative,** **Deprovisioned, Deprovisioned,** **Open,** **InGracePeriod,** **Closed**, e **Outros**. 

:::image type="content" source="images/insights/sub-report-sub-states.png" alt-text="distribuição do estado de subscrição.":::

## <a name="products-trend"></a>Tendência dos produtos

Esta vista mostra um gráfico de barras e dois gráficos de tortas. O gráfico de barras apresenta uma tendência mensal de subscrições discriminadas por produtos comerciais, como a Azure, Office e Dynamics.

Os dois gráficos de tartes mostram uma desagregação das subscrições atuais do cliente. O primeiro gráfico de tartes decompõe as subscrições por produtos. O segundo gráfico de tartes decompõe as subscrições por SKUs ou planos. Quando selecionar um produto na tabela de **tartes Products,** o gráfico de tartes adjacente mostrar-lhe-á uma repartição das subscrições desse produto por SKUs.

:::image type="content" source="images/insights/sub-report-prods-trend.png" alt-text="tendência dos produtos.":::

> [!NOTE]
 > A contagem de subscrições discriminada pela SKUs pode nem sempre corresponder à contagem total de subscrição desse produto. Isto pode ocorrer se um cliente tiver adquirido vários SKUs sob a mesma subscrição do produto.

## <a name="next-steps"></a>Passos seguintes

- Para mais relatórios, consulte [o Partner Center Informações](partner-center-insights.md).

>[!NOTE] 
> Pode descarregar os dados brutos que alimentam este relatório a partir da secção Relatórios de Descarregamento no painel de Informações. [Saiba mais](insights-download-reports.md) 
