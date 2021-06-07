---
title: Ofertas privadas no Azure Marketplace
description: Conheça as ofertas privadas no Azure Marketplace.
ms.service: marketplace-customer
ms.topic: article
author: Guyshu
ms.author: gushuchm
ms.date: 06/03/2021
ms.openlocfilehash: 55d0716b183e9e8905e631447e547396d6f55404
ms.sourcegitcommit: 9cb6bc9df20540f812b7932f88e520976c1aa85a
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/06/2021
ms.locfileid: "111534162"
---
# <a name="private-plans-in-azure-marketplace"></a><span data-ttu-id="bc31d-103">Planos privados no Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="bc31d-103">Private plans in Azure Marketplace</span></span>

<span data-ttu-id="bc31d-104">Os planos privados são como os editores fornecem planos personalizados a clientes específicos.</span><span class="sxs-lookup"><span data-stu-id="bc31d-104">Private plans are how publishers provide custom plans to specific customers.</span></span> <span data-ttu-id="bc31d-105">Os planos privados só estão disponíveis para ofertas pagas que podem ser compradas e instaladas diretamente a partir do portal Azure.</span><span class="sxs-lookup"><span data-stu-id="bc31d-105">Private plans are only available for paid offers that can be purchased and directly installed from the Azure portal.</span></span> <span data-ttu-id="bc31d-106">Os editores não podem criar planos privados para serviços de consultoria, qualquer serviço que **tenha contacte-me** como uma chamada à ação, ou qualquer serviço gratuito, independentemente de poder ou não ser instalado a partir do portal.</span><span class="sxs-lookup"><span data-stu-id="bc31d-106">Publishers cannot create private plans for consulting services, any service that has **Contact me** as a call-to-action, or any free service, regardless of whether it can be installed from the portal or not.</span></span>

## <a name="find-private-plans-in-the-azure-portal"></a><span data-ttu-id="bc31d-107">Encontre planos privados no portal Azure</span><span class="sxs-lookup"><span data-stu-id="bc31d-107">Find private plans in the Azure portal</span></span>

<span data-ttu-id="bc31d-108">Quando um parceiro publica um plano privado, é visível apenas para utilizadores elegíveis na secção **Marketplace** do portal Azure.</span><span class="sxs-lookup"><span data-stu-id="bc31d-108">When a partner publishes a private plan, it is visible only to eligible users in the **Marketplace** section of the Azure portal.</span></span> <span data-ttu-id="bc31d-109">Estes utilizadores são definidos por ID de subscrição ou ID do inquilino, dependendo do tipo de oferta.</span><span class="sxs-lookup"><span data-stu-id="bc31d-109">These users are defined by subscription ID or tenant ID, depending on the offer type.</span></span> <span data-ttu-id="bc31d-110">Se você é elegível para planos privados, há duas maneiras de encontrá-los no portal.</span><span class="sxs-lookup"><span data-stu-id="bc31d-110">If you are eligible for private plans, there are two ways to find them in the portal.</span></span>

> [!NOTE]
> <span data-ttu-id="bc31d-111">Os planos privados são pescáveis mas não filtram (por categoria) no portal Azure.</span><span class="sxs-lookup"><span data-stu-id="bc31d-111">Private plans are searchable but not filterable (by category) in the Azure portal.</span></span>

<span data-ttu-id="bc31d-112">No portal Azure, selecione **+ Crie um recurso** ou procure por "marketplace" para ir à página do **Marketplace.**</span><span class="sxs-lookup"><span data-stu-id="bc31d-112">In the Azure portal, select **+ Create a resource** or search for “marketplace” to go to the **Marketplace** page.</span></span> <span data-ttu-id="bc31d-113">Se você é elegível para planos privados, você verá o **Você tem planos privados disponíveis** banner no topo da página.</span><span class="sxs-lookup"><span data-stu-id="bc31d-113">If you are eligible for private plans, you will see the **You have private plans available** banner on the top of the page.</span></span> <span data-ttu-id="bc31d-114">**Selecione Ver ofertas privadas + planeia** ir para a página de planos privados.</span><span class="sxs-lookup"><span data-stu-id="bc31d-114">Select **View private offers + plans** to go to your private plans page.</span></span>

:::image type="content" source="media/private-offers/private-offers-banner.png" alt-text="O banner que exibe quando tem planos privados disponíveis.":::

## <a name="review-private-plans"></a><span data-ttu-id="bc31d-116">Rever planos privados</span><span class="sxs-lookup"><span data-stu-id="bc31d-116">Review private plans</span></span>

<span data-ttu-id="bc31d-117">Um plano privado faz parte de vários planos numa oferta.</span><span class="sxs-lookup"><span data-stu-id="bc31d-117">A private plan is part of several plans in an offer.</span></span> <span data-ttu-id="bc31d-118">Cada oferta pode ter múltiplos planos, tanto públicos como privados, mas os planos privados são mostrados sob uma lista geminada separada dos planos públicos.</span><span class="sxs-lookup"><span data-stu-id="bc31d-118">Each offer can have multiple plans, both public and private, but private plans are shown under a separate listing from public plans.</span></span>

<span data-ttu-id="bc31d-119">Pode ver os planos privados disponíveis no **separador Planos,** marcado com um distintivo **privado** distinto:</span><span class="sxs-lookup"><span data-stu-id="bc31d-119">You can see the available private plans under the **Plans** tab, marked with a distinctive **Private** badge:</span></span>

:::image type="content" source="media/private-offers/private-badge.png" alt-text="Uma página de planos marcados como Privado.":::

<span data-ttu-id="bc31d-121">Se tiver mais de uma subscrição, verá todos os planos privados disponíveis para todas as suas subscrições.</span><span class="sxs-lookup"><span data-stu-id="bc31d-121">If you have more than one subscription, you will see all private plans available for all your subscriptions.</span></span> <span data-ttu-id="bc31d-122">Quando seleciona **Criar,** é encaminhado para a página de criação de recursos para começar a configurar o seu recurso.</span><span class="sxs-lookup"><span data-stu-id="bc31d-122">When you select **Create**, you are routed to the resource creation page to start configuring your resource.</span></span>

<span data-ttu-id="bc31d-123">Se selecionar **Criar** e tiver várias subscrições, mas nem todas são adicionadas ao plano privado, a sua subscrição por defeito pode não ser a subscrição elegível para este plano privado.</span><span class="sxs-lookup"><span data-stu-id="bc31d-123">If you select **Create** and have multiple subscriptions, but not all of them are added to the private plan, your default subscription may not be the subscription eligible for this private plan.</span></span> <span data-ttu-id="bc31d-124">Neste caso, selecione a subscrição correta.</span><span class="sxs-lookup"><span data-stu-id="bc31d-124">In this case, select the correct subscription.</span></span>

:::image type="content" source="media/private-offers/select-correct-subscription.png" alt-text="O link que mostra que há mais planos privados disponíveis.":::

## <a name="next-steps"></a><span data-ttu-id="bc31d-126">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="bc31d-126">Next steps</span></span>

- [<span data-ttu-id="bc31d-127">O que é o Azure Marketplace?</span><span class="sxs-lookup"><span data-stu-id="bc31d-127">What is Azure Marketplace?</span></span>](azure-marketplace-overview.md)
