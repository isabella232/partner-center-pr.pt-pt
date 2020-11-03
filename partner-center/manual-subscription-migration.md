---
title: Migrar Dinâmicas 365 subscrições
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como migrar de subscrições básicas e qualificadas da Dynamics 365 para uma nova subscrição antes de expirarem as subscrições existentes.
author: Brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8575d87ab3c4c7970135a87b7ef7564c4fe06232
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/17/2020
ms.locfileid: "92529280"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a><span data-ttu-id="40e53-103">Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions (Migrar o Dynamics 365 e o Customer Engagement Plan da versão Básica (ofertas qualificadas) para versões mais recentes)</span><span class="sxs-lookup"><span data-stu-id="40e53-103">Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions</span></span>

<span data-ttu-id="40e53-104">**Aplica-se a**</span><span class="sxs-lookup"><span data-stu-id="40e53-104">**Applies to**</span></span>

-  <span data-ttu-id="40e53-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="40e53-105">Partner Center</span></span>

<span data-ttu-id="40e53-106">**Funções adequadas**</span><span class="sxs-lookup"><span data-stu-id="40e53-106">**Appropriate roles**</span></span>
-   <span data-ttu-id="40e53-107">Administrador global</span><span class="sxs-lookup"><span data-stu-id="40e53-107">Global admin</span></span>
-   <span data-ttu-id="40e53-108">Administrador de utilizadores</span><span class="sxs-lookup"><span data-stu-id="40e53-108">User admin</span></span>
-   <span data-ttu-id="40e53-109">Agente administrativo</span><span class="sxs-lookup"><span data-stu-id="40e53-109">Admin agent</span></span>
-   <span data-ttu-id="40e53-110">Agente comercial</span><span class="sxs-lookup"><span data-stu-id="40e53-110">Sales agent</span></span>

<span data-ttu-id="40e53-111">A partir de 1 de janeiro de 2019, os clientes com Dinâmica 365 para Vendas/Plano de Envolvimento com o Cliente a partir de assinaturas Básicas (Ofertas Qualificadas) já não podem renovar estas ofertas antigas; as subscrições existentes não renovarão automaticamente quando expirarem.</span><span class="sxs-lookup"><span data-stu-id="40e53-111">Effective January 1, 2019, customers with Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) subscriptions can no longer renew these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="40e53-112">Na página de pormenor da subscrição, o estado de subscrição mudará para "Expira na [data]" de "Renovações automáticas em [data]".</span><span class="sxs-lookup"><span data-stu-id="40e53-112">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="40e53-113">Para garantir a continuidade dos clientes, deve transitar aqueles com subscrições caducadas para uma opção suportada, listada abaixo.</span><span class="sxs-lookup"><span data-stu-id="40e53-113">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="40e53-114">Recomendamos que os clientes mudem os clientes para novas subscrições antes da data de fim anual da subscrição para evitar eventuais interrupções de serviço para os clientes.</span><span class="sxs-lookup"><span data-stu-id="40e53-114">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="40e53-115">Se utilizar a API (CREST ou Partner Center), pode encontrar subscrições caducadas avaliando a data final da subscrição juntamente com a renovação automática = Propriedade falsa.</span><span class="sxs-lookup"><span data-stu-id="40e53-115">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="40e53-116">As subscrições em questão serão definidas para renovação automática=Falsa a 1 de janeiro de 2019.</span><span class="sxs-lookup"><span data-stu-id="40e53-116">The subscriptions in question will be set to auto renew=False on Jan 1, 2019.</span></span> <span data-ttu-id="40e53-117">Pode mover os clientes para um novo plano a qualquer momento.</span><span class="sxs-lookup"><span data-stu-id="40e53-117">You can move customers to a new plan at any time.</span></span> 

### <a name="the-dynamics-365-offers-being-retired"></a><span data-ttu-id="40e53-118">A Dynamics 365 oferece a reforma</span><span class="sxs-lookup"><span data-stu-id="40e53-118">The Dynamics 365 offers being retired</span></span>

- <span data-ttu-id="40e53-119">Dinâmica 365 para Venda Enterprise Edition CRMOL Basic (Oferta Qualificada)</span><span class="sxs-lookup"><span data-stu-id="40e53-119">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="40e53-120">Dinâmica 365 para Venda Enterprise Edition CRMOL Basic (Oferta Qualificada) para Faculdade</span><span class="sxs-lookup"><span data-stu-id="40e53-120">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="40e53-121">Dinâmica 365 para Sales Enterprise Edition CRMOL Basic (Oferta Qualificada) para Estudantes</span><span class="sxs-lookup"><span data-stu-id="40e53-121">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="40e53-122">Dinâmica 365 para Venda Enterprise Edition (Preço do Governo) CRMOL Basic (Oferta Qualificada)</span><span class="sxs-lookup"><span data-stu-id="40e53-122">Dynamics 365 for Sales Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="40e53-123">Dinâmica 365 para Venda Enterprise Edition Da SA para CRM Basic (Oferta Qualificada)</span><span class="sxs-lookup"><span data-stu-id="40e53-123">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="40e53-124">Dinâmica 365 para Venda Enterprise Edition From SA for CRM Basic (Oferta Qualificada) para Faculdade</span><span class="sxs-lookup"><span data-stu-id="40e53-124">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="40e53-125">Dinâmica 365 para Venda Enterprise Edition From SA for CRM Basic (Oferta Qualificada) para Estudantes</span><span class="sxs-lookup"><span data-stu-id="40e53-125">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="40e53-126">Dinâmica 365 para Venda Enterprise Edition (Preço do Governo) A partir de SA para CRM Basic (Oferta Qualificada)</span><span class="sxs-lookup"><span data-stu-id="40e53-126">Dynamics 365 for Sales Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="40e53-127">Dinâmica 365 para Venda Enterprise Edition Add-On para CRM Basic (Oferta Qualificada)</span><span class="sxs-lookup"><span data-stu-id="40e53-127">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="40e53-128">Dinâmica 365 para Venda Enterprise Edition Add-On para CRM Basic (Oferta Qualificada) para Faculdade</span><span class="sxs-lookup"><span data-stu-id="40e53-128">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="40e53-129">Dinâmica 365 para Venda Enterprise Edition Add-On para CRM Basic (Oferta Qualificada) para Estudantes</span><span class="sxs-lookup"><span data-stu-id="40e53-129">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="40e53-130">Dinâmica 365 para Venda Enterprise Edition (Preço do Governo) Add-On para CRM Basic (Oferta Qualificada)</span><span class="sxs-lookup"><span data-stu-id="40e53-130">Dynamics 365 for Sales Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="40e53-131">Dinâmica 365 Plano de Envolvimento com o Cliente Enterprise Edition CRMOL Basic (Oferta Qualificada)</span><span class="sxs-lookup"><span data-stu-id="40e53-131">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="40e53-132">Dinâmica 365 Plano de Envolvimento com o Cliente Enterprise Edition (Preço do Governo) CRMOL Basic (Oferta Qualificada)</span><span class="sxs-lookup"><span data-stu-id="40e53-132">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="40e53-133">Dinâmica 365 Plano de Envolvimento com o Cliente Enterprise Edition CRMOL Basic (Oferta Qualificada) para Estudantes</span><span class="sxs-lookup"><span data-stu-id="40e53-133">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="40e53-134">Dinâmica 365 Plano de Envolvimento com o Cliente Enterprise Edition CRMOL Basic (Oferta Qualificada) para Faculdade</span><span class="sxs-lookup"><span data-stu-id="40e53-134">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="40e53-135">Dinâmica 365 Plano de Envolvimento com o Cliente Edição Empresarial da SA para CRM Basic (Oferta Qualificada)</span><span class="sxs-lookup"><span data-stu-id="40e53-135">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="40e53-136">Dinâmica 365 Plano de Envolvimento com o Cliente Enterprise Edition (Preço do Governo) A partir de SA para CRM Basic (Oferta Qualificada)</span><span class="sxs-lookup"><span data-stu-id="40e53-136">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="40e53-137">Dinâmica 365 Plano de Envolvimento com o Cliente Edição Empresarial da SA para CRM Basic (Oferta Qualificada) para Estudantes</span><span class="sxs-lookup"><span data-stu-id="40e53-137">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="40e53-138">Dinâmica 365 Plano de Envolvimento com o Cliente Edição Empresarial da SA para CRM Basic (Oferta Qualificada) para Faculdade</span><span class="sxs-lookup"><span data-stu-id="40e53-138">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="40e53-139">Dinâmica 365 Plano de Envolvimento com o Cliente Enterprise Edition Add-On para CRM Basic (Oferta Qualificada)</span><span class="sxs-lookup"><span data-stu-id="40e53-139">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="40e53-140">Dinâmica 365 Plano de Envolvimento com o Cliente Enterprise Edition (Preço do Governo) Add-On para CRM Basic (Oferta Qualificada)</span><span class="sxs-lookup"><span data-stu-id="40e53-140">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="40e53-141">Dinâmica 365 Plano de Envolvimento com o Cliente Enterprise Edition Add-On para CRM Basic (Oferta Qualificada) para Estudantes</span><span class="sxs-lookup"><span data-stu-id="40e53-141">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="40e53-142">Dinâmica 365 Plano de Envolvimento com o Cliente Enterprise Edition Add-On para CRM Basic (Oferta Qualificada) para Faculdade</span><span class="sxs-lookup"><span data-stu-id="40e53-142">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a><span data-ttu-id="40e53-143">Dinâmica 365 para Plano de Venda/Envolvimento do Cliente a partir de planos básicos de substituição (Ofertas Qualificadas)</span><span class="sxs-lookup"><span data-stu-id="40e53-143">Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) replacement plans</span></span>

<span data-ttu-id="40e53-144">**Ofertas aposentadas**</span><span class="sxs-lookup"><span data-stu-id="40e53-144">**Retired offers**</span></span>   

- <span data-ttu-id="40e53-145">Dinâmica 365 para Vendas da CRM Basic ou CRMOL Basic (Oferta Qualificada)</span><span class="sxs-lookup"><span data-stu-id="40e53-145">Dynamics 365 for Sales from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="40e53-146">Dinâmica 365 Plano de Envolvimento do Cliente da CRM Basic ou CRMOL Basic (Oferta Qualificada)</span><span class="sxs-lookup"><span data-stu-id="40e53-146">Dynamics 365 Customer Engagement Plan from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>

<span data-ttu-id="40e53-147">**Opções de substituição**</span><span class="sxs-lookup"><span data-stu-id="40e53-147">**Replacement options**</span></span>
- <span data-ttu-id="40e53-148">Dinâmica 365 para Profissional de Vendas (NOVO)</span><span class="sxs-lookup"><span data-stu-id="40e53-148">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="40e53-149">Dinâmica 365 para Profissional de Vendas (NOVO)</span><span class="sxs-lookup"><span data-stu-id="40e53-149">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="40e53-150">Dynamics 365 for Customer Service</span><span class="sxs-lookup"><span data-stu-id="40e53-150">Dynamics 365 for Customer Service</span></span>
- <span data-ttu-id="40e53-151">Dinâmica 365 Plano de Envolvimento do Cliente ou</span><span class="sxs-lookup"><span data-stu-id="40e53-151">Dynamics 365 Customer Engagement Plan or</span></span>
- <span data-ttu-id="40e53-152">Dinâmica 365 Membros da equipa</span><span class="sxs-lookup"><span data-stu-id="40e53-152">Dynamics 365 Team Members</span></span>



## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="40e53-153">Transição de clientes para novos planos de produtos</span><span class="sxs-lookup"><span data-stu-id="40e53-153">Transition customers to new product plans</span></span>

<span data-ttu-id="40e53-154">A transferência de clientes de SKUs reformados para os mais recentes requer os seguintes passos nesta ordem:</span><span class="sxs-lookup"><span data-stu-id="40e53-154">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="40e53-155">Comprar a nova subscrição</span><span class="sxs-lookup"><span data-stu-id="40e53-155">Purchase the new subscription</span></span>
- <span data-ttu-id="40e53-156">Reatribuir licenças de utilizador atuais</span><span class="sxs-lookup"><span data-stu-id="40e53-156">Reassign current user licenses</span></span>
- <span data-ttu-id="40e53-157">Cancelar subscrição antiga</span><span class="sxs-lookup"><span data-stu-id="40e53-157">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="40e53-158">Compre o novo plano para o seu cliente</span><span class="sxs-lookup"><span data-stu-id="40e53-158">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="40e53-159">Selecione **Clientes** a partir da navegação esquerda e, em seguida, selecione o cliente que pretende mover-se para a nova subscrição.</span><span class="sxs-lookup"><span data-stu-id="40e53-159">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="40e53-160">Selecione **Adicionar Subscrição** .</span><span class="sxs-lookup"><span data-stu-id="40e53-160">Select **Add Subscription** .</span></span>
3. <span data-ttu-id="40e53-161">Selecione a subscrição que pretende adquirir no catálogo (neste caso, uma das opções acima), introduza o número de licenças e, em seguida, **selecione Enviar por isso** .</span><span class="sxs-lookup"><span data-stu-id="40e53-161">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit** .</span></span> 

<span data-ttu-id="40e53-162">O seu cliente terá agora a subscrição antiga e a nova.</span><span class="sxs-lookup"><span data-stu-id="40e53-162">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="40e53-163">O seu próximo passo é reatribuir licenças aos utilizadores do cliente.</span><span class="sxs-lookup"><span data-stu-id="40e53-163">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="40e53-164">Selecione **clientes** a partir da navegação esquerda e, em seguida, selecione o cliente em que está a mover-se.</span><span class="sxs-lookup"><span data-stu-id="40e53-164">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="40e53-165">Selecione **Utilizadores e licenças.**</span><span class="sxs-lookup"><span data-stu-id="40e53-165">Select **Users and licenses** .</span></span>
3. <span data-ttu-id="40e53-166">Para reatribuir uma licença a um utilizador, selecione o utilizador e, em seguida, **selecione Gerir licenças** .</span><span class="sxs-lookup"><span data-stu-id="40e53-166">To reassign a license to a user, select the user and then select **Manage licenses** .</span></span> 
4. <span data-ttu-id="40e53-167">Na página **'Gerir licenças',** limpe a caixa de verificação da licença Dynamics 365 para Vendas/Cliente a partir da caixa de verificação de licença Básica (Oferta Qualificada) e selecione um novo plano de serviço para a subscrição para a qual o cliente está a mover-se.</span><span class="sxs-lookup"><span data-stu-id="40e53-167">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="40e53-168">Selecione **Submeter** .</span><span class="sxs-lookup"><span data-stu-id="40e53-168">Select **Submit** .</span></span> <span data-ttu-id="40e53-169">Fá-lo-ás por cada utilizador que precise da nova licença.</span><span class="sxs-lookup"><span data-stu-id="40e53-169">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="40e53-170">Uma vez transferidas as licenças para a nova subscrição, pode cancelar a subscrição antiga.</span><span class="sxs-lookup"><span data-stu-id="40e53-170">Once you've moved the licenses over to the new subscription you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="40e53-171">Selecione **clientes** a partir da navegação esquerda e, em seguida, selecione o cliente em que está a mover-se.</span><span class="sxs-lookup"><span data-stu-id="40e53-171">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="40e53-172">Na página de detalhes da subscrição, desafie a subscrição antiga para **Suspender** e selecione **Enviar** .</span><span class="sxs-lookup"><span data-stu-id="40e53-172">On the subscription detail page, set the old subscription to **Suspended** and select **Submit** .</span></span>

<span data-ttu-id="40e53-173">A subscrição antiga está agora suspensa e a nova subscrição está ativa.</span><span class="sxs-lookup"><span data-stu-id="40e53-173">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="40e53-174">A subscrição suspensa será desavisionada automaticamente após 120 dias.</span><span class="sxs-lookup"><span data-stu-id="40e53-174">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="40e53-175">O seu cliente não incorrerá em custos adicionais para a subscrição antiga.</span><span class="sxs-lookup"><span data-stu-id="40e53-175">Your customer will incur no additional costs for the old subscription.</span></span>
 

 



