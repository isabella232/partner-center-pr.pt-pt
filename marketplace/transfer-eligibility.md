---
title: Elegibilidade de transferência – Orientações para a transferência de uma subscrição entre contas de faturação, Azure Marketplace
description: Diretrizes para verificações comerciais antes de transferir uma subscrição entre contas de faturação no portal Azure.
ms.service: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 11/20/2020
ms.openlocfilehash: 4b235bd462915fc205813ae86e92f98b4fd49fe4
ms.sourcegitcommit: 3a2415ab9833d5c574ad76d462f526a131c24f33
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/12/2021
ms.locfileid: "103412561"
---
# <a name="transfer-eligibility-for-a-subscription-between-billing-accounts"></a><span data-ttu-id="dacaa-103">Elegibilidade de transferência para uma subscrição entre contas de faturação</span><span class="sxs-lookup"><span data-stu-id="dacaa-103">Transfer eligibility for a subscription between billing accounts</span></span>

<span data-ttu-id="dacaa-104">Pode [transferir uma subscrição](/azure/cost-management-billing/understand/subscription-transfer) de uma conta de faturação para outra na secção de faturação do portal Azure.</span><span class="sxs-lookup"><span data-stu-id="dacaa-104">You can [transfer a subscription](/azure/cost-management-billing/understand/subscription-transfer) from one billing account to another in the billing section of the Azure portal.</span></span> <span data-ttu-id="dacaa-105">Antes de uma transferência, a subscrição é digitalizada para produtos de terceiros.</span><span class="sxs-lookup"><span data-stu-id="dacaa-105">Prior to a transfer, the subscription is scanned for third-party products.</span></span> <span data-ttu-id="dacaa-106">A transferência só é permitida se *todos os* produtos forem autorizados para transferência (ver [os critérios](#criteria-for-transfer-approval-or-denial) abaixo).</span><span class="sxs-lookup"><span data-stu-id="dacaa-106">The transfer is permitted only if *all* products are cleared for transfer (see the [criteria](#criteria-for-transfer-approval-or-denial) below).</span></span> <span data-ttu-id="dacaa-107">O sistema irá gerar mensagens de erro relevantes para as aplicações que não conseguiram limpar para o ajudar a determinar os próximos passos.</span><span class="sxs-lookup"><span data-stu-id="dacaa-107">The system will generate relevant error messages for the apps that failed to clear to help you determine next steps.</span></span>

> [!NOTE]
> <span data-ttu-id="dacaa-108">Este artigo não se aplica às ofertas do SaaS porque os recursos do SaaS estão ligados a um inquilino, e não a uma subscrição.</span><span class="sxs-lookup"><span data-stu-id="dacaa-108">This article does not apply to SaaS offers because SaaS resources are attached to a tenant, not a subscription.</span></span> <span data-ttu-id="dacaa-109">Os recursos do SAAS são transferíveis de uma conta de faturação para outra, mas isso é feito por recurso e pelo apoio da Azure como um pedido de apoio.</span><span class="sxs-lookup"><span data-stu-id="dacaa-109">SaaS resources are transferable from one billing account to another, but this is done per resource and by Azure support as a support request.</span></span>

## <a name="criteria-for-transfer-approval-or-denial"></a><span data-ttu-id="dacaa-110">Critérios para aprovação de transferência ou negação</span><span class="sxs-lookup"><span data-stu-id="dacaa-110">Criteria for transfer approval or denial</span></span>

<span data-ttu-id="dacaa-111">Não é possível transferir uma subscrição se alguma das suas aplicações de terceiros cumprir qualquer um dos seguintes critérios:</span><span class="sxs-lookup"><span data-stu-id="dacaa-111">You cannot transfer a subscription if any of its third-party apps meet any of the following criteria:</span></span>

- <span data-ttu-id="dacaa-112">A conta-alvo é comercial e a app é opt-out para ser vendida através de parceiros.</span><span class="sxs-lookup"><span data-stu-id="dacaa-112">The target account is commercial and the app is opt-out to be sold via partners.</span></span>
- <span data-ttu-id="dacaa-113">A aplicação é opt-in para parceiros selecionados e a conta-alvo não está na lista de autorizações.</span><span class="sxs-lookup"><span data-stu-id="dacaa-113">The app is opt-in for selected partners and the target account is not in the allow list.</span></span>
- <span data-ttu-id="dacaa-114">A oferta foi uma oferta de pré-visualização no passado para subscrições selecionadas ou era uma oferta privada e a subscrição já não está na lista de autorizações.</span><span class="sxs-lookup"><span data-stu-id="dacaa-114">The offer was a preview offer in the past for selected subscriptions or was a private offer and the subscription is no longer in the allow list.</span></span>
- <span data-ttu-id="dacaa-115">A nova conta de faturação encontra-se numa região diferente da de onde a oferta é vendida e a oferta não deve ser vendida naquela região.</span><span class="sxs-lookup"><span data-stu-id="dacaa-115">The new billing account is in a region different from where the offer is sold AND the offer is not to be sold in that region.</span></span>

<span data-ttu-id="dacaa-116">Uma transferência bloqueada permanece em vigor até remover o recurso da subscrição, após o qual pode tentar a transferência novamente.</span><span class="sxs-lookup"><span data-stu-id="dacaa-116">A blocked transfer remains in effect until you remove the resource from the subscription, after which you can try the transfer again.</span></span>

## <a name="next-steps"></a><span data-ttu-id="dacaa-117">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="dacaa-117">Next steps</span></span>

[<span data-ttu-id="dacaa-118">Obtenha suporte para Microsoft AppSource e Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="dacaa-118">Get support for Microsoft AppSource and Azure Marketplace</span></span>](get-support.md)

