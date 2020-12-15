---
title: Insights definições de dados
ms.topic: article
ms.date: 12/14/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: O documento fornece a lista de vários relatórios e as definições de dados de cada relatório, que podem ser descarregados a partir da página do relatório Insights Download.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d4a805957fac7c7cff373d807347b7c6d0b13d6f
ms.sourcegitcommit: 4e36d1a4ca2f074b55f9b9a08e300734eae1f06d
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/15/2020
ms.locfileid: "97502132"
---
# <a name="export--data-definitions"></a>Exportação - Definições de dados 

 **Funções adequadas** 

- Espectador de relatório 
- Espectador de relatório executivo 

## <a name="introduction"></a>Introdução 

O centro de Relatórios de Descarregamento no dashboard Insights permite-lhe exportar os conjuntos de dados brutos.  

Os vários relatórios, que podem ser descarregados juntamente com a definição de dados são os seguintes: 

**Perfil do parceiro**: As definições de dados dos vários campos do relatório de perfil são: 


| **Nome da coluna** | **Descrição de Dados** |
|---------|:---------|
|MPNId|ID da rede de parceiros da Microsoft|
|PartnerName|Nome do parceiro |
|PGA_MPNId|Parceiro Global Account MPN ID|
|PGA_PartnerName|Nome da conta global do parceiro|
|City|Localização da cidade do parceiro |
|País|Localização do país do Parceiro |
|HierarquiaLevel|Indica se é um ID MPN global ou iD MPN de localização|

**Detalhes do cliente**: As definições de dados das várias áreas do relatório Dados do Cliente são:

| **Nome da coluna** | **Descrição de Dados** |
|---------|:---------|
|CustomerName|Nome do Cliente |
|CustomerTenantId|ID do Inquilino do Cliente |
|CustomerTpid|Identificador principal do cliente |
|Gestão de Clientes|Segmento de Clientes |
|Mercado de Clientes|Mercado Geográfico do Cliente  |
|CustomerStatus|Estado do Cliente (Ativo /Inativo) |
|Produto|O produto vendido ao cliente pela MPN. Este será um de O365, D365, Enterprise Mobility, Power BI, Microsoft Azure.|
|SKU|   SKU de produto|
|Mensal| Mês para o qual é reportada a utilização e receitas|
|MPNId| ID da rede de parceiros da Microsoft|
|PartnerName|   Nome do Parceiro|
|PartnerLocation|   Localização geográfica do parceiro|
|PartnerAttributionType|    Tipo de parceiro de atribuição|
|SalesChannel|  Canal de Vendas|
|Lugares disponíveis|    Lugares disponíveis| 
|RevenueUSD|    Receitas em USD|

**Desempenho do revendedor**: As definições de dados dos vários campos dos relatórios de desempenho do Revendedor são:

> [!Note]
> As receitas e os dados ACR só estão disponíveis para utilizadores que sejam telespectadores do Relatório Executivo.

| **Nome da coluna** | **Descrição de Dados** |
|---------|:---------|
|RevendedorMpnid|Revendedor Identificador de Rede de Parceiros microsoft| 
|ResellerName|Nome do revendedor|
|RevendedorMarket|País de Mercado Revendedor| 
|IndiretoProviderMPNId|Identificador de rede de parceiros de fornecedor indireto microsoft|
|Nome IndiretoProvider|Nome do fornecedor indireto|
|Mensal|Mês para o qual é reportada a utilização e receitas|
|Produto|Nome do Produto|
|SubscriçãoID|Identificador de Assinatura|
|Lugares disponíveis|Número de lugares disponíveis|
|Caixas designadas|Número de lugares atribuídos|
|BilledRevenueusd|Receitas Faturadas (em $)|
|CustomerName|Nome do Cliente| 
|CustomerTPid|Identificador principal do cliente| 
|Gestão de Clientes|Segmento de Clientes |
|Mercado de Clientes|Mercado Geográfico do Cliente |
|RevendedorStatus|Estado do revendedor| 

**Detalhes das assinaturas**: As definições de dados dos vários campos do relatório Detalhes de Subscrição são:

>[!Note]
>Receitas e dados ACR só estão disponíveis para utilizadores que sejam telespectadores do Relatório Executivo

| **Nome da coluna** | **Descrição de Dados** |
|---------|:---------|
|SubscriptionId|    GUIA da Assinatura|
|SubscriçãoStartDate| Data de Início da Subscrição|
|SubscriçãoEndDate|   Data de Fim da Subscrição|
|Estado de Subscrição| Estado da Subscrição (Ativo ou Churned)|
|Mensal| Mês para o qual é reportada a utilização e receitas|
|IsautoRenew|   Indica se a Subscrição é Renovação Automática ou Não (Y/N)|
|CustomerName|  Nome do Cliente| 
|CustomerTenantId|  Guia do Cliente|
|CustomerTpid|  Identificador de pais de topo do cliente| 
|Gestão de Clientes|   Segmento de Mercado do Cliente| 
|Mercado de Clientes|    Mercado Geográfico do Cliente|
|Produto|   Produto vendido ao Cliente pelo Parceiro| 
|SKU|   Sku do Produto |
|MPNId| ID da Rede de Parceiros microsoft do parceiro |
|PartnerName|   Nome do Parceiro |
|PartnerLocation|   Localização Geográfica do Parceiro |
|PartnerAttributionType|    Tipo de atribuição para a subscrição|
|SalesChannel|  Canal das Vendas (Direto/CSP, etc.) |
|Lugares disponíveis|    Assento disponível atual|
|RevenueUSD|    Receitas em USD|
|ID de inscrição| ID de inscrição da assinatura|

**Utilização Azure**: As definições de dados dos vários campos do relatório de utilização do Azure são:

| **Nome da coluna** | **Descrição de Dados** |
|---------|:---------|
|SubscriptionId|    GUIA da Assinatura|
|SubscriçãoStartDate| A data do início da subscrição.|
|SubscriçãoEndDate|   A data em que a subscrição termina.|
|Estado de Subscrição| Estado atual da Subscrição (Período Aberto/Fechado/Ativo/InGrace)|
|Mensal| Data agregada por mês |
|ServiceName|   Nome do serviço Azure|
|MeterCategory| Nome da categoria de contador|
|Unidades de utilização|    O número de unidades utilizadas durante o ciclo de faturação |
|CustomerName|  Nome do Cliente |
|CustomerTenantId|  ID do cliente do inquilino |
|CustomerTpid|  ID do pai de topo do cliente |
|Gestão de Clientes|   Segmento do Cliente |
|Mercado de Clientes|    Mercado Geográfico do Cliente |
|MPNId  |ID da Rede de Parceiros microsoft do cliente |
|PartnerName|   Nome do Parceiro |
|PartnerLocation    |Localização geográfica do país do parceiro |
|PartnerAttributionType |Tipo de parceiro de atribuição|
|SalesChannel|  Canal das Vendas (Direto/CSP Indirect/CSP Direto, etc.) |
|ACR_USD|   Azure consumiu receitas em USD|
|ID de inscrição| ID de inscrição da assinatura Azure|

**Office 365 -Licença De utilização**: As definições de dados dos vários campos do Office 365 -Relatório de Utilização da Licença são:

| **Nome da coluna** | **Descrição de Dados** |
|---------|:---------|
|CustomerTenantId|  ID do cliente do inquilino| 
|CustomerTpid|  ID do pai de topo do cliente |
|Nome da carga de trabalho|  Sfb, Equipas, EXO |
|Mensal| Mês para o qual o uso é reportado|
|Unidades Pagas|    Número de unidades disponíveis pagas|
|MensaisActiveUsers|    Número de utilizadores ativos mensais|
|CustomerName|  Nome do Cliente|
|Mercado de Clientes|    Localização do País Geográfico do Mercado do Cliente |
|Gestão de Clientes|   Segmento de Clientes |
|MPNId| ID da rede de parceiros da Microsoft|
|PartnerName|   Nome do Parceiro|
|PartnerLocation|   Localização geográfica do parceiro|
|PartnerAttributionType|    Tipo de parceiro de atribuição|

**Mobilidade Empresarial – Utilização de Licenças**: A definição de dados dos vários campos do EMS – Relatório de Utilização de Licenças são:

| **Nome da coluna** | **Descrição de Dados** |
|---------|:---------|
|CustomerTenantId|  ID do cliente do inquilino| 
|CustomerTpid|  ID do pai de topo do cliente |
|Nome da carga de trabalho|  Nome da carga de trabalho EMS |
|Mensal| Mês para o qual o uso é reportado|
|Unidades Pagas|    Número de unidades disponíveis pagas|
|MensaisActiveUsers|    Número de utilizadores ativos mensais|
|CustomerName|  Nome do Cliente|
|Mercado de Clientes|Localização do País Geográfico do Mercado do Cliente |
|Gestão de Clientes|   Segmento de Clientes |
|MPNId| ID da rede de parceiros da Microsoft|
|PartnerName|   Nome do Parceiro|
|PartnerLocation|   Localização geográfica do parceiro|
|PartnerAttributionType|    Tipo de parceiro de atribuição|

**Dinâmica 365 – Utilização da Licença**: A definição de dados dos vários campos da Dinâmica 365 – Relatório de Utilização de Licenças são:

| **Nome da coluna** | **Descrição de Dados** |
|---------|:---------|
|SubscriptionId|GUIA da Assinatura|
|SubscriçãoStartDate| Data de Início da Subscrição|
|SubscriçãoEndDate|   Data de Fim da Subscrição|
|Subscrição Estatísticas|    Estado da Assinatura |
|Mensal| Mês para o qual o uso é reportado|
|Nome revSumDivision|    Nome da divisão de soma rev|
|Nome revsumCategoria|    Nome da categoria de soma rev|
|SKU|   Sku do produto |
|SKUId| Sku ID do produto |
|FreeVsPaidSKU| Indica se é um SKU gratuito ou pago |
|SalesModel|    Canal de vendas utilizado para a venda da subscrição|
|Modelo de Vendas Detalhadas|    Modelo de vendas detalhado para a subscrição|
|CustomerName|  Nome do Cliente |
|CustomerTenantId|  Inquilino cliente GUID |
|CustomerTpid|  Identificador principal do cliente |
|Gestão de Clientes|   Segmento de mercado do Cliente |
|Mercado de Clientes|    Mercado Geográfico do Cliente |
|MPNId| ID da rede de parceiros da Microsoft |
|PartnerName|   Nome do Parceiro |
|PartnerLocation|   Localização geográfica do país do parceiro |
|PartnerAttachType| Tipo de atribuição para a subscrição|
|Lugares disponíveis|    Assento disponível atual|
|Caixas designadas| Assento atual atribuído |
|ActiveSeats|   Assentos ativos atuais |
|ImplantaçãoOpportunidade| Oportunidade de implantação atual|
|ActiveUsagePercent|    Percent de utilização ativa atual|
 
**Utilização da licença Power BI**: A definição de dados dos vários campos do Power BI – Relatório de Utilização de Licenças são:

| **Nome da coluna** | **Descrição de Dados** |
|---------|:---------|
|SubscriptionId|    GUIA da Assinatura|
|SubscriçãoStartDate| Data de Início da Subscrição|
|SubscriçãoEndDate|   Data de Fim da Subscrição|
|Subscrição Estatísticas|    Estado da Subscrição (Período Ativo ou In-Active ou In-Grace)|
|Mensal| Data agregada por mês |
|SKU|   Sku do Produto |
|SKUId| Sku ID do produto |
|FreeVsPaidSKU| Diferenciador Sku gratuito ou pago |
|SalesModel|    Modelo de vendas usado para vender a subscrição|
|Modelo de Vendas Detalhadas|    Modelo de vendas detalhado para a subscrição|
|CustomerName|  Nome do Cliente |
|CustomerTenantId|  Inquilino cliente GUID |
|CustomerTpid|  Identificador principal do cliente| 
|Gestão de Clientes|   Segmento de Mercado do Cliente |
|Mercado de Clientes|    Mercado Geográfico do Cliente |
|MPNId| ID da rede de parceiros da Microsoft |
|PartnerName|   Nome do Parceiro |
|PartnerLocation|   Localização geográfica do país do parceiro |
|PartnerAttachType| Tipo de atribuição para a subscrição|
|Lugares disponíveis|    Lugares disponíveis atuais|
|Caixas designadas| Assentos Atuais Atribuídos|
|ActiveSeats|   Assentos ativos atuais|
|ImplantaçãoOpportunidade| Oportunidade de implantação atual|
|ActiveUsagePercent|    Percent de utilização ativa atual|

**Utilização de Equipas – Reuniões e chamadas**: As definições de dados dos vários campos são:

| **Nome da coluna** | **Descrição de Dados** |
|---------|:---------|
|CustomerTenantId|  ID do cliente do inquilino |
|CustomerTpid|  ID do pai de topo do cliente |
|Mensal| Mês para o qual o uso é reportado|
|Subtrabalho|   Sub carga de trabalho para a qual é reportada a utilização (Reuniões, chamadas, sistemas telefónicos)|
|Contagem de reuniões| Número de reuniões|
|Duração da reunião|  Duração total da reunião em horas|

**Equipas - Detalhes mensais de utilização**: As definições de dados dos vários campos são:

| **Nome da coluna** | **Descrição de Dados** |
|---------|:---------|
|CustomerTenantId|  ID do cliente do inquilino |
|CustomerTpid|  ID do pai de topo do cliente |
|Mensal| Mês para o qual o uso é reportado|
|Subtrabalho|   Sub carga de trabalho para a qual é reportada a utilização (Reuniões, chamadas, sistemas telefónicos)|
|Utilizadores de desktop| Número de utilizadores que usam equipas no ambiente de trabalho|
|Utilizadores Móveis|  Número de utilizadores que usam equipas em mobile|
|Utilizadores da Web| Número de utilizadores que usam equipas na Web|
|AllUpParticipants| Número de utilizadores distintos de Equipas para o mês|

**Utilização de equipas – aplicativos 3P**: As definições de dados dos vários campos são:

| **Nome da coluna** | **Descrição de Dados** |
|---------|:---------|
|CustomerTenantId|  ID do cliente do inquilino| 
|CustomerTpid|  ID do pai de topo do cliente |
|Mensal| Mês para o qual o uso é reportado|
|Nome da aplicação 3P|   Nome da app Teams|
|Contagem de utilizadores|    Número de utilizadores para a app|


**Detalhes da Formação**: As definições de dados das várias áreas do relatório Detalhes da Formação são:

| **Nome da coluna** | **Descrição de Dados** |
|---------|:---------|
|TrainingActivityId|    Identificador da Formação |
|TrainingTitle| Título da Formação |
|Célula de Formação|  Tipo de Formação (Certificação/Exame)|
|Nome IndividualFirst|   Primeiro Nome do Cliente| 
|Nome IndividualLast|    Último Nome do Cliente| 
|E-mail| ID de e-mail pessoal do cliente|
|CorpEmail| ID de e-mail do escritório do cliente|
|Curso de FormaçãoDate|    Data de conclusão da formação |
|Mensal| Mês para o qual os dados são reportados|
|ICMCP| Indica se o utilizador é um Microsoft Certified Professional|
|MCPID| ID MCP do utilizador|
|MPNId| ID da rede de parceiros da Microsoft |
|PartnerName|   Nome do Parceiro |
|PartnerCityLocation|   Localização geográfica da cidade do parceiro |
|PartnerCountryLocation|    Localização geográfica do país do parceiro |

**Microsoft Learn**: As definições de dados dos vários campos do relatório Microsoft Learn são:

| **Nome da coluna** | **Descrição de Dados** |
|---------|:---------|
|Nome de Utilizador|Nome do utilizador| 
|IDUtilizador|User GUID |
|Nome de formação|Nome do treino |
|Célula de Formação|Tipo de formação (Módulo/Caminho de Aprendizagem)|
|Produtos|Produto para o qual o módulo de aprendizagem é aplicável|
|Funções|Funções aplicáveis da Formação |
|ConclusãoDate|Data de Conclusão da Formação |
|MPNId|ID da rede de parceiros da Microsoft |
|PartnerName|Nome do Parceiro |
|País|Localização geográfica do país do parceiro |

**Resumo e história da competência**: A definição de dados dos vários domínios do resumo da Competência e do relatório de história são:

| **Nome da coluna** | **Descrição de Dados** |
|---------|:---------|
|CompetênciaName|Nome da competência |
|CompetênciaLevel|Nível de competência (Ouro /Prata)|
|CompetênciaSStatus|Estado atual da competência (Período Ativo/Inativo/Em Período de Graça)|
|CompetênciaStartDate|Data de início da competência dada| 
|CompetênciaEndDate|Data de fim da competência dada |

**Desempenho da competência**: As definições de dados das várias áreas do relatório de desempenho da competência são:

| **Nome da coluna** | **Descrição de Dados** |
|---------|:---------|
|CompetênciaName|    Nome da competência |
|CompetênciaAttainmentOptionName|    Nome da opção de obtenção de competências|
|Mensal| Mês para o qual as métricas são reportadas|
|MetricName|    Nome da métrica relevante para a competência|
|MétricaMonthlyContribution| Contribuição mensal da métrica|
|TTMAggregate|  Métrica agregada para os 12 meses de fuga|
|AniversárioYearAggregate|  Métrica agregada para o ano de aniversário em curso|
|GoldThreshold| Requisito de desempenho para satisfazer a competência gold|
|SilverThreshold|   Requisito de desempenho para satisfazer a competência silver|

**A proposta cloud Ascent-M365**: As definições de dados dos vários campos do relatório de propensity Cloud Ascent-M365 são:

| **Nome da coluna** | **Descrição de Dados** |
|---------|:---------|
|ID do MPN|    ID da rede de parceiros da Microsoft|
|Nome do parceiro|  Nome do Parceiro|
|ID de Cliente|   Número de identificador de clientes |
|Número duns|   O Dun & número de Bradstreet do Cliente sendo marcado para propensão|
|Nome da Conta|  Nome da Conta |
|Domínio|    Domínio da conta|
|Tamanho org|  Tamanho da Organização|
|Setor|  Setor  |
|Vertical|  A vertical do Cliente a ser pontuada para propensão, identificada pela Microsoft e outros padrões da indústria (D&B)|
|Área|  Área Geográfica da Localização|
|Subsidiária|    A subsidiária do Cliente a ser pontuada por propensão|
|Território de Vendas|   O território de vendas do Cliente sendo pontuado para propensão|
|City|  Localização geográfica da cidade |
|Estado| Localização geográfica do estado|
|Código Postal|   Código Postal|
|País|   Localização do País Geográfico |
|Segment|   Segmento de mercado |
|Sub-Segmento|   Subsegmento de mercado |
|Resumo do tipo SMC|  Tipo SMC |
|Top Unmanaged - Base de Computação|  Principais clientes não geridos - computação|
|Top Unmanaged - Base de Utilizador| Principais clientes não geridos – utilizador|
|IsNonProfit|   Sem fins lucrativos ou com fins lucrativos (sim/não)|
|Ativar trabalho remoto - Troca de alvos online|   Clientes que têm uma subscrição on-line de intercâmbio ativa, Upsell para M365|
|Ativar trabalho remoto - Aquisição on-prem (Versão Atual) com Propensity CLAS - +10 Licenças|Cliente que tem Atual On-prem Office ou Win Client (isto é, versões que estão atrás de produtos EOS). O cliente tem 10 ou mais licenças. Cliente que tem uma pontuação de propensão. Os parceiros devem ter como alvo a conversão para M365.|
|Ativar trabalho remoto - Aquisição on-prem (Versão Atual) com Propensity CLAS - <10 Licenças|Cliente que tem Atual On-prem Office ou Win Client (isto é, versões que estão atrás de produtos EOS). O cliente tem menos de 10 licenças. Cliente que tem uma pontuação de propensão. Os parceiros devem ter como alvo a conversão para M365.|
|Ativar trabalho remoto - Aquisição on-prem (Versão Atual) sem Propensity CLAS - +10 Licenças| Cliente que tem Atual On-prem Office ou Win Client (isto é, versões que estão atrás de produtos EOS). O cliente tem 10 ou mais licenças. O cliente não tem uma pontuação de propensão. Os parceiros devem ter como alvo a conversão para M365.|
|Ativar trabalho remoto - Aquisição on-prem (Versão Atual) sem a propensity CLAS - <10 Licenças| Cliente que tem Atual On-prem Office ou Win Client (isto é, versões que estão atrás de produtos EOS). O cliente tem menos de 10 licenças. O cliente não tem uma pontuação de propensão. Os parceiros devem ter como alvo a conversão para M365.|
|Ativar trabalho remoto - Aquisição on-prem (EOS) com propensity CLAS - +10 Licenças|Cliente que tem EOS On-prem Office ou Win Client (isto é, versões que são anteriores e incluindo produtos EOS. O cliente tem 10 ou mais licenças. O cliente tem uma pontuação de propensão. Os parceiros devem ter como alvo a conversão para M365.|
|Ativar trabalho remoto - Aquisição on-prem (EOS) com propensity CLAS - <10 Licenças|Cliente que tem EOS On-prem Office ou Win Client (isto é, versões que são anteriores e incluindo produtos EOS. O cliente tem menos de 10 licenças. O cliente tem uma pontuação de propensão. Os parceiros devem ter como alvo a conversão para M365.|
|Ativar trabalho remoto - Aquisição on-prem (EOS) sem propensity CLAS - +10 Licenças| Cliente que tem Atual On-prem Office ou Win Client (isto é, versões que são anteriores e incluindo produtos EOS). O cliente tem 10 ou mais licenças. O cliente não tem uma pontuação de propensão. Os parceiros devem ter como alvo a conversão para M365.|
|Ativar trabalho remoto - Aquisição on-prem (EOS) sem a propensity CLAS - <10 Licenças| Cliente que tem Atual On-prem Office ou Win Client (isto é, versões que são anteriores e incluindo produtos EOS). O cliente tem menos de 10 licenças. O cliente não tem uma pontuação de propensão. Os parceiros devem ter como alvo a conversão para M365.|
|Ativar o trabalho remoto - Perspetiva de Alta Propensity para M365 (Act Now/Assess)| Prospect cliente com elevada propensity para M365.|
|Ativar trabalho remoto - Competir (Zoom) com M365| Clientes com Zoom e M365, alvo de conversão para equipas|
|Ativar trabalho remoto - Competir (Zoom) sem M365|  Clientes com Zoom, alvo de conversão para equipas|
|Reduzir Custo e Gestão - M365 E3 direcionado para M365 E5| Cliente existente com M365 E3, alvo de M365 E5|
|Reduzir custos e gerir - clientes M365 BB e BS direcionados para M365 BP|    Clientes M365 BB e BS existentes, direcionam-nos para M365 BP|
|Transformar produtividade organizacional - Propensão de superfície|    O cliente está a mostrar propensão para o Surface.|
|M365Cluster|Identifica a propensão do cliente para comprar m365.  Clusters Act Now e Assess devem ser direcionados, uma vez que produzirão um rendimento mais elevado.  Os clientes de educação e educação só devem ser direcionados se ainda houver capacidade após a direcionar os clientes Act Now e Avaliar.|
|M365Fit|   Pontos de dados internos e externos que definem firmográficos. Fit scoreing usa um modelo semelhante ao nosso melhor SMB para comparar clientes e ver se eles são um potencial apto para Produtos Microsoft Cloud. A pontuação de ajuste é atualizada trimestralmente.|
|M365Intente|    Sinais relacionados com as redes sociais e o comportamento online de um cliente definem a Intenção. A pontuação intencional é sobreposta em cima de apto para definir os clusters. A pontuação de intenção é atualizada mensalmente.|
|SurfaceCluster|    Isto identifica a propensão do cliente para comprar a Surface, consolidando as recomendações fit e intenta num cluster.  Clusters Act Now e Assess devem ser direcionados, uma vez que produzirão um rendimento mais elevado.  Os clientes de educação e educação só devem ser direcionados se ainda houver capacidade após a direcionar os clientes Act Now e Avaliar.|
|SurfaceFit|    Pontos de dados internos e externos que definem firmográficos. Fit scoreing usa um modelo semelhante ao nosso melhor SMB para comparar clientes e ver se eles são um potencial apto para Produtos Microsoft Cloud. A pontuação de ajuste é atualizada trimestralmente.|
|SuperfícieIntente| Sinais relacionados com as redes sociais e o comportamento online de um cliente definem a Intenção. A pontuação intencional é sobreposta em cima de apto para definir os clusters. A pontuação de intenção é atualizada mensalmente.|
|O365Cluster|   Isto identifica a propensão do cliente para comprar o O365.  Clusters Act Now e Assess devem ser direcionados, uma vez que produzirão um rendimento mais elevado.  Os clientes de educação e educação só devem ser direcionados se ainda houver capacidade após a direcionar os clientes Act Now e Avaliar.|
|O365Fit|   Pontos de dados internos e externos que definem firmográficos. Fit scoreing usa um modelo semelhante ao nosso melhor SMB para comparar clientes e ver se eles são um potencial apto para Produtos Microsoft Cloud. A pontuação de ajuste é atualizada trimestralmente.|
|O365Intente|    Sinais relacionados com as redes sociais e o comportamento online de um cliente definem a Intenção. A pontuação intencional é sobreposta em cima de apto para definir os clusters. A pontuação de intenção é atualizada mensalmente.|
|M365UpsellCustomer|    Isto identifica se o cliente está mostrando a propensão de venda para M365|
|Tem Google|    Esta bandeira identifica se um cliente está a mostrar sinais competitivos para possuir produtos da Google|
|Tem aws|   Esta bandeira identifica se um cliente está mostrando sinais competitivos para possuir produtos AWS|
|Tem EA|    Isto identifica se uma renovação é um acordo de empresa (EA) ou uma subscrição da EA|
|Tem Aberto|  Isto identifica se uma renovação é um Acordo de Valor Aberto ou Aberto|

**A propensity Cloud Ascent-D365**: As definições de dados dos vários campos do relatório de propensity Cloud Ascent-D365 são:

| **Nome da coluna** | **Descrição de Dados** |
|---------|:---------|
|ID do MPN|    ID da rede de parceiros da Microsoft|
|Nome do parceiro|  Nome do Parceiro|
|ID de Cliente|   Número de identificador de clientes |
|Número duns|   O Dun & número de Bradstreet do Cliente sendo marcado para propensão|
|Nome da Conta|  Nome da Conta |
|Domínio|    Domínio da conta|
|Tamanho org|  Tamanho da Organização|
|Setor|  Setor  |
|Vertical|  A vertical do Cliente a ser pontuada para propensão, identificada pela Microsoft e outros padrões da indústria (D&B)
|Área|  Área Geográfica da Localização|
|Subsidiária|    A subsidiária do Cliente a ser pontuada por propensão|
|Território de Vendas|   Território de Vendas|
|City|  Localização geográfica da cidade |
|Estado| Localização geográfica do estado|
|Código Postal|   Código Postal|
|País|   Localização do País Geográfico |
|Segment|   Segmento de mercado |
|Sub-Segmento|   Subsegmento de mercado |
|Resumo do tipo SMC|  A categorização de um cliente: Top Ungeraged User Bases são clientes com mais de 300 colaboradores, Top Unmanaged Compute Base são Clientes com $10k em Azure 3 anos potencial, média negócio são Clientes com 25 ou maiores, Pequenas empresas são clientes com menos de 25 colaboradores|
|Top Unmanaged - Base de Computação   |Principais clientes não geridos - computação|
|Top Unmanaged - Base de Utilizador| Principais clientes não geridos – utilizadores|
|IsNonProfit|   Sem fins lucrativos ou com fins lucrativos (sim/não)|
|Ativar a venda digital - M365 - Tamanho do assento >= 25 lugares (Modelo de Propensity SalesPro)|   Cliente sem D365. Tamanho do assento: 25+. Parceiros devem visar cross-sell da D365 Salespro|
|Ativar a venda digital - D365 SalesPro Propensity (Act Now/Assess) |Clientes de Alta Propensity sem D365.  Os parceiros devem ter como alvo a D365 SalesPro.|
|Gestão de risco financeiro & fraude - Base de instalação dinâmica on-prem - Navision (modelo de propensity BC)|Cliente existente com OnPrem Navision.  Parceiro Deve ser alvo de D365 a.C.|
|Gestão de risco financeiro & fraude - Base de instalação dinâmica on-prem - AX (F&O Propensity Model)    |Cliente existente com OnPrem AX.  Parceiro Deve ser alvo de D365 F&O|
|Gestão de risco financeiro & fraude - Base de instalação dinâmica on-prem - Grandes Planícies (Modelo de Propensity BC)|  Cliente existente com OnPrem Great Plains.  Parceiro Deve ser alvo de D365 a.C.|
|Gestão de Risco Financeiro & Fraude - Base de Instalação Dinâmica On-prem - Salomão (Modelo de Propensity BC)|Cliente existente com OnPrem Solomon.  Parceiro Deve ser alvo de D365 a.C.|
|Gestão de Risco Financeiro & Fraude - Base de Instalação Dinâmica On-prem - Outros (Modelo de Propensity BC) |Cliente existente com outras soluções OnPrem não listadas acima.  Parceiro Deve ser alvo de D365 a.C.|
|Construir Processos Empresariais Ágeis - Base de Instalação Dinâmica On-prem - AX/GP/SL/NAV/Outros (Modelo de Propensity D365)|   Construir Processos Empresariais Ágeis - Base de Instalação Dinâmica On-prem - AX/GP/SL/NAV/Outros (Modelo de Propensity D365)|
|Construir Processos Empresariais Áile - Base de Competição Dinâmica - Mendix/Outsystems/Salesforce (Modelo de Propensity D365)| Construir Processos Empresariais Áile - Base de Competição Dinâmica - Mendix/Outsystems/Salesforce (Modelo de Propensity D365)|
|Construir Processos Empresariais Ágeis - D365 F&Base de Instalação O |Clientes D365 F&O existentes.  Parceiro para direcionar as Aplicações de Energia.|
|Construir Processos empresariais Ágeis - D365 BC Base de instalação| Clientes D365 a.C. existentes. Parceiro para direcionar as Aplicações de Energia.|
|Construir Processos Empresariais Ágeis - Base de Instalação CE D365| Clientes D365 CE existentes. Parceiro para direcionar as Aplicações de Energia.|
|Construir uma cadeia de fornecimento resiliente - Ganhe e Ative a primeira carga de trabalho D365 como cadeia de fornecimento D365 com clientes ERP não-Oráculo/SAP|  Clientes-alvo da Cadeia de Abastecimento D365.|
|Construir uma cadeia de fornecimento resiliente - Cross-Sell D365 Cadeia de Fornecimento E/OR Retalho/Comércio a Clientes D365 CE existentes |Clientes D365 CE existentes para venda cruzada cadeia de fornecimento D365|
|Construa uma cadeia de fornecimento resiliente - Cross-Sell D365 Sup. Cadeia E/OR Retalho/Comércio a D365 CE E (Oráculo ou SAP)| Clientes D365 CE existentes com Oracle ou SAP para a cadeia de abastecimento D365|
|D365BCCluster| Isto identifica a propensão do cliente para a compra da D365 Business Central.  Os clientes que apresentem propensão para BC estarão nas categorias Média e Pequena.  Clusters Act Now e Assess devem ser direcionados, uma vez que produzirão um rendimento mais elevado.  Os clientes de educação e educação só devem ser direcionados se ainda houver capacidade após a direcionar os clientes Act Now e Avaliar.|
|D365BCFit| Pontos de dados internos e externos que definem firmográficos. Fit scoreing usa um modelo semelhante ao nosso melhor SMB para comparar clientes e ver se eles são um potencial apto para Produtos Microsoft Cloud. A pontuação de ajuste é atualizada trimestralmente.|
|D365BCIntente|  Sinais relacionados com as redes sociais e o comportamento online de um cliente definem a Intenção. A pontuação intencional é sobreposta em cima de apto para definir os clusters. A pontuação de intenção é atualizada mensalmente.|
|D365FOCluster| Isto identifica a propensão do cliente para a compra de Finanças e Operações D365.  Os clientes que mostrem propensão para F&O estarão nas categorias de topo não geridos. Clusters Act Now e Assess devem ser direcionados, uma vez que produzirão um rendimento mais elevado.  Os clientes de educação e educação só devem ser direcionados se ainda houver capacidade após a direcionar os clientes Act Now e Avaliar.|
|D365FOFit| Pontos de dados internos e externos que definem firmográficos. Fit scoreing usa um modelo semelhante ao nosso melhor SMB para comparar clientes e ver se eles são um potencial apto para Produtos Microsoft Cloud. A pontuação de ajuste é atualizada trimestralmente.|
|D365FOIntente|  Sinais relacionados com as redes sociais e o comportamento online de um cliente definem a Intenção. A pontuação intencional é sobreposta em cima de apto para definir os clusters. A pontuação de intenção é atualizada mensalmente.|
|D365CECluster| Isto identifica a propensão do cliente para comprar o Envolvimento do Cliente D365.  Os clientes que apresentem propensão para CE estarão nas categorias Média e Pequena.  Clusters Act Now e Assess devem ser direcionados, uma vez que produzirão um rendimento mais elevado.  Os clientes de educação e educação só devem ser direcionados se ainda houver capacidade após a direcionar os clientes Act Now e Avaliar.|
|D365CEFit| Apto para D365 CE|
|D365CEIntente|  Intenção para D365 CE|
|DynamicsOnPremAXorCRM_HasOpenRenewal|  Isto identifica se um cliente tem uma renovação aberta para Dynamics On-prem AX ou CRM.|
|M365UpsellCustomer|    Isto identifica se o cliente está mostrando a propensão de venda para M365|
|Tem Google|    Esta bandeira identifica se um cliente está a mostrar sinais competitivos para possuir produtos da Google|
|Tem aws|   Esta bandeira identifica se um cliente está mostrando sinais competitivos para possuir produtos AWS|
|Tem EA |Isto identifica se uma renovação é um acordo de empresa (EA) ou uma subscrição da EA|
|Tem Aberto|  Isto identifica se uma renovação é um Acordo de Valor Aberto ou Aberto|

**Cloud Ascent-Azure Propensity**: As definições de dados dos vários campos do relatório de propensity cloud Ascent-Azure são:

|**Nome da coluna** |**Descrição de Dados** |
|---------|:---------|
|ID do MPN|    ID da rede de parceiros da Microsoft|
|Nome do parceiro|  Nome do Parceiro|
|ID de Cliente|   Número de identificador de clientes |
|Número duns|   O Dun & número de Bradstreet do Cliente sendo marcado para propensão|
|Nome da Conta|  Nome da Conta |
|Domínio|    Domínio da conta|
|Tamanho org|  Tamanho da Organização|
|Setor|  Setor  |
|Vertical|  A vertical do Cliente a ser pontuada para propensão, identificada pela Microsoft e outros padrões da indústria (D&B)|
|Área|  Área Geográfica da Localização|
|Subsidiária|    A subsidiária do Cliente a ser pontuada por propensão|
|Território de Vendas|   Território de Vendas|
|City|  Localização geográfica da cidade |
|Estado| Localização geográfica do estado|
|Código Postal|   Código Postal|
|País|   Localização do País Geográfico |
|Segment|   Segmento de mercado |
|Sub-Segmento|   Subsegmento de mercado |
|Resumo do tipo SMC|  Tipo SMC |
|Top Unmanaged - Base de Computação|  Principais clientes não geridos - computação|
|Top Unmanaged - Base de Utilizador| Principais clientes não geridos – utilizadores|
|IsNonProfit|   Sem fins lucrativos ou com fins lucrativos (sim/não)|
|Migrar - EOS Win Server - EOS Windows Server IB com a propensity CLAS - 5+ Licenças|   Cliente que tem EOS On-prem Win Server (isto é, versões que são anteriores e incluindo produtos EOS). O cliente tem 5 ou mais licenças. Cliente que tem uma pontuação de propensão.  Os parceiros devem direcionar estes clientes para a migração para Azure.|
|Migrar - EOS Win Server - EOS Windows Server IB com a propensity CLAS - <5 Licenças|   Cliente que tem EOS (End of Service) On-prem Win Server (isto é, versões que são anteriores e incluindo produtos EOS). O Cliente tem menos de 5 licenças. Cliente que tem uma pontuação de propensão.  Os parceiros devem direcionar estes clientes para a migração para Azure.|
|Migrar - EOS Win Server - EOS Windows Server IB sem a propensity CLAS - 5+ Licenças |Cliente que tem EOS On-prem Win Server (isto é, versões que são anteriores e incluindo produtos EOS). O cliente tem mais de 5 licenças. O cliente não tem uma pontuação de propensão. Os parceiros devem direcionar estes clientes para a migração para Azure.|
|Migrar - EOS Win Server - EOS Windows Server IB sem a propensity CLAS - <5 Licenças|    Cliente que tem EOS On-prem Win Server (isto é, versões que são anteriores e incluindo produtos EOS). Tem menos de 5 licenças. O cliente não tem uma pontuação de propensão. Os parceiros devem direcionar estes clientes para a migração para Azure.|
|Migrar - EOS SQL - EOS SQL Server IB com Clas Propensity - 5+ Licenças|  Cliente que tem EOS On-prem SQL Server (isto é, versões que são anteriores e incluindo produtos EOS). O cliente tem mais de 5 licenças. O cliente tem uma pontuação de propensão.  Os parceiros devem direcionar estes clientes para a migração para Azure.|
|Migrar - EOS SQL - EOS SQL Server IB com a propensity CLAS - <5 Licenças|  Cliente que tem EOS On-prem SQL Server (isto é, versões que são anteriores e incluindo produtos EOS). Tem menos de 5 licenças. Cliente que tem uma pontuação de propensão. Os parceiros devem direcionar estes clientes para a migração para Azure.|
|Migrar - EOS SQL - EOS SQL Server IB sem a propensity CLAS - 5+ Licenças|   Cliente que tem EOS On-prem SQL Server (isto é, versões que são anteriores e incluindo produtos EOS). O cliente tem 5 ou mais licenças. O cliente não tem uma pontuação de propensão. Os parceiros devem direcionar estes clientes para a migração para Azure.|
|Migrar - EOS SQL - EOS SQL Server IB sem a propensity CLAS - <5 Licenças|   Cliente que tem EOS On-prem SQL Server (isto é, versões que são anteriores e incluindo produtos EOS). O cliente tem menos de 5 licenças. O cliente não tem uma pontuação de propensão. Os parceiros devem direcionar estes clientes para a migração para Azure.|
|Migrar - Migrar on-prem Win Server - Atual Servidor windows IB com propensity CLAS - 5+ Licenças|   Cliente que tem Corrente On-prem Win Server (isto é, versões que estão atrás de produtos EOS). O cliente tem mais de 5 licenças. O cliente tem uma pontuação de propensão. Os parceiros devem direcionar estes clientes para a migração para Azure.|
|Migrar - Migrar no pré-prem Win Server - Atual Servidor do Windows IB com propensity CLAS - <5 Licenças|   Cliente que tem Corrente On-prem Win Server (isto é, versões que estão atrás de produtos EOS). O cliente tem menos de 5 licenças. O cliente tem uma pontuação de propensão para o Azure. Os parceiros devem direcionar estes clientes para a migração para Azure.|
|Migrar - Migrar on-prem Win Server - Atual Servidor do Windows IB sem a propensity CLAS - 5+ Licenças|    Cliente que tem Corrente On-prem Win Server (isto é, versões que estão atrás de produtos EOS). O cliente tem mais de 5 licenças. O cliente não tem uma pontuação de propensão. Os parceiros devem direcionar estes clientes para a migração para Azure.|
|Migrar - Migrar on-prem Win Server - Atual Servidor do Windows IB sem a propensity CLAS - <5 Licenças |Cliente que tem Corrente On-prem Win Server (isto é, versões que estão atrás de produtos EOS). O cliente tem menos de 5 licenças. O cliente não tem uma pontuação de propensão. Os parceiros devem direcionar estes clientes para a migração para Azure.|
|Migrar - Migrar para Azure SQL ou SQL VMs - Atual SQL Server IB com propensity CLAS - 5+ Licenças|  Cliente que tem Corrente On-prem SQL Server (isto é, versões que estão atrás de produtos EOS). O cliente tem mais de 5 licenças. O cliente tem uma pontuação de propensão. Os parceiros devem direcionar estes clientes para a migração para Azure.|
|Migrar - Migrar para Azure SQL ou SQL VMs - Atual SQL Server IB com propensity CLAS - <5 Licenças|  Cliente que tem Corrente On-prem SQL Server (isto é, versões que estão atrás de produtos EOS). O cliente tem menos de 5 licenças. O cliente tem uma pontuação de propensão. Os parceiros devem direcionar estes clientes para a migração para Azure.|
|Migrar - Migrar para Azure SQL ou SQL VMs - Atual SQL Server IB sem a propensity CLAS - 5+ Licenças|   Cliente que tem Corrente On-prem SQL Server (isto é, versões que estão atrás de produtos EOS). O cliente tem mais de 5 licenças. O cliente não tem uma pontuação de propensão. Os parceiros devem direcionar estes clientes para a migração para Azure.|
|Migrar - Migrar para Azure SQL ou SQL VMs - Atual SQL Server IB sem a propensity CLAS - <5 Licenças|   Cliente que tem Corrente On-prem SQL Server (isto é, versões que estão atrás de produtos EOS). O cliente tem menos de 5 licenças. O cliente não tem uma pontuação de propensão. Os parceiros devem direcionar estes clientes para a migração para Azure.|
|Migrar - OSS - Migrar para a OSS DB| Cliente existente com qualquer um dos seguintes produtos de competição: PostgreSQL, MySQL, MariaDB. Os parceiros devem direcionar estes clientes para a migração para Azure.|
|Migrar - OSS - Linux em Azure |Cliente existente com o produto: Linux. Os parceiros devem direcionar estes clientes para a migração para Azure.|
|Migrar - SAP - SAP em Azure|  Cliente existente com o produto: SAP. Os parceiros devem direcionar estes clientes para a migração para Azure.|
|Migrar - WVD - RDS IB |Identifica clientes com serviços de desktop remotos do Windows ativos. Os parceiros devem direcionar estes clientes para a migração para Azure.|
|Migrar - WVD - Cross Sell Modern Work to Azure/WVD|   Identifica clientes com M365 e não tem Azure. Os parceiros devem direcionar estes clientes para a migração para Azure.|
|Migrar - VMware IB|   Cliente existente com o produto: VMware. Os parceiros devem direcionar estes clientes para a migração para Azure.|
|Migração - Citrix IB|   Cliente existente com o produto: Citrix Systems. Os parceiros devem direcionar estes clientes para a migração para Azure.|
|Inovar - Analytics - Power BI IB c/ alta propensão Azure|   Clientes com subscrição e Ative Power BI incluindo: Power BI - Standalone Pro, Power BI - Azure Suites, Power BI - Office Suites, Power BI Suites - M365|
|Ativar - DevOps com GitHub - VisualStudio/MSDN IB|    Clientes identificados com estúdios visuais ativos|
|Win Server Standard Version|   Isto mostra a versão das Compras Standard do Windows Server pelo cliente|
|Ganhe licença padrão do servidor|   Isto mostra o tipo de licença de Compras Standard do Windows Server pelo cliente|
|Win Server Data Center Versão|    Isto mostra a versão das Compras do Windows Data Center pelo cliente|
|Ganhe licença do Centro de Dados do Servidor| Isto mostra o tipo de licença de Compras do Windows Data Center pelo cliente|
|AzureFit|  Pontos de dados internos e externos que definem firmográficos. Fit scoreing usa um modelo semelhante ao nosso melhor SMB para comparar clientes e ver se eles são um potencial apto para Produtos Microsoft Cloud. A pontuação de ajuste é atualizada trimestralmente.|
|AzureIntente|   Sinais relacionados com as redes sociais e o comportamento online de um cliente definem a Intenção. A pontuação intencional é sobreposta em cima de apto para definir os clusters. A pontuação de intenção é atualizada mensalmente.|
|AzureCluster|  Isto identifica a propensão do cliente para comprar a Azure, consolidando as recomendações fit e intenta em um cluster.  Clusters Act Now e Assess devem ser direcionados, uma vez que produzirão um rendimento mais elevado.  Os clientes de educação e educação só devem ser direcionados se ainda houver capacidade após a direcionar os clientes Act Now e Avaliar.|
|WindowsServerDataCenter_HasOpenRenewal|    Isto identifica se um cliente tem uma renovação aberta para um centro de dados do servidor windows|
|WindowsServerStandard_HasOpenRenewal|  Isto identifica se um cliente tem uma renovação aberta para um padrão de servidor de janelas|
|AzureUpsellCustomer|   Isto identifica se o cliente está mostrando a propensão de venda para Azure|
|Tem Google|    Esta bandeira identifica se um cliente está a mostrar sinais competitivos para possuir produtos da Google|
|Tem aws|   Esta bandeira identifica se um cliente está mostrando sinais competitivos para possuir produtos AWS|
|Tem EA |Isto identifica se uma renovação é um acordo de empresa (EA) ou uma subscrição da EA|
|Tem Aberto|  Isto identifica se uma renovação é um Acordo de Valor Aberto ou Aberto|

**Cloud Ascent-Agreement Renovações Propensity**: As definições de dados dos vários campos do relatório de renovação do acordo de subida da nuvem são:

|**Nome da coluna** |**Descrição de Dados** |
|---------|:---------|
|ID do MPN|    ID da rede de parceiros da Microsoft|
|Nome do parceiro|  Nome do Parceiro|
|ID de Cliente|   Número de identificador de clientes |
|Número duns|   O Dun & número de Bradstreet do Cliente sendo marcado para propensão|
|Nome da Conta|  Nome da Conta |
|Domínio|    Domínio da conta|
|Tamanho org|  Tamanho da Organização|
|Setor|  Setor  |
|Vertical|  A vertical do Cliente a ser pontuada para propensão, identificada pela Microsoft e outros padrões da indústria (D&B)|
|Área|  Área Geográfica da Localização|
|Subsidiária|    A subsidiária do Cliente a ser pontuada por propensão|
|Território de Vendas|   Território de Vendas|
|City|  Localização geográfica da cidade |
|Estado| Localização geográfica do estado|
|Código Postal|   Código Postal|
|País|   Localização do País Geográfico |
|Segment|   Segmento de mercado |
|Sub-Segmento|   Subsegmento de mercado |
|Resumo do tipo SMC|  Tipo SMC |
|Top Unmanaged - Base de Computação|  Principais clientes não geridos - computação|
|Top Unmanaged - Base de Utilizador| Principais clientes não geridos – utilizadores|
|IsNonProfit|Sem fins lucrativos ou com fins lucrativos (sim/não)|
|Tem Google|Esta bandeira identifica se um cliente está mostrando sinais competitivos para possuir produtos AWS|
|Tem aws|Esta bandeira identifica se um cliente está mostrando sinais competitivos para possuir produtos AWS|
|Aglomerado de Azure|Isto identifica a propensão do cliente para comprar a Azure.  Clusters Act Now e Assess devem ser direcionados, uma vez que produzirão um rendimento mais elevado.  Os clientes de educação e educação só devem ser direcionados se ainda houver capacidade após a direcionar os clientes Act Now e Avaliar.|
|D365 F&O Cluster|  Isto identifica a propensão do cliente para a compra de Finanças e Operações D365.  Os clientes que mostrem propensão para F&O estarão nas categorias de topo não geridos.  Clusters Act Now e Assess devem ser direcionados, uma vez que produzirão um rendimento mais elevado.  Os clientes de educação e educação só devem ser direcionados se ainda houver capacidade após a direcionar os clientes Act Now e Avaliar.|
|D365 CE Cluster|   Isto identifica a propensão do cliente para comprar o Envolvimento do Cliente D365.  Os clientes que apresentem propensão para CE estarão nas categorias Média e Pequena.  Clusters Act Now e Assess devem ser direcionados, uma vez que produzirão um rendimento mais elevado.  Os clientes de educação e educação só devem ser direcionados se ainda houver capacidade após a direcionar os clientes Act Now e Avaliar.|
|Aglomerado D365 a.C.|   Isto identifica a propensão do cliente para a compra da D365 Business Central.  Os clientes que apresentem propensão para BC estarão nas categorias Média e Pequena.  Clusters Act Now e Assess devem ser direcionados, uma vez que produzirão um rendimento mais elevado.  Os clientes de educação e educação só devem ser direcionados se ainda houver capacidade após a direcionar os clientes Act Now e Avaliar.|
|M365 Cluster|  Isto identifica a propensão do cliente para comprar m365.  Clusters Act Now e Assess devem ser direcionados, uma vez que produzirão um rendimento mais elevado.  Os clientes de educação e educação só devem ser direcionados se ainda houver capacidade após a direcionar os clientes Act Now e Avaliar.|
|Programa de Licenças|   Isto identifica o tipo de programa de licença para a renovação|
|ID do acordo|  Identificador de Acordo|
|Data de Fim do Acordo|    Data de Fim do Acordo |
|Tipo de expiração|   Tipo de expiração|
|Receitas Caducidade|  Receitas associadas a assinaturas caducadas|
|Tem EA|    Isto identifica se uma renovação é um acordo de empresa (EA) ou uma subscrição da EA|
|Tem Aberto|  Isto identifica se uma renovação é um Acordo de Valor Aberto ou Aberto|
|Cliente Azure Upsell| Isto identifica se o cliente está mostrando a propensão de venda para Azure|
|Cliente M365 Upsell|  Isto identifica se o cliente está mostrando a propensão de venda para M365|
|Nome revSumDivision|    Isto identifica o produto que está à altura da renovação|

## <a name="next-steps"></a>Passos seguintes

Para obter relatórios, consulte [os relatórios do Download](pci-download-reports.md).
