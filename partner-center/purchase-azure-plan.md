---
title: Comprar o plano do Azure
ms.topic: how-to
ms.date: 07/21/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Utilizando o plano Azure, aprenda a comprar subscrições Azure individuais ou múltiplas, reservas Azure, para configurar recursos e para visualizar ou adicionar subscrições.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: af098c9ef57a9a40badded40cb457f8c8fd4855185ae6f10dfb71e51689994ea
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/06/2021
ms.locfileid: "115693917"
---
# <a name="purchase-the-azure-plan-for-customers-and-access-the-latest-azure-services"></a>Compre o plano Azure para clientes e aceda aos mais recentes serviços da Azure

**Aplica-se a**: Centro de Parceiros 

**Funções adequadas**: Administração global | Administração de administração de utilizadores | Agente comercial

Ao adquirir um plano Azure para os seus clientes ao abrigo do Microsoft Customer Agreement, tem acesso ao catálogo completo dos mais recentes serviços Azure a preços de pagamento. Fornecedor de Soluções em Nuvem parceiros (CSP) poderão agora aceder a qualquer serviço Azure quando estiver em geral disponível. Um parceiro pode ter várias subscrições Azure ao abrigo de um plano Azure. 

## <a name="countryregion-availability"></a>Disponibilidade país/região

A nova experiência de comércio na CSP para a Azure está atualmente prevista para estar disponível em 137 países. Consulte a lista completa desses [países/regiões.](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3QN0x) 

## <a name="how-to-purchase-azure-plan"></a>Como comprar o plano Azure

A forma como compra o plano Azure é semelhante à compra de qualquer outra subscrição. A diferença fundamental é que antes de fazer o seu pedido precisa confirmar que o seu cliente assinou o Microsoft Customer Agreement.

1. Selecione **Segment Commercial,** em seguida, escreva "Microsoft Azure".
2. De acordo com **o plano Azure,** selecione **Adicionar ao carrinho**.

   :::image type="content" source="images/azure/Azurepurchase1.png" alt-text="Compra.":::

O parceiro deve confirmar que o cliente reviu e aceitou os termos do Microsoft Customer Agreement. Para obter mais informações sobre como o parceiro pode fazê-lo, leia a [aceitação do cliente confirme o Acordo de Cliente da Microsoft.](./confirm-customer-agreement.md) Outros recursos estão disponíveis na [galeria de recursos.](https://partner.microsoft.com/resources/collection/Microsoft-Customer-Agreement-in-the-CSP-program#/)

Em seguida, confirme digitalmente ou convide o cliente a assinar o Microsoft Customer Agreement diretamente com a Microsoft. 

### <a name="to-invite-the-customer-to-sign-the-agreement-directly"></a>Convidar o cliente a assinar o contrato diretamente 

1. Na **página** conta do cliente, selecione **Update** ao lado do Microsoft **Customer Agreement**.

2. Preencha a informação sobre o indivíduo na empresa do cliente que aceitou o MCuA.

3. Selecione **Guardar e continuar**.  

Como parte da nova experiência de comércio para a Azure na CSP, introduzimos uma [nova oferta Azure.](./azure-plan-lp.md) Para datas importantes relacionadas com a oferta anterior do Azure (MS-AZR-0145p), consulte o documento de [oferta](https://go.microsoft.com/fwlink/p/?linkid=2164140).

**Se se matriculou *antes* de 21 de julho de 2021**
- Poderá adicionar a oferta anterior da Azure ao seu carrinho para clientes que o tenham comprado no passado.
- Se se matriculou antes de 21 de julho *e* tiver clientes que se matricularam depois de 21 de julho, não poderá adicionar a oferta anterior da Azure ao seu carrinho.

**Parceiros que se matricularam *em ou depois de* 21 de julho de 2021**
- Não poderá adicionar a oferta anterior do Azure ao seu carrinho.

O seguinte erro será encontrado se tentar adicionar a oferta anterior do Azure, mas não for elegível devido à política de negócios acima. 

:::image type="content" source="images/add-products.png" alt-text="Screenshot mostrando o ecrã de produtos Add.":::

Para encontrar o novo plano Azure com APIs do Partner Center, consulte [Criar um plano Azure](/partner-center/develop/create-azure-plan#get-the-catalog-item-for-azure-plan).

## <a name="review-and-buy"></a>Rever e comprar

Volte à página **adicionar um produto** onde pode ver que o plano Azure foi adicionado. Selecione **Rever** para rever a sua compra e, em seguida, selecione **Comprar**. 

> [!NOTE]
> Uma vez adquirido o plano Azure para um cliente, já não pode comprar Microsoft Azure (0145p) para esse cliente. Terá de criar futuras subscrições através do plano Azure.

## <a name="purchase-azure-reservations-under-the-azure-plan"></a>Comprar reservas da Azure ao abrigo do plano Azure 
  
Também pode comprar reservas Microsoft Azure ao abrigo do plano Azure em nome dos seus clientes no Partner Center. (Ou, se preferir, pode [autorizar os seus clientes a comprarem as suas próprias reservas Azure](give-customers-permission.md) a partir de uma subscrição prévia que adquiriu para eles.)

1. A partir do menu Partner Center no seu [painel de instrumentos,](https://partner.microsoft.com/dashboard/)selecione **Clientes**. Encontre o cliente que quer comprar reservas do Azure e, em seguida, selecione a seta para baixo para expandir a linha do cliente.

2. **Selecione Adicionar produtos** e, em seguida, selecione **Azure**. 

   - Escolha o segmento de mercado do cliente na lista **de Segmento.**
   - Escolha **Reservas** na lista de **tipos de produto.**
   - Escolha o tipo de reserva que o cliente quer na lista de **tipos reservas.**

As reservas do Azure devem ser associadas a um plano Azure ativo. Escolha o plano Azure a que pretende adicionar reservas Azure a partir da lista de subscrição do Cliente. 

> [!IMPORTANT] 
> Se o cliente ainda não tiver um plano Azure ativo, selecione Azure para adicionar um agora. Para mais instruções, leia [as reservas do Buy Azure](azure-reservations-buying.md#purchase-azure-reservations).

> [!NOTE]
> O âmbito de uma reserva só pode ser definido para **Shared,** atualmente no Partner Center. Para selecionar um único âmbito de subscrição ou atualização do âmbito de subscrição partilhado para um único, vá ao **portal Microsoft Azure Gestão** utilizando as seguintes instruções. 

:::image type="content" source="images/azure/addprods1.png" alt-text="Definição de reservas de âmbito compartilhado.":::

Para gerir a reserva do cliente no portal Azure: 

1. A partir dos **Clientes** selecione o cliente que pretende gerir. 

2. Utilizando a seta para baixo, expanda a linha do cliente e selecione **o portal Microsoft Azure Management**.  
 
## <a name="view-azure-subscriptions-under-the-azure-plan"></a>Ver subscrições do Azure ao abrigo do plano Azure

A partir da página **de Subscrições,** na secção baseada em uso, expanda o **plano Azure** para ver subscrições Azure associadas ao abrigo do plano Azure.

:::image type="content" source="images/azure/addprods2.png" alt-text="Ver lista de subscrições do Azure."::: 

## <a name="add-subscriptions-and-configure-resources"></a>Adicionar subscrições e configurar recursos

Irá adicionar subscrições e configurar recursos para o seu cliente no portal Azure. Também é capaz de separar o ambiente do seu cliente por carga de trabalho ou projeto. É possível gerir subscrições através [do Farol Azure](https://azure.microsoft.com/services/azure-lighthouse/) e do portal Azure. 

Para gerir os recursos e subscrições do seu cliente, precisa de **privilégios de Administração em nome dos** privilégios (AOBO). Para obter informações sobre a gestão do seu acesso, leia [Gerir subscrições e recursos ao abrigo do plano Azure](azure-plan-manage.md)

## <a name="next-steps"></a>Passos seguintes

- [Transições de clientes para plano Azure](azure-plan-transition.md)

- [Parceiro ganhou crédito - visão geral](partner-earned-credit.md)
