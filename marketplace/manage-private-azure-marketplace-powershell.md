---
title: 'Quickstart: Gerir um Mercado Azure Privado usando o PowerShell'
description: Este quickstart mostra-lhe como gerir ofertas num Private Azure Marketplace usando a Azure PowerShell.
author: keferna
ms.author: keferna
ms.topic: quickstart
ms.service: marketplace-customer
ms.devlang: azurepowershell
ms.date: 11/24/2020
ms.custom: devx-track-azurepowershell
ms.openlocfilehash: d7bd790eab2618822dbc5099ad1ad107794c82d2
ms.sourcegitcommit: 3a2415ab9833d5c574ad76d462f526a131c24f33
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/12/2021
ms.locfileid: "103412459"
---
# <a name="quickstart-manage-a-private-azure-marketplace-using-powershell"></a><span data-ttu-id="0ba27-103">Quickstart: Gerir um Mercado Azure Privado usando o PowerShell</span><span class="sxs-lookup"><span data-stu-id="0ba27-103">Quickstart: Manage a Private Azure Marketplace using PowerShell</span></span>

<span data-ttu-id="0ba27-104">Este artigo descreve como pode gerir ofertas num Mercado Azure Privado utilizando o módulo [Az.Marketplace](/powershell/module/az.marketplace) PowerShell.</span><span class="sxs-lookup"><span data-stu-id="0ba27-104">This article describes how you can manage offers in a Private Azure Marketplace using the [Az.Marketplace](/powershell/module/az.marketplace) PowerShell module.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="0ba27-105">O Private Azure Marketplace está atualmente em pré-visualização pública.</span><span class="sxs-lookup"><span data-stu-id="0ba27-105">Private Azure Marketplace is currently in public preview.</span></span> <span data-ttu-id="0ba27-106">Esta versão de pré-visualização é disponibilizada sem contrato de nível de serviço.</span><span class="sxs-lookup"><span data-stu-id="0ba27-106">This preview version is provided without a service level agreement.</span></span> <span data-ttu-id="0ba27-107">Não é recomendada para cargas de trabalho de produção.</span><span class="sxs-lookup"><span data-stu-id="0ba27-107">It's not recommended for production workloads.</span></span> <span data-ttu-id="0ba27-108">Algumas funcionalidades podem não ser suportadas ou podem ter capacidades restritas.</span><span class="sxs-lookup"><span data-stu-id="0ba27-108">Some features might not be supported or might have constrained capabilities.</span></span> <span data-ttu-id="0ba27-109">Para obter mais informações, veja [Termos Suplementares de Utilização para Pré-visualizações do Microsoft Azure](https://azure.microsoft.com/support/legal/preview-supplemental-terms/).</span><span class="sxs-lookup"><span data-stu-id="0ba27-109">For more information, see [Supplemental Terms of Use for Microsoft Azure Previews](https://azure.microsoft.com/support/legal/preview-supplemental-terms/).</span></span>

## <a name="requirements"></a><span data-ttu-id="0ba27-110">Requisitos</span><span class="sxs-lookup"><span data-stu-id="0ba27-110">Requirements</span></span>

* <span data-ttu-id="0ba27-111">Se não tiver uma subscrição do Azure, crie uma conta [gratuita](https://azure.microsoft.com/free/) antes de começar.</span><span class="sxs-lookup"><span data-stu-id="0ba27-111">If you don't have an Azure subscription, create a [free](https://azure.microsoft.com/free/) account before you begin.</span></span>

* <span data-ttu-id="0ba27-112">Se optar por utilizar a Azure PowerShell localmente:</span><span class="sxs-lookup"><span data-stu-id="0ba27-112">If you choose to use Azure PowerShell locally:</span></span>
  * <span data-ttu-id="0ba27-113">[Instale o módulo Az PowerShell](/powershell/azure/install-az-ps).</span><span class="sxs-lookup"><span data-stu-id="0ba27-113">[Install the Az PowerShell module](/powershell/azure/install-az-ps).</span></span>
  * <span data-ttu-id="0ba27-114">Ligue-se à sua conta Azure utilizando o [cmdlet Connect-AzAccount.](/powershell/module/az.accounts/connect-azaccount)</span><span class="sxs-lookup"><span data-stu-id="0ba27-114">Connect to your Azure account using the [Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount) cmdlet.</span></span>
* <span data-ttu-id="0ba27-115">Se optar por utilizar a Azure Cloud Shell:</span><span class="sxs-lookup"><span data-stu-id="0ba27-115">If you choose to use Azure Cloud Shell:</span></span>
  * <span data-ttu-id="0ba27-116">Consulte [a visão geral da Azure Cloud Shell](/azure/cloud-shell/overview) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="0ba27-116">See [Overview of Azure Cloud Shell](/azure/cloud-shell/overview) for more information.</span></span>

  > [!IMPORTANT]
  > <span data-ttu-id="0ba27-117">Enquanto o módulo **Az.Marketplace** PowerShell estiver em pré-visualização, deve instalá-lo separadamente utilizando o `Install-Module` cmdlet.</span><span class="sxs-lookup"><span data-stu-id="0ba27-117">While the **Az.Marketplace** PowerShell module is in preview, you must install it separately using the `Install-Module` cmdlet.</span></span> <span data-ttu-id="0ba27-118">Quando este módulo do PowerShell entrar em disponibilidade geral, fará parte das versões futuras do módulo Az PowerShell e estará disponível por predefinição a partir do Azure Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="0ba27-118">After this PowerShell module becomes generally available, it will be part of future Az PowerShell module releases and available by default from within Azure Cloud Shell.</span></span>

  ```azurepowershell-interactive
  Install-Module -Name Az.Marketplace
  ```

* <span data-ttu-id="0ba27-119">Se tiver várias subscrições do Azure, escolha a subscrição adequada na qual os recursos devem ser faturados.</span><span class="sxs-lookup"><span data-stu-id="0ba27-119">If you have multiple Azure subscriptions, choose the appropriate subscription in which the resources should be billed.</span></span> <span data-ttu-id="0ba27-120">Selecione uma subscrição específica utilizando o [cmdlet Set-AzContext.](/powershell/module/az.accounts/set-azcontext)</span><span class="sxs-lookup"><span data-stu-id="0ba27-120">Select a specific subscription using the [Set-AzContext](/powershell/module/az.accounts/set-azcontext) cmdlet.</span></span>

  ```azurepowershell-interactive
  Set-AzContext -SubscriptionId 00000000-0000-0000-0000-000000000000
  ```

## <a name="list-private-stores"></a><span data-ttu-id="0ba27-121">Listar lojas privadas</span><span class="sxs-lookup"><span data-stu-id="0ba27-121">List private stores</span></span>

<span data-ttu-id="0ba27-122">Para obter uma lista de lojas privadas, utilize o [cmdlet Get-AzMarketplacePrivateStore.](/powershell/module/az.marketplace/get-azmarketplaceprivatestore)</span><span class="sxs-lookup"><span data-stu-id="0ba27-122">To retrieve a list of private stores, you use the [Get-AzMarketplacePrivateStore](/powershell/module/az.marketplace/get-azmarketplaceprivatestore) cmdlet.</span></span> <span data-ttu-id="0ba27-123">O exemplo a seguir enumera lojas privadas que foram criadas no âmbito do arrendatário.</span><span class="sxs-lookup"><span data-stu-id="0ba27-123">The following example lists private stores that were created under the tenant scope.</span></span>

```azurepowershell-interactive
Get-AzMarketplacePrivateStore
```

```Output
Availability   : enabled
PrivateStoreId : 00000000-0000-0000-0000-000000000000
ETag           : "00000000-0000-0000-0000-000000000000"
Id             : /providers/Microsoft.Marketplace/privateStores/00000000-0000-0000-0000-000000000000
Name           : 00000000-0000-0000-0000-000000000000
Type           : Microsoft.Marketplace/privateStores
```

## <a name="add-an-offer-to-a-private-marketplace"></a><span data-ttu-id="0ba27-124">Adicione uma oferta a um mercado privado</span><span class="sxs-lookup"><span data-stu-id="0ba27-124">Add an offer to a private marketplace</span></span>

<span data-ttu-id="0ba27-125">Para adicionar uma oferta a uma loja privada, utilize o [cmdlet Set-AzMarketplacePrivateStoreOffer.](/powershell/module/az.marketplace/set-azmarketplaceprivatestoreoffer)</span><span class="sxs-lookup"><span data-stu-id="0ba27-125">To add an offer to a private store, you use the [Set-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/set-azmarketplaceprivatestoreoffer) cmdlet.</span></span> <span data-ttu-id="0ba27-126">O exemplo a seguir adiciona a oferta especificada a um mercado privado para uma loja privada que é criada sob o âmbito do arrendatário.</span><span class="sxs-lookup"><span data-stu-id="0ba27-126">The following example adds the specified offer to a private marketplace for a private store that is created under the tenant scope.</span></span>

```azurepowershell-interactive
$Params = @{
  privateStoreId = '00000000-0000-0000-0000-000000000000'
  offerId = 'publisherid.offerid'
  SpecificPlanIdsLimitation =@('PublisherEnterpriseLinux72',
                               'PublisherEnterpriseLinux72-ARM',
                               'PublisherEnterpriseLinux73',
                               'PublisherEnterpriseLinux73-ARM',
                               'PublisherEnterpriseLinux73-ARM-pr'
  )
}
Set-AzMarketplacePrivateStoreOffer @Params
```

```Output
UniqueOfferId             : publisherid.offerid
OfferDisplayName          :
PublisherDisplayName      :
ETag                      : "00000000-0000-0000-0000-000000000000"
PrivateStoreId            : 00000000-0000-0000-0000-000000000000
CreatedBy                 :
CreatedDate               : 01/01/0001 00:00:00
SpecificPlanIdsLimitation : {PublisherEnterpriseLinux72, PublisherEnterpriseLinux72-ARM,
PublisherEnterpriseLinux73, PublisherEnterpriseLinux73-ARM, PublisherEnterpriseLinux73-ARM-pr}
Id                        :
/providers/Microsoft.Marketplace/privateStores/00000000-0000-0000-0000-000000000000/offers/
                            publisherid.offerid
Name                      : publisherid.offerid
Type                      : Microsoft.Marketplace/privateStores/offers
```

## <a name="get-private-store-offers"></a><span data-ttu-id="0ba27-127">Receba ofertas de lojas privadas</span><span class="sxs-lookup"><span data-stu-id="0ba27-127">Get private store offers</span></span>

<span data-ttu-id="0ba27-128">Para obter uma ou mais ofertas de loja privada, utilize o [cmdlet Get-AzMarketplacePrivateStoreOffer.](/powershell/module/az.marketplace/get-azmarketplaceprivatestoreoffer)</span><span class="sxs-lookup"><span data-stu-id="0ba27-128">To get one or more private store offers, you use the [Get-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/get-azmarketplaceprivatestoreoffer) cmdlet.</span></span> <span data-ttu-id="0ba27-129">O exemplo a seguir obtém ofertas associadas à loja privada especificada que foram adicionadas no âmbito do arrendatário.</span><span class="sxs-lookup"><span data-stu-id="0ba27-129">The following example gets offers that are associated with the specified private store that were added under the tenant scope.</span></span>

```azurepowershell-interactive
Get-AzMarketplacePrivateStoreOffer -PrivateStoreId 00000000-0000-0000-0000-000000000000
```

```Output
UniqueOfferId             : publisherid.offerid
OfferDisplayName          :
PublisherDisplayName      :
ETag                      : "00000000-0000-0000-0000-000000000000"
PrivateStoreId            : 00000000-0000-0000-0000-000000000000
CreatedBy                 :
CreatedDate               : 01/01/0001 00:00:00
SpecificPlanIdsLimitation : {small, medium-with-upgraded-bandwidth, medium-with-upgraded-apps, large, large-pr,
small-pr}
Id                        :
/providers/Microsoft.Marketplace/privateStores/00000000-0000-0000-0000-000000000000/offers/
                            publisherid.offerid
Name                      : publisherid.offerid
Type                      : Microsoft.Marketplace/privateStores/offers

UniqueOfferId             : publisherid1.offerid1
OfferDisplayName          :
PublisherDisplayName      :
ETag                      : "00000000-0000-0000-0000-000000000000"
PrivateStoreId            : 00000000-0000-0000-0000-000000000000
CreatedBy                 :
CreatedDate               : 01/01/0001 00:00:00
SpecificPlanIdsLimitation : {azure_managedservices_professional ,azure_managedservices_professional-pr}
Id                        :
/providers/Microsoft.Marketplace/privateStores/00000000-0000-0000-0000-000000000000/offers/
                            publisherid1.offerid1
Name                      : publisherid1.offerid1
Type                      : Microsoft.Marketplace/privateStores/offers
```

## <a name="remove-an-offer"></a><span data-ttu-id="0ba27-130">Remover uma oferta</span><span class="sxs-lookup"><span data-stu-id="0ba27-130">Remove an offer</span></span>

<span data-ttu-id="0ba27-131">Para remover uma oferta de uma loja privada, utilize o [cmdlet Remove-AzMarketplacePrivateStoreOffer.](/powershell/module/az.marketplace/remove-azmarketplaceprivatestoreoffer)</span><span class="sxs-lookup"><span data-stu-id="0ba27-131">To remove an offer from a private store, you use the [Remove-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/remove-azmarketplaceprivatestoreoffer) cmdlet.</span></span> <span data-ttu-id="0ba27-132">O exemplo seguinte remove uma oferta de uma loja privada que foi criada no âmbito do arrendatário.</span><span class="sxs-lookup"><span data-stu-id="0ba27-132">The following example removes an offer from a private store that was created in the tenant scope.</span></span>

```azurepowershell-interactive
Remove-AzMarketplacePrivateStoreOffer -privateStoreId 00000000-0000-0000-0000-000000000000 -offerId publisherid.offerid
```

## <a name="next-steps"></a><span data-ttu-id="0ba27-133">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="0ba27-133">Next steps</span></span>

<span data-ttu-id="0ba27-134">[Criar e gerir o Private Azure Marketplace.](create-manage-private-azure-marketplace.md)</span><span class="sxs-lookup"><span data-stu-id="0ba27-134">[Create and manage Private Azure Marketplace](create-manage-private-azure-marketplace.md).</span></span>