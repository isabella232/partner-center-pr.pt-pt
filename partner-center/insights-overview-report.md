---
title: Painel de visão geral do centro de Informações do parceiro
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: Veja uma imagem de como está a fazer com vendas e implementação, crescimento de clientes e crescimento de receitas com licenças, subscrições e consumo de Azure.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 439d49a7286ae9a2a1d61a088d86ec32b3f8fcb5
ms.sourcegitcommit: d731813da1d31519dc2dc583d17899e5cf4ec1b2
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/27/2021
ms.locfileid: "129071884"
---
# <a name="overview-dashboard-reports-available-in-partner-center-insights"></a>Relatórios do painel de visão geral disponíveis no Partner Center Informações
 
**Funções adequadas**: Administração global | Agente administrativo | Relatório | do espectador Espectador de relatório executivo

O dashboard Informações Overview fornece uma visão instantânea dos principais indicadores de desempenho (KPI's) tais como Clientes, Subscrições, Receitas de Consumo Azure e Licenças. Pode visualizar os seguintes gráficos no relatório do Resumo.

- Resumo  
- Spread geográfico dos seus clientes, subscrições e licenças  
- Tendência de crescimento dos clientes 
- Tendência de crescimento das subscrições 
- Azure consumiu tendência de crescimento da receita 
- Tendência de crescimento das licenças 

## <a name="summary"></a>Resumo

O Resumo inclui informações sobre clientes, Azure Consumed Revenue (ACR), subscrições vendidas, subscrições ativas e licenças implementadas. 

:::image type="content" source="images/insights/summary.png" alt-text="Licenças de resumo.":::

Seguem-se mais informações sobre cada secção do Resumo.

### <a name="customers"></a>Clientes

A área **de Clientes** inclui:

- A contagem atual de todos os clientes com pelo menos uma subscrição ativa associada à sua empresa através de diferentes tipos de atribuição e em todos os produtos cloud.
- O crescimento percentual dos clientes durante a gama de datas selecionadas.
- O micro-gráfico apresenta a tendência mensal da contagem de clientes dentro da gama de datas selecionadas.

### <a name="azure-consumed-revenue-acr"></a>Receitas Consumidas Azure (ACR)

A área **de Azure Consumed Revenue (ACR)** no Resumo inclui:

- O total de ACR (em dólares americanos) atribuído ao longo da gama de datas selecionadas.
- O crescimento percentual ou o declínio do ACR atribuído (em dólares americanos) durante o intervalo de datas selecionados.
- O micro gráfico apresenta uma tendência mensal de ACR em dólares americanos atribuídos ao longo da gama de datas selecionadas 

> [!NOTE]
> Os dados da ACR estão disponíveis para os utilizadores que tenham sido designados para o papel de visualizador de relatório executivo.
 
### <a name="subscriptions-sold"></a>Assinaturas vendidas

A área **de subscrições vendida** no Resumo inclui:

- A contagem atual total de subscrições de produtos Cloud (ativas e inativas) vendidas ou geridas por si.  
- O crescimento percentual ou o declínio das subscrições durante o intervalo de datas selecionadas.
- O micro-gráfico apresenta a tendência mensal de subscrições totais ao longo da gama de datas selecionadas.

### <a name="active-subscriptions"></a>Assinaturas ativas

A área **de subscrições Ativa** no Resumo inclui:

- A contagem atual de subscrições de produtos Cloud com utilização ativa medida com base na telemetria do produto. Isto exclui todas as subscrições do Azure.  
- O crescimento percentual das subscrições ativas ao longo da gama de datas selecionadas.
- O micro-gráfico apresenta a tendência mensal de subscrições ativas ao longo da gama de datas selecionadas.
 
### <a name="licenses-deployed"></a>Licenças implantadas

A área **de licenças implantadas** no Resumo inclui:
 
- A contagem de todas as licenças de produtos Cloud implementadas nas subscrições do seu cliente durante o período de tempo selecionado. 
- O crescimento percentual ou o declínio destas licenças durante o intervalo de datas selecionadas. 
- O micro gráfico mostra a tendência mensal destas licenças atribuídas contando ao longo da gama de datas selecionadas.

## <a name="geographical-spread-of-your-customers-subscriptions-and-licenses"></a>Spread geográfico dos seus clientes, subscrições e licenças

Esta vista é uma distribuição geográfica do total de clientes, subscrições e licenças por país cliente. Selecione os diferentes separadores para visualizar cada uma destas informações no mapa. Pode pesquisar e selecionar um país na grelha para ampliar a localização no mapa. Reverta para a vista original premindo o botão Home no mapa. Clicar em cada separador (por exemplo, Clientes, Subscrições) mostra o valor da métrica para cada país e a percentagem de Total para o país.  

:::image type="content" source="images/insights/geosummary.png" alt-text="Resumo geográfico.":::

## <a name="customers-growth-trend"></a>Tendência de crescimento dos clientes

A tendência mensal do total de clientes conta para a gama de datas selecionadas. O eixo X representa meses da gama de datas selecionadas e o eixo Y representa a contagem total do cliente para esse mês. 

:::image type="content" source="images/insights/customer-growth.png" alt-text="tendência de crescimento dos clientes.":::

## <a name="subscriptions-growth-trend"></a>Tendência de crescimento das subscrições

Isto indica que a tendência das subscrições do seu cliente conta para a gama de datas selecionadas. O eixo X representa meses da gama de datas selecionadas e o eixo Y representa a contagem de subscrições do produto selecionado. Percorra o slider no topo da tabela para ampliar a tabela para um período de tempo específico. 

:::image type="content" source="images/insights/subscription-growth.png" alt-text="Tendência de crescimento de assinaturas.":::

## <a name="azure-consumed-revenue-growth-trend"></a>Tendência de crescimento da receita consumida do Azure

A tendência mensal do Azure consumiu receitas em dólares americanos atribuídos ao longo da gama de datas selecionadas. O eixo X representa meses da gama de datas selecionadas e o eixo Y representa a receita total consumida pelo Azure em dólares americanos que lhe foram atribuídos durante o mês.

> [!NOTE]
> A ACR só será visível para os utilizadores que tenham sido designados para o papel de espectador de relatório executivo. 

:::image type="content" source="images/insights/azure-consumed.png" alt-text="Consumo azul.":::

## <a name="licenses-growth-trend"></a>Tendência de crescimento das licenças
 
Tendência das licenças atribuídas por todos os clientes durante o intervalo de datas selecionados. O eixo X representa meses da gama de datas selecionadas e o eixo Y representa a contagem de licenças do produto selecionado. Percorra o slider no topo da tabela para ampliar a tabela para um período de tempo específico.  

:::image type="content" source="images/insights/licenses-growth.png" alt-text="licenças.":::

## <a name="next-steps"></a>Passos seguintes

Para mais relatórios, consulte [o Partner Center Informações](partner-center-insights.md).
