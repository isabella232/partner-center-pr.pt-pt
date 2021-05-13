---
title: Acesso baseado em funções do Partner Center Insights
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Conheça as funções específicas necessárias para ver relatórios do Partner Center Insights. Estes incluem os papéis de Visualizador de Relatórios Executivos e Observador de Relatórios.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 803c299311f129c4842a92a27abd9b9addb49f17
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854439"
---
# <a name="role-based-access-control-to-the-partner-center-insights-dashboard"></a>Controlo de acesso baseado em funções ao painel Partner Center Insights

**Funções adequadas**: Administração global | Agente administrativo | Relatório | do espectador Espectador de relatório executivo

O dashboard Insights usa duas novas funções no Partner Center para gerir o acesso dos colaboradores aos relatórios - Visualização de Relatórios Executivos e Visualização de Relatórios.  Os utilizadores na função de Visualizador de Relatório Executivo têm acesso a todos os conjuntos de dados de reporte, enquanto os utilizadores na função 'Observador' de relatórios não terão acesso a conjuntos de dados sensíveis, tais como receitas e dados pessoais do cliente/colaborador.  

Tal como acontece com outras funções do Partner Center, o administrador Global ou o administrador da Conta poderão atribuir os utilizadores a essas funções na página de gestão do Utilizador. As funções podem ser aplicáveis em toda a empresa ou para localizações específicas de MPN. As funções atribuídas para localizações específicas de MPN limitam o utilizador a visualizar dados de reporte associados apenas à localização(s) de MPN selecionada. O parceiro pode selecionar uma ou várias localizações a partir da vista abaixo.

:::image type="content" source="images/pci/roles.png" alt-text="Mostra as definições de funções do Partner Center Insights específicas para visualização de relatórios e visualização de relatórios executivos.":::

>[!Note]
> Os utilizadores que são administradores da MPN a partir de 20 de janeiro de 2020 são automaticamente adicionados ao papel de **Espectador de Relatório Executivo** da empresa para todos os locais para esse inquilino. Estes utilizadores podem, assim, aceder aos relatórios como um visualizador do Relatório Executivo sem qualquer ação explícita exigida pela Administração Global ou Administração de Contas. Os administradores e administradores globais podem sobrepor-se às funções autoatribuídas destes utilizadores para aumentar ou limitar ainda mais as suas capacidades.

## <a name="next-steps"></a>Passos seguintes

- Saiba mais sobre [a Partner Center Insights](partner-center-insights.md) e os seus vários relatórios.
