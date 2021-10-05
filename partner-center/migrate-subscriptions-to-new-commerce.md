---
title: Migrar subscrições para novo comércio
ms.topic: article
ms.date: 10/04/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Conheça novas experiências de comércio para subscrições migratórias.
author: iragulati1
ms.author: iragulati
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: bad50c36cd0e0523fe70115e0b39d88e0e68ab68
ms.sourcegitcommit: 462d6026287b85c9feea602af5bcdf924f3e6976
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/05/2021
ms.locfileid: "129454669"
---
# <a name="introduction-migrate-subscriptions-to-new-commerce"></a>Introdução: Migrar Subscrições para o Novo Comércio

**Funções adequadas**: Agente administrador | Agente comercial | Administrador global

> [!NOTE]
> As novas mudanças na experiência de comércio estão atualmente disponíveis apenas para parceiros que fazem parte da Microsoft 365/Dynamics 365 nova experiência técnica de experiência técnica.
Os parceiros podem migrar subscrições para o Novo Comércio se a subscrição cumprir os critérios de elegibilidade e houver uma oferta de like like disponíveis.

## <a name="ineligible-subscriptions"></a>Assinaturas não elegíveis ##

Nem todas as assinaturas serão elegíveis para migração neste momento. As seguintes categorias de subscrições não são atualmente elegíveis: 

- Subscrições inativas (não ocorrerão alterações no serviço se uma subscrição estiver inativa) 

- Assinaturas de ensaio (sem benefícios monetários ou implicações; expectativa será deixar os ensaios executarem o seu curso no Legado) 

- Assinaturas com promoções (as promoções na NCE são independentes dessas promoções no Legado) 

- As subscrições com addons (as subscrições migratórias com addons serão ativadas mais tarde; neste momento, não podemos apoiar a migração de coterminous) 

- Assinaturas para audiências Gov, Edu ou Sem Fins Lucrativos (o mapeamento de ofertas qualificadas do Legado para a NCE não é suportado) 

- Assinaturas aposentadas ou prevadizadas (para estas subscrições, não haverá uma oferta semelhante a uma oferta semelhante existente no Novo Comércio) 

As migrações das subscrições acima referidas estão fora de alcance para esta funcionalidade neste momento. Além disso, uma única subscrição será a unidade de migração, em vez de lotes de subscrições. 

## <a name="suspending-a-legacy-subscription-during-migration"></a>Suspender uma assinatura de legado durante a migração ##

Uma subscrição antiga só será suspensa uma vez que seja previsto um caminho bem sucedido para o Novo Comércio para a subscrição. Esta capacidade evitará a perda de serviço se existirem bloqueadores na sequência de um Parceiro que inicia a migração de uma subscrição. Além disso, não ocorrerá uma faturação dupla tanto para a subscrição legacy como para o New Commerce. Uma vez iniciada a migração, a faturação para a subscrição legacy será interrompida para evitar qualquer sobreposição com a faturação para a subscrição NCE.

## <a name="billing-term-and-frequency"></a>Prazo de faturação e frequência ##

O prazo de faturação e a frequência de faturação para a subscrição migrada permanecerão os mesmos que o termo de faturação e a frequência de faturação para a subscrição do Legado; prazo final será o mesmo.

## <a name="new-commerce-promotions"></a>Novas Promoções de Comércio ##

As assinaturas em Legado com Promoções não são elegíveis para migração. As assinaturas migradas podem ser elegíveis para promoções introdutórias do New Commerce. As promoções serão promovidas até ao final do período de subscrição no ponto de migração. 

## <a name="cancelling-subscriptions-or-decreasing-licenses"></a>Cancelamento de assinaturas ou diminuição de licenças ##

Após a migração, há uma janela de cancelamento de 72 horas. Nestas 72 horas, os Parceiros podem cancelar a subscrição ou diminuir a quantidade de licença nesta janela. Na marca de tempo de 24 horas desde que a migração esteja concluída, os cancelamentos da subscrição ou das licenças serão prossa para um dia de utilização; na marca de 48 horas desde que a migração é concluída, cancelamentos da subscrição ou de licenças serão prostilizados para dois dias de utilização. 

## <a name="migration-history"></a>História da Migração ##

Através das APIs, os detalhes relativos ao histórico de migração, tais como os termos de início e conclusão da migração podem ser acedidos através do novo campo GetMigration API e MigrationID. No UX, o ID de subscrição a partir do qual a nova assinatura NCE migrará será visível no topo da página de detalhes, que é acedida ao clicar no item da linha de subscrição na página "Subscrições" do cliente. 

## <a name="apis"></a>APIs ##

Para a migração de subscrições similares, haverá 3 novas APIs de repouso lançadas. A primeira API "CheckMigration" verificará a elegibilidade da migração para uma subscrição. A segunda API "CreateMigration" criará a migração se a subscrição for elegível. Por último, a terceira API "GetMigration" permitirá que a Partner verifique o estado da migração. 
