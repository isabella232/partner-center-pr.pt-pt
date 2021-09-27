---
title: Centro de Informações
description: Explore este painel de relatórios unificado do Partner Center. Veja como está em KPI's para vendas e implementação, desenvolvimento de clientes e muito mais.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 05/26/2020
ms.openlocfilehash: 297f63aa4777f7a5448ec915e727b18dacdd0bc5
ms.sourcegitcommit: d731813da1d31519dc2dc583d17899e5cf4ec1b2
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/27/2021
ms.locfileid: "129075042"
---
# <a name="partner-center-insights---a-dashboard-that-shows-how-a-microsoft-commercial-partner-is-doing"></a>Partner Center Informações - um dashboard que mostra como um parceiro comercial da Microsoft está a fazer

**Funções adequadas**: Administração global | Administração de contas | | do espectador de relatório executivo Espectador de relatório

## <a name="introduction"></a>Introdução

O dashboard Informações é um painel de reporte unificado no Partner Center para parceiros comerciais da Microsoft que estão inscritos no programa Microsoft Partner Network (MPN). O dashboard Informações fornece uma visão de 360 graus dos seus principais indicadores de desempenho (KPI) em todos os produtos Cloud, tais como Office, Azure, Dynamics e modelos de licenciamento como CSP e EA. Expõe um rico conjunto de relatórios KPI que podem ajudá-lo a tomar decisões orientadas por dados para a sua organização. 

## <a name="role-based-access-control-to-the-insights-dashboard"></a>Controlo de acesso baseado em funções ao painel de Informações

Existem duas novas funções no Partner Center projetadas especificamente para o acesso a Informações: **Report Viewer** e **Executive Report Viewer**. Os utilizadores na função de Visualizador de Relatório Executivo têm acesso a todos os conjuntos de dados de reporte, enquanto os utilizadores na função 'Observador de Relatórios' não terão acesso a conjuntos de dados sensíveis, tais como receitas e dados pessoais cliente/colaborador. 

O administrador Global ou o administrador da Conta podem atribuir aos utilizadores estas funções e são atribuídos quer para toda a empresa, quer para uma localização MPN específica.  

>[!Note] 
>Os utilizadores que eram administradores da MPN a partir de 20 de janeiro de 2020 foram automaticamente adicionados ao papel de espectador de relatórios da empresa. Podem aceder aos relatórios como um espectador de relatório sem qualquer ação explícita exigida pela Administração Global ou Administração de Contas. Os administradores globais ou administradores de contas podem sobrepor-se a estas atribuições, se necessário. 

## <a name="reports-available"></a>Relatórios disponíveis

Os seguintes relatórios estão disponíveis como parte do painel de Informações.

**Visão geral**: O relatório geral apresenta uma visão instantânea de vários KPI's de interesse para si, tais como contagem de clientes, contagem de subscrições ativas, receitas de consumo azure, licenças ativas, etc.

**Cliente**: O relatório do Cliente apresenta análises em torno dos seus clientes, tais como dados de aquisição de clientes, clientes ativos, etc.

**Produto - Subscrições**: O relatório de subscrições apresenta análises de aquisição e utilização para as suas subscrições cloud (tais como O365, Azure, Dynamics etc.)

**Licenças de Produtos**: O dashboard licenses apresenta análise de licença para produtos Cloud baseados em licenças como O365, Dynamics, Power BI etc.

**Produto - Utilização Azure**: O relatório de utilização do Azure apresenta métricas relacionadas com as assinaturas Azure dos seus clientes, incluindo as receitas de consumo da Azure e a utilização por categorias de contadores.

**Competências**: O relatório de Competências apresenta métricas nas suas competências ativas, qualificadas e em risco.

**Benefícios**: O relatório Benefits apresenta análises sobre os benefícios do parceiro que obteve vs consumidos.

## <a name="navigating-the-insights-reports"></a>Navegando nos relatórios de Informações

**Filtros de gama de datas**: Pode encontrar uma seleção de intervalo de datas no canto superior direito de cada página. A saída dos gráficos de página de visão geral pode ser personalizada selecionando uma gama de datas baseada nos últimos 3, 6 ou 12 meses, ou selecionando um intervalo de datas personalizado. A seleção do intervalo de datas padrão é de 12 meses. 

:::image type="content" source="images/insights/introduction.png" alt-text="Mapa de introdução.":::

**Botão de feedback**: Cada gráfico/controlo em todos os relatórios Informações é incorporado com um botão de feedback para permitir que forneça feedback de instância sobre uma função de relatório. 

 
**Filtros de nível de página**: Com exceção dos relatórios de visão geral, benefícios e competências, todos os relatórios Informações permitem aplicar filtros de nível de página. 

- Os filtros selecionados serão aplicáveis a todos os gráficos e métricas de uma página, incluindo a secção de resumo. Um item de filtro estará disponível se tiver algum dado dentro desses critérios de filtragem. 

- A seleção predefinida de cada lista de **filtros** é toda . Por exemplo, se não tiver selecionado um produto específico no filtro de produtos, a seleção predefinida será de todos os produtos.

- Os filtros selecionados serão apresentados no topo da página. 

:::image type="content" source="images/insights/filters.png" alt-text="Screenshot parcial mostra barra de filtros aplicada com seleções de filtros para Produtos, Mercados de Clientes, Atribuições de Parceiros e Canais de Vendas.":::

### <a name="filters-definitions"></a>Filtra definições:

- Produtos: Lista de todos os produtos Microsoft Cloud vendidos/geridos pela sua organização, por exemplo, O365, Azure, D365, EMS, Power BI, etc.
- Mercados de clientes: Lista de países de clientes
- Atribuições de parceiros: O seu tipo de associação com as assinaturas dos seus clientes, por exemplo, parceiro digital de registo (DPOR), privilégio de administração delegado (DAP) e link Partner Admin (PAL). 
- Localizações do parceiro: Lista de todas as localizações mpn da sua organização.
- Canais de vendas: Todos os canais de vendas/preços através dos quais está a adquirir/a forragem de produtos e serviços, nomeadamente CSP, EA, CSP indireto, Direct, Advisor, Open, outros
- Segmentos de cliente: Lista de segmentos de clientes em toda a base de clientes dos parceiros.

## <a name="read-about-each-of-the-dashboards-and-reports"></a>Leia sobre cada um dos dashboards e relatórios:

- [Partner Center Informações - Painel de visão geral](insights-overview-report.md)

- [Centro de Parceiros Informações - Painel de clientes](insights-customer-report.md)

- [Relatório do Centro de Parceiros Informações - Relatório de Assinaturas](insights-product-subscriptions-report.md)

- [Partner Center Informações - Relatório de Licenças](insights-product-licenses-report.md)

- [Partner Center Informações - Relatório de utilização do Azure](insights-azure-usage-report.md)

- [Partner Center Informações - Relatório de Competências](insights-competencies-report.md)

- [Partner Center Informações - Relatório de benefícios](insights-benefits-report.md)
