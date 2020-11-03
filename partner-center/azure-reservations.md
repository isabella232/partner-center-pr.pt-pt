---
title: Vender reservas microsoft Azure
description: Como Cloud Solution Provider, pode comprar, vender ou gerir reservas da Azure para os clientes. Use Partner Center, o portal Azure ou a API do Centro Parceiro.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 08/06/2020
ms.openlocfilehash: 317d1f0295b79b79bf06f1091ae365bc7012b749
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/22/2020
ms.locfileid: "92529912"
---
# <a name="sell-microsoft-azure-reservations-to-customers-using-partner-center-the-azure-portal-or-apis"></a><span data-ttu-id="9ac1b-104">Venda reservas do Microsoft Azure a clientes que usam Partner Center, o portal Azure ou APIs</span><span class="sxs-lookup"><span data-stu-id="9ac1b-104">Sell Microsoft Azure reservations to customers using Partner Center, the Azure portal, or APIs</span></span>

<span data-ttu-id="9ac1b-105">**Aplica-se a**</span><span class="sxs-lookup"><span data-stu-id="9ac1b-105">**Applies to**</span></span>

- <span data-ttu-id="9ac1b-106">Partner Center</span><span class="sxs-lookup"><span data-stu-id="9ac1b-106">Partner Center</span></span>
- <span data-ttu-id="9ac1b-107">Portal do Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="9ac1b-107">Microsoft Azure portal</span></span>
- <span data-ttu-id="9ac1b-108">Parceiros no programa CSP</span><span class="sxs-lookup"><span data-stu-id="9ac1b-108">Partners in the CSP program</span></span>

<span data-ttu-id="9ac1b-109">**Funções adequadas**</span><span class="sxs-lookup"><span data-stu-id="9ac1b-109">**Appropriate roles**</span></span>

- <span data-ttu-id="9ac1b-110">Agente administrativo</span><span class="sxs-lookup"><span data-stu-id="9ac1b-110">Admin agent</span></span>
- <span data-ttu-id="9ac1b-111">Administrador global</span><span class="sxs-lookup"><span data-stu-id="9ac1b-111">Global admin</span></span>
- <span data-ttu-id="9ac1b-112">Agente helpdesk</span><span class="sxs-lookup"><span data-stu-id="9ac1b-112">Helpdesk agent</span></span>
- <span data-ttu-id="9ac1b-113">Agente comercial</span><span class="sxs-lookup"><span data-stu-id="9ac1b-113">Sales agent</span></span>
- <span data-ttu-id="9ac1b-114">Administração de gestão de utilizadores</span><span class="sxs-lookup"><span data-stu-id="9ac1b-114">User management admin</span></span>

> [!NOTE]
> <span data-ttu-id="9ac1b-115">Este artigo aplica-se apenas aos parceiros do programa Cloud Solution Provider (CSP).</span><span class="sxs-lookup"><span data-stu-id="9ac1b-115">This article applies only to partners in the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="9ac1b-116">Os clientes que utilizem outros tipos de subscrições (tais como, pay-as-you-go, individual, Microsoft Customer Agreement ou Enterprise Agreement) devem, em vez disso, ler [esta documentação de reservas Azure](/azure/cost-management-billing/reservations).</span><span class="sxs-lookup"><span data-stu-id="9ac1b-116">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>

<span data-ttu-id="9ac1b-117">Os parceiros do programa CSP podem oferecer reservas aos seus clientes Microsoft Azure.</span><span class="sxs-lookup"><span data-stu-id="9ac1b-117">Partners in the CSP program can offer their customers Microsoft Azure reservations.</span></span> <span data-ttu-id="9ac1b-118">Os clientes podem obter poupanças significativas quando reservam antecipadamente.</span><span class="sxs-lookup"><span data-stu-id="9ac1b-118">Customers can gain significant savings when they reserve in advance.</span></span> <span data-ttu-id="9ac1b-119">As reservas Azure oferecem aos clientes simplicidade e flexibilidade das seguintes formas:</span><span class="sxs-lookup"><span data-stu-id="9ac1b-119">Azure reservations offer customers simplicity and flexibility in the following ways:</span></span>

- <span data-ttu-id="9ac1b-120">Termos de reserva de um ou três anos</span><span class="sxs-lookup"><span data-stu-id="9ac1b-120">One or three-year reservation terms</span></span>
- <span data-ttu-id="9ac1b-121">Fácil de começar; configuração concluída em segundos</span><span class="sxs-lookup"><span data-stu-id="9ac1b-121">Easy to get started; setup completed in seconds</span></span>
- <span data-ttu-id="9ac1b-122">Cancelar ou trocar instâncias reservadas a qualquer momento para reembolso ajustado</span><span class="sxs-lookup"><span data-stu-id="9ac1b-122">Cancel or exchange reserved instances at any time for adjusted refund</span></span>
- <span data-ttu-id="9ac1b-123">Gerir o uso de instâncias reservadas a nível organizacional ou individual</span><span class="sxs-lookup"><span data-stu-id="9ac1b-123">Manage reserved instances usage at the organizational or individual department level</span></span>

<span data-ttu-id="9ac1b-124">As reservas da Azure podem apelar aos clientes das seguintes formas:</span><span class="sxs-lookup"><span data-stu-id="9ac1b-124">Azure reservations can appeal to customers in the following ways:</span></span>

- <span data-ttu-id="9ac1b-125">As reservas podem oferecer poupanças significativas em relação aos preços de pay-as-you-go (PAYG)</span><span class="sxs-lookup"><span data-stu-id="9ac1b-125">Reservations can offer significant savings over pay-as-you-go (PAYG) pricing</span></span>
- <span data-ttu-id="9ac1b-126">Melhor orçamentação e previsão com pagamento antecipado para prazos de um ano ou três anos</span><span class="sxs-lookup"><span data-stu-id="9ac1b-126">Better budgeting and forecasting with upfront payment for one-year or three-year terms</span></span>
- <span data-ttu-id="9ac1b-127">Capacidade de computação prioritária na região de Azure mais próxima dos seus escritórios</span><span class="sxs-lookup"><span data-stu-id="9ac1b-127">Prioritized computing capacity in the Azure region closest to their offices</span></span>
- <span data-ttu-id="9ac1b-128">As reservas do Azure fornecem as bases para soluções de infraestrutura final quando combinadas com software como o Microsoft Windows Server e a Azure SQL Database</span><span class="sxs-lookup"><span data-stu-id="9ac1b-128">Azure reservations provide the foundation for end to end infrastructure solutions when combined with software like Microsoft Windows Server and Azure SQL Database</span></span>

>[!NOTE]
> <span data-ttu-id="9ac1b-129">Você pode comprar, vender e gerir reservas Azure tanto no Centro de Parceiros como no portal Azure, e usando a API do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="9ac1b-129">You can buy, sell, and manage Azure reservations in both the Partner Center and the Azure portal, and using the Partner Center API.</span></span> <span data-ttu-id="9ac1b-130">Também pode dar permissão aos seus clientes para comprarem as suas próprias reservas Azure a partir de uma subscrição da Azure que adquiriu para eles.</span><span class="sxs-lookup"><span data-stu-id="9ac1b-130">You can also give your customers permission to buy their own Azure reservations from an Azure subscription you purchased for them.</span></span> <span data-ttu-id="9ac1b-131">Siga os links abaixo para saber como.</span><span class="sxs-lookup"><span data-stu-id="9ac1b-131">Follow the links below to learn how.</span></span>

## <a name="azure-reservations-resources"></a><span data-ttu-id="9ac1b-132">Recursos de reservas Azure</span><span class="sxs-lookup"><span data-stu-id="9ac1b-132">Azure reservations resources</span></span>

|<span data-ttu-id="9ac1b-133">**Para obter informações sobre**</span><span class="sxs-lookup"><span data-stu-id="9ac1b-133">**For information about**</span></span>   |<span data-ttu-id="9ac1b-134">**Leia isto**</span><span class="sxs-lookup"><span data-stu-id="9ac1b-134">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
| <span data-ttu-id="9ac1b-135">Documentação de reservas Azure para os seus clientes</span><span class="sxs-lookup"><span data-stu-id="9ac1b-135">Azure reservations documentation for your customers</span></span> | [<span data-ttu-id="9ac1b-136">O que são reservas do Azure?</span><span class="sxs-lookup"><span data-stu-id="9ac1b-136">What are Azure reservations?</span></span>](/azure/billing/billing-save-compute-costs-reservations)
|<span data-ttu-id="9ac1b-137">Comprar reservas da Azure para os seus clientes no Partner Center</span><span class="sxs-lookup"><span data-stu-id="9ac1b-137">Purchasing Azure reservations for your customers in Partner Center</span></span>   |[<span data-ttu-id="9ac1b-138">Comprar reservas Azure</span><span class="sxs-lookup"><span data-stu-id="9ac1b-138">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="9ac1b-139">Gerir reservas da Azure no Partner Center</span><span class="sxs-lookup"><span data-stu-id="9ac1b-139">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="9ac1b-140">Gerir reservas da Azure no Partner Center</span><span class="sxs-lookup"><span data-stu-id="9ac1b-140">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="9ac1b-141">Determinar o tamanho vm correto e verificar a utilização do VM do cliente</span><span class="sxs-lookup"><span data-stu-id="9ac1b-141">Determining the correct VM size and verifying customer VM usage</span></span>   |[<span data-ttu-id="9ac1b-142">Tamanho VM para o máximo uso da reserva Azure</span><span class="sxs-lookup"><span data-stu-id="9ac1b-142">VM sizing for maximum Azure reservation usage</span></span>](azure-usage.md)   |
|<span data-ttu-id="9ac1b-143">Compras Reservas Azure usando a API do Centro Parceiro</span><span class="sxs-lookup"><span data-stu-id="9ac1b-143">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="9ac1b-144">[Comprar Azure Reservado VM Instances](/partner-center/develop/purchase-azure-reservations) na documentação do desenvolvedor do Partner Center</span><span class="sxs-lookup"><span data-stu-id="9ac1b-144">[Purchase Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="9ac1b-145">Dando permissão aos clientes para comprarem as suas próprias reservas Azure a partir da sua assinatura CSP.</span><span class="sxs-lookup"><span data-stu-id="9ac1b-145">Giving customers permission to buy their own Azure reservations from your CSP subscription.</span></span> | [<span data-ttu-id="9ac1b-146">Dê permissão aos clientes para comprarem as suas próprias reservas Azure</span><span class="sxs-lookup"><span data-stu-id="9ac1b-146">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |