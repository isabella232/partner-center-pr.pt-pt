---
title: Adicionar serviços partilhados a parceiro Azure
description: Use os Serviços Partilhados Azure Partner para comprar subscrições Azure para seu próprio uso, e para ter um método uniforme para comprar, rastrear e gerir a Azure.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 11/11/2020
ms.openlocfilehash: 756fbfda3438933b50fc51936b396291986472a7
ms.sourcegitcommit: ec33c2352a9dd3e5a941f0f42ff1e8d256bb2399
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/24/2021
ms.locfileid: "105028286"
---
# <a name="add-azure-partner-shared-services-so-partners-can-buy-azure-subscriptions-for-their-own-use"></a>Adicione serviços partilhados azure partner para que os parceiros possam comprar subscrições Azure para seu próprio uso

**Funções adequadas**

- Administrador global
- Agente administrativo
- Agente comercial

A Azure Partner Shared Services é um novo tipo de oferta para parceiros no programa CSP que permite aos parceiros adquirir subscrições Azure para seu próprio uso.Cria a oportunidade para os parceiros usarem um método uniforme para comprar, rastrear e gerir o Azure, além da capacidade de consolidar os seus acordos de licenciamento e revenda da Azure com a Microsoft. Com a Azure Partner Shared Services, os parceiros têm agora a mesma flexibilidade para usar subscrições Azure em CSP como fazem no Microsoft Enterprise Agreement e programas Web Direct, abrindo cenários como: construir ambientes de desenvolvimento e teste, implementar cargas de trabalho internas e hospedar serviços partilhados ou aplicações multi-arrendatários.  

## <a name="create-the-shared-services-tenant"></a>Crie o inquilino de serviços partilhados

1. Ir para **Definições**  >  **definições de conta Serviços**  >  **partilhados**.

   :::image type="content" source="images/sharedservices2.png" alt-text="Definições de conta > Serviços Partilhados":::

2. Se ainda não tem um inquilino de serviços partilhados, clique em **Criar serviços partilhados.**

   :::image type="content" source="images/sharedservices3.png" alt-text="Criar serviços partilhados":::

3. Isto cria um inquilino de serviços partilhados e compra a assinatura Azure CSP Shared Services, para ser usada para recursos partilhados e carga de trabalho interna.

   :::image type="content" source="images/sharedservices5.png" alt-text="Crie o inquilino e compre a subscrição":::

## <a name="about-the-azure--internalshared-services-offer"></a>Sobre a oferta de Serviços Internos/Partilhados Azure

- A subscrição Azure - Serviços Internos/Partilhados é um novo tipo de oferta Azure em CSP acedido através do Partner Center que os parceiros obtêm para o seu próprio uso do Azure.

- As subscrições de Serviços Partilhados Azure Partner são elegíveis e podem ser usadas para comprar RIs.

- A oferta Azure - Serviços Internos/Partilhados só pode ser aplicada ao arrendatário de serviços partilhados.

- A utilização primária para a subscrição Azure - Serviços Internos/Partilhados é para que possa utilizar o Azure para os seus próprios fins de desenvolvimento. O inquilino partilhado que utiliza para oferecer esta oferta não pode ser usado para outros serviços, como licenças Office 365 ou Dynamics.

- Pode cancelar a subscrição como qualquer outra subscrição. Ir às **definições**  >  **Ver todas as definições**  >  **Serviços partilhados**. Selecione a subscrição Azure - Serviços Internos/Partilhados e cancele-a.

## <a name="accessing-azure-partner-shared-services-consumption-details"></a>Aceder aos detalhes do consumo de serviços partilhados do Azure Partner

Encontrará o consumo do Azure na sua fatura CSP e no ficheiro de reconciliação. Será incluído como parte do item da linha Microsoft Azure na fatura. A informação detalhada sobre o consumo estará disponível no ficheiro de reconciliação registado contra o inquilino que foi criado para esta oferta.

## <a name="azure-partner-shared-services-pricing"></a>Preços dos Serviços Partilhados Azure Partner

Para ver o novo ficheiro de preços dos Serviços Partilhados do Azure Partner, vá à **Venda**  >  **de Preços e Ofertas** e selecione a lista de preços do mês em curso. Nas próximas semanas, será também lançado um cartão de tarifa específico api.

## <a name="marketplace-offers-and-azure-partner-shared-services"></a>Ofertas de Marketplace e Serviços Partilhados parceiros Azure

A partir de 1 de março de 2019, a Azure Partner Shared Services (APSS) já não suporta ofertas do Marketplace.

|**Apoio ao mercado**   |**APSS apoiado antes de 1 de março de 2019**|**Depois de 1 de março de 2019**|
|---------------------------|:----------------------------|:-------------------|
|Traga a sua própria licença (BYOL) e serviços gratuitos   | Yes   | No|
|Outras ofertas de mercado de terceiros   | No   |No|

Os parceiros que tenham BYOL ou serviços gratuitos implantados através da APSS não serão afetados; no entanto, após 1 de março de 2019 não poderão adquirir novos serviços BYOL ou gratuitos.

Para tirar partido do catálogo completo de ofertas do Marketplace disponíveis (não apenas BYOL e serviços gratuitos), recomendamos que os parceiros da CSP implementem serviços partilhados utilizando subscrições da Web Direct Azure.  Os parceiros da CSP que já implementaram recursos de serviços gratuitos de terceiros byol e que desejam continuar a usá-los e implementar mais ofertas de terceiros são encorajados a migrar a subscrição APSS para subscrições de [Azure migrando diretamente](/azure/cloud-solution-provider/migration/migration#migrating-existing-azure-subscriptions)na Web.

Os parceiros, que planeiam continuar a utilizar a subscrição da APSS após o dia 1 de março de 2019 e desejam implementar novos [serviços BYOL](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol) de terceiros ou serviços gratuitos, podem seguir as instruções dos ISVs para os implementar nas suas subscrições APSS.

## <a name="next-steps"></a>Passos seguintes

- [Sell software subscriptions through CSP](csp-software-subscriptions.md) (Vender subscrições de software através do CSP)