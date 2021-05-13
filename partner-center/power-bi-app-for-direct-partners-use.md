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
ms.openlocfilehash: 96fe57f6e89928a69051c2e201c444882500b844
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855034"
---
# <a name="view-your-business-data-with-the-partner-center-analytics-app-for-microsoft-power-bi"></a><span data-ttu-id="1ec98-103">Veja os seus dados de negócio com a aplicação Partner Center Analytics para Microsoft Power BI</span><span class="sxs-lookup"><span data-stu-id="1ec98-103">View your business data with the Partner Center Analytics app for Microsoft Power BI</span></span>



<span data-ttu-id="1ec98-104">**Funções adequadas**: Administração global | Administração de administração de utilizadores | Agente comercial | Agente administrativo</span><span class="sxs-lookup"><span data-stu-id="1ec98-104">**Appropriate roles**: Global admin | User management admin | Sales agent | Admin agent</span></span>

## <a name="view-your-business-data"></a><span data-ttu-id="1ec98-105">Ver os seus dados de negócio</span><span class="sxs-lookup"><span data-stu-id="1ec98-105">View your business data</span></span>

<span data-ttu-id="1ec98-106">Obtenha uma representação visual dos seus dados de negócio com a aplicação Partner Center Analytics para Power BI, incluindo:</span><span class="sxs-lookup"><span data-stu-id="1ec98-106">Get a visual representation of your business data with the Partner Center Analytics app for Power BI, including:</span></span>

- <span data-ttu-id="1ec98-107">Crescimento da sua base de clientes, subscrições e licenças</span><span class="sxs-lookup"><span data-stu-id="1ec98-107">Growth of your customer base, subscriptions, and licenses</span></span>

- <span data-ttu-id="1ec98-108">Utilização dos produtos Office 365, Microsoft Dynamics e Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="1ec98-108">Usage of Office 365, Microsoft Dynamics, and Microsoft Azure products</span></span>

- <span data-ttu-id="1ec98-109">Unidades de consumo diário para cada recurso medido em cada subscrição do Azure nos últimos 60 dias</span><span class="sxs-lookup"><span data-stu-id="1ec98-109">Daily consumption units for each metered resource in each Azure subscription for the last 60 days</span></span>

- <span data-ttu-id="1ec98-110">Custo estimado (com base no cartão de tarifa mais recente)</span><span class="sxs-lookup"><span data-stu-id="1ec98-110">Estimated cost (based on latest rate card)</span></span>

- <span data-ttu-id="1ec98-111">Capacidade de exportar conjuntos de dados e criar relatórios personalizados, incluindo por cliente.</span><span class="sxs-lookup"><span data-stu-id="1ec98-111">Ability to export datasets and create custom reports, including per customer.</span></span>

### <a name="about-the-partner-center-analytics-app-preview-release"></a><span data-ttu-id="1ec98-112">Sobre o lançamento da pré-visualização da aplicação Partner Center Analytics</span><span class="sxs-lookup"><span data-stu-id="1ec98-112">About the Partner Center Analytics app preview release</span></span>

- <span data-ttu-id="1ec98-113">Esta aplicação destina-se apenas a parceiros diretos no programa Cloud Solution Provider.</span><span class="sxs-lookup"><span data-stu-id="1ec98-113">This app is for direct partners in the Cloud Solution Provider program only.</span></span> <span data-ttu-id="1ec98-114">Outros parceiros na CSP (revendedores indiretos, por exemplo) não poderão assinar.</span><span class="sxs-lookup"><span data-stu-id="1ec98-114">Other partners in CSP (indirect resellers, for example) will not be able to sign in.</span></span>

- <span data-ttu-id="1ec98-115">Quaisquer custos estimados são dados de faturação/fatura prévia, e não são juridicamente vinculativos.</span><span class="sxs-lookup"><span data-stu-id="1ec98-115">Any estimated costs are pre-tax billing / invoice data, and are not legally binding.</span></span> <span data-ttu-id="1ec98-116">Os custos estimados devem ser utilizados apenas para informações sobre dados.</span><span class="sxs-lookup"><span data-stu-id="1ec98-116">Estimated costs are meant to be used for data insights only.</span></span>

- <span data-ttu-id="1ec98-117">A informação do cliente baseia-se em subscrições.</span><span class="sxs-lookup"><span data-stu-id="1ec98-117">Customer information is based on subscriptions.</span></span> <span data-ttu-id="1ec98-118">Quaisquer clientes que tenha criado recentemente, mas que ainda não tenham subscrições, não estão incluídos nas contagens.</span><span class="sxs-lookup"><span data-stu-id="1ec98-118">Any customers that you've recently created accounts for, but who don't yet have subscriptions, aren't included in counts.</span></span>

- <span data-ttu-id="1ec98-119">O custo estimado baseia-se no cartão de tarifa mais recente, que se baseia nos preços da CSP.</span><span class="sxs-lookup"><span data-stu-id="1ec98-119">Estimated cost is based on latest rate card, which is based on CSP pricing.</span></span>

- <span data-ttu-id="1ec98-120">Dias são dias de calendário.</span><span class="sxs-lookup"><span data-stu-id="1ec98-120">Days are calendar days.</span></span>

### <a name="business-insights-report"></a><span data-ttu-id="1ec98-121">Relatório de Insights de Negócios</span><span class="sxs-lookup"><span data-stu-id="1ec98-121">Business Insights report</span></span>

- <span data-ttu-id="1ec98-122">**Inquilinos do cliente**: Número de inquilinos distintos da AZure AD de clientes que adquiriram assinaturas</span><span class="sxs-lookup"><span data-stu-id="1ec98-122">**Customer tenants**: Number of distinct Azure AD tenants of customers that have purchased subscriptions</span></span>

- <span data-ttu-id="1ec98-123">**Novo (últimos 30 dias)**: Novos clientes que compram pelo menos uma subscrição nos últimos 30 dias</span><span class="sxs-lookup"><span data-stu-id="1ec98-123">**New (last 30 days)**: New customers purchasing at least one subscription in last 30 days</span></span>

- <span data-ttu-id="1ec98-124">**Churn (últimos 30 dias)**: Clientes sem assinaturas "ativas", "em graça" ou "desativadas"</span><span class="sxs-lookup"><span data-stu-id="1ec98-124">**Churn (last 30 days)**: Customers without any “active", “in grace" or “disabled" subscriptions</span></span>

- <span data-ttu-id="1ec98-125">**Novo (últimas 24 horas)**: Novos clientes que compram pelo menos uma subscrição nas últimas 24 horas</span><span class="sxs-lookup"><span data-stu-id="1ec98-125">**New (last 24 hours)**: New customers purchasing at least one subscription in last 24 hours</span></span>

- <span data-ttu-id="1ec98-126">**Custo mensal estimado nos últimos 12 meses**: Mês ao longo do mês tendência da fatura estimada antes de impostos valor do dólar agregado mensalmente durante o período dos últimos 12 meses</span><span class="sxs-lookup"><span data-stu-id="1ec98-126">**Estimated monthly cost over last 12 months**: Month over month trend of estimated pre-tax invoice dollar amount aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="1ec98-127">**Custo estimado por produto ao longo dos últimos 12 meses**: Produtos vendidos classificados pela estimativa de fatura de imposto em dólares agregados durante o período dos últimos 12 meses.</span><span class="sxs-lookup"><span data-stu-id="1ec98-127">**Estimated cost by product over last 12 months**: Products sold sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="1ec98-128">Este estatuto indica que os produtos de topo trazem a maioria das receitas.</span><span class="sxs-lookup"><span data-stu-id="1ec98-128">This status indicates top products bringing most revenue.</span></span>

- <span data-ttu-id="1ec98-129">**Clientes nos últimos 12 meses**: Mês ao longo do mês tendência de novos clientes e clientes agregados mensalmente ao longo do período dos últimos 12 meses</span><span class="sxs-lookup"><span data-stu-id="1ec98-129">**Customers over last 12 months**: Month over month trend of new customers and churn customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="1ec98-130">**Custo estimado pelo cliente ao longo dos últimos 12 meses**: Clientes classificados pelo valor estimado da fatura antes de impostos em dólares agregados ao longo do período dos últimos 12 meses.</span><span class="sxs-lookup"><span data-stu-id="1ec98-130">**Estimated cost by customer over last 12 months**: Customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="1ec98-131">Este estado indica que os principais clientes trazem a maioria das receitas.</span><span class="sxs-lookup"><span data-stu-id="1ec98-131">This status indicates top customers bringing most revenue.</span></span>

- <span data-ttu-id="1ec98-132">**Contagem de clientes por produto**: Produtos vendidos por clientes associados.</span><span class="sxs-lookup"><span data-stu-id="1ec98-132">**Customer count by product**: Products sold sorted by associated customers.</span></span> <span data-ttu-id="1ec98-133">Este estado indica produtos de topo vendidos à maioria dos clientes.</span><span class="sxs-lookup"><span data-stu-id="1ec98-133">This status indicates top products sold to most customers.</span></span>

### <a name="subscription-insights-report"></a><span data-ttu-id="1ec98-134">Relatório de Insights de Subscrição</span><span class="sxs-lookup"><span data-stu-id="1ec98-134">Subscription Insights report</span></span>

- <span data-ttu-id="1ec98-135">**Estado da subscrição**:</span><span class="sxs-lookup"><span data-stu-id="1ec98-135">**Subscription status**:</span></span>

- <span data-ttu-id="1ec98-136">Ativo: Assinaturas pertencentes ao estado "ativo" ou "em graça"</span><span class="sxs-lookup"><span data-stu-id="1ec98-136">Active: Subscriptions belonging to either “active" or “in grace" state</span></span>

  - <span data-ttu-id="1ec98-137">Suspenso: Assinaturas pertencentes ao estado "deficiente"</span><span class="sxs-lookup"><span data-stu-id="1ec98-137">Suspended: Subscriptions belonging to “disabled" state</span></span>

  - <span data-ttu-id="1ec98-138">Desestado: Assinaturas pertencentes ao estatuto de "desestado" ou "caducado"</span><span class="sxs-lookup"><span data-stu-id="1ec98-138">De-provisioned: Subscriptions belonging to “de-provisioned" or “expired" status</span></span>

- <span data-ttu-id="1ec98-139">**Estado da caducidade:**</span><span class="sxs-lookup"><span data-stu-id="1ec98-139">**Expiry status**:</span></span>

  - <span data-ttu-id="1ec98-140">Expirado: Assinaturas que já expiraram (onde a data de fim da subscrição é anterior)</span><span class="sxs-lookup"><span data-stu-id="1ec98-140">Expired: Subscriptions that have already expired (where subscription end date is in past)</span></span>

  - <span data-ttu-id="1ec98-141">Expiração após 30 dias: Assinaturas que expirarão após 30 dias (onde a data de fim da subscrição é após os próximos 30 dias)</span><span class="sxs-lookup"><span data-stu-id="1ec98-141">Expiring after 30 days: Subscriptions that will expire after 30 days (where subscription end date is after next 30 days)</span></span>

  - <span data-ttu-id="1ec98-142">Expiração em 30 dias: Assinaturas que caducarão nos próximos 30 dias (onde a data de fim da subscrição é entre hoje e os próximos 30 dias)</span><span class="sxs-lookup"><span data-stu-id="1ec98-142">Expiring in 30 days: Subscriptions that will expire within next 30 days (where subscription end date is between today and next 30 days)</span></span>

- <span data-ttu-id="1ec98-143">**Total de assinaturas**: Assinaturas em estado "ativo", "em graça" ou "deficiente"</span><span class="sxs-lookup"><span data-stu-id="1ec98-143">**Total subscriptions**: Subscriptions in “active," “in grace" or “disabled" status</span></span>

- <span data-ttu-id="1ec98-144">**Novidade (últimos 30 dias)**: Novas subscrições compradas pelos clientes nos últimos 30 dias</span><span class="sxs-lookup"><span data-stu-id="1ec98-144">**New (last 30 days)**: New subscriptions purchased by customers within last 30 days</span></span>

- <span data-ttu-id="1ec98-145">**Novidade (últimas 24 horas)**: Novas subscrições compradas pelos clientes nas últimas 24 horas</span><span class="sxs-lookup"><span data-stu-id="1ec98-145">**New (last 24 hours)**: New subscriptions purchased by customers within last 24 hours</span></span>

- <span data-ttu-id="1ec98-146">**Expiração em 30 dias**: Assinaturas que caducarão nos próximos 30 dias</span><span class="sxs-lookup"><span data-stu-id="1ec98-146">**Expiring in 30 days**: Subscriptions that will expire within next 30 days</span></span>

- <span data-ttu-id="1ec98-147">**Churn (últimos 30 dias)**: Assinaturas que tenham sido desavisionadas ou suspensas (desativadas) nos últimos 30 dias</span><span class="sxs-lookup"><span data-stu-id="1ec98-147">**Churn (last 30 days)**: Subscriptions that have been de-provisioned or Suspended (disabled) within last 30 days</span></span>

- <span data-ttu-id="1ec98-148">**Distribuição por tipos de subscrição**: % distribuição de subscrições totais por tipo de subscrição baseada em licença e por uso</span><span class="sxs-lookup"><span data-stu-id="1ec98-148">**Distribution by subscription types**: % distribution of total subscriptions by License based and usage-based subscription type</span></span>

- <span data-ttu-id="1ec98-149">**Contagem ativa de subscrição por produto**: Produtos vendidos classificados por subscrições ativas contam</span><span class="sxs-lookup"><span data-stu-id="1ec98-149">**Active subscription count by product**: Products sold sorted by active subscriptions count</span></span>

- <span data-ttu-id="1ec98-150">**Assinaturas ao longo dos últimos 12 meses**: Mês ao longo do mês tendência de novas subscrições e subscrições de churn agregadas mensalmente ao longo do período dos últimos 12 meses</span><span class="sxs-lookup"><span data-stu-id="1ec98-150">**Subscriptions over last 12 months**: Month over month trend of new subscriptions and churn subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="1ec98-151">**Detalhes da subscrição** do cliente : Vista detalhada dos clientes, subscrições e ofertas</span><span class="sxs-lookup"><span data-stu-id="1ec98-151">**Customer subscription details**: Detailed view of the customers, subscriptions, and offers</span></span>

### <a name="license-insights-report"></a><span data-ttu-id="1ec98-152">Relatório de Insights de Licença:</span><span class="sxs-lookup"><span data-stu-id="1ec98-152">License Insights report:</span></span>

- <span data-ttu-id="1ec98-153">**Total de licenças**: Número total de licenças agregadas em todas as subscrições baseadas em licenças</span><span class="sxs-lookup"><span data-stu-id="1ec98-153">**Total licenses**: Total number of licenses aggregated across all license-based subscriptions</span></span>

- <span data-ttu-id="1ec98-154">**Novo (últimos 30 dias)**: Adição de licença nos últimos 30 dias</span><span class="sxs-lookup"><span data-stu-id="1ec98-154">**New (last 30 days)**: License addition within last 30 days</span></span>

- <span data-ttu-id="1ec98-155">**Churn (últimos 30 dias)**: Redução da licença nos últimos 30 dias</span><span class="sxs-lookup"><span data-stu-id="1ec98-155">**Churn (last 30 days)**: License reduction within last 30 days</span></span>

- <span data-ttu-id="1ec98-156">**Novo (último 24 horas)**: Adição de licença nas últimas 24 horas</span><span class="sxs-lookup"><span data-stu-id="1ec98-156">**New (last 24 hours)**: License addition within last 24 hours</span></span>

- <span data-ttu-id="1ec98-157">**Licenças nos últimos 90 dias**: Mês ao longo do mês tendência de aditamentos e reduções de licenças agregadas mensalmente durante o período dos últimos 90 dias</span><span class="sxs-lookup"><span data-stu-id="1ec98-157">**Licenses over last 90 days**: Month over month trend of license additions and reductions aggregated monthly over the period of last 90 days</span></span>

- <span data-ttu-id="1ec98-158">**Contagem de licença ativa por produto**: Produtos vendidos classificados por contagem de licença ativa</span><span class="sxs-lookup"><span data-stu-id="1ec98-158">**Active license count by product**: Products sold sorted by active license count</span></span>

- <span data-ttu-id="1ec98-159">**Contagem de licença ativa por cliente**: Clientes classificados por contagem de licença ativa</span><span class="sxs-lookup"><span data-stu-id="1ec98-159">**Active license count by customer**: Customers sorted by active license count</span></span>

- <span data-ttu-id="1ec98-160">Detalhes do evento da licença do cliente ao longo dos **últimos 90 dias**: Vista detalhada dos clientes, subscrições e eventos de subscrição, incluindo data do evento, nome do evento, quantidade e alteração de quantidade.</span><span class="sxs-lookup"><span data-stu-id="1ec98-160">**Customer license event details over last 90 days**: Detailed view of the customers, subscriptions, and subscription events including event date, event name, quantity, and change in quantity.</span></span>

### <a name="licenses-usage-report"></a><span data-ttu-id="1ec98-161">Relatório de utilização das licenças:</span><span class="sxs-lookup"><span data-stu-id="1ec98-161">Licenses Usage report:</span></span>

- <span data-ttu-id="1ec98-162">**Licenças atribuídas por produto**: Produtos vendidos classificados por contagem de atribuição de licença</span><span class="sxs-lookup"><span data-stu-id="1ec98-162">**Licenses assigned by product**: Products sold sorted by license assignment count</span></span>

- <span data-ttu-id="1ec98-163">**Licenças em uso por produto**: Produtos vendidos classificados por contagem de utilização de licença</span><span class="sxs-lookup"><span data-stu-id="1ec98-163">**Licenses in use by product**: Products sold sorted by license usage count</span></span>

- <span data-ttu-id="1ec98-164">**Distribuição de clientes das licenças atribuídas:**% distribuição do total de clientes quebrados em baldes de 20% de intervalo por atribuição de licenças %</span><span class="sxs-lookup"><span data-stu-id="1ec98-164">**Customer distribution of licenses assigned**: % distribution of total customers broken in buckets of 20% range by license assignment %</span></span>

- <span data-ttu-id="1ec98-165">**Distribuição do cliente de licenças em uso**: % distribuição do total de clientes quebrados em baldes de 20% de intervalo por utilização de licença %</span><span class="sxs-lookup"><span data-stu-id="1ec98-165">**Customer distribution of licenses in use**: % distribution of total customers broken in buckets of 20% range by license usage %</span></span>

- <span data-ttu-id="1ec98-166">**Licenças atribuídas pelo cliente**: Vista detalhada das licenças vendidas e licenças atribuídas por clientes e produtos</span><span class="sxs-lookup"><span data-stu-id="1ec98-166">**Licenses assigned by customer**: Detailed view of licenses sold and licenses assigned by customers and products</span></span>

- <span data-ttu-id="1ec98-167">**Licenças em uso por cliente**: Vista detalhada das licenças vendidas e licenças em uso por clientes e produtos</span><span class="sxs-lookup"><span data-stu-id="1ec98-167">**Licenses in use by customer**: Detailed view of licenses sold and licenses in use by customers and products</span></span>

### <a name="azure-insights-report"></a><span data-ttu-id="1ec98-168">Relatório Azure Insights:</span><span class="sxs-lookup"><span data-stu-id="1ec98-168">Azure Insights report:</span></span>

- <span data-ttu-id="1ec98-169">**Clientes baseados em uso nos últimos 12 meses**: Mês ao longo do mês tendência de novos clientes baseados em uso e clientes com base em uso agregados mensalmente durante o período dos últimos 12 meses</span><span class="sxs-lookup"><span data-stu-id="1ec98-169">**Usage-based customers over last 12 months**: Month over month trend of new usage-based customers and churned usage-based customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="1ec98-170">**Subscrições baseadas em uso ao longo dos últimos 12 meses**: Tendência mensal de novas subscrições baseadas em uso e subscrições baseadas em uso agregadas mensalmente durante o período dos últimos 12 meses</span><span class="sxs-lookup"><span data-stu-id="1ec98-170">**Usage-based subscriptions over last 12 months**: Month over month trend of new usage-based subscriptions and churned usage-based subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="1ec98-171">**Custo estimado de utilização por parte do cliente ao longo dos últimos 60 dias**: Clientes baseados no uso classificados pelo valor estimado da fatura antes de impostos em dólares agregados ao longo do período dos últimos 60 dias.</span><span class="sxs-lookup"><span data-stu-id="1ec98-171">**Estimated cost of usage by customer over last 60 days**: Usage-based customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span> <span data-ttu-id="1ec98-172">Este estado indica que os clientes de topo baseados em uso trazem a maioria das receitas</span><span class="sxs-lookup"><span data-stu-id="1ec98-172">This status indicates top usage-based customers bringing most revenue</span></span>

- <span data-ttu-id="1ec98-173">**Custo estimado de utilização por categoria ao longo dos últimos 60 dias**: Categorias de contadores de assinaturas baseadas em uso ordenadas por valor estimado de fatura antes de impostos em dólares agregados ao longo do período dos últimos 60 dias.</span><span class="sxs-lookup"><span data-stu-id="1ec98-173">**Estimated cost of usage by category over last 60 days**: Meter categories of usage-based subscriptions sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="1ec98-174">**Custo estimado de utilização por subscrição ao longo dos últimos 60 dias**: Subscrições baseadas em uso por valor estimado em dólares de fatura pré-impostos agregados ao longo do período dos últimos 60 dias.</span><span class="sxs-lookup"><span data-stu-id="1ec98-174">**Estimated cost of usage by subscription over last 60 days**: Usage-based subscriptions by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="1ec98-175">**Custo de utilização estimado pelo cliente através do orçamento de gastos**: Clientes classificados em percentagem do seu orçamento atual de despesas de utilização excedendo o limiar (100%).</span><span class="sxs-lookup"><span data-stu-id="1ec98-175">**Customer estimated usage cost by spending budget**: Customers sorted by percentage of their current usage spending budget exceeding threshold (100%).</span></span>

### <a name="azure-resource-usage-report"></a><span data-ttu-id="1ec98-176">Relatório de utilização de recursos Azure:</span><span class="sxs-lookup"><span data-stu-id="1ec98-176">Azure Resource Usage report:</span></span>

- <span data-ttu-id="1ec98-177">**Utilização de recursos Azure por dia durante o período selecionado**: Unidades de consumo diário para cada recurso medido em cada subscrição baseada em utilização durante o período selecionado nos últimos 60 dias.</span><span class="sxs-lookup"><span data-stu-id="1ec98-177">**Usage of Azure resources by day for selected period**: Daily consumption units for each metered resource in each usage-based subscription for selected period within the last 60 days.</span></span>

- <span data-ttu-id="1ec98-178">**Custo estimado de utilização dos recursos Azure para o período selecionado**: Custo estimado com base no cartão de tarifa mais recente para cada recurso medido em cada subscrição baseada em uso para o período selecionado nos últimos 60 dias.</span><span class="sxs-lookup"><span data-stu-id="1ec98-178">**Estimated usage cost of Azure resources for selected period**: Estimated cost based on latest rate card for each metered resource in each usage-based subscription for selected period within the last 60 days.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="1ec98-179">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="1ec98-179">Next steps</span></span>

- [<span data-ttu-id="1ec98-180">Partner Center Analytics for Power BI app overview</span><span class="sxs-lookup"><span data-stu-id="1ec98-180">Partner Center Analytics for Power BI app overview</span></span>](power-bi-app-for-direct-partners.md)

- <span data-ttu-id="1ec98-181">[Install and preview the Partner Center Analytics app for Microsoft Power BI](power-bi-app-for-direct-partners-install.md) (Instalar e pré-visualizar a aplicação de Análise do Centro de Parceiros do Microsoft Power BI)</span><span class="sxs-lookup"><span data-stu-id="1ec98-181">[Install and preview the Partner Center Analytics app for Microsoft Power BI](power-bi-app-for-direct-partners-install.md)</span></span>
