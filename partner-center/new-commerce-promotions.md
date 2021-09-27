---
title: Novas promoções de comércio
ms.topic: article
ms.date: 09/24/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Conheça novas experiências de comércio para descobrir e comprar promoções.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: b5b4e3ec2ef4c37b742102d287e5eddd93690fdb
ms.sourcegitcommit: d731813da1d31519dc2dc583d17899e5cf4ec1b2
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/27/2021
ms.locfileid: "129075181"
---
# <a name="introduction-new-commerce-promotions"></a>Introdução: Novas promoções de comércio

**Funções adequadas**

- Agente administrativo
- Agente comercial
- Administrador global

> [!Note] 
> As novas mudanças na experiência de comércio estão atualmente disponíveis apenas para parceiros que fazem parte da Microsoft 365/Dynamics 365 nova experiência técnica de experiência técnica.

A Microsoft apoiará promoções em novos comércios. Estas promoções terão diferentes valores e durações de desconto. 

## <a name="discovering-promotions"></a>Descobrir promoções ##

Os parceiros podem descobrir promoções visitando o atraso das promoções ou chamando a API getPromotions. O atraso nas promoções é uma lista da Microsoft de promoções disponíveis que os parceiros precisam de saber. A lista é mantida editorialmente e atualizada mensalmente. 


## <a name="operationalize-promotions"></a>Operacionalizar promoções ##

Os parceiros podem operacionalizar as promoções implementando a API getPromotions. Esta API devolve todas as promoções existentes para um determinado mercado (país do cliente) e segmento. A API devolve a lista de promoções e informações importantes para ajudar o parceiro a entender quais as promoções disponíveis para clientes em diferentes países. 


A API getPromotions inclui os seguintes dados para uma determinada promoção:

- Duração da promoção
- O desconto percentual para a promoção
- Os produtos e SKUs a promoção está disponível para

As promoções são aplicadas pelo centro parceiro quando o parceiro compra o produto SKU para o qual a promoção está disponível. As promoções de parceiros estão disponíveis na interface de utilizador do catálogo do parceiro center nos detalhes do produto SKU. Podem clicar nos "Ver detalhes da promoção" para obter mais informações sobre a promoção. A capacidade de visualizar os detalhes da promoção pode ser acedida a partir da página de catálogo ver detalhes SKU, a página de revisão antes de submeter a compra, a confirmação após a submissão da encomenda e a página do histórico da encomenda. 

## <a name="verify-eligibility"></a>Verificar elegibilidade ##

Os parceiros podem ver se uma compra de cliente é elegível para uma promoção vendo a informação na página de revisão no centro de parceiros antes de comprar o produto. Os parceiros também podem ligar para a API de API de verificação de Elegografia, passando o ID do inquilino do cliente e o ID de promoção. A chamada retorna verdadeira se o cliente for elegível. Se o cliente não for elegível, a API devolve as condições que não foram satisfeitas para que a promoção seja aplicável. 

Os parceiros podem ligar para validar a elegibilidade e obter resultados de volta. Os erros de elegibilidade podem basear-se em contagens de assentos, termos incompatíveis ou limites em quantas vezes uma promoção pode ser aplicada ao produto de um cliente SKU.

>[!IMPORTANT]
> Os parceiros devem verificar as promoções antes de submeterem uma transação. Na página de *revisão* do Partner Center se os parceiros não virem uma promoção, não será aplicada na transação, o parceiro receberá o preço de não promoção. Os parceiros também podem olhar para o item da linha do carrinho API para ver se a promoção está presente antes de submeter uma transação. Os parceiros podem ligar para verificar promoções API antes de submeter transações para verificar se a combinação de sku de produto de cliente é elegível para a promoção e, se não, as razões da inelegibilidade.

Existem três razões para um cliente não ser elegível para uma promoção. Estes tipos não elegíveis serão devolvidos na API de promoção validada nos casos em que o cliente não seja elegível.

### <a name="seat-count"></a>Contagem de assentos ###

Muitas promoções têm um lugar máximo declarado de 2400 lugares. Nestes casos, uma transação que inclua mais de 2400 será submetida a preços de não promoção. Estas contagens de assentos também são aplicadas ao adicionar lugares a uma subscrição de promoção com estes limites. Os parceiros terão um erro se tentarem aumentar uma subscrição ativada por promoção para além dos limites. Os limites de lugares das promoções são aplicados entre parceiros, pelo que se um parceiro comprar uma promoção de 2300 lugares com um limite de contagem de assentos de promoção, um segundo parceiro que compre 200 lugares obteria o preço de subscrição pelo preço de não promoção. A promoção é elegível a nível de sku de produto que o parceiro está a transacionar, para que um parceiro possa obter preços promocionais para 2400 lugares de Microsoft 365 E3 e também para um produto diferente SKU Microsoft 365 E5. Os parceiros podem ligar para a [API subscrita](/partner-center/develop/get-a-list-of-available-licenses) para ver quantas licenças um cliente tem para um determinado SKU provisionado.

### <a name="term"></a>Termo ###

Restrições de prazo definem quais os termos SKU do produto alinhados com uma determinada promoção. Muitas promoções têm descontos diferentes definidos com base no termo. Se um parceiro submeter uma transação e o prazo não se alinhar com a promoção, esperam que a transação seja ao preço de não promoção que esperam. Exemplos de termos são *anuais* ou *mensais.*

### <a name="first-purchase"></a>Primeira Compra ###

Algumas promoções impõem que só sejam adquiridas uma vez. Um parceiro verá uma elegibilidade de *falso* usando a API de elegibilidade validada com o tipo de erro de *FirstPurchase*. Um parceiro ainda pode comprar o produto SKU dado, mas a subscrição será pelo preço de não promoção. Esta restrição é por cliente, não por parceiro. Uma vez que um cliente tem uma promoção com esta regra, eles não podem obter uma segunda instância da promoção aplicada por um segundo parceiro.

## <a name="promotions-and-renewals"></a>Promoções e renovações ##

Os descontos promocionais quando aplicados são para o prazo de compra. As subscrições com promoções aplicadas manterão o preço promocional se a data de renovação estiver na gama de datas de duração da promoção. As renovações fora da gama de datas de duração da promoção renovar-se-ão para o preço de não promoção (a partir da tabela de preços). Os parceiros podem acompanhar o estado de renovação dos pontos de preços na página de detalhes da subscrição e nas instruções de renovação de dados de subscrição.

## <a name="promotions-and-upgrades"></a>Promoções e atualizações ##
Os parceiros que atualizam de uma subscrição para outro SKU deixarão o preço de promoção para trás. Esta ação ocorre porque a promoção foi configurada para o SKU que eles estão deixando quando eles fazem upgrade para outro SKU. Os parceiros que fazem upgrade para um SKU que pode ter uma promoção não obterão automaticamente o preço de promoção. Se precisarem ou quiserem o preço de promoção para o SKU para onde querem mudar-se, precisam de comprar manualmente o novo SKU como uma nova subscrição. Atualmente, as promoções só são aplicadas em novas compras e renovações por subscrição.

## <a name="promotions-and-migrations"></a>Promoções e migrações ##
Os parceiros podem migrar as subscrições dos seus clientes do Microsoft 365/Dynamics 365 para novas versões de comércio das suas subscrições. As migrações estão disponíveis tanto a partir da interface de utilizador do Partner Center como da chamada apis de migração. Os parceiros que a migração de uma subscrição tradicional para o novo comércio receberão a promoção quando migrarem, desde que o produto se movam para alinhar com a definição de promoção. Os parceiros devem ligar para a API de elegibilidade para garantir que o produto-alvo SKU aplicará o preço de promoção antes da migração.
