---
title: Definições de dados do Insights
ms.topic: article
ms.date: 12/14/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: O documento lista vários relatórios e as suas definições de dados, que pode descarregar a partir da página do relatório Insights Download.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 23ca20fbb2febfd4b1ea92f72fbfda5ac83d7eb6
ms.sourcegitcommit: 4118de5cf55d1bd618ecca13c1b2ec59d80f43db
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/24/2021
ms.locfileid: "112565513"
---
# <a name="export--data-definitions"></a>Exportação - Definições de dados 

**Funções apropriadas**: Report viewer | Espectador de relatório executivo

## <a name="introduction"></a>Introdução 

Ao utilizar o hub de Relatórios de Descarregamento no dashboard Insights, pode exportar os conjuntos de dados brutos. 

Os vários relatórios, que pode descarregar juntamente com as suas definições de dados, estão listados nas seguintes tabelas: 

### <a name="partner-profile-report"></a>**Relatório de perfil do parceiro**

| Nome da coluna | Descrição dos dados | 
| :--------- | :--------- | 
| MPNId | Microsoft Partner Network (MPN) ID| 
| PartnerName | Nome do parceiro | 
| PGA_MPNId | Identificador da conta global do parceiro MPN | 
| PGA_PartnerName | Nome da conta global do parceiro | 
| City | Localização da cidade do parceiro | 
| País | Localização do país do parceiro | 
| HierarquiaLevel | Indica se é um ID MPN global ou localização MPN ID | 

### <a name="customer-details-report"></a>**Relatório de detalhes do cliente**

| Nome da coluna | Descrição dos dados | 
| :--------- | :--------- | 
| CustomerName | Nome do cliente | 
| CustomerTenantId | Identificador do inquilino do cliente | 
| CustomerTpid | Identificador do principal cliente do progenitor | 
| Gestão de Clientes | Segmento de cliente | 
| Mercado de Clientes | Mercado geográfico do cliente | 
| CustomerStatus | Estado do cliente (Ativo ou Inativo) | 
| Produto | O produto vendido ao cliente pela MPN: Office 365, Dynamics 365, Enterprise Mobility and Security, Power BI ou Microsoft Azure | 
| SKU | SKU de produto | 
| Mensal | Mês para o qual são reportadas as receitas e o uso | 
| MPNId | Identificador da Microsoft Partner Network | 
| PartnerName | Nome do parceiro | 
| PartnerLocation | Localização geográfica do parceiro | 
| PartnerAttributionType | Tipo de atribuição do parceiro | 
| SalesChannel | Canal de vendas | 
| Lugares disponíveis | Lugares disponíveis | 
| RevenueUSD | Receitas em dólares americanos | 

### <a name="reseller-performance-report"></a>**Relatório de desempenho do revendedor**

> [!Note]
> Receitas e dados de receitas consumidas (ACR) estão disponíveis apenas para utilizadores que são espectadores de relatório executivo.

| Nome da coluna | Descrição dos dados | 
| :--------- | :--------- | 
| RevendedorMPNid | Reconvendar o identificador da Rede de Parceiros da Microsoft | 
| ResellerName | Nome do revendedor | 
| RevendedorMarket | País de mercado revendedor | 
| IndiretoProviderMPNId | Identificador do fornecedor indireto Microsoft Partner Network | 
| Nome IndiretoProvider | Nome do fornecedor indireto | 
| Mensal | Mês para o qual é reportada a utilização e receitas | 
| Produto | Nome do produto | 
| SubscriçãoID | Identificador da assinatura | 
| Lugares disponíveis | Número de lugares disponíveis | 
| Caixas designadas | Número de lugares atribuídos | 
| BilledRevenueusd | Receitas faturadas em dólares americanos | 
| CustomerName | Nome do cliente | 
| CustomerTPid | Identificador do principal cliente do progenitor | 
| Gestão de Clientes | Segmento de cliente | 
| Mercado de Clientes | Mercado geográfico do cliente | 
| RevendedorStatus | Estado do revendedor | 

### <a name="subscription-details-report"></a>**Relatório de detalhes da subscrição**

>[!Note]
>As receitas e os dados ACR estão disponíveis apenas para utilizadores que sejam espectadores de relatórios executivos.

| Nome da coluna | Descrição dos dados | 
| :--------- | :--------- | 
| SubscriptionId | GUID da subscrição | 
| SubscriçãoStartDate | Data de início da subscrição | 
| SubscriçãoEndDate | Data de fim da subscrição | 
| Estado de Subscrição | Estado da subscrição (Ativo ou Churned) | 
| Mensal | Mês para o qual são reportadas as receitas e o uso | 
| IsautoRenew | Indica se a subscrição é auto-automática (Sim ou Não) | 
| CustomerName | Nome do cliente | 
| CustomerTenantId | GUIA do cliente | 
| CustomerTpid | Identificador de pais de topo do cliente | 
| Gestão de Clientes | Segmento de mercado do cliente | 
| Mercado de Clientes | Mercado geográfico do cliente | 
| Produto | Produto vendido ao cliente pelo parceiro | 
| SKU | SKU do produto | 
| MPNId | ID da Rede de Parceiros microsoft do parceiro | 
| PartnerName | Nome do parceiro | 
| PartnerLocation | Localização geográfica do parceiro | 
| PartnerAttributionType | Tipo de atribuição para a subscrição | 
| SalesChannel | Canal das vendas - Direct, Cloud Solution Provider (CSP), e assim por diante | 
| Lugares disponíveis | Assento disponível atual | 
| RevenueUSD | Receitas em dólares americanos | 
| ID de inscrição | ID de inscrição da assinatura | 

### <a name="azure-usage-report"></a>**Relatório de utilização do Azure**

| Nome da coluna | Descrição dos dados | 
| :--------- | :--------- | 
| SubscriptionId | GUID da subscrição | 
| SubscriçãoStartDate | A data do início da subscrição | 
| SubscriçãoEndDate | A data do fim da subscrição | 
| Estado de Subscrição | Estado atual da subscrição (Aberto, Fechado, Ativo ou Em Período de Graça) | 
| Mensal | Data agregada por mês | 
| ServiceName | Nome do serviço Azure | 
| MeterCategory | Nome da categoria de contador | 
| Unidades de utilização | O número de unidades que são utilizadas durante o ciclo de faturação | 
| CustomerName | Nome do cliente | 
| CustomerTenantId | ID do inquilino do cliente | 
| CustomerTpid | ID do pai de topo do cliente | 
| Gestão de Clientes | Segmento do cliente | 
| Mercado de Clientes | Mercado geográfico do cliente | 
| MPNId | ID da Rede de Parceiros microsoft do cliente | 
| PartnerName | Nome do parceiro | 
| PartnerLocation | Localização geográfica do país do parceiro | 
| PartnerAttributionType | Tipo de atribuição do parceiro | 
| SalesChannel | Canal das vendas (Direto/CSP, Indirect/CSP, Direto, e assim por diante) | 
| ACR_USD | Azure consumiu receitas (ACR) em dólares dos EUA | 
| ID de inscrição | ID de inscrição da assinatura Azure | 

### <a name="office-365-license-usage-report"></a>**Relatório de utilização da licença do Office 365**

| Nome da coluna | Descrição dos dados | 
| :--------- | :--------- | 
| CustomerTenantId | ID do inquilino do cliente | 
| CustomerTpid | ID do pai de topo do cliente | 
| Nome da carga de trabalho | Skype para Negócios, Equipas, Troca Online | 
| Mensal | Mês para o qual o uso é reportado | 
| Unidades Pagas | Número de unidades disponíveis pagas | 
| MensaisActiveUsers | Número de utilizadores ativos mensais | 
| CustomerName | Nome do cliente | 
| Mercado de Clientes | Localização geográfica do mercado do cliente | 
| Gestão de Clientes | Segmento de cliente | 
| MPNId | Identificador da Microsoft Partner Network | 
| PartnerName | Nome do parceiro | 
| PartnerLocation | Localização geográfica do parceiro | 
| PartnerAttributionType | Tipo de atribuição do parceiro | 

### <a name="enterprise-mobility-license-usage-report"></a>**Relatório de utilização da licença de mobilidade empresarial**

| Nome da coluna | Descrição dos dados | 
| :--------- | :--------- | 
| CustomerTenantId | ID do inquilino do cliente | 
| CustomerTpid | ID do pai de topo do cliente | 
| Nome da carga de trabalho | Nome da carga de trabalho da Mobilidade Empresarial + Segurança (EMS) | 
| Mensal | Mês para o qual o uso é reportado | 
| Unidades Pagas | Número de unidades disponíveis pagas | 
| MensaisActiveUsers | Número de utilizadores ativos mensais | 
| CustomerName | Nome do cliente | 
| Mercado de Clientes | Localização geográfica do mercado do cliente | 
| Gestão de Clientes | Segmento de cliente | 
| MPNId | Identificador da Microsoft Partner Network | 
| PartnerName | Nome do parceiro | 
| PartnerLocation | Localização geográfica do parceiro | 
| PartnerAttributionType | Tipo de atribuição do parceiro | 

### <a name="dynamics-365-license-usage-report"></a>**Relatório de utilização da licença Dynamics 365**

| Nome da coluna | Descrição dos dados | 
| :--------- | :--------- | 
| SubscriptionId | GUID da subscrição | 
| SubscriçãoStartDate | Data de início da subscrição | 
| SubscriçãoEndDate | Data de fim da subscrição | 
| Subscrição Estatísticas | Estado da assinatura | 
| Mensal | Mês para o qual o uso é reportado | 
| Nome revSumDivision | Nome da divisão de soma rev | 
| Nome revsumCategoria | Nome da categoria de soma rev | 
| SKU | SKU do produto | 
| SKUId | SKU ID do produto | 
| FreeVsPaidSKU | Indica se é um SKU gratuito ou pago | 
| SalesModel | Canal de vendas que é usado para vender a subscrição | 
| Modelo de Vendas Detalhadas | Modelo de vendas detalhado para a subscrição | 
| CustomerName | Nome do cliente | 
| CustomerTenantId | GUIA do inquilino do cliente | 
| CustomerTpid | Identificador de pais de topo do cliente | 
| Gestão de Clientes | Segmento de mercado do cliente | 
| Mercado de Clientes | Mercado geográfico do cliente | 
| MPNId | Identificador da Microsoft Partner Network | 
| PartnerName | Nome do parceiro | 
| PartnerLocation | Localização geográfica do país do parceiro | 
| PartnerAttachType | Tipo de atribuição para a subscrição | 
| Lugares disponíveis | Assento disponível atual | 
| Caixas designadas | Assento designado atual | 
| ActiveSeats | Assentos ativos atuais | 
| ImplantaçãoOpportunidade | Oportunidade de implementação atual | 
| ActiveUsagePercent | Percentagem de utilização ativa atual | 

### <a name="power-bi-license-usage-report"></a>**Relatório de utilização da licença power BI**

| Nome da coluna | Descrição dos dados | 
| :--------- | :--------- | 
| SubscriptionId | GUID da subscrição | 
| SubscriçãoStartDate | Data de início da subscrição | 
| SubscriçãoEndDate | Data de fim da subscrição | 
| Subscrição Estatísticas | Estado da subscrição (Ative, Inative ou Em Período de Graça) | 
| Mensal | Data agregada por mês | 
| SKU | SKU do produto | 
| SKUId | SKU ID do produto | 
| FreeVsPaidSKU | Diferenciador SKU gratuito ou pago | 
| SalesModel | Modelo de vendas que é usado para vender a subscrição | 
| Modelo de Vendas Detalhadas | Modelo de vendas detalhado para a subscrição | 
| CustomerName | Nome do cliente | 
| CustomerTenantId | GUIA do inquilino do cliente | 
| CustomerTpid | Identificador do principal cliente do progenitor | 
| Gestão de Clientes | Segmento de mercado do cliente | 
| Mercado de Clientes | Mercado geográfico do cliente | 
| MPNId | Identificador da Microsoft Partner Network | 
| PartnerName | Nome do parceiro | 
| PartnerLocation | Localização geográfica do país do parceiro | 
| PartnerAttachType | Tipo de atribuição para a subscrição | 
| Lugares disponíveis | Lugares disponíveis atuais | 
| Caixas designadas | Lugares atuais atribuídos | 
| ActiveSeats | Assentos ativos atuais | 
| ImplantaçãoOpportunidade | Oportunidade de implementação atual | 
| ActiveUsagePercent | Percentagem de utilização ativa atual | 

### <a name="teams-meetings-and-calls-report"></a>**Reuniões de equipas e relatório de chamadas**

| Nome da coluna | Descrição dos dados | 
| :--------- | :--------- | 
| CustomerTenantId | ID do inquilino do cliente | 
| CustomerTpid | Identificador do principal cliente do progenitor | 
| Mensal | Mês para o qual o uso é reportado | 
| Subtrabalho | Subtrabalho para o qual é reportada a utilização (reuniões, chamadas ou sistemas telefónicos) | 
| Contagem de reuniões | Número de reuniões | 
| Duração da reunião | Duração total da reunião em horas | 

### <a name="teams-monthly-usage-report"></a>**Relatório mensal de utilização das equipas**

| Nome da coluna | Descrição dos dados | 
| :--------- | :--------- | 
| CustomerTenantId | ID do inquilino do cliente | 
| CustomerTpid | Identificador do principal cliente do progenitor | 
| Mensal | Mês para o qual o uso é reportado | 
| Subtrabalho | Subtrabalho para o qual é reportada a utilização (reuniões, chamadas ou sistemas telefónicos) | 
| Utilizadores de desktop | Número de utilizadores que usam equipas no ambiente de trabalho | 
| Utilizadores Móveis | Número de utilizadores que usam equipas no telemóvel | 
| Utilizadores da Web | Número de utilizadores que usam Equipas na web | 
| AllUpParticipants | Número de utilizadores únicos de Equipas para o mês | 

### <a name="teams-usage-3p-apps-report"></a>**Relatório de aplicações de utilização 3P das equipas**

| Nome da coluna | Descrição dos dados | 
| :--------- | :--------- | 
| CustomerTenantId | ID do inquilino do cliente | 
| CustomerTpid | ID do pai de topo do cliente | 
| Mensal | Mês para o qual o uso é reportado | 
| Nome da aplicação 3P | Nome da app Teams | 
| Contagem de utilizadores | Número de utilizadores para a app | 


### <a name="training-details-report"></a>**Relatório de detalhes da formação**

| Nome da coluna | Descrição dos dados | 
| :--------- | :--------- | 
| TrainingActivityId | Identificador da formação | 
| TrainingTitle | Título da formação | 
| Célula de Formação | Tipo de formação (certificação ou exame) | 
| Nome IndividualFirst | Primeiro nome do cliente | 
| Nome IndividualLast | Último nome do cliente | 
| E-mail | ID de e-mail pessoal do cliente | 
| CorpEmail | ID de e-mail do cliente | 
| Curso de FormaçãoDate | Data de conclusão da formação | 
| Mensal | Mês para o qual os dados são reportados | 
| ICMCP | Indica se o utilizador é um Microsoft Certified Professional (MCP) | 
| MCPID | ID MCP do utilizador | 
| MPNId | Identificador da Microsoft Partner Network | 
| PartnerName | Nome do parceiro | 
| PartnerCityLocation | Localização geográfica da cidade do parceiro | 
| PartnerCountryLocation | Localização geográfica do país do parceiro | 

### <a name="microsoft-learn-report"></a>**Relatório microsoft learn**

| Nome da coluna | Descrição dos dados | 
| :--------- | :--------- | 
| Nome de Utilizador | Nome do utilizador | 
| IDUtilizador | GUIA do utilizador | 
| Nome de formação | Nome do treino | 
| Célula de Formação | Tipo de formação (módulo ou caminho de aprendizagem) | 
| Produtos | Produto para o qual o módulo de aprendizagem é aplicável | 
| Funções | Funções aplicáveis da formação | 
| ConclusãoDate | Data de conclusão da formação | 
| MPNId | Identificador da Microsoft Partner Network | 
| PartnerName | Nome do parceiro | 
| País | Localização geográfica do país do parceiro | 

### <a name="competency-summary-and-history-report"></a>**Resumo da competência e relatório de história**

| Nome da coluna | Descrição dos dados | 
| :--------- | :--------- | 
| CompetênciaName | Nome da competência | 
| CompetênciaLevel | Nível da competência (Ouro ou Prata) | 
| CompetênciaSStatus | Estado atual da competência (Ative, Inativo ou Em Período de Graça) | 
| CompetênciaStartDate | Data de início da competência | 
| CompetênciaEndDate | Data de fim da competência | 

### <a name="competency-performance-report"></a>**Relatório de desempenho da competência**

| Nome da coluna | Descrição dos dados | 
| :--------- | :--------- | 
| CompetênciaName | Nome da competência | 
| CompetênciaAttainmentOptionName | Nome da opção de obtenção de competências | 
| Mensal | Mês para o qual as métricas são reportadas | 
| MetricName | Nome da métrica que é relevante para a competência | 
| MétricaMonthlyContribution | Contribuição mensal da métrica | 
| TTMAggregate | Métrica agregada para os 12 meses de fuga | 
| AniversárioYearAggregate | Métrica agregada para o ano de aniversário em curso | 
| GoldThreshold | Requisito de desempenho para satisfazer a competência gold | 
| SilverThreshold | Requisito de desempenho para satisfazer a competência silver | 

### <a name="cloud-ascent---microsoft-365-propensity-report"></a>**Cloud Ascent - Relatório de propensão da Microsoft 365**

| Nome da coluna | Descrição dos dados | 
| :--------- | :--------- | 
| ID do MPN | ID da rede de parceiros da Microsoft | 
| Nome do parceiro | Nome do parceiro | 
| ID de Cliente | Número de identificador do cliente | 
| Número duns | O número do & Deso de Bradstreet (D&B) do cliente que está a ser marcado para propensão | 
| Nome da Conta | Nome da conta | 
| Domínio | Domínio da conta | 
| Tamanho org | Tamanho da organização | 
| Setor | Indústria a que a organização pertence | 
| Vertical | A vertical do cliente que está a ser pontuado para a propensão, identificada pela Microsoft, D&B, e outros padrões da indústria | 
| Área | Área geográfica da localização | 
| Subsidiária | A subsidiária do cliente que está a ser pontuada por propensão | 
| Território de Vendas | O território de vendas do cliente que está sendo marcado para propensão | 
| City | Localização geográfica da cidade da organização | 
| Estado | Localização geográfica do estado da organização | 
| Código Postal | Código postal da organização | 
| País | Localização geográfica do país da organização | 
| Segment | Segmento de mercado | 
| Sub-Segmento | Subsegmento do mercado | 
| Resumo do tipo SMC | Tipo SMC | 
| Top Unmanaged - Base de Computação | Principais clientes não geridos - computação | 
| Top Unmanaged - Base de Utilizador | Principais clientes não geridos – utilizador | 
| IsNonProfit | Indica se a organização é sem fins lucrativos (Sim ou Não) | 
| Ativar o Trabalho Remoto - troca de alvo online | Clientes que tenham uma subscrição ativa do Exchange Online, subvenda para o Microsoft 365 | 
| Ativar trabalho remoto - aquisição no local (versão atual) com propensão Cloud Ascent - +10 licenças | Cliente que tem um cliente atual no local, Office ou cliente Windows. Ou seja, a versão do cliente é mais tarde do que um fim de vida (versão EOL). O cliente tem 10 ou mais licenças. Cliente que tem uma pontuação de propensão. O parceiro deverá ser alvo de conversão para o Microsoft 365. | 
| Ativar o Trabalho Remoto - aquisição no local (versão atual) com propensão Cloud Ascent - <10 licenças | Cliente que tem um cliente atual no local Office ou cliente Windows (isto é, uma versão mais tarde do que o EOL). O cliente tem menos de 10 licenças. Cliente que tem uma pontuação de propensão. O parceiro deverá ser alvo de conversão para o Microsoft 365. | 
| Ativar trabalho remoto - aquisição no local (versão atual) sem propensão Cloud Ascent - +10 licenças | Cliente que tem um cliente atual no local Office ou cliente Windows (isto é, uma versão mais tarde do que o EOL). O cliente tem 10 ou mais licenças. O cliente não tem uma pontuação de propensão. O parceiro deverá ser alvo de conversão para o Microsoft 365. | 
| Ativar o Trabalho Remoto - aquisição no local (versão atual) sem propensão Cloud Ascent - <10 licenças | Cliente que tem um cliente atual no local Office ou cliente Windows (isto é, uma versão mais tarde do que o EOL). O cliente tem menos de 10 licenças. O cliente não tem uma pontuação de propensão. O parceiro deverá ser alvo de conversão para o Microsoft 365. | 
| Ativar trabalho remoto - aquisição no local (versão EOL) com propensão Cloud Ascent - +10 licenças | Cliente que tenha um EOL no local Office ou cliente Windows (isto é, uma versão EOL ou anterior). O cliente tem 10 ou mais licenças. O cliente tem uma pontuação de propensão. O parceiro deverá ser alvo de conversão para o Microsoft 365. | 
| Ativar o Trabalho Remoto - aquisição no local (versão EOL) com propensão Cloud Ascent - <10 licenças | Cliente que tenha um EOL no local Office ou cliente Windows (isto é, uma versão EOL ou anterior). O cliente tem menos de 10 licenças. O cliente tem uma pontuação de propensão. O parceiro deverá ser alvo de conversão para o Microsoft 365. | 
| Ativar trabalho remoto - aquisição no local (versão EOL) sem propensão Cloud Ascent - +10 licenças | Cliente que tem um cliente atual no local Office ou cliente Windows (isto é, uma versão EOL ou anterior). O cliente tem 10 ou mais licenças. O cliente não tem uma pontuação de propensão. O parceiro deverá ser alvo de conversão para o Microsoft 365. | 
| Ativar o Trabalho Remoto - aquisição no local (versão EOL) sem propensão Cloud Ascent - <10 licenças | Cliente que tem um cliente atual no local Office ou cliente Windows (isto é, uma versão EOL ou anterior). O cliente tem menos de 10 licenças. O cliente não tem uma pontuação de propensão. O parceiro deverá ser alvo de conversão para o Microsoft 365. | 
| Enable Remote Work - perspetiva de alta propensão para a Microsoft 365 (Act NowithEvaluate) | Prospect cliente com elevada propensão para a Microsoft 365 | 
| Enable Remote Work - competir (Zoom) com a Microsoft 365 | Cliente com Zoom e Microsoft 365, alvo de conversão para Equipas | 
| Enable Remote Work - competir (Zoom) sem a Microsoft 365 | Cliente com Zoom, alvo de conversão para Equipas | 
| Reduzir custos e gerir - Microsoft 365 E3 direcionado para o Microsoft 365 E5 | Cliente existente com Microsoft 365 E3, alvo para Microsoft 365 E5 | 
| Reduzir custos e gerir - Microsoft 365 Business Basic e business standard clientes direcionados para Microsoft 365 Business Premium | Clientes Microsoft 365 Business Basic e Business Standard existentes, alvo para Microsoft 365 Business Premium | 
| Transformar produtividade organizacional - Propensão de superfície | Cliente mostra uma propensão para Superfície | 
| M365Cluster | Identifica a propensão de um cliente para comprar o Microsoft 365. Target Act Now e Avaliar os clusters porque eles vão produzir um rendimento mais alto. Destino Nutrir e Educar os clientes apenas se ainda houver capacidade após a Act Now e avaliar os clientes são direcionados. | 
| M365Fit | Pontos de dados internos e externos que definem firmográficos. Fit scoreing usa um modelo sósia para os nossos melhores pequenos ou médios negócios (SMBs) para comparar clientes e ver se eles são um potencial ajuste para produtos cloud microsoft. A pontuação de ajuste é atualizada trimestralmente. | 
| M365Intente | Sinais relacionados com as redes sociais e o comportamento online de um cliente definem a Intenção. A pontuação intencional está sobreposta em Fit para definir os clusters. A pontuação de intenção é atualizada mensalmente. | 
| SurfaceCluster | Identifica a propensão de um cliente para comprar a Surface, consolidando as recomendações fit e intenta num cluster. Target Act Now e Avaliar os clusters porque eles vão produzir um rendimento mais alto. Destino Nutrir e Educar os clientes apenas se ainda houver capacidade após a Act Now e avaliar os clientes são direcionados. | 
| SurfaceFit | Pontos de dados internos e externos que definem firmográficos. Fit scoreing usa um modelo sósia para os nossos melhores SMBs para comparar clientes e ver se eles são um potencial apto para produtos cloud microsoft. A pontuação de ajuste é atualizada trimestralmente. | 
| SuperfícieIntente | Sinais relacionados com as redes sociais e o comportamento online de um cliente definem a Intenção. A pontuação intencional está sobreposta em Fit para definir os clusters. A pontuação de intenção é atualizada mensalmente. | 
| O365Cluster | Identifica a propensão do cliente para a compra do Office 365. Target Act Now e Avaliar os clusters porque eles vão produzir um rendimento mais alto. Destino Nutrir e Educar os clientes apenas se ainda houver capacidade após a Act Now e avaliar os clientes são direcionados. | 
| O365Fit | Pontos de dados internos e externos que definem firmográficos. Fit scoreing usa um modelo sósia para os nossos melhores SMBs para comparar clientes e ver se eles são um potencial apto para produtos cloud microsoft. A pontuação de ajuste é atualizada trimestralmente. | 
| O365Intente | Sinais relacionados com as redes sociais e o comportamento online de um cliente definem a Intenção. A pontuação intencional está sobreposta em Fit para definir os clusters. A pontuação de intenção é atualizada mensalmente. | 
| M365UpsellCustomer | Identifica se o cliente aparece a vender propensão para a Microsoft 365 | 
| Tem Google | Identifica se o cliente apresenta sinais competitivos para possuir produtos da Google | 
| Tem aws | Identifica se o cliente apresenta sinais competitivos para possuir produtos amazon Web Services (AWS) | 
| Tem EA | Identifica se uma renovação é um acordo de empresa (EA) ou uma subscrição da EA | 
| Tem Aberto | Identifica se uma renovação é um contrato de Valor Aberto ou Aberto | 

### <a name="cloud-ascent---dynamics-365-propensity-report"></a>**Cloud Ascent - Relatório de propensão dinâmica 365**

| Nome da coluna | Descrição dos dados | 
| :--------- | :--------- | 
| ID do MPN | Microsoft Partner Network (MPN) ID | 
| Nome do parceiro | Nome do parceiro | 
| ID de Cliente | Número do identificador do cliente | 
| Número duns | O Dun & número de Bradstreet do cliente que está a ser marcado por propensão | 
| Nome da Conta | Nome da conta | 
| Domínio | Domínio da conta | 
| Tamanho org | Tamanho da organização | 
| Setor | Indústria a que a organização pertence | 
| Vertical | A vertical do cliente que está a ser pontuado para a propensão, identificada pela Microsoft, D&B, e outros padrões da indústria
| Área | Área geográfica da localização | 
| Subsidiária | A subsidiária do cliente que está a ser pontuada por propensão | 
| Território de Vendas | O território de vendas do cliente que está sendo marcado para propensão | 
| City | Localização geográfica da cidade | 
| Estado | Localização geográfica do estado | 
| Código Postal | Código postal da organização | 
| País | Localização geográfica do país | 
| Segment | Segmento de mercado | 
| Sub-Segmento | Subsegmento do mercado | 
| Resumo do tipo SMC | A categorização de um cliente: As principais bases de utilizadores não geridas são clientes com mais de 300 colaboradores, as bases de computação não geridas são clientes com USD 10.000 em potencial de três anos Azure, médias empresas são clientes com 25 empregados ou mais, e as pequenas empresas são clientes com menos de 25 colaboradores. | 
| Top Unmanaged - Base de Computação | Principais clientes não geridos - computação | 
| Top Unmanaged - Base de Utilizador | Principais clientes não geridos – utilizadores | 
| IsNonProfit | Indica se a organização é sem fins lucrativos (Sim ou Não) | 
| Ativar a venda digital - Microsoft 365 - tamanho do assento >= 25 lugares (modelo de propensão SalesPro) | Cliente sem Dinâmica 365. Tamanho do assento: 25+. O parceiro deverá ser alvo de cross-sell da Dynamics 365 SalesPro. | 
| Ativar a venda digital - Dinâmica 365 SalesPro propensão (Act Now ou Avaliar) | Clientes de alta propensão sem a Dynamics 365. O parceiro deverá ser alvo da Dynamics 365 SalesPro. | 
| Gestão de Risco Financeiro & Fraude - Base de instalação de instalações dinâmicas - Navision (modelo de propensão Business Central) | Cliente existente com nana no local. O parceiro deverá ser o alvo da Dynamics 365 Business Central. | 
| Gestão do risco financeiro & Fraude - Base de instalação de instalações dinâmicas - Dynamics AX (Dynamics 365 Finance + Operations propensity model) | Cliente existente com AX no local. O parceiro deverá ser alvo da Dynamics 365 Finance + Operations. | 
| Gestão de Risco Financeiro & Fraude - Base de instalação de instalações dinâmicas - Great Plains (modelo de propensão Business Central) | Cliente existente com grandes planícies no local. O parceiro deverá ser o alvo da Dynamics 365 Business Central. | 
| Gestão de Risco Financeiro & Fraude - Base de instalação de instalações dinâmicas - Solomon (modelo de propensão Business Central) | Cliente existente com Salomão no local. O parceiro deverá ser o alvo da Dynamics 365 Business Central. | 
| Gestão de Risco Financeiro & Fraude - Base de instalação de instalações dinâmicas - Outros (modelo de propensão Business Central) | Cliente existente com outras soluções no local não listadas anteriormente. O parceiro deverá ser o alvo da Dynamics 365 Business Central. | 
| Construir Agile Business Processes - Base de instalação dinâmica - AX/GP/SL/NAV/Outros (modelo de propensão Dinâmica 365) | Construir Agile Business Processes - Base de instalação dinâmica - AX/GP/SL/NAV/Outros (modelo de propensão Dinâmica 365) | 
| Construir Agile Business Processes - Base de competição dinâmica - Mendix/OutSystems/Salesforce (modelo de propensão Dinâmica 365) | Construir processos de negócio ágeis - Base de competição dinâmica - Mendix/OutSystems/Salesforce (modelo de propensão Dinâmica 365) | 
| Construir Agile Business Processes - Dinâmica 365 Finanças + Bases de instalação de operações | Dinâmicas existentes 365 Clientes de Finanças + Operações. Parceiro para direcionar as Aplicações de Energia. | 
| Construir Agile Business Processes - Dynamics 365 Business Central instalar base | Clientes Existentes Dynamics 365 Business Central. Parceiro para direcionar as Aplicações de Energia. | 
| Construir Processos Empresariais Áile - Base de instalação de envolvimento com clientes Dynamics 365 | Clientes de Envolvimento de Clientes da Dynamics 365 existentes. Parceiro para direcionar as Aplicações de Energia. | 
| Construir uma cadeia de fornecimento resiliente - Windows e ativar a primeira carga de trabalho Dynamics 365 como Dynamics 365 Supply Chain Management com clientes não-Oracle ou SAP ERP (planeamento de recursos empresariais) | Clientes-alvo da Dynamics 365 Supply Chain Management | 
| Construir uma cadeia de fornecimento resiliente - cross-sell Dynamics 365 Supply Chain Management e/ou Retail or Commerce para os clientes existentes Dynamics 365 Customer Engagement | Os clientes existentes da Dynamics 365 Customer Engagement visam a cross-selling Dynamics 365 Supply Chain Management. | 
| Construir uma cadeia de fornecimento resiliente - cross-sell Dynamics 365 Supply Chain Management e/ou Retail or Commerce to Dynamics 365 Customer Engagement and Oracle ou SAP | Dinâmicas existentes 365 Clientes de Envolvimento com Clientes com Oracle ou SAP para alvo para a Dynamics 365 Supply Chain Management | 
| D365BCCluster | Identifica a propensão do cliente para comprar a Dynamics 365 Business Central. Os clientes que mostrarem uma propensão para a Business Central estarão nas categorias Média e Pequena. Target Act Now e Avaliar os clusters, porque eles vão produzir um rendimento mais alto. Destino Nutrir e Educar clientes apenas se ainda houver capacidade depois de ter como alvo a Act Now e avaliar os clientes. | 
| D365BCFit | Pontos de dados internos e externos que definem firmográficos. Fit scoreing usa um modelo sósia para o nosso melhor SMB para comparar clientes e ver se eles são um potencial apto para produtos cloud microsoft. A pontuação de ajuste é atualizada trimestralmente. | 
| D365BCIntente | Sinais relacionados com as redes sociais e o comportamento online de um cliente definem a Intenção. A pontuação intencional está sobreposta em Fit para definir os clusters. A pontuação de intenção é atualizada mensalmente. | 
| D365FOCluster | Identifica a propensão do cliente para comprar a Dynamics 365 Finanças e Operações. Os clientes que mostrarem uma propensão para Finanças + Operações estarão nas categorias de topo não geridos. Target Act Now e Avaliar os clusters, porque eles vão produzir um rendimento mais alto. Destino Nutrir e Educar clientes apenas se ainda houver capacidade depois de ter como alvo a Act Now e avaliar os clientes. | 
| D365FOFit | Pontos de dados internos e externos que definem firmográficos. Fit scoreing usa um modelo sósia para o nosso melhor SMB para comparar clientes e ver se eles são um potencial apto para produtos cloud microsoft. A pontuação de ajuste é atualizada trimestralmente. | 
| D365FOIntente | Sinais relacionados com as redes sociais e o comportamento online de um cliente definem a Intenção. A pontuação intencional está sobreposta em Fit para definir os clusters. A pontuação de intenção é atualizada mensalmente. | 
| D365CECluster | Identifica a propensão do cliente para comprar o Envolvimento do Cliente Dynamics 365. Os clientes que mostrarem uma propensão para o Envolvimento do Cliente estarão nas categorias Média e Pequena. Target Act Now e Avaliar os clusters, porque eles vão produzir um rendimento mais alto. Destino Nutrir e Educar clientes apenas se ainda houver capacidade depois de ter como alvo a Act Now e avaliar os clientes. | 
| D365CEFit | Indica ajuste para dinâmica 365 envolvimento do cliente | 
| D365CEIntente | Indica intenção para a dinâmica 365 envolvimento do cliente | 
| DynamicsOnPremAXorCRM_HasOpenRenewal | Identifica se o cliente tem uma renovação aberta para a Dynamics no local AX ou CRM | 
| M365UpsellCustomer | Identifica se o cliente aparece a vender propensão para a Microsoft 365 | 
| Tem Google | Identifica se o cliente apresenta sinais competitivos para possuir produtos da Google | 
| Tem aws | Identifica se o cliente apresenta sinais competitivos para possuir produtos AWS | 
| Tem EA | Identifica se uma renovação é uma subscrição da EA ou da EA | 
| Tem Aberto | Identifica se uma renovação é um contrato de Valor Aberto ou Aberto | 

### <a name="cloud-ascent---azure-propensity-report"></a>**Cloud Ascent - Relatório de propensão do Azure**

| Nome da coluna | Descrição dos dados | 
| :--------- | :--------- | 
| ID do MPN | Microsoft Partner Network (MPN) ID | 
| Nome do parceiro | Nome do parceiro | 
| ID de Cliente | Número do identificador do cliente | 
| Número duns | O Dun & número de Bradstreet do cliente que está a ser marcado por propensão | 
| Nome da Conta | Nome da conta | 
| Domínio | Domínio da conta | 
| Tamanho org | Tamanho da organização | 
| Setor | Setor | 
| Vertical | A vertical do cliente que está a ser pontuado para a propensão, identificada pela Microsoft, D&B, e outros padrões da indústria | 
| Área | Área geográfica da localização | 
| Subsidiária | A subsidiária do cliente que está a ser pontuada por propensão | 
| Território de Vendas | O território de vendas do cliente que está sendo marcado para propensão | 
| City | Localização geográfica da cidade | 
| Estado | Localização geográfica do estado | 
| Código Postal | Código postal da organização | 
| País | Localização geográfica do país | 
| Segment | Segmento de mercado | 
| Sub-Segmento | Subsegmento do mercado | 
| Resumo do tipo SMC | Tipo SMC | 
| Top Unmanaged - Base de Computação | Principais clientes não geridos - computação | 
| Top Unmanaged - Base de Utilizador | Principais clientes não geridos – utilizadores | 
| IsNonProfit | Indica se a organização é sem fins lucrativos (Sim ou Não) | 
| Migrar - EOL Windows Server - EOL Windows Server IB com propensão Cloud Ascent - 5+ licenças | Cliente que tem um EOL no local Do Windows Server (isto é, uma versão EOL ou anterior). O cliente tem 5 ou mais licenças. Cliente que tem uma pontuação de propensão. O parceiro deve direcionar este cliente para a migração para Azure. | 
| Migrar - EOL Windows Server - EOL Windows Server IB com propensão cloud ascent - <5 licenças | Cliente que tem um EOL no local Do Windows Server (isto é, uma versão EOL ou anterior). O Cliente tem menos de 5 licenças. Cliente que tem uma pontuação de propensão. O parceiro deve direcionar este cliente para a migração para Azure. | 
| Migrar - EOL Windows Server - EOL Windows Server IB sem propensão cloud Ascent - 5+ licenças | Cliente que tem um EOL no local Do Windows Server (isto é, uma versão EOL ou anterior). O cliente tem mais de 5 licenças. O cliente não tem uma pontuação de propensão. O parceiro deve direcionar este cliente para a migração para Azure. | 
| Migrar - EOL Windows Server - EOL Windows Server IB sem propensão cloud Ascent - <5 licenças | Cliente que tem um EOL no local Do Windows Server (isto é, uma versão EOL ou anterior). Tem menos de 5 licenças. O cliente não tem uma pontuação de propensão. O parceiro deve direcionar este cliente para a migração para Azure. | 
| Migrar - EOL SQL - EOL SQL Server IB com propensão Cloud Ascent - 5+ licenças | Cliente que tem um EOL no local SQL Server (isto é, uma versão EOL ou anterior). O cliente tem mais de 5 licenças. O cliente tem uma pontuação de propensão. O parceiro deve direcionar este cliente para a migração para Azure. | 
| Migrar - EOL SQL - EOL SQL Server IB com propensão cloud ascent - <5 licenças | Cliente que tem um EOL no local SQL Server (isto é, uma versão EOL ou anterior). Tem menos de 5 licenças. Cliente que tem uma pontuação de propensão. O parceiro deve direcionar este cliente para a migração para Azure. | 
| Migrar - EOL SQL - EOL SQL Server IB sem propensão cloud ascent - 5+ licenças | Cliente que tem um EOL no local SQL Server (isto é, uma versão EOL ou anterior). O cliente tem 5 ou mais licenças. O cliente não tem uma pontuação de propensão. O parceiro deve direcionar este cliente para a migração para Azure. | 
| Migrar - EOL SQL - EOL SQL Server IB sem propensão cloud ascent - <5 licenças | Cliente que tem um EOL no local SQL Server (isto é, uma versão EOL ou anterior). O cliente tem menos de 5 licenças. O cliente não tem uma pontuação de propensão. O parceiro deve direcionar este cliente para a migração para Azure. | 
| Migrar - Migrar no local Windows Server - atual Servidor do Windows IB com propensão cloud ascent - 5+ licenças | Cliente que tem um atual Windows Server (isto é, uma versão mais tarde que o EOL). O cliente tem mais de 5 licenças. O cliente tem uma pontuação de propensão. O parceiro deve direcionar este cliente para a migração para Azure. | 
| Migrar - Migrar no local Windows Server - atual Servidor do Windows IB com propensity Cloud Ascent - <5 licenças | Cliente que tem um atual Windows Server (isto é, uma versão mais tarde que o EOL). O cliente tem menos de 5 licenças. O cliente tem uma pontuação de propensão para o Azure. O parceiro deve direcionar este cliente para a migração para Azure. | 
| Migrar - Migrar no local Windows Server - atual Servidor do Windows IB sem propensão cloud Ascent - 5+ licenças | Cliente que tem um atual Windows Server (isto é, uma versão mais tarde que o EOL). O cliente tem mais de 5 licenças. O cliente não tem uma pontuação de propensão. O parceiro deve direcionar este cliente para a migração para Azure. | 
| Migrar - Migrar no local Windows Server - atual Servidor do Windows IB sem propensão cloud Ascent - <5 licenças | Cliente que tem um atual Windows Server (isto é, uma versão mais tarde que o EOL). O cliente tem menos de 5 licenças. O cliente não tem uma pontuação de propensão. O parceiro deve direcionar este cliente para a migração para Azure. | 
| Migrar - Migrar para Azure SQL ou SQL máquinas virtuais (VMs) - atual SQL Server IB com propensão cloud ascent - 5+ licenças | Cliente que tem um servidor SQL no local atual (isto é, uma versão mais tarde que o EOL). O cliente tem mais de 5 licenças. O cliente tem uma pontuação de propensão. O parceiro deve direcionar este cliente para a migração para Azure. | 
| Migrar - Migrar para Azure SQL ou SQL VMs - atual SQL Server IB com propensão cloud ascent - <5 licenças | Cliente que tem um servidor SQL no local atual (isto é, uma versão mais tarde que o EOL). O cliente tem menos de 5 licenças. O cliente tem uma pontuação de propensão. O parceiro deve direcionar este cliente para a migração para Azure. | 
| Migrar - Migrar para Azure SQL ou SQL VMs - atual SQL Server IB sem propensão cloud ascent - 5+ licenças | Cliente que tem um servidor SQL no local atual (isto é, uma versão mais tarde que o EOL). O cliente tem mais de 5 licenças. O cliente não tem uma pontuação de propensão. O parceiro deve direcionar este cliente para a migração para Azure. | 
| Migrar - Migrar para Azure SQL ou SQL VMs - atual SQL Server IB sem propensão cloud ascent - <5 licenças | Cliente que tem um servidor SQL no local atual (isto é, uma versão mais tarde que o EOL). O cliente tem menos de 5 licenças. O cliente não tem uma pontuação de propensão. O parceiro deve direcionar este cliente para a migração para Azure. | 
| Migrar - OSS - Migrar para Open Source Shakespeare (OSS) DB | Cliente existente com qualquer um dos seguintes produtos de competição: PostgreSQL, MySQL, MariaDB. O parceiro deve direcionar este cliente para a migração para Azure. | 
| Migrar - OSS - Linux em Azure | Cliente existente com a Linux. O parceiro deve direcionar este cliente para a migração para Azure. | 
| Migrar - SAP - SAP em Azure | Cliente existente com SAP. O parceiro deve direcionar este cliente para a migração para Azure. | 
| Migrar - Windows Virtual Desktop - Remote Desktop Services IB | Identifica clientes com serviços de desktop remotos do Windows ativos. O parceiro deve direcionar este cliente para a migração para Azure. | 
| Migrar - Windows Virtual Desktop - Cross Sell Modern Work to Azure/WVD | Identifica clientes com a Microsoft 365 e não tem Azure. O parceiro deve direcionar este cliente para a migração para Azure. | 
| Migrar - VMware IB | Cliente existente com o produto: VMware. O parceiro deve direcionar este cliente para a migração para Azure. | 
| Migração - Citrix IB | Cliente existente com o produto: Citrix Systems. O parceiro deve direcionar este cliente para a migração para Azure. | 
| Inovar - Analytics - Power BI IB com alta propensão Azure | Clientes com subscrição e Ative Power BI incluindo: Power BI - Standalone Pro, Power BI - Azure Suites, Power BI - Office Suites, Power BI Suites - Microsoft 365 | 
| Ativar - DevOps com GitHub - Estúdio Visual/MSDN IB | Identifica clientes com versões ativas do Visual Studio | 
| Versão Standard do Servidor do Windows | Exibe a versão das compras Standard do Windows Server pelo cliente | 
| Licença padrão do Servidor do Windows | Exibe o tipo de licença de compras Standard do Windows Server pelo cliente | 
| Versão do Centro de Dados do Servidor do Windows | Exibe a versão das compras do Windows Data Center pelo cliente | 
| Licença do Centro de Dados do Servidor do Windows | Exibe o tipo de licença de compras do Windows Data Center pelo cliente | 
| AzureFit | Pontos de dados internos e externos que definem firmográficos. Fit scoreing usa um modelo sósia para o nosso melhor SMB para comparar clientes e ver se eles são um potencial apto para produtos cloud microsoft. A pontuação de ajuste é atualizada trimestralmente. | 
| AzureIntente | Sinais relacionados com as redes sociais e o comportamento online de um cliente definem a Intenção. A pontuação intencional está sobreposta em Fit para definir os clusters. A pontuação de intenção é atualizada mensalmente. | 
| AzureCluster | Identifica a propensão do cliente para comprar a Azure consolidando as recomendações fit e intenta num cluster. Target Act Now e Avaliar os clusters, porque eles vão produzir um rendimento mais alto. Destino Nutrir e Educar clientes apenas se ainda houver capacidade depois de ter como alvo a Act Now e avaliar os clientes. | 
| WindowsServerDataCenter_HasOpenRenewal | Identifica se o cliente tem uma renovação aberta para o Centro de Dados do Windows Server | 
| WindowsServerStandard_HasOpenRenewal | Identifica se o cliente tem uma renovação aberta para o Windows Server Standard | 
| AzureUpsellCustomer | Identifica se o cliente mostra a propensão de upsell para a Azure | 
| Tem Google | Identifica se o cliente apresenta sinais competitivos para possuir produtos da Google | 
| Tem aws | Identifica se o cliente apresenta sinais competitivos para possuir produtos AWS | 
| Tem EA | Identifica se uma renovação é uma subscrição da EA ou da EA | 
| Tem Aberto | Identifica se uma renovação é um contrato de Valor Aberto ou Aberto | 

### <a name="cloud-ascent---agreement-renewal-propensity-report"></a>**Cloud Ascent - relatório de renovação do acordo**

| Nome da coluna | Descrição dos dados | 
| :--------- | :--------- | 
| ID do MPN | ID da rede de parceiros da Microsoft | 
| Nome do parceiro | Nome do parceiro | 
| ID de Cliente | Número do identificador do cliente | 
| Número duns | O Dun & número de Bradstreet do cliente que está a ser marcado por propensão | 
| Nome da Conta | Nome da conta | 
| Domínio | Domínio da conta | 
| Tamanho org | Tamanho da organização | 
| Setor | Setor | 
| Vertical | A vertical do cliente que está a ser pontuado para a propensão, identificada pela Microsoft, D&B, e outros padrões da indústria | 
| Área | Área geográfica da localização | 
| Subsidiária | A subsidiária do cliente que está a ser pontuada por propensão | 
| Território de Vendas | O território de vendas do cliente que está sendo marcado para propensão | 
| City | Localização geográfica da cidade | 
| Estado | Localização geográfica do estado | 
| Código Postal | Código postal da organização | 
| País | Localização geográfica do país | 
| Segment | Segmento de mercado | 
| Sub-Segmento | Subsegmento do mercado | 
| Resumo do tipo SMC | Tipo SMC | 
| Top Unmanaged - Base de Computação | Principais clientes não geridos - computação | 
| Top Unmanaged - Base de Utilizador | Principais clientes não geridos – utilizadores | 
| IsNonProfit | Indica se a organização é sem fins lucrativos (Sim ou Não) | 
| Tem Google | Identifica se o cliente apresenta sinais competitivos para possuir produtos AWS | 
| Tem aws | Identifica se o cliente apresenta sinais competitivos para possuir produtos AWS | 
| Aglomerado de Azure | Identifica a propensão do cliente para comprar a Azure. Target Act Now e Avaliar os clusters, porque eles vão produzir um rendimento mais alto. Destino Nutrir e Educar clientes apenas se ainda houver capacidade depois de ter como alvo a Act Now e avaliar os clientes. | 
| D365 Finanças + Agrupamento de Operações | Identifica a propensão do cliente para comprar a Dynamics 365 Finanças e Operações. Os clientes que mostrarem uma propensão para Finanças + Operações estarão nas categorias de topo não geridos. Target Act Now e Avaliar os clusters, porque eles vão produzir um rendimento mais alto. Destino Nutrir e Educar clientes apenas se ainda houver capacidade depois de ter como alvo a Act Now e avaliar os clientes. | 
| D365 CE Cluster | Identifica a propensão do cliente para comprar o Envolvimento do Cliente Dynamics 365. Os clientes que mostrarem uma propensão para o Envolvimento do Cliente estarão nas categorias Média e Pequena. Target Act Now e Avaliar os clusters, porque eles vão produzir um rendimento mais alto. Destino Nutrir e Educar clientes apenas se ainda houver capacidade depois de ter como alvo a Act Now e avaliar os clientes. | 
| Aglomerado D365 a.C. | Identifica a propensão do cliente para comprar a Dynamics 365 Business Central. Os clientes que mostrarem uma propensão para a Business Central estarão nas categorias Média e Pequena. Target Act Now e Avaliar os clusters, porque eles vão produzir um rendimento mais alto. Destino Nutrir e Educar clientes apenas se ainda houver capacidade depois de ter como alvo a Act Now e avaliar os clientes. | 
| Microsoft 365 Cluster | Identifica a propensão do cliente para comprar o Microsoft 365. Target Act Now e Avaliar os clusters, porque eles vão produzir um rendimento mais alto. Destino Nutrir e Educar clientes apenas se ainda houver capacidade depois de ter como alvo a Act Now e avaliar os clientes. | 
| Programa de Licenças | Identifica o tipo de programa de licença para a renovação | 
| ID do acordo | Identificador do acordo | 
| Data de Fim do Acordo | Data de fim do acordo | 
| Tipo de expiração | Tipo de expiração | 
| Receitas Caducidade | Receitas associadas a assinaturas caducadas | 
| Tem EA | Identifica se uma renovação é uma subscrição da EA ou da EA | 
| Tem Aberto | Identifica se uma renovação é um contrato de Valor Aberto ou Aberto | 
| Cliente Azure Upsell | Identifica se o cliente mostra a propensão de upsell para a Azure | 
| Cliente Microsoft 365 Upsell | Identifica se o cliente aparece a vender propensão para a Microsoft 365 | 
| Nome revSumDivision | Identifica o produto que está em cima da renovação | 

## <a name="next-steps"></a>Passos seguintes

Para mais informações, consulte [os relatórios do Download.](pci-download-reports.md)
