---
title: Deixe os clientes comprarem os seus próprios serviços em CSP
description: Saiba como os parceiros de programas da CSP podem permitir que os clientes comprem os seus próprios serviços, como reservas Azure, para uma subscrição adquirida para eles no Partner Center.
ms.topic: how-to
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
author: amitravat
ms.author: amrava
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 23ca72fada539b5036dfd6cf0ac04a5c18b5d96d
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/13/2021
ms.locfileid: "126247298"
---
# <a name="give-customers-permission-in-partner-center-to-buy-their-own-products-or-services"></a>Dê permissão aos clientes no Partner Center para comprarem os seus próprios produtos ou serviços

**Funções adequadas**: Agente administrador | Agente comercial

Este artigo mostra como um parceiro no programa Fornecedor de Soluções em Nuvem (CSP) pode dar permissão a um cliente para comprar alguns dos seus próprios serviços ou recursos.

Os parceiros do programa CSP usam frequentemente o Partner Center e o seu mercado comercial para comprar soluções e serviços para os seus clientes. Os parceiros permitem então que alguns clientes prestem estes serviços diretamente a partir do portal Azure.

Eis um exemplo. Digamos que compre uma subscrição do plano Azure para um cliente no Partner Center. Em seguida, decide adicionar outros recursos ou serviços a essa subscrição em nome do cliente. Neste caso, poderá adicionar reservas Azure à subscrição do cliente (tais como, adicionar casos de máquinas virtuais e reservados). Poderá então permitir que o cliente adida ainda mais os recursos de reserva Azure no portal Azure.

Agora, com a funcionalidade **de permissões do Cliente,** você dá aos clientes mais opções de self-service com recursos Azure. Ao ligar permissões para o cliente, permite que os clientes comprem os seus próprios recursos (tais como, comprar as suas próprias reservas Azure).  

## <a name="overview-of-customer-permissions-in-partner-center"></a>Visão geral das permissões dos clientes no Partner Center

Utilize a página **Conta** do Cliente para ligar (ou desligar) as permissões do cliente. Atualmente, esta funcionalidade suporta:

- **Reservas Azure:** Ligar esta permissão permite ao cliente adquirir as suas próprias reservas Azure para uma subscrição específica da Azure que adquiriu para eles.

Antes de ligar as permissões do cliente, observe estes pontos importantes:

- Por predefinição, as permissões do cliente são automaticamente desativadas (desligadas) no Centro de Parceiros.

- Antes de poder ligar (ou desligar) permissões para um cliente, deve ser-lhe atribuída a função de Agente Administrador no Partner Center.

  Os parceiros atribuídos ao papel de Sales Agent ou Help Desk Agent têm acesso apenas de leitura e não podem ligar ou desligar as permissões do cliente.

- Pode ativar permissões (ativar) para qualquer cliente que escolher.

- Pode ligar (ou desligar) permissões de clientes utilizando o painel de instrumentos do Partner Center ou [as APIs do Partner Center](/partner-center/develop/manage-customers).

- Depois de ligar (ativar) permissões para um cliente específico, será responsável por pagar quaisquer compras posteriores efetuadas por esse cliente. Se os clientes quiserem trocar, cancelar ou renovar uma compra que tenham feito (ou quiserem alterar o âmbito inicial de uma reserva), não poderão fazê-lo por si mesmos. Eles precisam pedir-lhe, como parceiro, para ajudá-los a trocar, cancelar e renovar compras, ou fazer alterações posteriores no âmbito de uma reserva.  

- Depois de ligar permissões para um cliente específico, **não será** notificado de quaisquer compras posteriores efetuadas pelo cliente.

- As compras posteriores efetuam-se no Partner Center juntamente com quaisquer compras efetuadas por si. Pode encontrar estas compras na página de histórico da **Encomenda** do Cliente, na sua página reservas ou no Registo de **Atividades.** [](activity-logs.md)

>[!NOTE]
> Para obter informações sobre os preços que o cliente pagará e como ajudar os clientes a gerir as suas compras, consulte [os clientes da Help para gerir as reservas que comprarem.](give-customers-permission.md#help-customers-manage-reservations-they-purchase)

## <a name="give-customers-permission-to-buy-their-own-azure-reservations"></a>Dê permissão aos clientes para comprarem as suas próprias reservas Azure

As reservas Azure são uma ótima maneira de comprar serviços Azure a uma tarifa com desconto. Para saber mais sobre os benefícios das reservas do Azure, veja [o que são Reservas Azure?](/azure/cost-management-billing/reservations/save-compute-costs-reservations)

Agora tem a opção de comprar reservas da Azure em nome dos seus clientes, como já deve ter feito. Ou, você pode dar permissão aos clientes para comprar as suas próprias reservas Azure.

>[!NOTE]
> Depois de dar permissão aos clientes para comprarem as suas próprias reservas Azure, ajude-os a gerir quaisquer reservas que comprem. Para mais informações, consulte [os clientes da Ajuda a gerir as reservas que compram.](give-customers-permission.md#help-customers-manage-reservations-they-purchase)

### <a name="to-enable-customers-to-buy-their-own-azure-reservations"></a>Para permitir que os clientes comprem as suas próprias reservas Azure

1. Verifique se o cliente tem um plano Azure existente ou subscrição Azure Global que adquiriu em seu nome.

2. Verifique se o cliente foi atribuído à função **Proprietário** para esta subscrição.

3. Habilita as permissões do cliente (ligue esta funcionalidade **On)** para adquirir as suas próprias reservas Azure.

Cada passo aparece abaixo.

### <a name="verify-the-customer-has-an-existing-azure-subscription"></a>Verifique se o cliente tem uma subscrição Azure existente

Antes de dar permissão aos clientes para comprarem as suas próprias reservas Azure, tem de verificar se o cliente tem um plano Azure existente ou uma subscrição da Azure Global. Se o cliente não apresentar nenhuma subscrição atual do Azure no Partner Center, tem de comprar uma subscrição para eles antes de ligar as permissões do cliente.

- Para ver se um cliente já tem uma subscrição Azure, inscreva-se no painel partner center e, em seguida, selecione **CSP** seguido por **Clientes**. Selecione o cliente específico da lista. Em seguida, **selecione Subscrições** e procure quaisquer subscrições baseadas em uso para o plano Azure ou Azure Global.

- Se um cliente não tiver uma subscrição Azure existente, pode comprar uma subscrição para eles. Ver [Comprar o plano Azure](purchase-azure-plan.md).

### <a name="verify-the-customer-has-been-assigned-the-correct-role-in-azure"></a>Verifique se o cliente foi atribuído o papel correto no Azure

Depois de verificar se o cliente tem uma subscrição Azure existente, também precisa verificar se os utilizadores-chave associados ao seu cliente foram atribuídos a função correta **de Proprietário** para essa subscrição Azure. Este é o acesso baseado em funções (RBAC) que o cliente precisa para comprar reservas Azure para uma subscrição Azure que adquiriu.

Alguns parceiros podem já ter atribuído a função **de Proprietário** a clientes que pretendam gerir e a provisionar ativamente os seus próprios recursos Azure. Se já atribuiu o estatuto **de Proprietário** a um cliente para gerir subscrições anteriores que adquiriu para eles, pode saltar este passo.  

> [!IMPORTANT]
> Se um cliente não tiver sido atribuído a função **Proprietário,** receberá um erro no portal Azure impedindo-os de comprar reservas Azure.

Para verificar se o cliente foi atribuído a função **Proprietário** para uma subscrição Azure:

1. Inscreva-se no painel do Centro [de Parceiros](https://partner.microsoft.com/dashboard).

2. Selecione **CSP,** em **seguida, Clientes** e selecione o cliente específico.

3. Selecione **Subscrições** para esse cliente e localize a subscrição específica do Azure.

4. Selecione o botão **Gerir** ao lado da subscrição do cliente. Ao fazê-lo, abre-se o [portal Azure](https://portal.azure.com/).

5. Para atribuir a função **Proprietário** a um utilizador específico, siga estes passos [Para atribuir um utilizador como administrador](/azure/cost-management-billing/manage/add-change-subscription-administrator#to-assign-a-user-as-an-administrator).

### <a name="turn-on-or-turn-off-customer-permissions-to-purchase-their-own-azure-reservations"></a>Ligue ou desligue as permissões do cliente para comprar as suas próprias reservas Azure

Depois de verificar se o cliente tem uma subscrição Azure existente e os utilizadores recebem a função **Proprietário** para essa subscrição, está pronto para ativar (ativar) permissões de clientes. Também pode usar estes passos para desativar (desativar) as permissões do cliente. Pode ativar ou desativar as permissões do cliente utilizando o painel de instrumentos do Partner Center ou [as APIs do Partner Center](/partner-center/develop/manage-customers).

Para ligar (ou desligar) permissões de clientes no Partner Center:

1. Inscreva-se no painel do Centro [de Parceiros](https://partner.microsoft.com/dashboard).

2. A partir do menu de navegação à esquerda, selecione **CSP,** em **seguida, Clientes**. Aparece uma lista de clientes.

3. Selecione um nome específico do cliente.

4. Selecione **Conta** no menu do cliente. A página **conta do** cliente aparece.

5. Localize a área de **permissões** do Cliente na parte inferior da página.

   :::image type="content" source="images/give-customers-permission-reservations.png" alt-text="Permissões do cliente na página conta." border="true":::

6. Sob **reservas Azure,** localize a opção **de compra do cliente.**

7. Para ativar as permissões do cliente, mova o interruptor ao lado desta opção para a posição **On.** Para desligar as permissões do cliente, mova o interruptor para a posição **desligada.**

>[!NOTE]
> Para saber o que mais acontece quando liga as permissões de um cliente para comprar as suas próprias reservas Azure, consulte [a visão geral das permissões dos clientes no Partner Center.](give-customers-permission.md#overview-of-customer-permissions-in-partner-center)
>
>Quando liga (ou desliga) as permissões do cliente, o registo de registos de atividade regista cada ação. (Este registo é acessível quando seleciona o ícone De Engrenagem a partir da parte superior do painel Partner Center). Quando ligar ou desligar as permissões do cliente, a ação aparecerá como **Criar Permissões de Compra de Clientes** ou **eliminar permissões de compra** do cliente no registo de Atividade.

## <a name="help-customers-manage-reservations-they-purchase"></a>Ajude os clientes a gerir as reservas que compram

Assim que der permissão aos clientes para adquirirem as suas próprias reservas Azure, pode ajudá-los a gerir melhor os recursos que comprarem. Os clientes podem gerir muitos aspetos das reservas do Azure diretamente a partir do [portal Azure.](https://portal.azure.com/) Eles vão precisar da sua ajuda para gerir alguns outros aspetos das reservas Azure que eles compram dentro da sua assinatura CSP.  

Ajude os clientes a entender mais sobre a gestão destes aspetos das reservas da Azure:

- Preços que os clientes vão pagar pelas reservas da Azure
- Como os clientes podem otimizar o uso das reservas do Azure
- O que acontece quando os clientes compram reservas com âmbito partilhado?
- O que acontece se os clientes quiserem alterar, cancelar e renovar uma reserva, ou alterar o seu âmbito de aplicação?

**Preços que os clientes pagarão pelas suas reservas.** O seu cliente irá comprar reservas Azure com base numa subscrição que comprou anteriormente na sua conta de faturação de parceiro CSP. O preço do cliente por quaisquer reservas Azure que comprem com base nesta subscrição também é definido por si. Este preço pode ser diferente do preço Web Direct que o cliente vê no portal Azure.

**Como os clientes podem otimizar o seu uso de uma reserva.** Alguns clientes poderão beneficiar de aprender mais sobre como otimizar o uso de uma reserva ou como atribuir o âmbito inicial de uma reserva durante a sua compra. Para mais informações, peça aos clientes para [lerEmsarsagens de gestão de recursos da Azure.](/azure/cost-management-billing/reservations/manage-reserved-vm-instance)

**O que acontece quando um cliente compra uma reserva com âmbito partilhado?** Quando os clientes adquirem uma reserva com base numa subscrição CSP anterior e atribuem um âmbito partilhado a essa reserva, quaisquer descontos que o cliente tenha sido dado pela CSP aplicar-se-ão à utilização correspondente para todas as subscrições que o parceiro CSP adquiriu para esse cliente.

**O que devem os clientes fazer se quiserem trocar, cancelar ou renovar uma compra que fizeram ou alterar o âmbito inicial de uma reserva?** Os clientes precisam de pedir ao seu parceiro que os ajude a alterar o âmbito inicial de uma reserva. Também precisam da ajuda de um parceiro para trocar, cancelar ou renovar uma reserva. Não podem realizar estas tarefas por si próprias com reservas baseadas em assinaturas adquiridas por um parceiro da CSP.

## <a name="next-steps"></a>Passos seguintes

- [Compre reservas da Azure em nome dos seus clientes](azure-reservations-buying.md)

- [Partner Center - Vender reservas da Microsoft](azure-reservations.md)

- [Gerir reservas da Azure em nome dos seus clientes](azure-reservations-manage.md)