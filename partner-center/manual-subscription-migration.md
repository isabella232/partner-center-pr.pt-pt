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
ms.openlocfilehash: 363c97b8c2b62e8d6b62cbe3b2807fb3c0ef3e38
ms.sourcegitcommit: f24089cd27b1de6ecf6ddbefb6cbb2d340e144de
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/01/2021
ms.locfileid: "106132745"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a><span data-ttu-id="04d60-103">Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions (Migrar o Dynamics 365 e o Customer Engagement Plan da versão Básica (ofertas qualificadas) para versões mais recentes)</span><span class="sxs-lookup"><span data-stu-id="04d60-103">Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions</span></span>

<span data-ttu-id="04d60-104">**Funções adequadas**</span><span class="sxs-lookup"><span data-stu-id="04d60-104">**Appropriate roles**</span></span>

- <span data-ttu-id="04d60-105">Administrador global</span><span class="sxs-lookup"><span data-stu-id="04d60-105">Global admin</span></span>
- <span data-ttu-id="04d60-106">Administração de gestão de utilizadores</span><span class="sxs-lookup"><span data-stu-id="04d60-106">User management admin</span></span>
- <span data-ttu-id="04d60-107">Agente administrativo</span><span class="sxs-lookup"><span data-stu-id="04d60-107">Admin agent</span></span>
- <span data-ttu-id="04d60-108">Agente comercial</span><span class="sxs-lookup"><span data-stu-id="04d60-108">Sales agent</span></span>

<span data-ttu-id="04d60-109">A partir de 1 de janeiro de 2019, os clientes com Dinâmica 365 para Vendas/Plano de Envolvimento com o Cliente a partir de assinaturas Básicas (Ofertas Qualificadas) já não podem renovar estas ofertas antigas; as subscrições existentes não renovarão automaticamente quando expirarem.</span><span class="sxs-lookup"><span data-stu-id="04d60-109">Effective January 1, 2019, customers with Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) subscriptions can no longer renew these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="04d60-110">Na página de pormenor da subscrição, o estado de subscrição mudará para "Expira na [data]" de "Renovações automáticas em [data]".</span><span class="sxs-lookup"><span data-stu-id="04d60-110">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="04d60-111">Para garantir a continuidade dos clientes, deve transitar aqueles com subscrições caducadas para uma opção suportada, listada abaixo.</span><span class="sxs-lookup"><span data-stu-id="04d60-111">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="04d60-112">Recomendamos que os clientes mudem os clientes para novas subscrições antes da data de fim anual da subscrição para evitar eventuais interrupções de serviço para os clientes.</span><span class="sxs-lookup"><span data-stu-id="04d60-112">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="04d60-113">Se utilizar a API (CREST ou Partner Center), pode encontrar subscrições caducadas avaliando a data final da subscrição juntamente com a renovação automática = Propriedade falsa.</span><span class="sxs-lookup"><span data-stu-id="04d60-113">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="04d60-114">As subscrições em questão serão definidas para renovação automática=Falsa a 1 de janeiro de 2019.</span><span class="sxs-lookup"><span data-stu-id="04d60-114">The subscriptions in question will be set to auto renew=False on January 1, 2019.</span></span> <span data-ttu-id="04d60-115">Pode mover os clientes para um novo plano a qualquer momento.</span><span class="sxs-lookup"><span data-stu-id="04d60-115">You can move customers to a new plan at any time.</span></span> 

### <a name="the-dynamics-365-offers-being-retired"></a><span data-ttu-id="04d60-116">A Dynamics 365 oferece a reforma</span><span class="sxs-lookup"><span data-stu-id="04d60-116">The Dynamics 365 offers being retired</span></span>

- <span data-ttu-id="04d60-117">Dinâmica 365 para Venda Enterprise Edition CRMOL Basic (Oferta Qualificada)</span><span class="sxs-lookup"><span data-stu-id="04d60-117">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="04d60-118">Dinâmica 365 para Venda Enterprise Edition CRMOL Basic (Oferta Qualificada) para Faculdade</span><span class="sxs-lookup"><span data-stu-id="04d60-118">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="04d60-119">Dinâmica 365 para Sales Enterprise Edition CRMOL Basic (Oferta Qualificada) para Estudantes</span><span class="sxs-lookup"><span data-stu-id="04d60-119">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="04d60-120">Dinâmica 365 para Venda Enterprise Edition (Preço do Governo) CRMOL Basic (Oferta Qualificada)</span><span class="sxs-lookup"><span data-stu-id="04d60-120">Dynamics 365 for Sales Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="04d60-121">Dinâmica 365 para Venda Enterprise Edition Da SA para CRM Basic (Oferta Qualificada)</span><span class="sxs-lookup"><span data-stu-id="04d60-121">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="04d60-122">Dinâmica 365 para Venda Enterprise Edition From SA for CRM Basic (Oferta Qualificada) para Faculdade</span><span class="sxs-lookup"><span data-stu-id="04d60-122">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="04d60-123">Dinâmica 365 para Venda Enterprise Edition From SA for CRM Basic (Oferta Qualificada) para Estudantes</span><span class="sxs-lookup"><span data-stu-id="04d60-123">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="04d60-124">Dinâmica 365 para Venda Enterprise Edition (Preço do Governo) A partir de SA para CRM Basic (Oferta Qualificada)</span><span class="sxs-lookup"><span data-stu-id="04d60-124">Dynamics 365 for Sales Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="04d60-125">Dinâmica 365 para Venda Enterprise Edition Add-On para CRM Basic (Oferta Qualificada)</span><span class="sxs-lookup"><span data-stu-id="04d60-125">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="04d60-126">Dinâmica 365 para Venda Enterprise Edition Add-On para CRM Basic (Oferta Qualificada) para Faculdade</span><span class="sxs-lookup"><span data-stu-id="04d60-126">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="04d60-127">Dinâmica 365 para Venda Enterprise Edition Add-On para CRM Basic (Oferta Qualificada) para Estudantes</span><span class="sxs-lookup"><span data-stu-id="04d60-127">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="04d60-128">Dinâmica 365 para Venda Enterprise Edition (Preço do Governo) Add-On para CRM Basic (Oferta Qualificada)</span><span class="sxs-lookup"><span data-stu-id="04d60-128">Dynamics 365 for Sales Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="04d60-129">Dinâmica 365 Plano de Envolvimento com o Cliente Enterprise Edition CRMOL Basic (Oferta Qualificada)</span><span class="sxs-lookup"><span data-stu-id="04d60-129">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="04d60-130">Dinâmica 365 Plano de Envolvimento com o Cliente Enterprise Edition (Preço do Governo) CRMOL Basic (Oferta Qualificada)</span><span class="sxs-lookup"><span data-stu-id="04d60-130">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="04d60-131">Dinâmica 365 Plano de Envolvimento com o Cliente Enterprise Edition CRMOL Basic (Oferta Qualificada) para Estudantes</span><span class="sxs-lookup"><span data-stu-id="04d60-131">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="04d60-132">Dinâmica 365 Plano de Envolvimento com o Cliente Enterprise Edition CRMOL Basic (Oferta Qualificada) para Faculdade</span><span class="sxs-lookup"><span data-stu-id="04d60-132">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="04d60-133">Dinâmica 365 Plano de Envolvimento com o Cliente Edição Empresarial da SA para CRM Basic (Oferta Qualificada)</span><span class="sxs-lookup"><span data-stu-id="04d60-133">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="04d60-134">Dinâmica 365 Plano de Envolvimento com o Cliente Enterprise Edition (Preço do Governo) A partir de SA para CRM Basic (Oferta Qualificada)</span><span class="sxs-lookup"><span data-stu-id="04d60-134">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="04d60-135">Dinâmica 365 Plano de Envolvimento com o Cliente Edição Empresarial da SA para CRM Basic (Oferta Qualificada) para Estudantes</span><span class="sxs-lookup"><span data-stu-id="04d60-135">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="04d60-136">Dinâmica 365 Plano de Envolvimento com o Cliente Edição Empresarial da SA para CRM Basic (Oferta Qualificada) para Faculdade</span><span class="sxs-lookup"><span data-stu-id="04d60-136">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="04d60-137">Dinâmica 365 Plano de Envolvimento com o Cliente Enterprise Edition Add-On para CRM Basic (Oferta Qualificada)</span><span class="sxs-lookup"><span data-stu-id="04d60-137">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="04d60-138">Dinâmica 365 Plano de Envolvimento com o Cliente Enterprise Edition (Preço do Governo) Add-On para CRM Basic (Oferta Qualificada)</span><span class="sxs-lookup"><span data-stu-id="04d60-138">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="04d60-139">Dinâmica 365 Plano de Envolvimento com o Cliente Enterprise Edition Add-On para CRM Basic (Oferta Qualificada) para Estudantes</span><span class="sxs-lookup"><span data-stu-id="04d60-139">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="04d60-140">Dinâmica 365 Plano de Envolvimento com o Cliente Enterprise Edition Add-On para CRM Basic (Oferta Qualificada) para Faculdade</span><span class="sxs-lookup"><span data-stu-id="04d60-140">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a><span data-ttu-id="04d60-141">Dinâmica 365 para Plano de Venda/Envolvimento do Cliente a partir de planos básicos de substituição (Ofertas Qualificadas)</span><span class="sxs-lookup"><span data-stu-id="04d60-141">Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) replacement plans</span></span>

<span data-ttu-id="04d60-142">**Ofertas aposentadas**</span><span class="sxs-lookup"><span data-stu-id="04d60-142">**Retired offers**</span></span>   

- <span data-ttu-id="04d60-143">Dinâmica 365 para Vendas da CRM Basic ou CRMOL Basic (Oferta Qualificada)</span><span class="sxs-lookup"><span data-stu-id="04d60-143">Dynamics 365 for Sales from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="04d60-144">Dinâmica 365 Plano de Envolvimento do Cliente da CRM Basic ou CRMOL Basic (Oferta Qualificada)</span><span class="sxs-lookup"><span data-stu-id="04d60-144">Dynamics 365 Customer Engagement Plan from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>

<span data-ttu-id="04d60-145">**Opções de substituição**</span><span class="sxs-lookup"><span data-stu-id="04d60-145">**Replacement options**</span></span>
- <span data-ttu-id="04d60-146">Dinâmica 365 para Profissional de Vendas (NOVO)</span><span class="sxs-lookup"><span data-stu-id="04d60-146">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="04d60-147">Dinâmica 365 para Profissional de Vendas (NOVO)</span><span class="sxs-lookup"><span data-stu-id="04d60-147">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="04d60-148">Dynamics 365 for Customer Service</span><span class="sxs-lookup"><span data-stu-id="04d60-148">Dynamics 365 for Customer Service</span></span>
- <span data-ttu-id="04d60-149">Dinâmica 365 Plano de Envolvimento do Cliente ou</span><span class="sxs-lookup"><span data-stu-id="04d60-149">Dynamics 365 Customer Engagement Plan or</span></span>
- <span data-ttu-id="04d60-150">Dinâmica 365 Membros da equipa</span><span class="sxs-lookup"><span data-stu-id="04d60-150">Dynamics 365 Team Members</span></span>



## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="04d60-151">Transição de clientes para novos planos de produtos</span><span class="sxs-lookup"><span data-stu-id="04d60-151">Transition customers to new product plans</span></span>

<span data-ttu-id="04d60-152">A transferência de clientes de SKUs reformados para os mais recentes requer os seguintes passos nesta ordem:</span><span class="sxs-lookup"><span data-stu-id="04d60-152">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="04d60-153">Comprar a nova subscrição</span><span class="sxs-lookup"><span data-stu-id="04d60-153">Purchase the new subscription</span></span>
- <span data-ttu-id="04d60-154">Reatribuir licenças de utilizador atuais</span><span class="sxs-lookup"><span data-stu-id="04d60-154">Reassign current user licenses</span></span>
- <span data-ttu-id="04d60-155">Cancelar subscrição antiga</span><span class="sxs-lookup"><span data-stu-id="04d60-155">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="04d60-156">Compre o novo plano para o seu cliente</span><span class="sxs-lookup"><span data-stu-id="04d60-156">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="04d60-157">Selecione **Clientes** a partir da navegação esquerda e, em seguida, selecione o cliente que pretende mover-se para a nova subscrição.</span><span class="sxs-lookup"><span data-stu-id="04d60-157">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="04d60-158">Selecione **Adicionar Subscrição**.</span><span class="sxs-lookup"><span data-stu-id="04d60-158">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="04d60-159">Selecione a subscrição que pretende adquirir no catálogo (neste caso, uma das opções acima), introduza o número de licenças e, em seguida, **selecione Enviar por isso**.</span><span class="sxs-lookup"><span data-stu-id="04d60-159">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="04d60-160">O seu cliente terá agora a subscrição antiga e a nova.</span><span class="sxs-lookup"><span data-stu-id="04d60-160">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="04d60-161">O seu próximo passo é reatribuir licenças aos utilizadores do cliente.</span><span class="sxs-lookup"><span data-stu-id="04d60-161">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="04d60-162">Selecione **clientes** a partir da navegação esquerda e, em seguida, selecione o cliente em que está a mover-se.</span><span class="sxs-lookup"><span data-stu-id="04d60-162">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="04d60-163">Selecione **Utilizadores e licenças.**</span><span class="sxs-lookup"><span data-stu-id="04d60-163">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="04d60-164">Para reatribuir uma licença a um utilizador, selecione o utilizador e, em seguida, **selecione Gerir licenças**.</span><span class="sxs-lookup"><span data-stu-id="04d60-164">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="04d60-165">Na página **'Gerir licenças',** limpe a caixa de verificação da licença Dynamics 365 para Vendas/Cliente a partir da caixa de verificação de licença Básica (Oferta Qualificada) e selecione um novo plano de serviço para a subscrição para a qual o cliente está a mover-se.</span><span class="sxs-lookup"><span data-stu-id="04d60-165">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="04d60-166">Selecione **Submeter**.</span><span class="sxs-lookup"><span data-stu-id="04d60-166">Select **Submit**.</span></span> <span data-ttu-id="04d60-167">Fá-lo-ás por cada utilizador que precise da nova licença.</span><span class="sxs-lookup"><span data-stu-id="04d60-167">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="04d60-168">Uma vez transferidas as licenças para a nova subscrição, pode cancelar a subscrição antiga.</span><span class="sxs-lookup"><span data-stu-id="04d60-168">Once you've moved the licenses over to the new subscription, you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="04d60-169">Selecione **clientes** a partir da navegação esquerda e, em seguida, selecione o cliente em que está a mover-se.</span><span class="sxs-lookup"><span data-stu-id="04d60-169">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="04d60-170">Na página de detalhes da subscrição, desafie a subscrição antiga para **Suspender** e selecione **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="04d60-170">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="04d60-171">A subscrição antiga está agora suspensa e a nova subscrição está ativa.</span><span class="sxs-lookup"><span data-stu-id="04d60-171">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="04d60-172">A subscrição suspensa será desavisionada automaticamente após 120 dias.</span><span class="sxs-lookup"><span data-stu-id="04d60-172">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="04d60-173">O seu cliente não incorrerá em custos adicionais para a subscrição antiga.</span><span class="sxs-lookup"><span data-stu-id="04d60-173">Your customer will incur no additional costs for the old subscription.</span></span>
 

 



