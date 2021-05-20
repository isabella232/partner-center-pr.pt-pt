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
ms.openlocfilehash: 430aea81964d1b75514b6e1377bd2ba1af41b538
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110153043"
---
# <a name="cloudascent-propensity-reports-available-from-partner-center-dashboard"></a><span data-ttu-id="cfbfd-104">Relatórios de Propensity CloudAscent disponíveis no painel de instrumentos do Partner Center</span><span class="sxs-lookup"><span data-stu-id="cfbfd-104">CloudAscent Propensity reports available from Partner Center dashboard</span></span>

<span data-ttu-id="cfbfd-105">**Funções apropriadas**: | do espectador de relatório executivo Espectador de relatório</span><span class="sxs-lookup"><span data-stu-id="cfbfd-105">**Appropriate roles**: Executive report viewer | Report viewer</span></span>

<span data-ttu-id="cfbfd-106">O painel Partner Center fornece dados de propensão descarregáveis do programa CloudAscent.</span><span class="sxs-lookup"><span data-stu-id="cfbfd-106">The Partner Center dashboard provides downloadable propensity data from the CloudAscent program.</span></span> <span data-ttu-id="cfbfd-107">Os dados mostram a probabilidade dos clientes comprarem produtos microsoft.</span><span class="sxs-lookup"><span data-stu-id="cfbfd-107">The data shows the customers' likelihood to purchase Microsoft products.</span></span>  <span data-ttu-id="cfbfd-108">Este artigo descreve a desagregação destes dados, como usar a pontuação, e o que significa.</span><span class="sxs-lookup"><span data-stu-id="cfbfd-108">This article describes the breakdown of this data, how to use the scoring, and what it means.</span></span>

## <a name="summary-definitions"></a><span data-ttu-id="cfbfd-109">Definições sumárias</span><span class="sxs-lookup"><span data-stu-id="cfbfd-109">Summary definitions</span></span>

- <span data-ttu-id="cfbfd-110">**Clientes SMC**– Este é o número total de clientes nos downloads de propensão.</span><span class="sxs-lookup"><span data-stu-id="cfbfd-110">**SMC Customers**– This is the total number of customers in the propensity downloads.</span></span>  <span data-ttu-id="cfbfd-111">Os clientes são identificados pelo parceiro de registo.</span><span class="sxs-lookup"><span data-stu-id="cfbfd-111">Customers are identified by partner of record.</span></span>
- <span data-ttu-id="cfbfd-112">**Contratos de Vencimento**– No ano fiscal em curso, estamos a fornecer o número de contratos caducados.</span><span class="sxs-lookup"><span data-stu-id="cfbfd-112">**Expire Agreements**– Within the current fiscal year, we're providing the number of expiring agreements.</span></span>
- <span data-ttu-id="cfbfd-113">**Receitas De Caducidade Abertas**– As receitas associadas aos contratos de caducidade abertos.</span><span class="sxs-lookup"><span data-stu-id="cfbfd-113">**Open Expiring Revenue**– The revenue associated to the open expiring agreements.</span></span>

:::image type="content" source="images/pci/cust-oppor-11.png" alt-text="Screenshot do painel de resumo das oportunidades dos clientes.":::

## <a name="cloudascent-smb-segmentation"></a><span data-ttu-id="cfbfd-115">Segmentação cloudAscent SMB</span><span class="sxs-lookup"><span data-stu-id="cfbfd-115">CloudAscent SMB segmentation</span></span>

<span data-ttu-id="cfbfd-116">O segmento das pequenas e médias empresas (SMB) está dividido em três subsegmentos distintos.</span><span class="sxs-lookup"><span data-stu-id="cfbfd-116">The small to medium business (SMB) segment is divided into three distinct sub segments.</span></span>

1. <span data-ttu-id="cfbfd-117">**Top Unmanaged** inclui os maiores clientes SMB com mais oportunidades para a Microsoft.</span><span class="sxs-lookup"><span data-stu-id="cfbfd-117">**Top Unmanaged** includes the largest SMB customers with the most opportunity for Microsoft.</span></span> <span data-ttu-id="cfbfd-118">Os clientes típicos das Principais Empresas não geridas partilham características semelhantes às contas geridas, com um grande número de colaboradores, grandes orçamentos de TI e gastos, e grandes quantidades de receitas potenciais para a Microsoft.</span><span class="sxs-lookup"><span data-stu-id="cfbfd-118">Typical Top Unmanaged customers share similar characteristics to Managed accounts, with large number of employees, large IT budgets and spend, and large amounts of potential revenue for Microsoft.</span></span>

   <span data-ttu-id="cfbfd-119">Definimos Top Unmanaged de duas maneiras:</span><span class="sxs-lookup"><span data-stu-id="cfbfd-119">We define Top Unmanaged in two ways:</span></span>

   - <span data-ttu-id="cfbfd-120">**Top Ungeraged User Based**– inclui contas com 300 ou mais funcionários.</span><span class="sxs-lookup"><span data-stu-id="cfbfd-120">**Top Unmanaged User Based**– includes accounts with 300 or more employees.</span></span> <span data-ttu-id="cfbfd-121">User-Based contas são grandes alvos para compra pela primeira vez, ou expansão de produtos de subscrição baseados no utilizador, como Microsoft 365, Dynamics 365 ou Surface.</span><span class="sxs-lookup"><span data-stu-id="cfbfd-121">User-Based accounts are great targets for first-time purchase, or expansion of user-based subscription products such as Microsoft 365, Dynamics 365, or Surface.</span></span>
   - <span data-ttu-id="cfbfd-122">**Top Unmanaged Compute Based** – inclui contas com potencial Azure superior a $10k.</span><span class="sxs-lookup"><span data-stu-id="cfbfd-122">**Top Unmanaged Compute Based** – includes accounts with Azure potential greater than $10k.</span></span> <span data-ttu-id="cfbfd-123">As contas baseadas em computação incluem o Azure existente.</span><span class="sxs-lookup"><span data-stu-id="cfbfd-123">Compute based accounts include existing Azure.</span></span> <span data-ttu-id="cfbfd-124">contas com potencial significativo para o futuro e contas que ainda não compraram o Azure, mas têm potencial para o Azure superior a $10k.</span><span class="sxs-lookup"><span data-stu-id="cfbfd-124">accounts with significant future year potential and accounts who have yet to purchase Azure yet but have potential for Azure greater than $10k.</span></span>

2. <span data-ttu-id="cfbfd-125">**O Medium Business** inclui clientes existentes e contas de perspetiva com 25 a 300 colaboradores.</span><span class="sxs-lookup"><span data-stu-id="cfbfd-125">**Medium Business** includes existing customers and prospect accounts with 25 to 300 employees.</span></span>

3. <span data-ttu-id="cfbfd-126">**O Small Business** inclui empresas com 10-25 colaboradores.</span><span class="sxs-lookup"><span data-stu-id="cfbfd-126">**Small Business** includes businesses with 10-25 employees.</span></span>

4. <span data-ttu-id="cfbfd-127">**A Very Small Business** inclui empresas com 1-9 colaboradores.</span><span class="sxs-lookup"><span data-stu-id="cfbfd-127">**Very Small Business** includes businesses with 1-9 employees.</span></span>

:::image type="content" source="images/pci/cust-oppor-2.png" alt-text="Cliente por tipo SMC.":::

<span data-ttu-id="cfbfd-129">Os subsegmentos **top Unmanaged** e **Medium Business** representam clientes de elevado valor de vida (LTV) para a Microsoft e Microsoft Partners.</span><span class="sxs-lookup"><span data-stu-id="cfbfd-129">**Top Unmanaged** and **Medium Business** subsegments represent high life-time value (LTV) customers for Microsoft, and Microsoft Partners.</span></span> <span data-ttu-id="cfbfd-130">Por isso, são as principais áreas de foco para impulsionar o crescimento neste segmento.</span><span class="sxs-lookup"><span data-stu-id="cfbfd-130">Because of this, they're the lead areas of focus for driving growth in this segment.</span></span> <span data-ttu-id="cfbfd-131">Nestes dois subsegmentos, estamos mais bem posicionados para adquirir a tomada com a Microsoft 365, rentabilizar ainda mais com aplicações de linha de negócios D365/Azure (LOB) e realizar um LTV elevado para a Microsoft.</span><span class="sxs-lookup"><span data-stu-id="cfbfd-131">In these two subsegments, we're better positioned to acquire the socket with Microsoft 365, monetize further with D365/Azure line of business (LOB) apps, and realize a high LTV for Microsoft.</span></span>

<span data-ttu-id="cfbfd-132">Hoje temos duas áreas-chave de oportunidade – 1.</span><span class="sxs-lookup"><span data-stu-id="cfbfd-132">Today we have two key areas of opportunity – 1.</span></span> <span data-ttu-id="cfbfd-133">o nosso cliente adiciona crescimento; 2.</span><span class="sxs-lookup"><span data-stu-id="cfbfd-133">our customer adds growth; 2.</span></span> <span data-ttu-id="cfbfd-134">enquanto adquirimos bem as tomadas em nuvem que lideram com o Microsoft 365, temos uma grande oportunidade em Dynamics 365 e Azure.</span><span class="sxs-lookup"><span data-stu-id="cfbfd-134">while we do well acquiring cloud sockets leading with Microsoft 365, we have a large opportunity in Dynamics 365 and Azure.</span></span>

<span data-ttu-id="cfbfd-135">A imagem que se segue representa os quatro Subsegmentos SMB.</span><span class="sxs-lookup"><span data-stu-id="cfbfd-135">The following screenshot represents the four SMB Subsegments.</span></span> <span data-ttu-id="cfbfd-136">A CloudAscent prioriza o perfil, pontuação e modelação de todas as contas top unmanaged e medium business.</span><span class="sxs-lookup"><span data-stu-id="cfbfd-136">CloudAscent prioritize the profiling, scoring, and modeling of all Top Unmanaged and Medium Business accounts.</span></span>

:::image type="content" source="images/pci/cust-oppor-32.png" alt-text="Screenshot dos subsegmentos SMB.":::

## <a name="cloudascent-machine-learning"></a><span data-ttu-id="cfbfd-138">CloudAscent Machine Learning</span><span class="sxs-lookup"><span data-stu-id="cfbfd-138">CloudAscent Machine Learning</span></span>

<span data-ttu-id="cfbfd-139">A SMB utiliza tecnologia de machine learning para impulsionar as previsões de clientes de vendas e marketing dentro dos segmentos Top Unmanaged e Medium Business.</span><span class="sxs-lookup"><span data-stu-id="cfbfd-139">SMB uses machine learning technology to drive sales and marketing customer predictions within the Top Unmanaged and Medium Business segments.</span></span> <span data-ttu-id="cfbfd-140">Como são recolhidos e transformados em recomendações de propensão?</span><span class="sxs-lookup"><span data-stu-id="cfbfd-140">How are signals collected and turned into propensity recommendations?</span></span>

- <span data-ttu-id="cfbfd-141">**Data Collection**: Web crawlers digitalizam e recolhem milhares de milhões de sinais de clientes, pingando os domínios da empresa, e monitorizando posts de blogs, comunicados de imprensa, streams sociais e fóruns técnicos.</span><span class="sxs-lookup"><span data-stu-id="cfbfd-141">**Data Collection**: Web crawlers scan and collect billions of customer signals by pinging the company domains, and monitoring blog posts, press releases, social streams, and technical forums.</span></span>  <span data-ttu-id="cfbfd-142">Além dos sinais recolhidos, as informações firmográficas são recolhidas de fontes internas e externas, tais como D&B, subscrição Interna da Microsoft e dados transacionais.</span><span class="sxs-lookup"><span data-stu-id="cfbfd-142">In addition to the collected signals, firmographics information is collected from both internal and external sources such as D&B, Microsoft Internal subscription and transactional data.</span></span>

- <span data-ttu-id="cfbfd-143">**Machine Learning**: Os sinais são introduzidos no modelo de machine learning que produz um conjunto de dados estruturado de previsões de Vendas e Marketing para cada cliente por produto e cluster em nuvem.</span><span class="sxs-lookup"><span data-stu-id="cfbfd-143">**Machine Learning**: The signals are fed into the machine learning model that outputs a structured data set of Sales and Marketing predictions for each customer by cloud product and cluster.</span></span>  <span data-ttu-id="cfbfd-144">Cada cliente é pontuado usando um modelo semelhante ao SMB de topo da Microsoft que determina o Ajuste do cliente, e algoritmos de aprendizagem automática que integram o comportamento online do cliente definem como Intenção.</span><span class="sxs-lookup"><span data-stu-id="cfbfd-144">Each customer is scored using a look alike model to Microsoft's top SMB that determines the customer's Fit, and machine learning algorithms that integrate the customer's online behavior define as Intent.</span></span> <span data-ttu-id="cfbfd-145">A pontuação é fundida em clusters que mostram a propensão de um cliente para comprar Produtos Microsoft Cloud.</span><span class="sxs-lookup"><span data-stu-id="cfbfd-145">The scoring is merged into clusters that show a customer's propensity to purchase Microsoft Cloud Products.</span></span>

- <span data-ttu-id="cfbfd-146">**Otimização**: O sistema machine learning otimiza os modelos consumindo os dados de transação mensalmente e os dados de subscrição trimestrais.</span><span class="sxs-lookup"><span data-stu-id="cfbfd-146">**Optimization**: The Machine Learning system optimizes the models by consuming the transaction data monthly and the subscription data quarterly.</span></span>  <span data-ttu-id="cfbfd-147">Utilizando os dados de vitória/perda, o Machine Learning ajusta os algoritmos e valida que os modelos estão a funcionar como esperado, comparando as recomendações do cluster às oportunidades atuadas no MSX.</span><span class="sxs-lookup"><span data-stu-id="cfbfd-147">Using the win/loss data, the Machine Learning adjusts the algorithms and validates that the models are working as expected by comparing cluster recommendations to opportunities acted upon in MSX.</span></span>

:::image type="content" source="images/pci/cust-oppor-4.png" alt-text="Screenshot da aprendizagem automática SMB.":::

## <a name="cloudascent-propensity"></a><span data-ttu-id="cfbfd-149">CloudAscent Propensity</span><span class="sxs-lookup"><span data-stu-id="cfbfd-149">CloudAscent Propensity</span></span>

<span data-ttu-id="cfbfd-150">Como são criadas as recomendações de propensão?</span><span class="sxs-lookup"><span data-stu-id="cfbfd-150">How are propensity recommendations created?</span></span>

<span data-ttu-id="cfbfd-151">Utilizando sinais recolhidos através de web crawlers e dados fornecidos de várias fontes, consolidamos os dados firmográficos e os sinais de redes sociais do cliente.</span><span class="sxs-lookup"><span data-stu-id="cfbfd-151">Using signals collected via web crawlers and data provided from various sources, we consolidate the firmographics data and customer's social media signals.</span></span>  <span data-ttu-id="cfbfd-152">A pontuação utiliza estes sinais e dados em modelos de comparação para modelos de ajuste e pontuação para Intenção.</span><span class="sxs-lookup"><span data-stu-id="cfbfd-152">The scoring uses these signals and data in comparison models for fit and scoring models for Intent.</span></span>

1. <span data-ttu-id="cfbfd-153">Ajuste da conta do cliente</span><span class="sxs-lookup"><span data-stu-id="cfbfd-153">Customer Account Fit</span></span>

   - <span data-ttu-id="cfbfd-154">Pontos de dados internos e externos que definem firmográficos.</span><span class="sxs-lookup"><span data-stu-id="cfbfd-154">Internal and External data points that define firmographics.</span></span>

   - <span data-ttu-id="cfbfd-155">Fit scoreing usa um modelo semelhante ao nosso melhor SMB para comparar clientes e ver se eles são um potencial apto para Produtos Microsoft Cloud.</span><span class="sxs-lookup"><span data-stu-id="cfbfd-155">Fit scoring uses a look alike model to our best SMB to compare customers and see if they're a potential  fit for Microsoft Cloud Products.</span></span>

   - <span data-ttu-id="cfbfd-156">A pontuação de ajuste é atualizada trimestralmente</span><span class="sxs-lookup"><span data-stu-id="cfbfd-156">Fit scoring is updated quarterly</span></span>

2. <span data-ttu-id="cfbfd-157">Intenção da Conta do Cliente</span><span class="sxs-lookup"><span data-stu-id="cfbfd-157">Customer Account Intent</span></span>

   - <span data-ttu-id="cfbfd-158">Sinais relacionados com as redes sociais e o comportamento online de um cliente definem a Intenção.</span><span class="sxs-lookup"><span data-stu-id="cfbfd-158">Signals related to Social media and a customer's online behavior define Intent.</span></span>

   - <span data-ttu-id="cfbfd-159">A pontuação intencional é sobreposta em cima de apto para definir os clusters.</span><span class="sxs-lookup"><span data-stu-id="cfbfd-159">Intent scoring is overlaid on top of fit to define the clusters.</span></span>

   - <span data-ttu-id="cfbfd-160">A pontuação de intenção é atualizada mensalmente.</span><span class="sxs-lookup"><span data-stu-id="cfbfd-160">Intent scoring is updated monthly.</span></span>

   :::image type="content" source="images/pci/cust-oppor-5.png" alt-text="Modelos preditivos CloudAscent SMB.":::

3. <span data-ttu-id="cfbfd-162">Clustering</span><span class="sxs-lookup"><span data-stu-id="cfbfd-162">Clustering</span></span>

   <span data-ttu-id="cfbfd-163">Os sinais de ajuste e intenção são consolidados numa pontuação de agrupamento.</span><span class="sxs-lookup"><span data-stu-id="cfbfd-163">The Signals for fit and intent are consolidated into a clustering score.</span></span> <span data-ttu-id="cfbfd-164">CloudAscent tem quatro aglomerados:</span><span class="sxs-lookup"><span data-stu-id="cfbfd-164">CloudAscent has four clusters:</span></span>

      - <span data-ttu-id="cfbfd-165">Act Now - clientes prontos para vendas</span><span class="sxs-lookup"><span data-stu-id="cfbfd-165">Act Now - sales ready customers</span></span>
      - <span data-ttu-id="cfbfd-166">Avaliar - marketing clientes prontos</span><span class="sxs-lookup"><span data-stu-id="cfbfd-166">Evaluate - marketing ready customers</span></span>
      - <span data-ttu-id="cfbfd-167">Nurture - impulsionar campanhas de sensibilização</span><span class="sxs-lookup"><span data-stu-id="cfbfd-167">Nurture - drive awareness campaigns</span></span>
      - <span data-ttu-id="cfbfd-168">Educar - educar e monitorizar as intenções</span><span class="sxs-lookup"><span data-stu-id="cfbfd-168">Educate - educate and monitor for intent</span></span>

   <span data-ttu-id="cfbfd-169">O clustering permite que os utilizadores direcionem clientes específicos para iniciativas de vendas e marketing com base em fatores de segmento, por exemplo: produto, geo, indústria e vertical.</span><span class="sxs-lookup"><span data-stu-id="cfbfd-169">The clustering allows users to target specific customers for sales and marketing initiatives based on segment factors, for example: product, geo, industry and vertical.</span></span>

   <span data-ttu-id="cfbfd-170">O separador **modelo de Proensity** nos Livros CloudAscent partilha a propensão e a receita estimada do espaço branco.</span><span class="sxs-lookup"><span data-stu-id="cfbfd-170">The **Propensity model** tab in the CloudAscent Workbooks shares the propensity and the estimated whitespace revenue.</span></span> <span data-ttu-id="cfbfd-171">Para definir o agrupamento de Fit e Intent, passamos pelos seguintes passos:</span><span class="sxs-lookup"><span data-stu-id="cfbfd-171">To define the clustering of Fit and Intent, we go through the following steps:</span></span>

      1. <span data-ttu-id="cfbfd-172">Utilizando modelos ML, calculamos primeiro a Pontuação de Ajuste do Cliente e a pontuação intencional numa escala de 100.</span><span class="sxs-lookup"><span data-stu-id="cfbfd-172">Using ML Models, we first calculate Customer Fit Score and intent Score on a scale of 100.</span></span>  <span data-ttu-id="cfbfd-173">As pontuações exatas variarão em função dos modelos ML.</span><span class="sxs-lookup"><span data-stu-id="cfbfd-173">Exact Scores will vary based on ML Models.</span></span>  <span data-ttu-id="cfbfd-174">Pontuações de exemplo abaixo:</span><span class="sxs-lookup"><span data-stu-id="cfbfd-174">Example Scores Below:</span></span>

         |<span data-ttu-id="cfbfd-175">**Classificação**</span><span class="sxs-lookup"><span data-stu-id="cfbfd-175">**Classification**</span></span>|<span data-ttu-id="cfbfd-176">**Pontuação**</span><span class="sxs-lookup"><span data-stu-id="cfbfd-176">**Score**</span></span>|
         |---------|:---------|
         |<span data-ttu-id="cfbfd-177">Alto</span><span class="sxs-lookup"><span data-stu-id="cfbfd-177">High</span></span>|<span data-ttu-id="cfbfd-178">75 - 100</span><span class="sxs-lookup"><span data-stu-id="cfbfd-178">75 - 100</span></span>|
         |<span data-ttu-id="cfbfd-179">Médio</span><span class="sxs-lookup"><span data-stu-id="cfbfd-179">Medium</span></span>|<span data-ttu-id="cfbfd-180">55 - 74</span><span class="sxs-lookup"><span data-stu-id="cfbfd-180">55 - 74</span></span>|
         |<span data-ttu-id="cfbfd-181">Baixo</span><span class="sxs-lookup"><span data-stu-id="cfbfd-181">Low</span></span>|<span data-ttu-id="cfbfd-182">30 - 54</span><span class="sxs-lookup"><span data-stu-id="cfbfd-182">30 - 54</span></span>|
         |<span data-ttu-id="cfbfd-183">Muito baixo</span><span class="sxs-lookup"><span data-stu-id="cfbfd-183">Very Low</span></span>|<span data-ttu-id="cfbfd-184">0 - 29</span><span class="sxs-lookup"><span data-stu-id="cfbfd-184">0 - 29</span></span>|

      2. <span data-ttu-id="cfbfd-185">Usando a regra acima, classificamos as empresas como Altas, Médias, Baixas e Muito Baixas em ambos os sinais de ajuste do cliente e de intenções.</span><span class="sxs-lookup"><span data-stu-id="cfbfd-185">Using the rule above, we classify companies to be High, Medium, Low, and Very Low across both Customer Fit and Intent Signals.</span></span>

      3. <span data-ttu-id="cfbfd-186">Traçamos sinais de ajuste de clientes e intenções numa matriz 2D com cada intersecção representando a propensão.</span><span class="sxs-lookup"><span data-stu-id="cfbfd-186">We plot customer fit and intent signals on a 2D matrix with each intersection representing the propensity.</span></span> <span data-ttu-id="cfbfd-187">Por exemplo, High Fit + High Intent = A1, representando a maior propensão.</span><span class="sxs-lookup"><span data-stu-id="cfbfd-187">For Example, High Fit + High Intent = A1, representing the highest propensity.</span></span>

      4. <span data-ttu-id="cfbfd-188">Finalmente, estes segmentos agrupam-se para formar clusters.</span><span class="sxs-lookup"><span data-stu-id="cfbfd-188">Finally, these segments group to form clusters.</span></span>  <span data-ttu-id="cfbfd-189">Por exemplo, A1, A2, A3, A4 formam o cluster Act Now.</span><span class="sxs-lookup"><span data-stu-id="cfbfd-189">For Example, A1, A2, A3, A4 form the Act Now cluster.</span></span>

         :::image type="content" source="images/pci/cust-oppor-6.png" alt-text="Modelos CloudAscent.":::

   <span data-ttu-id="cfbfd-191">Para estes clientes, recomendamos direcionar os clientes Act Now e Avaliar.</span><span class="sxs-lookup"><span data-stu-id="cfbfd-191">For these customers, we recommend targeting Act Now and Evaluate customers.</span></span>

## <a name="cloudascent-products--models"></a><span data-ttu-id="cfbfd-192">CloudAscent Produtos & Modelos</span><span class="sxs-lookup"><span data-stu-id="cfbfd-192">CloudAscent Products & Models</span></span>

<span data-ttu-id="cfbfd-193">O gráfico a seguir proporciona uma visão de cada modelo de propensão dentro da CloudAscent:</span><span class="sxs-lookup"><span data-stu-id="cfbfd-193">The following graphic provides a view of each propensity model within CloudAscent:</span></span>

:::image type="content" source="images/pci/cust-oppor-7.png" alt-text="Modelo de propensão CloudAscent.":::

<span data-ttu-id="cfbfd-195">Os modelos Whitespace são compostos por previsões para os clientes existentes da Microsoft onde não têm um produto e/ou são novos clientes de perspetiva líquida.</span><span class="sxs-lookup"><span data-stu-id="cfbfd-195">Whitespace models are composed of predictions for existing Microsoft customers where they don't have a product and/or are net new prospect customers.</span></span>

<span data-ttu-id="cfbfd-196">Os modelos upsell utilizam dados de transações para prever o potencial de upsell em Azure e Microsoft 365 SKUs.</span><span class="sxs-lookup"><span data-stu-id="cfbfd-196">Upsell models use transaction data to predict the potential for upsell in Azure and Microsoft 365 SKUs.</span></span>

<span data-ttu-id="cfbfd-197">Estes clientes já terão tanto o Azure como o Microsoft 365 e o modelo de upsell mostra que é provável que comprem mais do seu SKU existente.</span><span class="sxs-lookup"><span data-stu-id="cfbfd-197">These customers will already have both Azure or Microsoft 365 and the upsell model shows that they’re likely to purchase more of their existing SKU.</span></span>

<span data-ttu-id="cfbfd-198">O EOS partilha o fim dos clientes de serviço (EOS) para o Win 7, Office 2010, SQL Server e Windows Server.</span><span class="sxs-lookup"><span data-stu-id="cfbfd-198">EOS shares the end of service (EOS) customers for Win 7, Office 2010, SQL Server, and Windows Server.</span></span> <span data-ttu-id="cfbfd-199">Os dados do EOS são retirados da MS Sales e sobrepostos com o modelo de propensão CloudAscent, sempre que disponível.</span><span class="sxs-lookup"><span data-stu-id="cfbfd-199">The EOS data is pulled from MS Sales and overlaid with the CloudAscent propensity modeling where available.</span></span> <span data-ttu-id="cfbfd-200">Os dados do EOS vivem nas peças de Trabalho Moderno e Azure Sales.</span><span class="sxs-lookup"><span data-stu-id="cfbfd-200">EOS data lives in the Modern Work and Azure Sales plays.</span></span>
