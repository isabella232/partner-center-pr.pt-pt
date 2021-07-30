---
title: Transferir subscrição da Azure ao abrigo de um plano Azure para outro parceiro da CSP
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Saiba como alterar o parceiro de programa Fornecedor de Soluções em Nuvem associado às subscrições Azure de um cliente ao abrigo de um plano Azure.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: mckennaville
ms.author: mcville
ms.date: 07/21/2021
ms.openlocfilehash: 14f03a8eb899f7224a38b0f998edd72077b34b3b
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/29/2021
ms.locfileid: "114844280"
---
# <a name="transfer-a-customers-azure-subscriptions-to-a-different-csp-under-an-azure-plan"></a>Transferir as subscrições Azure de um cliente para um CSP diferente (ao abrigo de um plano Azure)

**Funções adequadas**: Administração de contas | Agente comercial | Agente de faturação

Este artigo descreve como os clientes podem alterar as suas subscrições Azure de um parceiro no programa Fornecedor de Soluções em Nuvem (CSP) para outro, ao abrigo de um plano Azure.

Para trocar as subscrições Azure de um cliente de um parceiro diferente, siga estes passos. O atual parceiro, o futuro parceiro, e o cliente têm todos passos a completar.

> [!Note]  
> Apenas os parceiros que tenham uma relação de faturação direta com a Microsoft podem aceder à ferramenta de transição. Os revendedores indiretos precisam de trabalhar com os seus fornecedores indiretos para utilizar esta ferramenta de transição.

O cliente precisa de comunicar com o parceiro atual e futuro antes de a ferramenta de transição poder ser utilizada. É necessário que ocorra uma conversa offline para evitar confusões e agitação. Os parceiros e clientes devem compreender as seguintes considerações e pré-requisitos antes de iniciar uma transição.

## <a name="considerations"></a>Considerações

- A Azure Reservations não se move com uma subscrição do futuro parceiro.
- Os preços da CSP para os serviços da Azure no âmbito do atual parceiro não vão transitar.
- Se transferir [subscrições anteriores da oferta Azure (MS-AZR-0145p),](https://go.microsoft.com/fwlink/p/?linkid=2164140) essas subscrições Azure serão simultaneamente convertidas para novas subscrições de ofertas Azure dentro de um plano Azure.
- As responsabilidades de apoio para o cliente passarão para o futuro parceiro.
- A faturação e a faturação passarão para o futuro parceiro quando a subscrição for transferida.
- O controlo de acesso baseado em funções (RBAC) não é afetado por transferências.
- A Administração em Nome da AOBO não será concedida por defeito ao futuro parceiro.
- Os produtos Azure Marketplace de terceiros serão transferidos desde que os produtos passem na verificação de elegibilidade do Azure Marketplace.
    - Não existem descontos especiais ou restrições regionais.
    - Os produtos não são baseados em subscrição.
    - O futuro parceiro deve trabalhar com a editora para garantir que a editora está na lista de admissões para a implementação do produto.
    - Se alguma destas condições não for satisfeita, os produtos Azure Marketplace devem ser cancelados. Em seguida, as assinaturas Azure devem ser transferidas e os produtos Azure Marketplace devem ser comprados com o novo parceiro.

## <a name="prerequisites"></a>Pré-requisitos

- O cliente notifica o atual parceiro da CSP da intenção de transição.
- O futuro parceiro da CSP trabalha com o cliente para garantir que as necessidades do cliente podem ser satisfeitas.
- O futuro parceiro da CSP estabelece uma relação com o cliente e compra um plano Azure antes do início da transição.
- O cliente assina um Acordo de Cliente da Microsoft com o futuro parceiro CSP.
- O futuro parceiro CSP assina o Microsoft Partner Agreement antes de utilizar a ferramenta de transição.

> [!NOTE]
> A ferramenta de transição de autosserviço pode ser utilizada quando o atual parceiro do cliente tem a oferta anterior do Azure (MS-AZR-0145p) ou a nova oferta Azure (plano Azure). Em qualquer dos casos, quando a transferência estiver concluída, as assinaturas Azure estarão ao abrigo de um plano Azure com o futuro parceiro.

## <a name="customer-tasks"></a>Tarefas do cliente

Para transferir subscrições da Azure, o cliente deve iniciar o processo contactando o parceiro atual. O cliente deve recolher o nome da empresa do atual parceiro e o ID da Microsoft para que o futuro parceiro possa preencher o formulário de pedido de transferência em nome do cliente.

Os clientes também devem identificar as subscrições que pretendem transferir do atual parceiro. Não pode mudar de parceiros para Office 365, Suíte de Mobilidade Empresarial ou Microsoft Dynamics CRM subscrições.

> [!NOTE]  
> É da responsabilidade do futuro parceiro completar o formulário de pedido de transferência que inicia o processo de transferência. A Microsoft não pode intervir em nome do cliente ou do parceiro atual. O cliente deve planear trabalhar em estreita colaboração com o futuro e os atuais parceiros para garantir que a transição desa correr sem problemas.

## <a name="future-partner-tasks"></a>Futuras tarefas de parceiros 

O futuro parceiro da subscrição precisa de preencher um formulário de pedido de transferência do Partner Center para solicitar uma transferência de assinatura:

1.  No painel esquerdo do Partner Center, selecione **Clientes** e, em seguida, selecione o cliente para quem deseja completar o pedido de transferência.
2.  No menu específico do cliente, **selecione Subscrições**.
3.  No separador **pedidos de transferência,** selecione **Adicionar novo pedido**:

    :::image type="content" source="images/modernazuretransfers/Transferrequestheader.png" alt-text="Screenshot que mostra o separador de pedidos de transferência.":::

5.  Preencha o novo formulário **de pedido de transferência:**

    :::image type="content" source="images/modernazuretransfers/CompleteTrnasferRequestForm.png" alt-text="Screenshot que mostra o novo formulário de pedido de transferência.":::

6.  Selecione **Enviar pedido de transferência**  >  **Enviar**.

7.  Reveja a confirmação do pedido de transferência:

    :::image type="content" source="images/modernazuretransfers/TransferPending.png" alt-text="Screenshot que mostra uma confirmação de pedido de transferência.":::

    > [!NOTE]
    > O futuro parceiro pode cancelar o pedido de transferência selecionando o **pedido de Cancelamento** no canto superior direito da janela apenas quando o estado do pedido de transferência estiver "pendente". Após o estado do pedido de transferência estar "em andamento" ou "completo", os cancelamentos não são possíveis.

## <a name="current-partner-tasks"></a>Tarefas de parceiro atuais 

O agente administrador do atual parceiro para o cliente receberá um e-mail indicando que um cliente está solicitando uma transferência de subscrições:

:::image type="content" source="images/modernazuretransfers/SourceReviewEmail.png" alt-text="Screenshot que mostra uma notificação de e-mail de um pedido de transferência do cliente.":::

O parceiro atual precisa de rever e aceitar o formulário de pedido de transferência do Partner Center para completar a transferência de subscrição.

> [!NOTE]  
> Se o atual parceiro não responder no prazo de 30 dias, o pedido expirará e o futuro parceiro necessitará de um para criar um novo pedido de transferência.

1. Efetue uma das seguintes ações: 
   - Selecione **Pedido de transferência de Revisão** no e-mail.

     ou

    - No painel esquerdo do Partner Center, selecione **Clientes** e, em seguida, selecione o cliente para o qual o pedido de transferência foi submetido.
      1. No menu específico do cliente, **selecione Subscrições**.
      1. No separador **pedidos de transferência,** expanda as informações de transferência selecionando o **ID** do pedido de transferência nos **pedidos recebidos:**

      :::image type="content" source="images/modernazuretransfers/ReviewRequest.png" alt-text="Screenshot que mostra o separador de pedidos de transferência, como visto pelo parceiro atual.":::

5. Reveja o pedido de transferência. Selecione as subscrições solicitadas do Azure para transferir.
 
   Antes de continuar, note:
   - Deixará de ter acesso às subscrições selecionadas.
   - Não será faturado para mais uso.
   - As reservas do Azure não transferem com subscrições.

6. Selecione **Aceitar e transferir** para completar o processo de transferência:

   :::image type="content" source="images/modernazuretransfers/SelectSubs.png" alt-text="Screenshot que mostra o ecrã de pedido de transferência de Revisão.":::

   Se tiver um cliente com subscrições anteriores da oferta Azure (MS-AZR-0145p), continue da mesma forma, escolhendo as subscrições para transferir e, em seguida, selecionando **Aceitar e transferir** para completar o processo de transferência.

7. Consulte a confirmação de aceitação da transferência.

   Neste momento, um e-mail notifica o futuro parceiro, o cliente e o atual parceiro sobre o pedido de transferência aceite.

   Após a aceitação da transição, o estado de transferência pode permanecer "pendente" até 15 minutos enquanto o sistema é atualizado. Se este processo demorar mais tempo, o sistema continuará a tentar durante três dias. Se o estado de transferência permanecer em "pendente" por mais de três dias, o parceiro deverá apresentar um pedido de serviço.

   Após a conclusão da transferência, as subscrições incluídas no pedido aparecerão no plano Azure do futuro parceiro. Deixará de estar listado com o atual parceiro.

>[!Note]  
>Os fornecedores indiretos devem informar os seus revendedores indiretos de que o pedido de transferência foi aceite.

### <a name="managing-your-transferred-customer-subscriptions"></a>Gerir as subscrições de clientes transferidas

O acesso aos utilizadores, grupos ou princípios de serviço existentes que foram atribuídos através do RBAC Azure não é afetado durante a transição. [O Azure RBAC](/azure/role-based-access-control/overview) ajuda o seu cliente a gerir quem tem acesso aos recursos da Azure, o que pode fazer com esses recursos e quais as áreas a que tem acesso. 

Como novo parceiro, não terá qualquer acesso RBAC aos recursos do seu cliente após a transferência de subscrição. O parceiro anterior do seu cliente mantém o acesso ao RBAC. Trabalhe com o seu cliente para entender quem tem informações sobre as subscrições e como fazer as alterações necessárias.

O seu cliente terá de remover o acesso do Azure RBAC ao parceiro anterior e adicionar-lhe acesso. Para obter mais informações sobre o acesso, consulte [o que é o controlo de acesso baseado em funções do Azure (Azure RBAC)?](/azure/role-based-access-control/overview) Para obter mais informações sobre a remoção do acesso, consulte [Remover uma atribuição de funções](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment).

Além disso, não obtém automaticamente acesso da [Administração em nome da (AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) às suas subscrições. A AOBO é necessária para que possa gerir as subscrições Azure do seu cliente. Para obter mais informações sobre os privilégios do Azure, veja [Obter permissões para gerir o serviço ou a subscrição de um cliente](./customers-revoke-admin-privileges.md).

## <a name="next-steps"></a>Passos seguintes

- [RBAC do Azure](/azure/role-based-access-control/overview)
- [Obter permissões para gerir o serviço ou subscrição de um cliente](./customers-revoke-admin-privileges.md)
