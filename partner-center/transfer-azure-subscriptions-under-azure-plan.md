---
title: Transferir subscrição da Azure ao abrigo de um plano Azure para outro parceiro da CSP
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como alterar o parceiro de programa Fornecedor de Soluções em Nuvem associado às subscrições Azure de um cliente ao abrigo de um plano Azure.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: mckennaville
ms.author: mcville
ms.date: 07/21/2021
ms.openlocfilehash: 258b593935e9fd599e0f5c524cd7ec935c50bcad
ms.sourcegitcommit: d133c8b923b90ac5518cb989c0ce4dd69713abf4
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/22/2021
ms.locfileid: "114434137"
---
# <a name="transfer-a-customers-azure-subscriptions-to-a-different-partner-in-csp-under-an-azure-plan"></a>Transferir as subscrições Azure de um cliente para um parceiro diferente em CSP (ao abrigo de um plano Azure)

**Funções adequadas**: Administração de contas | Agente comercial | Agente de faturação

Este artigo descreve como um cliente pode mudar as suas subscrições Azure de um parceiro dentro do Fornecedor de Soluções em Nuvem (CSP) para outro ao abrigo de um plano Azure.

Para trocar as subscrições Azure de um cliente de um parceiro diferente, siga estes passos. Tanto o parceiro como o cliente têm passos a completar.

> [!Note]  
> Apenas os parceiros com uma relação de faturação direta com a Microsoft podem aceder à ferramenta de transição. Os Revendedores Indiretos devem trabalhar com os seus Fornecedores Indiretos para alavancar esta ferramenta de transição.

O cliente deve estar em conversações com ambos os parceiros (atuais e futuros) antes de esta ferramenta ser alavancada. Uma conversa offline tem de ser teve de evitar confusões e agitação. Além disso, os parceiros e clientes devem compreender estas considerações e pré-requisitos antes de iniciar uma transição:

**Principais considerações:**

- A Azure Reservas não vai mover-se com a subscrição para futuro parceiro
- Preços da CSP para serviços Azure no âmbito do parceiro atual não vão transitar
- A transferência [de subscrições anteriores da Azure (MS-AZR-0145p)](https://go.microsoft.com/fwlink/p/?linkid=2164140) resultará na conversão simultâneo dessas subscrições da Azure para novas subscrições de ofertas Azure dentro de um plano Azure
- Responsabilidades de apoio para cliente passarão para futuro parceiro
- Faturação e faturação vão passar para futuro parceiro no momento da transferência
- O Azure Role-Based Access Control (RBAC) não é afetado pela transferência
- A Administração em Nome da AOBO não será concedida por defeito ao futuro parceiro
- Os produtos de mercado de terceiros serão transferidos desde que os produtos passem no controlo de elegibilidade do Marketplace.
    - Não há descontos especiais ou restrições regionais
    - Os produtos não são baseados em subscrição
    - O futuro parceiro deve trabalhar com a editora para garantir que estão na lista de admissões para a implementação do produto
    - Se nem todas estas condições forem satisfeitas para transferir os produtos marketplace devem ser canceladas, as assinaturas Azure transferidas e, em seguida, recomprar produtos marketplace com o novo parceiro

**Pré-requisitos:**

- Cliente contrata atual parceiro CSP na sua intenção de transição
- Futuro parceiro da CSP trabalha com o cliente para garantir que as necessidades dos clientes podem ser satisfeitas
- Futuro parceiro da CSP estabelece uma relação com o cliente e compra um plano Azure antes do início da transição  
- Cliente deve assinar Acordo de Cliente da Microsoft com futuro parceiro CSP
- O futuro parceiro da CSP deve ter assinado o Acordo de Parceiros da Microsoft para utilizar esta ferramenta

> [!NOTE]
> Esta ferramenta de self-serve pode ser utilizada quando o atual parceiro do cliente tem a oferta anterior da Azure (MS-AZR-0145p) ou a oferta new azure (plano Azure). Em qualquer dos casos, a conclusão desta transferência resultará nas subscrições do Azure ao abrigo de um plano Azure com o futuro parceiro.

## <a name="customer-tasks-to-be-completed"></a>Tarefas do cliente a serem concluídas

Para transferir subscrições da Azure, o cliente deve iniciar o processo contactando o seu parceiro atual. Devem recolher o nome da empresa do seu atual parceiro e o ID da Microsoft para que o seu futuro parceiro possa preencher o formulário de pedido de transferência em seu nome.

O cliente também deve identificar as subscrições que pretende transferir do seu parceiro atual. Não pode mudar de parceiros para Office 365, Suíte de Mobilidade Empresarial ou Microsoft Dynamics CRM subscrições.

> [!NOTE]  
> É da responsabilidade do futuro parceiro completar o formulário de pedido de transferência que inicia o processo de transferência. A Microsoft não pode intervir em nome do cliente ou do parceiro atual. O cliente deve planear trabalhar em estreita colaboração com o seu futuro e atual parceiro para que a transição corra bem.

## <a name="future-partner-tasks-to-be-completed"></a>Futuras tarefas parceiras a completar

O futuro parceiro da subscrição precisa de preencher um formulário de pedido de transferência do Partner Center para solicitar uma transferência de assinatura:

1.  A partir do menu Partner Center, selecione **Clientes,** em seguida, selecione o cliente que deseja preencher um formulário de pedido de transferência em nome de.
2.  A partir do menu Cliente, **selecione Subscrições.**
3.  Selecione a secção **de pedido de Transferência.**
4.  A partir da **secção de pedido de transferência,** selecione Adicionar novo **pedido.**

    :::image type="content" source="images/modernazuretransfers/Transferrequestheader.png" alt-text="Secção de transferências.":::

5.  Preencha o novo formulário **de pedido de transferência.**

6.  Selecione **Enviar pedido de transferência**  >  **Enviar**.

    :::image type="content" source="images/modernazuretransfers/CompleteTrnasferRequestForm.png" alt-text="Formulário completo de pedido de transferência.":::

7.  Confirmação do pedido de transferência de revisão

    :::image type="content" source="images/modernazuretransfers/TransferPending.png" alt-text="Revisão pendente de transferência.":::

    > [!NOTE]
    > O futuro parceiro pode cancelar o pedido de transferência selecionando o pedido de **cancelamento** no canto superior direito apenas quando o estado do pedido de transferência estiver "pendente". Uma vez que o estado do pedido de transferência esteja "em andamento" ou "completo", os cancelamentos não serão possíveis.

## <a name="current-partner-tasks-to-be-completed"></a>Tarefas atuais do parceiro a completar

O agente administrador do cliente do atual parceiro receberá um e-mail que o seu cliente está a solicitar uma transferência das suas subscrições:

:::image type="content" source="images/modernazuretransfers/SourceReviewEmail.png" alt-text="A revisão.":::

Reveja e aceite o formulário de pedido de transferência do Partner Center para completar a transferência de subscrição.

> [!NOTE]  
> Se o atual parceiro não tomar medidas no prazo de 30 dias, o pedido expirará e o futuro parceiro terá de criar um novo pedido de transferência.

- Selecione Pedido de transferência de **Revisão** a partir do e-mail

   -ou-

1. A partir do menu Partner Center, selecione **Clientes,** em seguida, selecione o cliente que um pedido de transferência foi submetido em nome de.
2. A partir do menu Cliente, **selecione Subscrições.**
3. Selecione a secção **de pedido de Transferência.**
4.Expandir as informações de transferência selecionando o **ID do pedido** de transferência escolhido ao abrigo **dos pedidos recebidos**

:::image type="content" source="images/modernazuretransfers/ReviewRequest.png" alt-text="Fonte revê pedido de transferência.":::

5. Reveja o pedido de transferência. Selecione as subscrições solicitadas do Azure para transferir.
 
Antes de prosseguir, por favor, note:
- Deixará de ter acesso às subscrições selecionadas.
- Não será faturado para posterior utilização.
- As reservas da Azure não transferem com as assinaturas.

6. Em seguida, **selecione Aceitar e transferir** para concluir o processo de transferência.

:::image type="content" source="images/modernazuretransfers/SelectSubs.png" alt-text="Selecione subscrições para serem transferidas ao abrigo dos seus planos Azure.":::

Se o atual parceiro tiver um cliente com subscrições anteriores da oferta Azure (MS-AZR-0145p), continuará da mesma forma, escolhendo as subscrições para transferir, selecionando Aceitar e transferir para completar o processo de transferência.

7. Ver confirmação de aceitação de transferência.

   Neste momento, o futuro parceiro, o cliente e atual parceiro será notificado do pedido de transferência aceite por e-mail.

   Depois, a transição foi aceite, o estado de transferência pode permanecer pendente até 15 minutos enquanto o sistema é atualizado. Se demorar mais, o sistema continuará a tentar durante três dias. Se o estado de transferência ainda estiver pendente, o parceiro deverá apresentar um pedido de serviço.

   Uma vez concluída a transferência, as subscrições incluídas no pedido aparecerão no plano Azure do futuro parceiro, e deixarão de ser listadas consigo.

>[!Note]  
>Para Fornecedores Indiretos: Informe o seu Revendedor Indireto de que o pedido de transferência foi aceite.

### <a name="managing-your-transferred-customer-subscriptions"></a>Gerir as subscrições de clientes transferidas

- O acesso a utilizadores, grupos ou principais de serviço existentes que tenham sido atribuídos através do RBAC (controlo de acesso baseado em funções) do Azure, não é afetado durante a transição. O controlo de acesso baseado em funções [(Azure RBAC)](/azure/role-based-access-control/overview) ajuda o seu cliente a gerir quem tem acesso aos recursos Azure, o que pode fazer com esses recursos e a que áreas têm acesso. Como novo parceiro, não lhe é dado qualquer acesso RBAC aos recursos do seu cliente após a transferência de subscrição. O parceiro anterior do seu cliente mantém o seu acesso AO RBAC. Trabalhe com o seu cliente para entender quem tem informações sobre as suas subscrições e como fazer quaisquer alterações desejadas.

- Consequentemente, é importante que o seu cliente remova o acesso do Azure RBAC para o seu parceiro anterior e adicione acesso ao novo parceiro. Para obter mais informações sobre o seu cliente que dá novo acesso, consulte [o que é o controlo de acesso baseado em funções do Azure (Azure RBAC)?](/azure/role-based-access-control/overview) Para obter mais informações sobre o acesso do seu cliente ao RBAC do seu parceiro anterior, consulte [Remover uma atribuição de função](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment).

- Além disso, não obtém automaticamente acesso da [Administração em nome da (AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) às suas subscrições. A AOBO é necessária para que os parceiros possam gerir as subscrições Azure dos seus clientes em seu nome. Para obter mais informações sobre os privilégios Azure, consulte [Obter permissões para gerir o serviço ou subscrição de um cliente.](./customers-revoke-admin-privileges.md)

## <a name="next-steps"></a>Passos seguintes:

- [(Azure RBAC)](/azure/role-based-access-control/overview)
- [Obtenha permissões para gerir o serviço ou subscrição de um cliente.](./customers-revoke-admin-privileges.md)
