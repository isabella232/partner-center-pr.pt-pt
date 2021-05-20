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
ms.openlocfilehash: b97cafea9ad2f36718418c7c7cfca5f91ee8849c
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149473"
---
# <a name="sell-microsoft-azure-reservations-to-customers-using-partner-center-the-azure-portal-or-apis"></a><span data-ttu-id="f51a4-104">Venda reservas do Microsoft Azure a clientes que usam Partner Center, o portal Azure ou APIs</span><span class="sxs-lookup"><span data-stu-id="f51a4-104">Sell Microsoft Azure reservations to customers using Partner Center, the Azure portal, or APIs</span></span>

<span data-ttu-id="f51a4-105">**Funções adequadas**: Agente administrador | Administração global | Agente helpdesk | Agente comercial | Administração de gestão de utilizadores</span><span class="sxs-lookup"><span data-stu-id="f51a4-105">**Appropriate roles**: Admin agent | Global admin | Helpdesk agent | Sales agent | User management admin</span></span>

<span data-ttu-id="f51a4-106">Como parceiro no programa Cloud Solution Provider (CSP), pode comprar, vender ou gerir reservas Azure para os clientes.</span><span class="sxs-lookup"><span data-stu-id="f51a4-106">As a partner in the Cloud Solution Provider program (CSP), you can buy, sell, or manage Azure reservations for customers.</span></span> <span data-ttu-id="f51a4-107">Use Partner Center, o portal Azure ou a API do Centro Parceiro.</span><span class="sxs-lookup"><span data-stu-id="f51a4-107">Use Partner Center, the Azure portal, or the Partner Center API.</span></span>

> [!NOTE]
> <span data-ttu-id="f51a4-108">Este artigo aplica-se apenas aos sócios da CSP.</span><span class="sxs-lookup"><span data-stu-id="f51a4-108">This article applies only to partners in CSP.</span></span> <span data-ttu-id="f51a4-109">Os clientes que utilizem outros tipos de subscrições (tais como, pay-as-you-go, individual, Microsoft Customer Agreement ou Enterprise Agreement) devem, em vez disso, ler [esta documentação de reservas Azure](/azure/cost-management-billing/reservations).</span><span class="sxs-lookup"><span data-stu-id="f51a4-109">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>

<span data-ttu-id="f51a4-110">Os parceiros do programa CSP podem oferecer reservas aos seus clientes Microsoft Azure.</span><span class="sxs-lookup"><span data-stu-id="f51a4-110">Partners in the CSP program can offer their customers Microsoft Azure reservations.</span></span> <span data-ttu-id="f51a4-111">Os clientes podem obter poupanças significativas quando reservam antecipadamente.</span><span class="sxs-lookup"><span data-stu-id="f51a4-111">Customers can gain significant savings when they reserve in advance.</span></span> <span data-ttu-id="f51a4-112">As reservas Azure oferecem aos clientes simplicidade e flexibilidade das seguintes formas:</span><span class="sxs-lookup"><span data-stu-id="f51a4-112">Azure reservations offer customers simplicity and flexibility in the following ways:</span></span>

- <span data-ttu-id="f51a4-113">Termos de reserva de um ou três anos</span><span class="sxs-lookup"><span data-stu-id="f51a4-113">One or three-year reservation terms</span></span>
- <span data-ttu-id="f51a4-114">Fácil de começar; configuração concluída em segundos</span><span class="sxs-lookup"><span data-stu-id="f51a4-114">Easy to get started; setup completed in seconds</span></span>
- <span data-ttu-id="f51a4-115">Cancelar ou trocar instâncias reservadas a qualquer momento para reembolso ajustado</span><span class="sxs-lookup"><span data-stu-id="f51a4-115">Cancel or exchange reserved instances at any time for adjusted refund</span></span>
- <span data-ttu-id="f51a4-116">Gerir o uso de instâncias reservadas a nível organizacional ou individual</span><span class="sxs-lookup"><span data-stu-id="f51a4-116">Manage reserved instances usage at the organizational or individual department level</span></span>

<span data-ttu-id="f51a4-117">As reservas da Azure podem apelar aos clientes das seguintes formas:</span><span class="sxs-lookup"><span data-stu-id="f51a4-117">Azure reservations can appeal to customers in the following ways:</span></span>

- <span data-ttu-id="f51a4-118">As reservas podem oferecer poupanças significativas em relação aos preços de pay-as-you-go (PAYG)</span><span class="sxs-lookup"><span data-stu-id="f51a4-118">Reservations can offer significant savings over pay-as-you-go (PAYG) pricing</span></span>
- <span data-ttu-id="f51a4-119">Melhor orçamentação e previsão com pagamento antecipado para prazos de um ano ou três anos</span><span class="sxs-lookup"><span data-stu-id="f51a4-119">Better budgeting and forecasting with upfront payment for one-year or three-year terms</span></span>
- <span data-ttu-id="f51a4-120">Capacidade de computação prioritária na região de Azure mais próxima dos seus escritórios</span><span class="sxs-lookup"><span data-stu-id="f51a4-120">Prioritized computing capacity in the Azure region closest to their offices</span></span>
- <span data-ttu-id="f51a4-121">As reservas do Azure fornecem as bases para soluções de infraestrutura final quando combinadas com software como o Microsoft Windows Server e a Azure SQL Database</span><span class="sxs-lookup"><span data-stu-id="f51a4-121">Azure reservations provide the foundation for end to end infrastructure solutions when combined with software like Microsoft Windows Server and Azure SQL Database</span></span>

>[!NOTE]
> <span data-ttu-id="f51a4-122">Você pode comprar, vender e gerir reservas Azure tanto no Centro de Parceiros como no portal Azure, e usando a API do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="f51a4-122">You can buy, sell, and manage Azure reservations in both the Partner Center and the Azure portal, and using the Partner Center API.</span></span> <span data-ttu-id="f51a4-123">Também pode dar permissão aos seus clientes para comprarem as suas próprias reservas Azure a partir de uma subscrição da Azure que adquiriu para eles.</span><span class="sxs-lookup"><span data-stu-id="f51a4-123">You can also give your customers permission to buy their own Azure reservations from an Azure subscription you purchased for them.</span></span> <span data-ttu-id="f51a4-124">Siga os links abaixo para saber como.</span><span class="sxs-lookup"><span data-stu-id="f51a4-124">Follow the links below to learn how.</span></span>

## <a name="azure-reservations-resources"></a><span data-ttu-id="f51a4-125">Recursos de reservas Azure</span><span class="sxs-lookup"><span data-stu-id="f51a4-125">Azure reservations resources</span></span>

|<span data-ttu-id="f51a4-126">**Para obter informações sobre**</span><span class="sxs-lookup"><span data-stu-id="f51a4-126">**For information about**</span></span>   |<span data-ttu-id="f51a4-127">**Leia isto**</span><span class="sxs-lookup"><span data-stu-id="f51a4-127">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
| <span data-ttu-id="f51a4-128">Documentação de reservas Azure para os seus clientes</span><span class="sxs-lookup"><span data-stu-id="f51a4-128">Azure reservations documentation for your customers</span></span> | [<span data-ttu-id="f51a4-129">O que são reservas do Azure?</span><span class="sxs-lookup"><span data-stu-id="f51a4-129">What are Azure reservations?</span></span>](/azure/billing/billing-save-compute-costs-reservations)
|<span data-ttu-id="f51a4-130">Comprar reservas da Azure para os seus clientes no Partner Center</span><span class="sxs-lookup"><span data-stu-id="f51a4-130">Purchasing Azure reservations for your customers in Partner Center</span></span>   |[<span data-ttu-id="f51a4-131">Comprar reservas Azure</span><span class="sxs-lookup"><span data-stu-id="f51a4-131">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="f51a4-132">Gerir reservas da Azure no Partner Center</span><span class="sxs-lookup"><span data-stu-id="f51a4-132">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="f51a4-133">Gerir reservas da Azure no Partner Center</span><span class="sxs-lookup"><span data-stu-id="f51a4-133">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="f51a4-134">Determinar o tamanho vm correto e verificar a utilização do VM do cliente</span><span class="sxs-lookup"><span data-stu-id="f51a4-134">Determining the correct VM size and verifying customer VM usage</span></span>   |[<span data-ttu-id="f51a4-135">Tamanho VM para o máximo uso da reserva Azure</span><span class="sxs-lookup"><span data-stu-id="f51a4-135">VM sizing for maximum Azure reservation usage</span></span>](azure-usage.md)   |
|<span data-ttu-id="f51a4-136">Compras Reservas Azure usando a API do Centro Parceiro</span><span class="sxs-lookup"><span data-stu-id="f51a4-136">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="f51a4-137">[Comprar Azure Reservado VM Instances](/partner-center/develop/purchase-azure-reservations) na documentação do desenvolvedor do Partner Center</span><span class="sxs-lookup"><span data-stu-id="f51a4-137">[Purchase Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="f51a4-138">Dando permissão aos clientes para comprarem as suas próprias reservas Azure a partir da sua assinatura CSP.</span><span class="sxs-lookup"><span data-stu-id="f51a4-138">Giving customers permission to buy their own Azure reservations from your CSP subscription.</span></span> | [<span data-ttu-id="f51a4-139">Dê permissão aos clientes para comprarem as suas próprias reservas Azure</span><span class="sxs-lookup"><span data-stu-id="f51a4-139">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |