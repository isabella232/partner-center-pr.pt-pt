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
ms.openlocfilehash: 8232ab165ea68ebefdfbb30f3ac52c907e1b7278
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151530"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a><span data-ttu-id="86c3f-103">Migrate Dynamics 365 Business Edition Offers to newer versions (Migrar as Ofertas do Dynamics 365 Business Edition para versões mais recentes)</span><span class="sxs-lookup"><span data-stu-id="86c3f-103">Migrate Dynamics 365 Business Edition Offers to newer versions</span></span>

<span data-ttu-id="86c3f-104">**Funções adequadas**: Administração global | Administração de administração de utilizadores | Agente administrativo | Agente comercial</span><span class="sxs-lookup"><span data-stu-id="86c3f-104">**Appropriate roles**: Global admin | User management admin | Admin agent | Sales agent</span></span>

<span data-ttu-id="86c3f-105">A partir de 1 de janeiro de 2019, os clientes com subscrições da Dynamics 365 Business Edition já não podem renovar-se nestas ofertas antigas; as subscrições existentes não renovarão automaticamente quando expirarem.</span><span class="sxs-lookup"><span data-stu-id="86c3f-105">Effective January 1, 2019, customers with Dynamics 365 Business Edition subscriptions can no longer renew into these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="86c3f-106">Na página de pormenor da subscrição, o estado de subscrição mudará para "Expira na [data]" de "Renovações automáticas em [data]".</span><span class="sxs-lookup"><span data-stu-id="86c3f-106">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span>

<span data-ttu-id="86c3f-107">Para garantir a continuidade dos clientes, deve transitar aqueles com subscrições caducadas para uma opção suportada, listada abaixo.</span><span class="sxs-lookup"><span data-stu-id="86c3f-107">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="86c3f-108">Recomendamos que os clientes mudem os clientes para novas subscrições antes da data de fim anual da subscrição para evitar eventuais interrupções de serviço para os clientes.</span><span class="sxs-lookup"><span data-stu-id="86c3f-108">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="86c3f-109">Se utilizar a API (CREST ou Partner Center), pode encontrar subscrições caducadas avaliando a data final da subscrição juntamente com a renovação automática = Propriedade falsa.</span><span class="sxs-lookup"><span data-stu-id="86c3f-109">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="86c3f-110">As subscrições em questão serão definidas para renovação automática=Falsa a 1 de janeiro de 2019.</span><span class="sxs-lookup"><span data-stu-id="86c3f-110">The subscriptions in question will be set to auto renew=False on January 1, 2019.</span></span> <span data-ttu-id="86c3f-111">Pode mover os clientes para um novo plano a qualquer momento.</span><span class="sxs-lookup"><span data-stu-id="86c3f-111">You can move customers to a new plan at any time.</span></span> 

## <a name="the-dynamics-365-business-editions-being-retired"></a><span data-ttu-id="86c3f-112">As Dynamics 365 Business Editions estão a ser aposentadas</span><span class="sxs-lookup"><span data-stu-id="86c3f-112">The Dynamics 365 Business Editions being retired</span></span>

- <span data-ttu-id="86c3f-113">Dinâmica 365 para Finanças e Operações, Edição de Negócios</span><span class="sxs-lookup"><span data-stu-id="86c3f-113">Dynamics 365 for Finance and Operations, Business edition</span></span>
- <span data-ttu-id="86c3f-114">Dinâmica 365 para Membros da Equipa, Edição de Negócios</span><span class="sxs-lookup"><span data-stu-id="86c3f-114">Dynamics 365 for Team Members, Business edition</span></span>

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a><span data-ttu-id="86c3f-115">Dynamics Business Central - as novas ofertas da Dynamics 365 Business Edition</span><span class="sxs-lookup"><span data-stu-id="86c3f-115">Dynamics Business Central - the Dynamics 365 Business Edition new offers</span></span>

<span data-ttu-id="86c3f-116">Com as novas ofertas da Dynamics Business Central, os seus clientes podem ligar as suas finanças, vendas, serviços e operações para agilizar processos de negócio, melhorar as interações dos clientes e tomar melhores decisões.</span><span class="sxs-lookup"><span data-stu-id="86c3f-116">With the new Dynamics Business Central offers, your customers can connect their financials, sales, service, and operations to streamline business processes, improve customer interactions, and make better decisions.</span></span> <span data-ttu-id="86c3f-117">A Dynamics 365 Business Central é baseada na nuvem e está disponível apenas através de parceiros de programas Cloud Solution Provider (CSP).</span><span class="sxs-lookup"><span data-stu-id="86c3f-117">Dynamics 365 Business Central is cloud-based and available through Cloud Solution Provider (CSP) program partners only.</span></span>
<span data-ttu-id="86c3f-118">Os clientes da Dynamics 365 Business Edition podem receber preços de transição descontados para as novas ofertas da Business Central até 30 de junho de 2020.</span><span class="sxs-lookup"><span data-stu-id="86c3f-118">Dynamics 365 Business Edition customers are eligible to receive discounted transition pricing for the new Business Central offers until June 30, 2020.</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="86c3f-119">Transição de clientes para novos planos de produtos</span><span class="sxs-lookup"><span data-stu-id="86c3f-119">Transition customers to new product plans</span></span>

 <span data-ttu-id="86c3f-120">A transferência de clientes de SKUs reformados para os mais recentes requer os seguintes passos nesta ordem:</span><span class="sxs-lookup"><span data-stu-id="86c3f-120">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="86c3f-121">Comprar a nova subscrição</span><span class="sxs-lookup"><span data-stu-id="86c3f-121">Purchase the new subscription</span></span>
- <span data-ttu-id="86c3f-122">Reatribuir licenças de utilizador atuais</span><span class="sxs-lookup"><span data-stu-id="86c3f-122">Reassign current user licenses</span></span>
- <span data-ttu-id="86c3f-123">Cancelar subscrição antiga</span><span class="sxs-lookup"><span data-stu-id="86c3f-123">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="86c3f-124">Compre o novo plano para o seu cliente</span><span class="sxs-lookup"><span data-stu-id="86c3f-124">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="86c3f-125">Selecione **Clientes** a partir da navegação esquerda e, em seguida, selecione o cliente que pretende mover-se para a nova subscrição.</span><span class="sxs-lookup"><span data-stu-id="86c3f-125">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="86c3f-126">Selecione **Adicionar Subscrição**.</span><span class="sxs-lookup"><span data-stu-id="86c3f-126">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="86c3f-127">Selecione a subscrição que pretende adquirir no catálogo (neste caso, uma das opções acima), introduza o número de licenças e, em seguida, **selecione Enviar por isso**.</span><span class="sxs-lookup"><span data-stu-id="86c3f-127">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="86c3f-128">O seu cliente terá agora a subscrição antiga e a nova.</span><span class="sxs-lookup"><span data-stu-id="86c3f-128">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="86c3f-129">O seu próximo passo é reatribuir licenças aos utilizadores do cliente.</span><span class="sxs-lookup"><span data-stu-id="86c3f-129">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="86c3f-130">Selecione **clientes** a partir da navegação esquerda e, em seguida, selecione o cliente em que está a mover-se.</span><span class="sxs-lookup"><span data-stu-id="86c3f-130">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="86c3f-131">Selecione **Utilizadores e licenças.**</span><span class="sxs-lookup"><span data-stu-id="86c3f-131">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="86c3f-132">Para reatribuir uma licença a um utilizador, selecione o utilizador e, em seguida, **selecione Gerir licenças**.</span><span class="sxs-lookup"><span data-stu-id="86c3f-132">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="86c3f-133">Na página **'Gerir licenças',** limpe a caixa de verificação da licença Dynamics 365 para Vendas/Cliente a partir da caixa de verificação de licença Básica (Oferta Qualificada) e selecione um novo plano de serviço para a subscrição para a qual o cliente está a mover-se.</span><span class="sxs-lookup"><span data-stu-id="86c3f-133">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="86c3f-134">Selecione **Submeter**.</span><span class="sxs-lookup"><span data-stu-id="86c3f-134">Select **Submit**.</span></span> <span data-ttu-id="86c3f-135">Fá-lo-ás por cada utilizador que precise da nova licença.</span><span class="sxs-lookup"><span data-stu-id="86c3f-135">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="86c3f-136">Uma vez transferidas as licenças para a nova subscrição, pode cancelar a subscrição antiga.</span><span class="sxs-lookup"><span data-stu-id="86c3f-136">Once you've moved the licenses over to the new subscription, you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="86c3f-137">Selecione **clientes** a partir da navegação esquerda e, em seguida, selecione o cliente em que está a mover-se.</span><span class="sxs-lookup"><span data-stu-id="86c3f-137">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="86c3f-138">Na página de detalhes da subscrição, desafie a subscrição antiga para **Suspender** e selecione **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="86c3f-138">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="86c3f-139">A subscrição antiga está agora suspensa e a nova subscrição está ativa.</span><span class="sxs-lookup"><span data-stu-id="86c3f-139">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="86c3f-140">A subscrição suspensa será desavisionada automaticamente após 120 dias.</span><span class="sxs-lookup"><span data-stu-id="86c3f-140">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="86c3f-141">O seu cliente não incorrerá em custos adicionais para a subscrição antiga.</span><span class="sxs-lookup"><span data-stu-id="86c3f-141">Your customer will incur no additional costs for the old subscription.</span></span>
