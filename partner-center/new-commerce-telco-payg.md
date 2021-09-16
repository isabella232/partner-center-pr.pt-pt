---
title: Novo comércio telco paga à medida que vai
ms.topic: article
ms.date: 09/03/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Conheça novas experiências de comércio para comprar ofertas que permitam pagar à medida que se sobreage.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: b7f3fa6ce3b92e7b182192290f5ebb4ee167ff7a
ms.sourcegitcommit: 986573bc4382b803bf4d641df6dd1e37c3af1955
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/16/2021
ms.locfileid: "127872191"
---
# <a name="introduction-new-commerce-overage-for-telco-pay-as-you-go"></a>Introdução: Novo excesso de comércio para telco pagar à medida que vai

**Funções adequadas**

- Agente administrativo
- Agente comercial
- Administrador global

> [!NOTE]
> As novas mudanças na experiência de comércio estão atualmente disponíveis apenas para parceiros que fazem parte da Microsoft 365/Dynamics 365 nova experiência técnica de experiência técnica.

Alguns produtos baseados em licenças incluem serviços com planos de chamada atribuídos. Estes planos de chamadas normalmente vêm com uma atribuição por licença por minutos por mês, geralmente 120 por licença.

Nos cenários tradicionais de parceiros baseados em licenças não havia forma de permitir o uso do serviço para além dos limites mensais. Os clientes que precisam de mais de 120 minutos necessários para comprar créditos de comunicação, ou créditos de *comunicação* diretamente da Microsoft.  Estes créditos de comunicação não foram oferecidos no Partner Center.

## <a name="using-new-commerce-telco-pay-as-you-go"></a>Usando o novo comércio telco pagar à medida que você vai ##

Esta limitação foi abordada em novos comércios, permitindo ao parceiro permitir capacidades de excesso de serviços que o permitam. Os parceiros podem comprar ofertas que incluam capacidades de excesso de peso. Estas ofertas estão identificadas na coluna de etiquetas de etiquetas de etiquetas de preços que *inclui a IncluiOverage.* O catálogo SKU também inclui uma propriedade para determinar que o SKU suporta a capacidade de overage. Os parceiros simplesmente compram as ofertas e o sistema configura e subscrição de overage que não é custo e só acumula faturação quando os utilizadores do cliente eclipsam as atas de chamada mensais atribuídas que vêm com a oferta comprada.

Os parceiros podem rastrear o uso excessivo indo ao portal Azure e usando as capacidades e funcionalidades de gestão de custos. Os parceiros também têm a opção de definir o excesso a *Nenhum* se quiserem desativar ou desligar o excesso a qualquer momento.

Os parceiros podem identificar quais os produtos que incluem capacidades de overage visualizando o produto de catálogo do centro parceiro SKUs. 

Os parceiros que compram produtos com excesso permitem o excesso de alimentos acedendo à *Overage Manage* na página 'Gerir Subscrições'. Isto permitirá ao parceiro ativar a sobreatenção e atribuir à subscrição de consumo pretendido que os encargos de sobreatenção fluirão. A qualquer momento, o parceiro pode desligar o excesso atribuindo a subscrição de consumo a *Nenhum*.

Os parceiros atribuem overage ou desativá-lo pela funcionalidade *Gerir o excesso* na lista de subscrições. Isto só será acessível se o parceiro tiver subscrições que permitam a sobre-agem. Os encargos mensais de excesso de idade serão acumulados na subscrição atribuída e serão identificados no ficheiro de reconciliação dos parceiros. Os parceiros podem rastrear o uso excessivo visitando as capacidades de gestão de custos do Azure no portal Azure. 

## <a name="important-details-about-overage"></a>Detalhes importantes sobre excesso de idade ##

A aquisição de um produto SKU que permita a sobreagem garantirá automaticamente que o cliente do parceiro está configurado para que o excesso de fluxo flua. Isto incluirá a criação de um plano Azure sem custos, uma subscrição Azure associada e uma subscrição especificamente para consumo excessivo. Os parceiros podem ver e atribuir a subscrição que quiserem que se acumule no overage da Manage.

A atribuição por excesso é determinada pela *primeira regra.* Se um parceiro comprar E5 com planos de chamada para um novo cliente este parceiro terá excesso atribuído à sua subscrição de consumo. Se um segundo parceiro comprar outra cópia da E5 com planos de chamada, o sistema respeitará a compra e atribuição do primeiro parceiro. Os parceiros podem sempre gerir o *excesso* a partir da página de subscrições para desativá-la ou desativá-la atribuindo overage a *Nenhum*.

As definições de sobrecarga são por serviço por cliente. Se um cliente tiver os mesmos serviços de excesso de peso de diferentes parceiros, apenas uma subscrição de excesso de idade pode ser atribuída de cada vez. Se a sobreposição tiver de ser alterada de um parceiro para outro, as três partes envolvidas têm primeiro de concordar. Uma vez que concordem que o parceiro existente pode simplesmente definir overage a *Nenhum,* permitindo que o outro parceiro desatar a sobrecarga à sua subscrição.

O suporte da API para o pagamento de telco à medida que vai, inclui:

- Propriedades SKU para ajudar o parceiro a identificar se um SKU permite excesso de tempo
- Uma nova API para atribuir excesso a uma subscrição existente ou para definir overage a *Nenhum*
