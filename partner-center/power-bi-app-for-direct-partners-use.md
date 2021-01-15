---
title: Use Partner Center Analytics para Power BI
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como ver os dados do seu negócio utilizando a app Partner Center Analytics para Power BI (para parceiros diretos em CSP).
fwlink: https://go.microsoft.com/fwlink/?linkid=852581
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 244cb852728d47360cf8ecd1d1e9ccb641466b1d
ms.sourcegitcommit: 1a0c83e2089cb58221bdb24525127378f5197ea8
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/14/2021
ms.locfileid: "98215752"
---
# <a name="view-your-business-data-with-the-partner-center-analytics-app-for-microsoft-power-bi"></a>Veja os seus dados de negócio com a aplicação Partner Center Analytics para Microsoft Power BI



**Funções adequadas**

- Administrador global
- Administrador de utilizadores
- Agente comercial
- Agente administrativo

## <a name="view-your-business-data"></a>Ver os seus dados de negócio

Obtenha uma representação visual dos seus dados de negócio com a aplicação Partner Center Analytics para Power BI, incluindo:

- Crescimento da sua base de clientes, subscrições e licenças

- Utilização dos produtos Office 365, Microsoft Dynamics e Microsoft Azure

- Unidades de consumo diário para cada recurso medido em cada subscrição do Azure nos últimos 60 dias

- Custo estimado (com base no cartão de tarifa mais recente)

- Capacidade de exportar conjuntos de dados e criar relatórios personalizados, incluindo por cliente.

### <a name="about-the-partner-center-analytics-app-preview-release"></a>Sobre o lançamento da pré-visualização da aplicação Partner Center Analytics

- Esta aplicação destina-se apenas a parceiros diretos no programa Cloud Solution Provider. Outros parceiros na CSP (revendedores indiretos, por exemplo) não poderão assinar.

- Quaisquer custos estimados são dados de faturação/fatura prévia, e não são juridicamente vinculativos. Os custos estimados devem ser utilizados apenas para informações sobre dados.

- A informação do cliente baseia-se em subscrições. Quaisquer clientes que tenha criado recentemente, mas que ainda não tenham subscrições, não estão incluídos nas contagens.

- O custo estimado baseia-se no cartão de tarifa mais recente, que se baseia nos preços da CSP.

- Dias são dias de calendário.

### <a name="business-insights-report"></a>Relatório de Insights de Negócios

- **Inquilinos do cliente**: Número de inquilinos distintos da AZure AD de clientes que adquiriram assinaturas

- **Novo (últimos 30 dias)**: Novos clientes que compram pelo menos uma subscrição nos últimos 30 dias

- **Churn (últimos 30 dias)**: Clientes sem assinaturas "ativas", "em graça" ou "desativadas"

- **Novo (últimas 24 horas)**: Novos clientes que compram pelo menos uma subscrição nas últimas 24 horas

- **Custo mensal estimado nos últimos 12 meses**: Mês ao longo do mês tendência da fatura estimada antes de impostos valor do dólar agregado mensalmente durante o período dos últimos 12 meses

- **Custo estimado por produto ao longo dos últimos 12 meses**: Produtos vendidos classificados pela estimativa de fatura de imposto em dólares agregados durante o período dos últimos 12 meses. Este estatuto indica que os produtos de topo trazem a maioria das receitas.

- **Clientes nos últimos 12 meses**: Mês ao longo do mês tendência de novos clientes e clientes agregados mensalmente ao longo do período dos últimos 12 meses

- **Custo estimado pelo cliente ao longo dos últimos 12 meses**: Clientes classificados pelo valor estimado da fatura antes de impostos em dólares agregados ao longo do período dos últimos 12 meses. Este estado indica que os principais clientes trazem a maioria das receitas.

- **Contagem de clientes por produto**: Produtos vendidos por clientes associados. Este estado indica produtos de topo vendidos à maioria dos clientes.

### <a name="subscription-insights-report"></a>Relatório de Insights de Subscrição

- **Estado da subscrição**:

- Ativo: Assinaturas pertencentes ao estado "ativo" ou "em graça"

  - Suspenso: Assinaturas pertencentes ao estado "deficiente"

  - Desestado: Assinaturas pertencentes ao estatuto de "desestado" ou "caducado"

- **Estado da caducidade:**

  - Expirado: Assinaturas que já expiraram (onde a data de fim da subscrição é anterior)

  - Expiração após 30 dias: Assinaturas que expirarão após 30 dias (onde a data de fim da subscrição é após os próximos 30 dias)

  - Expiração em 30 dias: Assinaturas que caducarão nos próximos 30 dias (onde a data de fim da subscrição é entre hoje e os próximos 30 dias)

- **Total de assinaturas**: Assinaturas em estado "ativo", "em graça" ou "deficiente"

- **Novidade (últimos 30 dias)**: Novas subscrições compradas pelos clientes nos últimos 30 dias

- **Novidade (últimas 24 horas)**: Novas subscrições compradas pelos clientes nas últimas 24 horas

- **Expiração em 30 dias**: Assinaturas que caducarão nos próximos 30 dias

- **Churn (últimos 30 dias)**: Assinaturas que tenham sido desavisionadas ou suspensas (desativadas) nos últimos 30 dias

- **Distribuição por tipos de subscrição**: % distribuição de subscrições totais por tipo de subscrição baseada em licença e por uso

- **Contagem ativa de subscrição por produto**: Produtos vendidos classificados por subscrições ativas contam

- **Assinaturas ao longo dos últimos 12 meses**: Mês ao longo do mês tendência de novas subscrições e subscrições de churn agregadas mensalmente ao longo do período dos últimos 12 meses

- **Detalhes da subscrição** do cliente : Vista detalhada dos clientes, subscrições e ofertas

### <a name="license-insights-report"></a>Relatório de Insights de Licença:

- **Total de licenças**: Número total de licenças agregadas em todas as subscrições baseadas em licenças

- **Novo (últimos 30 dias)**: Adição de licença nos últimos 30 dias

- **Churn (últimos 30 dias)**: Redução da licença nos últimos 30 dias

- **Novo (último 24 horas)**: Adição de licença nas últimas 24 horas

- **Licenças nos últimos 90 dias**: Mês ao longo do mês tendência de aditamentos e reduções de licenças agregadas mensalmente durante o período dos últimos 90 dias

- **Contagem de licença ativa por produto**: Produtos vendidos classificados por contagem de licença ativa

- **Contagem de licença ativa por cliente**: Clientes classificados por contagem de licença ativa

- Detalhes do evento da licença do cliente ao longo dos **últimos 90 dias**: Vista detalhada dos clientes, subscrições e eventos de subscrição, incluindo data do evento, nome do evento, quantidade e alteração de quantidade.

### <a name="licenses-usage-report"></a>Relatório de utilização das licenças:

- **Licenças atribuídas por produto**: Produtos vendidos classificados por contagem de atribuição de licença

- **Licenças em uso por produto**: Produtos vendidos classificados por contagem de utilização de licença

- **Distribuição de clientes das licenças atribuídas:**% distribuição do total de clientes quebrados em baldes de 20% de intervalo por atribuição de licenças %

- **Distribuição do cliente de licenças em uso**: % distribuição do total de clientes quebrados em baldes de 20% de intervalo por utilização de licença %

- **Licenças atribuídas pelo cliente**: Vista detalhada das licenças vendidas e licenças atribuídas por clientes e produtos

- **Licenças em uso por cliente**: Vista detalhada das licenças vendidas e licenças em uso por clientes e produtos

### <a name="azure-insights-report"></a>Relatório Azure Insights:

- **Clientes baseados em uso nos últimos 12 meses**: Mês ao longo do mês tendência de novos clientes baseados em uso e clientes com base em uso agregados mensalmente durante o período dos últimos 12 meses

- **Subscrições baseadas em uso ao longo dos últimos 12 meses**: Tendência mensal de novas subscrições baseadas em uso e subscrições baseadas em uso agregadas mensalmente durante o período dos últimos 12 meses

- **Custo estimado de utilização por parte do cliente ao longo dos últimos 60 dias**: Clientes baseados no uso classificados pelo valor estimado da fatura antes de impostos em dólares agregados ao longo do período dos últimos 60 dias. Este estado indica que os clientes de topo baseados em uso trazem a maioria das receitas

- **Custo estimado de utilização por categoria ao longo dos últimos 60 dias**: Categorias de contadores de assinaturas baseadas em uso ordenadas por valor estimado de fatura antes de impostos em dólares agregados ao longo do período dos últimos 60 dias.

- **Custo estimado de utilização por subscrição ao longo dos últimos 60 dias**: Subscrições baseadas em uso por valor estimado em dólares de fatura pré-impostos agregados ao longo do período dos últimos 60 dias.

- **Custo de utilização estimado pelo cliente através do orçamento de gastos**: Clientes classificados em percentagem do seu orçamento atual de despesas de utilização excedendo o limiar (100%).

### <a name="azure-resource-usage-report"></a>Relatório de utilização de recursos Azure:

- **Utilização de recursos Azure por dia durante o período selecionado**: Unidades de consumo diário para cada recurso medido em cada subscrição baseada em utilização durante o período selecionado nos últimos 60 dias.

- **Custo estimado de utilização dos recursos Azure para o período selecionado**: Custo estimado com base no cartão de tarifa mais recente para cada recurso medido em cada subscrição baseada em uso para o período selecionado nos últimos 60 dias. 

## <a name="next-steps"></a>Passos seguintes

- [Partner Center Analytics for Power BI app overview](power-bi-app-for-direct-partners.md)

- [Install and preview the Partner Center Analytics app for Microsoft Power BI](power-bi-app-for-direct-partners-install.md) (Instalar e pré-visualizar a aplicação de Análise do Centro de Parceiros do Microsoft Power BI)
