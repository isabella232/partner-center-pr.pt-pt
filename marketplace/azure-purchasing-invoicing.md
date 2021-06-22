---
title: Software de compra e soluções da Azure Marketplace
description: Saiba mais sobre ferramentas que simplificam e dinamizam compras e gestão de software no Azure Marketplace.
ms.service: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 01/18/2021
ms.openlocfilehash: 11145280aad1ecd9777ec2fb7540e7d6479acfae
ms.sourcegitcommit: bce54ddb9fff7332a03d6aa228ba9414a87d76b7
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/22/2021
ms.locfileid: "112431552"
---
# <a name="azure-marketplace-purchasing"></a>Compra do Azure Marketplace

O Azure Marketplace dispõe de inúmeras ferramentas e funcionalidades que simplificam e agilizam o processo de compra, faturação e gestão da política de compra.

## <a name="simplified-procurement"></a>Aquisição simplificada

O Azure Marketplace ajuda a simplificar o processo de aprovisionamento através de diversas opções de compra. Se comprar produtos usando um cartão de crédito associado à sua conta Azure, todas as compras serão consolidadas numa única fatura e faturadas no cartão de crédito de eleição. Se for um grande cliente, pode comprar através de um Contrato Empresarial. Com uma EA, quaisquer compras de software são automaticamente incluídas na sua fatura Azure. A fatura irá incluir os custos de utilização do Azure em primeiro lugar, seguido dos custos do Azure Marketplace.

Ao comprar através do Azure Marketplace, elimina-se a complexidade da gestão das relações e faturas individuais do fornecedor. Obtém uma única fatura mensal consolidada da Microsoft que inclui tanto as suas compras no Azure Marketplace como as suas taxas Azure.

## <a name="permission-to-purchase"></a>Permissão para comprar

Depois de encontrar a aplicação de software certa, concluir a compra é simples. No entanto, necessitará de permissões adequadas dentro da assinatura Azure. Uma vez que o Azure opera num modelo [de Controlo de Acesso Baseado em Função](/azure/role-based-access-control/overview) (RBAC), a sua conta precisa de permissões de **subscrição** ou **de colaboradores** para efetuar uma compra.

Antes de concluir uma compra, certifique-se de que o utilizador tem a configuração correta no inquilino Azure. Isto ajudará a prevenir erros durante a compra.

Na experiência Azure Marketplace no portal Azure, encontre a aplicação que pretende comprar e selecione **Criar** ou **Configurar + subscrever.** Será solicitado a completar algumas informações antes de poder usar a sua nova solução.

> [!CAUTION]
> A aprovação no Mercado Privado não indica a aquisição de uma solução.

:::image type="content" source="media/overview/offer-create-screen.png" alt-text="O botão Criar oferta.":::

:::image type="content" source="media/overview/button-set-up-and-subscribe.png" alt-text="O botão Configurar + subscrever.":::

Se pretender implementar uma solução a partir da loja online Azure Marketplace, **selecione Obtenha-a agora** na página de descrição do produto e, em seguida, inscreva-se com as suas credenciais de conta Azure.

:::image type="content" source="media/overview/sign-in-to-azure-marketplace.png" alt-text="A caixa de diálogo de entrada do Azure Marketplace.":::

Assim que iniciar seduca, será redirecionado para o produto no portal Azure para concluir a sua compra.

## <a name="purchase-policy-management"></a>Gestão de políticas de compra

A Microsoft permite-lhe gerir as compras de utilizadores através do seu perfil de faturação como administrador de subscrição do Azure. Escolha entre três opções:

- **Grátis + Pago** – Permite que os utilizadores adquiram qualquer aplicação de software Azure Marketplace.
- **Grátis** – Permite que os utilizadores implementem apenas software gratuito a partir do Azure Marketplace.
- **Não** – Impede que os utilizadores implementem qualquer software do Azure Marketplace.

Estas definições aplicam-se a todos os utilizadores com acesso à sua subscrição Azure, o que lhe dá a capacidade de controlar a aquisição de TI através do portal Azure.

:::image type="content" source="media/overview/billing-profile-policy-settings.png" alt-text="Controlando a aquisição de TI através do portal Azure.":::

## <a name="cost-management"></a>Gestão de custos

Ao comprar produtos no Azure Marketplace, pretende obter insights que o ajudem a gerir os custos. A Azure Cost Management é uma ferramenta gratuita para visualizar informações sobre os produtos que adquiriu. Você pode usar a Cost Management para ver detalhes de quais os serviços em que está a gastar dinheiro ao longo do tempo e como esses custos acompanham os orçamentos que definiu. Além de definir orçamentos, pode agendar relatórios e analisar os custos de subscrição. Saiba mais sobre a Azure Cost Management completando o módulo Microsoft Learn sobre [custos de análise e criar orçamentos com a Azure Cost Management.](/learn/modules/analyze-costs-create-budgets-azure-cost-management/)

Pode ver as suas cobranças e faturas do Azure Marketplace na ferramenta de análise de custos do Azure Cost Management.

:::image type="content" source="media/overview/azure-cost-management.png" alt-text="Use a Azure Cost Management para obter informações sobre os seus produtos adquiridos.":::

## <a name="purchase-validation-checks"></a>Cheques de validação de compras

A compra de uma oferta através do Azure Marketplace pode falhar por diferentes razões. A utilização da interface de linha de comando (CLI) para uma compra é mais provável que cause erros, uma vez que pode estar a tentar adquirir uma oferta que não esteja disponível ou visível no Azure Marketplace. Seguem-se os controlos que podem fazer com que uma compra falhe:

1. A subscrição pertence a um Acordo de Empresa (EA) e à administração da EA desativada as compras do Azure Marketplace.
1. O administrador da EA permitiu compras apenas para ofertas gratuitas e a oferta é uma oferta paga.
1. A oferta não se encontra no mercado.
1. O Fornecedor Independente de Software (ISV) deixou de vender a oferta, pelo menos na sua região.
1. A subscrição que está a utilizar pertence a uma conta de faturação numa região onde a oferta não está disponível.
1. A conta de subscrição/faturação não está associada a um instrumento de pagamento válido (como um cartão de crédito válido).
1. A subscrição pertence a um Fornecedor de Solução Cloud (CSP) e o ISV recusou-se a vender através de um CSP.
1. O Private Marketplace está habilitado para a subscrição e a oferta não está na lista de ofertas permitidas.
1. A oferta é Privada/Pré-visualização para clientes específicos e a subscrição não está na lista de clientes autorizados.

## <a name="next-steps"></a>Passos seguintes

- [Cobrança e faturação](billing-invoicing.md)