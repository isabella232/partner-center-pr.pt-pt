---
title: 'Quickstart: Gerir um Mercado Azure Privado usando o PowerShell'
description: Este quickstart mostra-lhe como gerir ofertas num Private Azure Marketplace usando a Azure PowerShell.
author: keferna
ms.author: keferna
ms.topic: quickstart
ms.prod: marketplace-customer
ms.devlang: azurepowershell
ms.date: 11/24/2020
ms.custom: devx-track-azurepowershell
ms.openlocfilehash: d0021be17ab12b6e549b0e5263772a4a1e42f8a3
ms.sourcegitcommit: 531151a5dbc999b8b7de478d72ea115e6d579ff1
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/13/2021
ms.locfileid: "98182346"
---
# <a name="quickstart-manage-a-private-azure-marketplace-using-powershell"></a>Quickstart: Gerir um Mercado Azure Privado usando o PowerShell

Este artigo descreve como pode gerir ofertas num Mercado Azure Privado utilizando o módulo [Az.Marketplace](/powershell/module/az.marketplace) PowerShell.

> [!IMPORTANT]
> O Private Azure Marketplace está atualmente em pré-visualização pública. Esta versão de pré-visualização é disponibilizada sem contrato de nível de serviço. Não é recomendada para cargas de trabalho de produção. Algumas funcionalidades podem não ser suportadas ou podem ter capacidades restritas. Para obter mais informações, veja [Termos Suplementares de Utilização para Pré-visualizações do Microsoft Azure](https://azure.microsoft.com/support/legal/preview-supplemental-terms/).

## <a name="requirements"></a>Requisitos

* Se não tiver uma subscrição do Azure, crie uma conta [gratuita](https://azure.microsoft.com/free/) antes de começar.

* Se optar por utilizar a Azure PowerShell localmente:
  * [Instale o módulo Az PowerShell](/powershell/azure/install-az-ps).
  * Ligue-se à sua conta Azure utilizando o [cmdlet Connect-AzAccount.](/powershell/module/az.accounts/connect-azaccount)
* Se optar por utilizar a Azure Cloud Shell:
  * Consulte [a visão geral da Azure Cloud Shell](/azure/cloud-shell/overview) para obter mais informações.

  > [!IMPORTANT]
  > Enquanto o módulo **Az.Marketplace** PowerShell estiver em pré-visualização, deve instalá-lo separadamente utilizando o `Install-Module` cmdlet. Quando este módulo do PowerShell entrar em disponibilidade geral, fará parte das versões futuras do módulo Az PowerShell e estará disponível por predefinição a partir do Azure Cloud Shell.

  ```azurepowershell-interactive
  Install-Module -Name Az.Marketplace
  ```

* Se tiver várias subscrições do Azure, escolha a subscrição adequada na qual os recursos devem ser faturados. Selecione uma subscrição específica utilizando o [cmdlet Set-AzContext.](/powershell/module/az.accounts/set-azcontext)

  ```azurepowershell-interactive
  Set-AzContext -SubscriptionId 00000000-0000-0000-0000-000000000000
  ```

## <a name="list-private-stores"></a>Listar lojas privadas

Para obter uma lista de lojas privadas, utilize o [cmdlet Get-AzMarketplacePrivateStore.](/powershell/module/az.marketplace/get-azmarketplaceprivatestore) O exemplo a seguir enumera lojas privadas que foram criadas no âmbito do arrendatário.

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

## <a name="add-an-offer-to-a-private-marketplace"></a>Adicione uma oferta a um mercado privado

Para adicionar uma oferta a uma loja privada, utilize o [cmdlet Set-AzMarketplacePrivateStoreOffer.](/powershell/module/az.marketplace/set-azmarketplaceprivatestoreoffer) O exemplo a seguir adiciona a oferta especificada a um mercado privado para uma loja privada que é criada sob o âmbito do arrendatário.

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

## <a name="get-private-store-offers"></a>Receba ofertas de lojas privadas

Para obter uma ou mais ofertas de loja privada, utilize o [cmdlet Get-AzMarketplacePrivateStoreOffer.](/powershell/module/az.marketplace/get-azmarketplaceprivatestoreoffer) O exemplo a seguir obtém ofertas associadas à loja privada especificada que foram adicionadas no âmbito do arrendatário.

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

## <a name="remove-an-offer"></a>Remover uma oferta

Para remover uma oferta de uma loja privada, utilize o [cmdlet Remove-AzMarketplacePrivateStoreOffer.](/powershell/module/az.marketplace/remove-azmarketplaceprivatestoreoffer) O exemplo seguinte remove uma oferta de uma loja privada que foi criada no âmbito do arrendatário.

```azurepowershell-interactive
Remove-AzMarketplacePrivateStoreOffer -privateStoreId 00000000-0000-0000-0000-000000000000 -offerId publisherid.offerid
```

## <a name="next-steps"></a>Passos seguintes

[Criar e gerir o Private Azure Marketplace.](create-manage-private-azure-marketplace.md)