---
title: Alterações de preços nos produtos de mercado postam publicação
description: Este artigo descreve questões comuns sobre a alteração dos preços nos planos após a publicação.
ms.service: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 08/27/2021
ms.openlocfilehash: bfb99986483d0aaaa5d685c266c8118c1345517c
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/09/2021
ms.locfileid: "123936980"
---
# <a name="price-changes-to-marketplace-products"></a>Variações de preços nos produtos do mercado

Os Fornecedores independentes de Software (ISV) que vendem os seus produtos através do Azure Marketplace são autorizados a atualizar os preços do plano (ou SKUs) de vez em quando. O novo preço do SKU pode ser superior ou inferior ao preço anterior. A variação de preço é atualizada a nível de produto/SKU/mercado. Assim, pode haver atualizações de preços que são relevantes para alguns mercados, mas não para todos.

Em certos casos (ver abaixo) a alteração de preço pode afetar os produtos que foram comprados no passado, e o cliente verá uma alteração de preço na sua fatura mensal. O Azure Marketplace notificará os clientes que utilizam estes produtos pelo menos 90 dias antes da nova origem do novo preço.

## <a name="which-offer-types-can-be-affected-from-price-change"></a>Que tipos de oferta podem ser afetados pela variação de preço?

Todos os produtos transacionáveis vendidos via Azure Marketplace e AppSource, por exemplo, produtos que têm um ou mais planos.

## <a name="can-a-free-sku-turn-one-day-into-a-paid-one"></a>Um SKU grátis pode transformar-se um dia num pago?

N.º O ISV não pode transformar um SKU grátis num SKU pago. Um ISV que queira fazer um produto faturado terá de publicar um novo SKU pago.

## <a name="price-increase-awareness-in-the-marketplace-product-pages"></a>Aumento de preços na consciencialização nas páginas de produtos do mercado

Como mencionado, os ISV que pretendam publicar um aumento de preço devem dar pelo menos 90 dias de aviso antes da tomada de vigor do novo preço. Isto é para dar aviso prévio aos clientes que planeiam comprar um produto. As páginas de produtos do mercado são atualizadas com pelo menos 90 dias de antecedência sobre a mudança que se aproxima. As páginas são atualizadas com uma mensagem detalhando a próxima data da alteração de preço e a nova taxa

:::image type="content" source="media/price-change/plan-pricing.png" alt-text="Ilustra a página de preços do plano":::

> [!NOTE]
> O preço na imagem acima é apenas para fins. Os preços reais podem variar.

Esta notificação só mostrará se o preço subir, e não se o preço descer.

## <a name="when-is-the-new-price-taking-effect"></a>Quando é que o novo preço vai fazer efeito?

 A nova data de vigoro do preço será sempre no início de um mês civil. Com o período de pré-aviso de 90 dias, uma linha de tempo típica de atualização de preços será assim:

Jan-15 – ISV atualize uma futura atualização de preços para um SKU no catálogo

Jan-16-18 – a página do produto é atualizada com uma mensagem de aviso sobre o próximo aumento de preço que irá assumir no dia 1 de maio (final de janeiro + 90 dias).

Maio-1º – novo preço entra em vigor

## <a name="customers-affected-from-a-price-change-post-purchase"></a>Clientes afetados por uma alteração de preço (pós-compra)

A compra de um produto antes do aumento do preço da data efetiva *não* garante o preço de compra para o tempo de vida da implantação do produto. Diferentes tipos de oferta que são afetados são:

- Produtos à base de consumo (por exemplo, VMs que são cobrados pela hora ou preço do uso medido de SaaS ou oferta de aplicações geridas), uma vez que o novo preço é eficaz, o seu custo unitário de consumo aumentará. No caso de clientes que são cobrados em meados do mês, haverá duas linhas no relatório mensal de utilização: uma para consumo até à nova data de preço efetiva (no exemplo acima: maio-1º) e uma para consumo pós-data efetiva
- Produtos à base de consumo com taxa mensal (como o SaaS com contadores personalizados), o preço das unidades de consumo será afetado à medida que o novo preço entrar em vigor no mercado. A mensalidade será mantida inalterada até ao termo do período de direito.
- Produtos à base de assento (como serviços SaaS baseados em licença), se a data efetiva de alteração de preço ocorrer após a compra, então o preço de compra é garantido até à próxima data de renovação, seja a renovação mensal ou a data de renovação anual.
    - Adicionar ou remover lugares após a data de alteração de preço, mas antes da data de renovação do contrato será mantido ao preço de compra original. Após a renovação, o novo preço entrará em vigor.
    - Mudar o SKU, alterar o SKU após a data efetiva de alteração de preço será considerado como nova compra e estará sujeito ao novo preço. Esta alteração aplica-se também a cenários em que a alteração do número de lugares requer a alteração do SKU do cliente. Por exemplo, passar de 400 lugares para 500 lugares, o que pode exigir que o cliente compre um novo nível/SKU do produto.

## <a name="customer-notifications"></a>Notificações de clientes

Os clientes que já estão a utilizar o produto/SKU num mercado que seja afetado pelo próximo aumento de preço serão notificados por e-mail sobre a mudança que se avizinha. Isto é para que possam tomar medidas se assim o desejarem. A notificação por e-mail será enviada 90 dias antes do novo preço a ter efeito e uma segunda mensagem será enviada 30 dias antes da data efetiva da alteração de preço. A mensagem será enviada para o proprietário da secção de faturas (projeto), proprietários do grupo de faturação e proprietários de conta de faturação da subscrição.

## <a name="next-steps"></a>Passos seguintes

- [O que é o Azure Marketplace?](azure-marketplace-overview.md)
- [Compra do Azure Marketplace](azure-purchasing-invoicing.md)