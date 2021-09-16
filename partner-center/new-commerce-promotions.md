---
title: Novas promoções de comércio
ms.topic: article
ms.date: 09/03/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Conheça novas experiências de comércio para descobrir e comprar promoções.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: dc2d52dd444168b32f0cadaeccec1e6d906348d1
ms.sourcegitcommit: 847ad384d44a5a673791cb2950af02225d8174c9
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/16/2021
ms.locfileid: "127886155"
---
# <a name="introduction-new-commerce-promotions"></a>Introdução: Novas promoções de comércio

**Funções adequadas**

- Agente administrativo
- Agente comercial
- Administrador global

> [!Note] 
> As novas mudanças na experiência de comércio estão atualmente disponíveis apenas para parceiros que fazem parte da Microsoft 365/Dynamics 365 nova experiência técnica de experiência técnica.

A Microsoft apoiará promoções em novos comércios. Estas promoções terão diferentes valores de desconto e durações. 

## <a name="discovering-promotions"></a>Descobrir promoções ##

Os parceiros podem descobrir promoções visitando o atraso das promoções ou chamando a API getPromotions. O atraso nas promoções é uma lista da Microsoft de promoções disponíveis que os parceiros precisam de saber. A lista é mantida editorialmente e atualizada mensalmente. 


## <a name="operationalize-promotions"></a>Operacionalizar promoções ##

Os parceiros podem operacionalizar as promoções implementando a API getPromotions. Esta API devolve todas as promoções que existem para um determinado mercado (país do cliente) e segmento. A API devolve a lista de promoções e informações importantes para ajudar o parceiro a entender quais as promoções disponíveis para clientes em diferentes países. 


A API getPromotions inclui os seguintes dados para uma determinada promoção:

- Duração da promoção
- O desconto percentual para a promoção
- Os produtos e SKUs a promoção está disponível para

As promoções são aplicadas pelo centro parceiro quando o parceiro compra o produto SKU para o qual a promoção está disponível. As promoções de parceiros estão disponíveis na interface de utilizador do catálogo do parceiro center nos detalhes do produto SKU. Podem clicar nos "Ver detalhes da promoção" para obter mais informações sobre a promoção. A capacidade de visualizar os detalhes da promoção pode ser acedida a partir da página do catálogo ver detalhes SKU, a página de revisão antes de submeter a compra, a confirmação após a submissão da encomenda e a página do histórico da encomenda. 


## <a name="verify-eligibility"></a>Verificar elegibilidade ##

Os parceiros podem ver se uma compra de cliente é elegível para uma promoção vendo a informação na página de revisão no centro de parceiros antes de comprar o produto. Os parceiros também podem ligar para a API de API de promoção, passando o ID do inquilino do cliente e o ID de promoção. A chamada retorna verdadeira se o cliente for elegível. Se o cliente não for elegível, a API devolve as condições que não foram satisfeitas para que a promoção seja aplicável. 



## <a name="promotions-and-renewals"></a>Promoções e renovações ##

Os descontos promocionais quando aplicados são para o prazo de compra. As subscrições com promoções aplicadas manterão o preço promocional se a data de renovação estiver na gama de datas de duração da promoção. As renovações fora da gama de datas de duração da promoção renovar-se-ão para o preço de não promoção (a partir da tabela de preços). Os parceiros podem acompanhar o estado de renovação dos pontos de preços na página de detalhes da subscrição e nas instruções de renovação de dados de subscrição.


## <a name="promotions-and-upgrades"></a>Promoções e atualizações ##
Os parceiros que atualizam de uma subscrição para outro SKU deixarão o preço de promoção para trás. Esta ação ocorre porque a promoção foi configurada para o SKU que eles estão deixando quando eles fazem upgrade para outro SKU. Os parceiros que fazem upgrade para um SKU que pode ter uma promoção não obterão automaticamente o preço de promoção. Se precisarem ou quiserem o preço de promoção para o SKU para onde querem mudar-se, precisam de comprar manualmente o novo SKU como uma nova subscrição. Atualmente, as promoções só são aplicadas em novas compras e renovações de assinaturas.



