---
title: Edição Empresarial Migrate Dynamics 365
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como migrar as ofertas qualificadas dynamics 365 Business Edition para versões mais recentes antes de expirarem.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e83c06c11638bdde508fd27904038bcb6d8c9e9c
ms.sourcegitcommit: f24089cd27b1de6ecf6ddbefb6cbb2d340e144de
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/01/2021
ms.locfileid: "106132643"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a><span data-ttu-id="3dae0-103">Migrate Dynamics 365 Business Edition Offers to newer versions (Migrar as Ofertas do Dynamics 365 Business Edition para versões mais recentes)</span><span class="sxs-lookup"><span data-stu-id="3dae0-103">Migrate Dynamics 365 Business Edition Offers to newer versions</span></span>

<span data-ttu-id="3dae0-104">**Funções adequadas**</span><span class="sxs-lookup"><span data-stu-id="3dae0-104">**Appropriate roles**</span></span>

- <span data-ttu-id="3dae0-105">Administrador global</span><span class="sxs-lookup"><span data-stu-id="3dae0-105">Global admin</span></span>
- <span data-ttu-id="3dae0-106">Administração de gestão de utilizadores</span><span class="sxs-lookup"><span data-stu-id="3dae0-106">User management admin</span></span>
- <span data-ttu-id="3dae0-107">Agente administrativo</span><span class="sxs-lookup"><span data-stu-id="3dae0-107">Admin agent</span></span>
- <span data-ttu-id="3dae0-108">Agente comercial</span><span class="sxs-lookup"><span data-stu-id="3dae0-108">Sales agent</span></span>

<span data-ttu-id="3dae0-109">A partir de 1 de janeiro de 2019, os clientes com subscrições da Dynamics 365 Business Edition já não podem renovar-se nestas ofertas antigas; as subscrições existentes não renovarão automaticamente quando expirarem.</span><span class="sxs-lookup"><span data-stu-id="3dae0-109">Effective January 1, 2019, customers with Dynamics 365 Business Edition subscriptions can no longer renew into these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="3dae0-110">Na página de pormenor da subscrição, o estado de subscrição mudará para "Expira na [data]" de "Renovações automáticas em [data]".</span><span class="sxs-lookup"><span data-stu-id="3dae0-110">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span>

<span data-ttu-id="3dae0-111">Para garantir a continuidade dos clientes, deve transitar aqueles com subscrições caducadas para uma opção suportada, listada abaixo.</span><span class="sxs-lookup"><span data-stu-id="3dae0-111">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="3dae0-112">Recomendamos que os clientes mudem os clientes para novas subscrições antes da data de fim anual da subscrição para evitar eventuais interrupções de serviço para os clientes.</span><span class="sxs-lookup"><span data-stu-id="3dae0-112">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="3dae0-113">Se utilizar a API (CREST ou Partner Center), pode encontrar subscrições caducadas avaliando a data final da subscrição juntamente com a renovação automática = Propriedade falsa.</span><span class="sxs-lookup"><span data-stu-id="3dae0-113">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="3dae0-114">As subscrições em questão serão definidas para renovação automática=Falsa a 1 de janeiro de 2019.</span><span class="sxs-lookup"><span data-stu-id="3dae0-114">The subscriptions in question will be set to auto renew=False on January 1, 2019.</span></span> <span data-ttu-id="3dae0-115">Pode mover os clientes para um novo plano a qualquer momento.</span><span class="sxs-lookup"><span data-stu-id="3dae0-115">You can move customers to a new plan at any time.</span></span> 

## <a name="the-dynamics-365-business-editions-being-retired"></a><span data-ttu-id="3dae0-116">As Dynamics 365 Business Editions estão a ser aposentadas</span><span class="sxs-lookup"><span data-stu-id="3dae0-116">The Dynamics 365 Business Editions being retired</span></span>

- <span data-ttu-id="3dae0-117">Dinâmica 365 para Finanças e Operações, Edição de Negócios</span><span class="sxs-lookup"><span data-stu-id="3dae0-117">Dynamics 365 for Finance and Operations, Business edition</span></span>
- <span data-ttu-id="3dae0-118">Dinâmica 365 para Membros da Equipa, Edição de Negócios</span><span class="sxs-lookup"><span data-stu-id="3dae0-118">Dynamics 365 for Team Members, Business edition</span></span>

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a><span data-ttu-id="3dae0-119">Dynamics Business Central - as novas ofertas da Dynamics 365 Business Edition</span><span class="sxs-lookup"><span data-stu-id="3dae0-119">Dynamics Business Central - the Dynamics 365 Business Edition new offers</span></span>

<span data-ttu-id="3dae0-120">Com as novas ofertas da Dynamics Business Central, os seus clientes podem ligar as suas finanças, vendas, serviços e operações para agilizar processos de negócio, melhorar as interações dos clientes e tomar melhores decisões.</span><span class="sxs-lookup"><span data-stu-id="3dae0-120">With the new Dynamics Business Central offers, your customers can connect their financials, sales, service, and operations to streamline business processes, improve customer interactions, and make better decisions.</span></span> <span data-ttu-id="3dae0-121">A Dynamics 365 Business Central é baseada na nuvem e está disponível apenas através de parceiros de programas Cloud Solution Provider (CSP).</span><span class="sxs-lookup"><span data-stu-id="3dae0-121">Dynamics 365 Business Central is cloud-based and available through Cloud Solution Provider (CSP) program partners only.</span></span>
<span data-ttu-id="3dae0-122">Os clientes da Dynamics 365 Business Edition podem receber preços de transição descontados para as novas ofertas da Business Central até 30 de junho de 2020.</span><span class="sxs-lookup"><span data-stu-id="3dae0-122">Dynamics 365 Business Edition customers are eligible to receive discounted transition pricing for the new Business Central offers until June 30, 2020.</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="3dae0-123">Transição de clientes para novos planos de produtos</span><span class="sxs-lookup"><span data-stu-id="3dae0-123">Transition customers to new product plans</span></span>

 <span data-ttu-id="3dae0-124">A transferência de clientes de SKUs reformados para os mais recentes requer os seguintes passos nesta ordem:</span><span class="sxs-lookup"><span data-stu-id="3dae0-124">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="3dae0-125">Comprar a nova subscrição</span><span class="sxs-lookup"><span data-stu-id="3dae0-125">Purchase the new subscription</span></span>
- <span data-ttu-id="3dae0-126">Reatribuir licenças de utilizador atuais</span><span class="sxs-lookup"><span data-stu-id="3dae0-126">Reassign current user licenses</span></span>
- <span data-ttu-id="3dae0-127">Cancelar subscrição antiga</span><span class="sxs-lookup"><span data-stu-id="3dae0-127">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="3dae0-128">Compre o novo plano para o seu cliente</span><span class="sxs-lookup"><span data-stu-id="3dae0-128">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="3dae0-129">Selecione **Clientes** a partir da navegação esquerda e, em seguida, selecione o cliente que pretende mover-se para a nova subscrição.</span><span class="sxs-lookup"><span data-stu-id="3dae0-129">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="3dae0-130">Selecione **Adicionar Subscrição**.</span><span class="sxs-lookup"><span data-stu-id="3dae0-130">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="3dae0-131">Selecione a subscrição que pretende adquirir no catálogo (neste caso, uma das opções acima), introduza o número de licenças e, em seguida, **selecione Enviar por isso**.</span><span class="sxs-lookup"><span data-stu-id="3dae0-131">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="3dae0-132">O seu cliente terá agora a subscrição antiga e a nova.</span><span class="sxs-lookup"><span data-stu-id="3dae0-132">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="3dae0-133">O seu próximo passo é reatribuir licenças aos utilizadores do cliente.</span><span class="sxs-lookup"><span data-stu-id="3dae0-133">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="3dae0-134">Selecione **clientes** a partir da navegação esquerda e, em seguida, selecione o cliente em que está a mover-se.</span><span class="sxs-lookup"><span data-stu-id="3dae0-134">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="3dae0-135">Selecione **Utilizadores e licenças.**</span><span class="sxs-lookup"><span data-stu-id="3dae0-135">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="3dae0-136">Para reatribuir uma licença a um utilizador, selecione o utilizador e, em seguida, **selecione Gerir licenças**.</span><span class="sxs-lookup"><span data-stu-id="3dae0-136">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="3dae0-137">Na página **'Gerir licenças',** limpe a caixa de verificação da licença Dynamics 365 para Vendas/Cliente a partir da caixa de verificação de licença Básica (Oferta Qualificada) e selecione um novo plano de serviço para a subscrição para a qual o cliente está a mover-se.</span><span class="sxs-lookup"><span data-stu-id="3dae0-137">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="3dae0-138">Selecione **Submeter**.</span><span class="sxs-lookup"><span data-stu-id="3dae0-138">Select **Submit**.</span></span> <span data-ttu-id="3dae0-139">Fá-lo-ás por cada utilizador que precise da nova licença.</span><span class="sxs-lookup"><span data-stu-id="3dae0-139">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="3dae0-140">Uma vez transferidas as licenças para a nova subscrição, pode cancelar a subscrição antiga.</span><span class="sxs-lookup"><span data-stu-id="3dae0-140">Once you've moved the licenses over to the new subscription, you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="3dae0-141">Selecione **clientes** a partir da navegação esquerda e, em seguida, selecione o cliente em que está a mover-se.</span><span class="sxs-lookup"><span data-stu-id="3dae0-141">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="3dae0-142">Na página de detalhes da subscrição, desafie a subscrição antiga para **Suspender** e selecione **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="3dae0-142">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="3dae0-143">A subscrição antiga está agora suspensa e a nova subscrição está ativa.</span><span class="sxs-lookup"><span data-stu-id="3dae0-143">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="3dae0-144">A subscrição suspensa será desavisionada automaticamente após 120 dias.</span><span class="sxs-lookup"><span data-stu-id="3dae0-144">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="3dae0-145">O seu cliente não incorrerá em custos adicionais para a subscrição antiga.</span><span class="sxs-lookup"><span data-stu-id="3dae0-145">Your customer will incur no additional costs for the old subscription.</span></span>
