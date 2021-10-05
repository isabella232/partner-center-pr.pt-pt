---
title: Novo comércio telco pay-as-you-go
ms.topic: article
ms.date: 09/03/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Conheça novas experiências de comércio para comprar ofertas que permitam o overage pay-as-you-go.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8265cb3ce77183c4919e9b8e4e028bb66e8cd2f7
ms.sourcegitcommit: 462d6026287b85c9feea602af5bcdf924f3e6976
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/05/2021
ms.locfileid: "129452501"
---
# <a name="introduction-new-commerce-overage-for-telco-pay-as-you-go"></a>Introdução: Novo excesso de comércio para telco pay-as-you-go

**Funções adequadas**

- Agente administrativo
- Agente comercial
- Administrador global

> [!NOTE]
> As novas mudanças na experiência de comércio estão atualmente disponíveis apenas para parceiros que fazem parte da Microsoft 365/Dynamics 365 nova experiência técnica de experiência técnica.

Alguns produtos baseados em licença incluem serviços com planos de chamada atribuídos que normalmente incluem uma atribuição por licença para minutos por mês, geralmente 120 por licença. 

Nos cenários tradicionais de parceiros baseados em licenças não havia forma de permitir o uso do serviço para além dos limites mensais. Os clientes que precisam de mais de 120 minutos necessários para comprar créditos de comunicação, ou créditos de *comunicação* diretamente da Microsoft.  Estes créditos de comunicação não foram oferecidos no Partner Center.

## <a name="using-new-commerce-telco-pay-as-you-go"></a>Usando o novo comércio telco pay-as-you-go

Esta limitação foi abordada em novos comércios, permitindo ao parceiro permitir capacidades de excesso de serviços que o permitam. Os parceiros podem comprar ofertas que incluam capacidades de excesso de peso. Estas ofertas estão identificadas na coluna de etiquetas de etiquetas de etiquetas de preços que *inclui a IncluiOverage.* O catálogo SKU também inclui uma propriedade para determinar que o SKU suporta a capacidade de overage. Os parceiros simplesmente compram as ofertas e o sistema configura uma subscrição overage que não tem custo e só acumula faturação quando os utilizadores do cliente eclipsam as atas de chamada mensais atribuídas que vêm com a oferta adquirida. 

Os parceiros podem identificar quais os skus de produtos que incluem capacidades de overage por 

- Visualização do produto de catálogo do centro parceiro SKUs
- Filtrar a nova lista de preços de comércio por **inclui aOverage** na coluna tags

Os parceiros que compram produtos com excesso permitem-no acedendo à **Gestão de Overage** na página 'Gerir Subscrições'. A interface de overage de gestão permite ao parceiro ativar e atribuir a que subscrição Azure os encargos de overage fluirão. A qualquer momento, o parceiro pode desligar o excesso atribuindo a subscrição de consumo a *Nenhum*. 

Os parceiros atribuem-no em excesso ou desativam-no pela funcionalidade *Gerir o excesso* na lista de subscrições. Isto só será acessível se o parceiro tiver subscrições que permitam a sobre-agem. Os encargos mensais de excesso de idade serão acumulados para a subscrição atribuída e serão identificados no ficheiro de reconciliação dos parceiros. Os parceiros podem rastrear o uso excessivo visitando as capacidades de gestão de custos do Azure no portal Azure. 

Os parceiros podem rastrear o uso excessivo indo ao portal Azure e usando as capacidades e funcionalidades de gestão de custos. 

## <a name="important-details-about-overage"></a>Detalhes importantes sobre excesso de idade

- A aquisição de um produto baseado em licença SKU que inclua capacidades de excesso de informação apenas comprará o produto baseado em licença. Os parceiros terão de dar mais um passo após a compra para se sobreotar, indo para a página de gestão de subscrição e clicando **gerir o overage**
- Apenas os Agentes Admin para o parceiro de transação podem permitir a sobreagem após a compra baseada na licença. 
- Permitir a sobreavalagem criará um plano Azure sem custos e uma subscrição Azure associada **1** especificamente para consumo excessivo. Se o plano Azure já existir, permitir a sobretratação criará a nova subscrição ao abrigo do plano Azure existente. Os parceiros podem sempre visualizar ou reatribuir excesso a outras subscrições no **Overage Manage**. Os clientes que ainda não estão no plano Azure (azure mais antigo) terão de transitar para o plano Azure antes de poderem permitir a sobrecarga.

A atribuição de excesso de tempo é determinada pela *primeira regra.* Se um parceiro comprar E5 com planos de chamada para um novo cliente este parceiro terá excesso de tempo atribuído à sua subscrição de consumo. Se um segundo parceiro comprar outra cópia da E5 com planos de chamada, o sistema respeitará a compra e atribuição do primeiro parceiro. Os parceiros podem sempre gerir o *excesso* a partir da página de subscrições para desativá-la ou desativá-la atribuindo overage a *Nenhum*.

As definições de sobrecarga são por serviço por cliente. Apenas uma subscrição de excesso de idade pode ser atribuída de cada vez. Se a sobreposição tiver de ser alterada de um parceiro para outro, as três partes envolvidas têm primeiro de concordar. Uma vez que concordem que o parceiro existente pode simplesmente definir overage a *Nenhum,* permitindo que o outro parceiro desauça a sua subscrição.

## <a name="telco-pay-as-you-go-apis"></a>Telco pay-as-you-go APIs

- [As propriedades do SKU](/partner-center/develop/product-resources#sku) incluem uma propriedade *de consumoType* para ajudar o parceiro a identificar se um SKU permite excesso de tempo
- [Obtenha um excesso para](/partner-center/develop/get-subscription-overage) entender se algum excesso está atualmente configurado para o seu cliente
- [Atualizar o excesso de tempo](/partner-center/develop/update-subscription-overage) para atualizar o excesso de tempo do cliente para uma subscrição do Azure ou para defini-lo para *Nenhum*
