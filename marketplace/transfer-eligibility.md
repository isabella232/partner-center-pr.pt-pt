---
title: Elegibilidade de transferência – Orientações para a transferência de uma subscrição entre contas de faturação, Azure Marketplace
description: Diretrizes para verificações comerciais antes de transferir uma subscrição entre contas de faturação no portal Azure.
ms.service: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 11/20/2020
ms.openlocfilehash: 4b235bd462915fc205813ae86e92f98b4fd49fe4
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/09/2021
ms.locfileid: "123936971"
---
# <a name="transfer-eligibility-for-a-subscription-between-billing-accounts"></a>Elegibilidade de transferência para uma subscrição entre contas de faturação

Pode [transferir uma subscrição](/azure/cost-management-billing/understand/subscription-transfer) de uma conta de faturação para outra na secção de faturação do portal Azure. Antes de uma transferência, a subscrição é digitalizada para produtos de terceiros. A transferência só é permitida se *todos os* produtos forem autorizados para transferência (ver [os critérios](#criteria-for-transfer-approval-or-denial) abaixo). O sistema irá gerar mensagens de erro relevantes para as aplicações que não conseguiram limpar para o ajudar a determinar os próximos passos.

> [!NOTE]
> Este artigo não se aplica às ofertas do SaaS porque os recursos do SaaS estão ligados a um inquilino, e não a uma subscrição. Os recursos do SAAS são transferíveis de uma conta de faturação para outra, mas isso é feito por recurso e pelo apoio da Azure como um pedido de apoio.

## <a name="criteria-for-transfer-approval-or-denial"></a>Critérios para aprovação de transferência ou negação

Não é possível transferir uma subscrição se alguma das suas aplicações de terceiros cumprir qualquer um dos seguintes critérios:

- A conta-alvo é comercial e a app é opt-out para ser vendida através de parceiros.
- A aplicação é opt-in para parceiros selecionados e a conta-alvo não está na lista de autorizações.
- A oferta foi uma oferta de pré-visualização no passado para subscrições selecionadas ou era uma oferta privada e a subscrição já não está na lista de autorizações.
- A nova conta de faturação encontra-se numa região diferente da de onde a oferta é vendida e a oferta não deve ser vendida naquela região.

Uma transferência bloqueada permanece em vigor até remover o recurso da subscrição, após o qual pode tentar a transferência novamente.

## <a name="next-steps"></a>Passos seguintes

[Obtenha suporte para Microsoft AppSource e Azure Marketplace](get-support.md)

