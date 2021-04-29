---
title: Partner Center Insights - Relatórios de Propensity CloudAscent
description: Conheça os relatórios de Propensity CloudAscent no Partner Center. Inclui informações sobre a propensão de um cliente para comprar produtos Microsoft.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 04/27/2021
ms.openlocfilehash: 91f64faeec0b97be2797d489e152cb84cbb2e192
ms.sourcegitcommit: 8bd2e2f2f0f6bcd0fa202787df5b3c1f786f88f9
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/29/2021
ms.locfileid: "108213467"
---
# <a name="cloudascent-propensity-reports-available-from-partner-center-dashboard"></a>Relatórios de Propensity CloudAscent disponíveis no painel de instrumentos do Partner Center

**Funções adequadas**

- Espectador de relatório executivo
- Espectador de relatório

O painel Partner Center fornece dados de propensão descarregáveis do programa CloudAscent. Os dados mostram a probabilidade dos clientes comprarem produtos microsoft.  Este artigo descreve a desagregação destes dados, como usar a pontuação, e o que significa.

## <a name="summary-definitions"></a>Definições sumárias

- **Clientes SMC**– Este é o número total de clientes nos downloads de propensão.  Os clientes são identificados pelo parceiro de registo.
- **Contratos de Vencimento**– No ano fiscal em curso, estamos a fornecer o número de contratos caducados.
- **Receitas De Caducidade Abertas**– As receitas associadas aos contratos de caducidade abertos.

:::image type="content" source="images/pci/cust-oppor-11.png" alt-text="Screenshot do painel de resumo das oportunidades dos clientes.":::

## <a name="cloudascent-smb-segmentation"></a>Segmentação cloudAscent SMB

O segmento das pequenas e médias empresas (SMB) está dividido em três subsegmentos distintos.

1. **Top Unmanaged** inclui os maiores clientes SMB com mais oportunidades para a Microsoft. Os clientes típicos das Principais Empresas não geridas partilham características semelhantes às contas geridas, com um grande número de colaboradores, grandes orçamentos de TI e gastos, e grandes quantidades de receitas potenciais para a Microsoft.

   Definimos Top Unmanaged de duas maneiras:

   - **Top Ungeraged User Based**– inclui contas com 300 ou mais funcionários. User-Based contas são grandes alvos para compra pela primeira vez, ou expansão de produtos de subscrição baseados no utilizador, como Microsoft 365, Dynamics 365 ou Surface.
   - **Top Unmanaged Compute Based** – inclui contas com potencial Azure superior a $10k. As contas baseadas em computação incluem o Azure existente. contas com potencial significativo para o futuro e contas que ainda não compraram o Azure, mas têm potencial para o Azure superior a $10k.

2. **O Medium Business** inclui clientes existentes e contas de perspetiva com 25 a 300 colaboradores.

3. **O Small Business** inclui empresas com 10-25 colaboradores.

4. **A Very Small Business** inclui empresas com 1-9 colaboradores.

:::image type="content" source="images/pci/cust-oppor-2.png" alt-text="Cliente por tipo SMC.":::

Os subsegmentos **top Unmanaged** e **Medium Business** representam clientes de elevado valor de vida (LTV) para a Microsoft e Microsoft Partners. Por isso, são as principais áreas de foco para impulsionar o crescimento neste segmento. Nestes dois subsegmentos, estamos mais bem posicionados para adquirir a tomada com a Microsoft 365, rentabilizar ainda mais com aplicações de linha de negócios D365/Azure (LOB) e realizar um LTV elevado para a Microsoft.

Hoje temos duas áreas-chave de oportunidade – 1. o nosso cliente adiciona crescimento; 2. enquanto adquirimos bem as tomadas em nuvem que lideram com o Microsoft 365, temos uma grande oportunidade em Dynamics 365 e Azure.

A imagem que se segue representa os quatro Subsegmentos SMB. A CloudAscent prioriza o perfil, pontuação e modelação de todas as contas top unmanaged e medium business.

:::image type="content" source="images/pci/cust-oppor-32.png" alt-text="Screenshot dos subsegmentos SMB.":::

## <a name="cloudascent-machine-learning"></a>CloudAscent Machine Learning

A SMB utiliza tecnologia de machine learning para impulsionar as previsões de clientes de vendas e marketing dentro dos segmentos Top Unmanaged e Medium Business. Como são recolhidos e transformados em recomendações de propensão?

- **Data Collection**: Web crawlers digitalizam e recolhem milhares de milhões de sinais de clientes, pingando os domínios da empresa, e monitorizando posts de blogs, comunicados de imprensa, streams sociais e fóruns técnicos.  Além dos sinais recolhidos, as informações firmográficas são recolhidas de fontes internas e externas, tais como D&B, subscrição Interna da Microsoft e dados transacionais.

- **Machine Learning**: Os sinais são introduzidos no modelo de machine learning que produz um conjunto de dados estruturado de previsões de Vendas e Marketing para cada cliente por produto e cluster em nuvem.  Cada cliente é pontuado usando um modelo semelhante ao SMB de topo da Microsoft que determina o Ajuste do cliente, e algoritmos de aprendizagem automática que integram o comportamento online do cliente definem como Intenção. A pontuação é fundida em clusters que mostram a propensão de um cliente para comprar Produtos Microsoft Cloud.

- **Otimização**: O sistema machine learning otimiza os modelos consumindo os dados de transação mensalmente e os dados de subscrição trimestrais.  Utilizando os dados de vitória/perda, o Machine Learning ajusta os algoritmos e valida que os modelos estão a funcionar como esperado, comparando as recomendações do cluster às oportunidades atuadas no MSX.

:::image type="content" source="images/pci/cust-oppor-4.png" alt-text="Screenshot da aprendizagem automática SMB.":::

## <a name="cloudascent-propensity"></a>CloudAscent Propensity

Como são criadas as recomendações de propensão?

Utilizando sinais recolhidos através de web crawlers e dados fornecidos de várias fontes, consolidamos os dados firmográficos e os sinais de redes sociais do cliente.  A pontuação utiliza estes sinais e dados em modelos de comparação para modelos de ajuste e pontuação para Intenção.

1. Ajuste da conta do cliente

   - Pontos de dados internos e externos que definem firmográficos.

   - Fit scoreing usa um modelo semelhante ao nosso melhor SMB para comparar clientes e ver se eles são um potencial apto para Produtos Microsoft Cloud.

   - A pontuação de ajuste é atualizada trimestralmente

2. Intenção da Conta do Cliente

   - Sinais relacionados com as redes sociais e o comportamento online de um cliente definem a Intenção.

   - A pontuação intencional é sobreposta em cima de apto para definir os clusters.

   - A pontuação de intenção é atualizada mensalmente.

   :::image type="content" source="images/pci/cust-oppor-5.png" alt-text="Modelos preditivos CloudAscent SMB.":::

3. Clustering

   Os sinais de ajuste e intenção são consolidados numa pontuação de agrupamento. CloudAscent tem quatro aglomerados:

      - Act Now - clientes prontos para vendas
      - Avaliar - marketing clientes prontos
      - Nurture - impulsionar campanhas de sensibilização
      - Educar - educar e monitorizar as intenções

   O clustering permite que os utilizadores direcionem clientes específicos para iniciativas de vendas e marketing com base em fatores de segmento, por exemplo: produto, geo, indústria e vertical.

   O separador **modelo de Proensity** nos Livros CloudAscent partilha a propensão e a receita estimada do espaço branco. Para definir o agrupamento de Fit e Intent, passamos pelos seguintes passos:

      1. Utilizando modelos ML, calculamos primeiro a Pontuação de Ajuste do Cliente e a pontuação intencional numa escala de 100.  As pontuações exatas variarão em função dos modelos ML.  Pontuações de exemplo abaixo:

         |**Classificação**|**Pontuação**|
         |---------|:---------|
         |Alto|75 - 100|
         |Médio|55 - 74|
         |Baixo|30 - 54|
         |Muito baixo|0 - 29|

      2. Usando a regra acima, classificamos as empresas como Altas, Médias, Baixas e Muito Baixas em ambos os sinais de ajuste do cliente e de intenções.

      3. Traçamos sinais de ajuste de clientes e intenções numa matriz 2D com cada intersecção representando a propensão. Por exemplo, High Fit + High Intent = A1, representando a maior propensão.

      4. Finalmente, estes segmentos agrupam-se para formar clusters.  Por exemplo, A1, A2, A3, A4 formam o cluster Act Now.

         :::image type="content" source="images/pci/cust-oppor-6.png" alt-text="Modelos CloudAscent.":::

   Para estes clientes, recomendamos direcionar os clientes Act Now e Avaliar.

## <a name="cloudascent-products--models"></a>CloudAscent Produtos & Modelos

O gráfico a seguir proporciona uma visão de cada modelo de propensão dentro da CloudAscent:

:::image type="content" source="images/pci/cust-oppor-7.png" alt-text="Modelo de propensão CloudAscent.":::

Os modelos Whitespace são compostos por previsões para os clientes existentes da Microsoft onde não têm um produto e/ou são novos clientes de perspetiva líquida.

Os modelos upsell utilizam dados de transações para prever o potencial de upsell em Azure e Microsoft 365 SKUs.

Estes clientes já terão tanto o Azure como o Microsoft 365 e o modelo de upsell mostra que é provável que comprem mais do seu SKU existente.

O EOS partilha o fim dos clientes de serviço (EOS) para o Win 7, Office 2010, SQL Server e Windows Server. Os dados do EOS são retirados da MS Sales e sobrepostos com o modelo de propensão CloudAscent, sempre que disponível. Os dados do EOS vivem nas peças de Trabalho Moderno e Azure Sales.
