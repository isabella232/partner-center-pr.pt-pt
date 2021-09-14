---
title: Partner Center Informações Microsoft Learn analytics
ms.topic: article
ms.date: 08/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: Acompanhe os alunos da sua empresa aproveitando dados sobre formação individual, módulos completos, percursos de aprendizagem completos e muito mais.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: b291ee52c9c6e72dc50aab9aa386177d9778cbd1
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/13/2021
ms.locfileid: "126247511"
---
# <a name="use-microsoft-learn-analytics-reports"></a>Utilize relatórios de análise do Microsoft Learn

**Funções adequadas**: Administração global | Administrador sócio da MPN

O relatório [microsoft Learn](/learn/) fornece-lhe informações sobre os alunos da sua empresa, incluindo os módulos que completaram e os caminhos de aprendizagem em que estão. O relatório apresenta o estado de cada aluno individual. Os administradores globais e os administradores da MPN para uma empresa podem ver os dados.

## <a name="how-to-read-the-report"></a>Como ler o relatório

### <a name="summary-charts"></a>Gráficos de resumo

Estes gráficos resumem a contagem e as tendências cumulativas mensais para indivíduos treinados, conclusão de módulos e caminhos de aprendizagem.

**Indivíduos treinados contam:** Uma contagem de todos os alunos distintos que completaram pelo menos um módulo durante a gama de datas selecionadas 

**Mini gráfico de tendência de indivíduos treinados**: Mês ao longo do mês contagem cumulativa dos alunos ativos 

**Contagem de conclusões** do módulo : Contagem de conclusões do Módulo pelos alunos da empresa do parceiro durante a gama de datas selecionadas.
Por exemplo, se o "Módulo 1" for concluído por 15 indivíduos, e o "Módulo 2" tiver sido concluído pelos mesmos 15 indivíduos, a contagem de conclusões do módulo será de 30. A data de conclusão do módulo deve cair na gama de datas selecionada.

**Mini gráfico de conclusão** do módulo : Mês ao longo do mês contagem cumulativa das conclusões do módulo 

**Aprendizagem contagem de conclusões** do percurso : Contagem de Aprendizagem conclusões do percurso pelos alunos da empresa do parceiro durante a gama de datas selecionadas.
Por exemplo, se Aprendizagem Caminho "Caminho 1" for concluído por 20 indivíduos, e o caminho Aprendizagem "caminho 2" tiver sido concluído pelos mesmos 20 indivíduos, a contagem de conclusão do caminho de Aprendizagem será de 40. A data de conclusão Aprendizagem caminho deve estar dentro do intervalo de datas selecionado.

**Aprendizagem percurso completa mini gráfico de tendência**: Mês ao mês contagem cumulativa das conclusões do percurso de aprendizagem 

### <a name="trained-individuals-monthly-trend"></a>Tendência mensal dos indivíduos treinados

Estes dados são a tendência dos utilizadores da sua empresa que completaram um módulo pela primeira vez nesse mês. 

**O Eixo X** é mensal para o filtro de tempo selecionado. 

**Y-Axis** é a contagem de alunos ativos que se registaram (primeira conclusão de um módulo) durante esse mês. Isto não é cumulativo.

### <a name="module-completions-monthly-trend"></a>Conclusão do módulo tendência mensal

Estes dados são a tendência dos módulos completados por todos os utilizadores da sua empresa durante esse mês. (não cumulativo) 

**O Eixo X** é mensal para o filtro de tempo selecionado. 

**Y-Axis** é a contagem das conclusões do módulo durante esse mês. Isto não é cumulativo.

### <a name="learning-path-completions-monthly-trend"></a>Aprendizagem percurso completa tendência mensal

Estes dados são a tendência de aprendizagem dos percursos concluídos pelos utilizadores da sua empresa durante esse mês. (não cumulativo) 

**O Eixo X** é mensal para o filtro de tempo selecionado. 

**Y-Axis** é a contagem de conclusões do módulo nesse mês. Isto não é cumulativo.

### <a name="learning-path-completion-tabs"></a>separadores de conclusão do caminho Aprendizagem

#### <a name="module-tab"></a>Separador de módulos

Este separador inclui a desagregação de módulos preenchidos na sua empresa pelos cinco principais nomes de módulos; O produto ao qual o módulo está associado; e a função de utilizador pertinente ao módulo.  

- Gráfico de donuts de conclusão do módulo: repartição das conclusões do módulo (contagem apresentada na secção resumo) pelos nomes do módulo.

Número exibido no centro do gráfico é o total de módulos concluídos

- Conclusões por função: desagregação das conclusões do módulo pelo papel do módulo. Se um módulo estiver associado a múltiplas funções, cada uma das funções é adicionada à contagem de conclusões do módulo.

Número apresentado no centro da tabela é o número de funções distintas para as conclusões do módulo. 

- Conclusão por produto: desagregação das conclusões do módulo pelo produto para o qual o módulo está mapeado. Se um módulo estiver associado a vários produtos, cada um dos produtos é adicionado à contagem de acabamentos do módulo.    

Número apresentado no centro da tabela é o número de produtos distintos para a conclusão do módulo.  

#### <a name="learning-path-tab"></a>separador de caminho Aprendizagem

Este separador inclui uma desagregação dos percursos de aprendizagem concluídos na sua empresa pelos cinco principais nomes de módulos; o produto para o qual o caminho de aprendizagem é mapeado; e o papel pertinente a este caminho de aprendizagem.  

- Aprendizagem caminhos completa gráfico de donuts: desagregação das Aprendizagem conclusões do caminho (contagem exibida na secção de resumo) pelo nome.

- Conclusão por função: desagregação dos caminhos de aprendizagem concluídos pelo papel. Se um módulo estiver associado a múltiplas funções, cada uma das funções é adicionada à contagem de conclusões do módulo.

- Conclusão por produto: desagregação dos caminhos de aprendizagem concluídos pelo Produto para o qual o caminho de aprendizagem está mapeado. Se um módulo estiver associado a vários produtos, cada um dos produtos é adicionado à contagem de acabamentos do módulo.

### <a name="completions-by-learning-individuals"></a>Conclusões através da aprendizagem de indivíduos

Isto lista os utilizadores treinados na sua empresa e detalhes dos seus módulos e caminhos de aprendizagem completos.

O Microsoft Learn identifica os alunos com um ID de objeto de utilizador. No **separador Módulos,** todos os alunos são classificados pelos módulos concluídos. São apresentados com o seu nome de utilizador Microsoft Learn, Object ID e os módulos contam. Pode pesquisar com o nome de utilizador. 

Sob o **Aprendizagem caminhos abas todos** os alunos classificados por caminhos de aprendizagem concluídos, são exibidos com o nome de visualização do aluno, ID de objeto e contagem de módulos.

Para obter os detalhes de um aprendiz usando o ID do objeto do utilizador: 

1. Inscreva-se no [Graph Explorer.](https://developer.microsoft.com/graph/graph-explorer ) (Você deve ser o administrador global do inquilino AZure AD da sua empresa.)

2. Copie o ID do objeto do utilizador para a [área realçada](https://graph.microsoft.com/v1.0/users/a9633ad7-c8dc-4587-b119-0bc286b0711f) no Graph Explorer. 

## <a name="frequently-asked-questions-faq"></a>Perguntas Mais Frequentes (FAQ)

1. Não consigo ver os detalhes da aprendizagem da minha empresa.

   Este relatório está disponível para parceiros que tenham uma conta no Partner Center. Se ainda estiver no Centro de Membros de Parceiros, não poderá ver este relatório.

2. Quem na minha empresa pode ver este relatório? 

   A administração global e o administrador da MPN podem ver o relatório.

3. Como posso certificar-me de que todos os nossos utilizadores associam as suas contas Microsoft Learn à sua conta Partner Center?

   *Após a administração global adicionar um novo utilizador,* esse utilizador deve ir ao [Microsoft Learn](/learn/) para ligar a sua conta corporativa de Azure Ative Directory (AD) ou conta de trabalho com a sua conta Learn. Isto garante que o separador Informações Aprendizagem mostrará os cursos e competências certos.
   
   O utilizador tem de:
   
   1. Inscreva-se no [Microsoft Learn](/learn/).
   2. Selecione a sua imagem de perfil e, em seguida, selecione **O meu perfil**.
   3. Selecione **Definições**.
   4. Sob **gestão de conta**, adicione a sua conta de trabalho em contas **ligadas**.

4. Posso ver todos os utilizadores da empresa que assinam no Microsoft Learn com uma conta MSA neste relatório?

   Atualmente, a melhor maneira de o fazer é adicionar estes utilizadores ao seu inquilino Azure AD e, em seguida, adicioná-los ao Partner Center para que possam associar a sua conta Microsoft Learn através **do meu perfil** no Partner Center. 

   Para os utilizadores que apenas utilizam a sua conta MSA para a formação, num futuro próximo, a equipa do Microsoft Learn permitirá associar o seu email de trabalho ao seu perfil Microsoft Learn. 

## <a name="next-steps"></a>Passos seguintes

Para mais relatórios, consulte [o Partner Center Informações](partner-center-insights.md).

>[!NOTE] 
> Pode descarregar os dados brutos que alimentam este relatório a partir da secção Relatórios de Descarregamento no painel de Informações. [Saiba mais](insights-download-reports.md) 
