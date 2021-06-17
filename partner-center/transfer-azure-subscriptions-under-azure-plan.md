---
title: Transferir subscrição da Azure ao abrigo de um plano Azure para outro parceiro da CSP
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como alterar o parceiro do programa Cloud Solution Provider associado às subscrições Azure de um cliente ao abrigo de um plano Azure.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: mckennaville
ms.author: mcville
ms.date: 07/29/2020
ms.openlocfilehash: 092c76fb874eb7308bdb69503223f722657db957
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/17/2021
ms.locfileid: "112277322"
---
# <a name="transfer-a-customers-azure-plan-subscriptions-to-a-different-partner"></a><span data-ttu-id="4c8ba-103">Transferir subscrições do plano Azure de um cliente para um parceiro diferente</span><span class="sxs-lookup"><span data-stu-id="4c8ba-103">Transfer a customer's Azure plan subscriptions to a different partner</span></span>

<span data-ttu-id="4c8ba-104">**Funções adequadas**: Administração de contas | Agente comercial | Agente de faturação</span><span class="sxs-lookup"><span data-stu-id="4c8ba-104">**Appropriate roles**: Account admin | Sales agent | Billing agent</span></span>

<span data-ttu-id="4c8ba-105">Este artigo descreve como um cliente pode mudar as suas subscrições Azure ao abrigo de um plano Azure de um Cloud Solution Provider (CSP) para outro.</span><span class="sxs-lookup"><span data-stu-id="4c8ba-105">This article describes how a customer can switch their Azure subscriptions under an Azure plan from one Cloud Solution Provider (CSP) to another.</span></span>

<span data-ttu-id="4c8ba-106">Para trocar as subscrições Azure de um cliente de um parceiro diferente, siga estes passos.</span><span class="sxs-lookup"><span data-stu-id="4c8ba-106">To switch a customer's Azure subscriptions from a different partner, follow these steps.</span></span> <span data-ttu-id="4c8ba-107">Tanto o parceiro como o cliente têm passos a completar.</span><span class="sxs-lookup"><span data-stu-id="4c8ba-107">Both the partner and the customer have steps to complete.</span></span>

>[!Note]  
><span data-ttu-id="4c8ba-108">Apenas os parceiros com uma relação de faturação direta com a Microsoft podem aceder à ferramenta de transição.</span><span class="sxs-lookup"><span data-stu-id="4c8ba-108">Only partners with a direct billing relationship with Microsoft can access the transition tooling.</span></span> <span data-ttu-id="4c8ba-109">Os Revendedores Indiretos devem trabalhar com os seus Fornecedores Indiretos para alavancar esta ferramenta de transição.</span><span class="sxs-lookup"><span data-stu-id="4c8ba-109">Indirect Resellers must work with their Indirect Providers to leverage this transition tool.</span></span>

<span data-ttu-id="4c8ba-110">O cliente deve estar em conversações com ambos os parceiros (atuais e futuros) antes de esta ferramenta ser alavancada.</span><span class="sxs-lookup"><span data-stu-id="4c8ba-110">The customer must be in conversation with both partners (current and future) prior to this tool being leveraged.</span></span> <span data-ttu-id="4c8ba-111">Uma conversa offline tem de ser teve de evitar confusões e agitação.</span><span class="sxs-lookup"><span data-stu-id="4c8ba-111">An offline conversation needs to be had to avoid confusion and churn.</span></span> <span data-ttu-id="4c8ba-112">Além disso, os parceiros e clientes devem compreender estas considerações e pré-requisitos antes de iniciar uma transição:</span><span class="sxs-lookup"><span data-stu-id="4c8ba-112">In addition, partners and customers should understand these considerations and prerequisites prior to initiating a transition:</span></span>

<span data-ttu-id="4c8ba-113">**Principais considerações:**</span><span class="sxs-lookup"><span data-stu-id="4c8ba-113">**Key considerations:**</span></span>

- <span data-ttu-id="4c8ba-114">A Azure Reservas não vai mover-se com a subscrição para futuro parceiro</span><span class="sxs-lookup"><span data-stu-id="4c8ba-114">Azure Reservations will not move with the subscription to future partner</span></span>
- <span data-ttu-id="4c8ba-115">Preços da CSP para serviços Azure no âmbito do parceiro atual não vão transitar</span><span class="sxs-lookup"><span data-stu-id="4c8ba-115">CSP pricing for Azure services under current partner will not transition</span></span>  
- <span data-ttu-id="4c8ba-116">Responsabilidades de apoio para cliente passarão para futuro parceiro</span><span class="sxs-lookup"><span data-stu-id="4c8ba-116">Support responsibilities for customer will move to future partner</span></span>
- <span data-ttu-id="4c8ba-117">Faturação e faturação vão passar para futuro parceiro no momento da transferência</span><span class="sxs-lookup"><span data-stu-id="4c8ba-117">Billing and invoicing will move to future partner at time of transfer</span></span>
- <span data-ttu-id="4c8ba-118">O Azure Role-Based Access Control (RBAC) não é afetado pela transferência</span><span class="sxs-lookup"><span data-stu-id="4c8ba-118">Azure Role-Based Access Control (RBAC) is not affected by the transfer</span></span>
- <span data-ttu-id="4c8ba-119">A Administração em Nome da AOBO não será concedida por defeito ao futuro parceiro</span><span class="sxs-lookup"><span data-stu-id="4c8ba-119">Admin on Behalf Of (AOBO) will not be granted by default to the future partner</span></span>
- <span data-ttu-id="4c8ba-120">Os produtos de mercado de terceiros serão transferidos desde que os produtos passem no controlo de elegibilidade do Marketplace.</span><span class="sxs-lookup"><span data-stu-id="4c8ba-120">Third-party marketplace products will transfer as long as the products pass the Marketplace eligibility check.</span></span>
    - <span data-ttu-id="4c8ba-121">Não há descontos especiais ou restrições regionais</span><span class="sxs-lookup"><span data-stu-id="4c8ba-121">There are no special discounts or regional restrictions</span></span>
    - <span data-ttu-id="4c8ba-122">Os produtos não são baseados em subscrição</span><span class="sxs-lookup"><span data-stu-id="4c8ba-122">The products are non-subscription based</span></span>
    - <span data-ttu-id="4c8ba-123">O futuro parceiro deve trabalhar com a editora para se certificar de que estão na lista de autorizações para a implementação do produto</span><span class="sxs-lookup"><span data-stu-id="4c8ba-123">The future partner should work with the publisher to make sure they are on the allow list for deployment of the product</span></span>
    - <span data-ttu-id="4c8ba-124">Se nem todas estas condições forem satisfeitas para transferir os produtos marketplace devem ser canceladas, as assinaturas Azure transferidas e, em seguida, recomprar produtos marketplace com o novo parceiro</span><span class="sxs-lookup"><span data-stu-id="4c8ba-124">If not all of these conditions are met in order to transfer the Marketplace products should be canceled, the Azure subscriptions transferred, and then repurchase of Marketplace products with the new partner</span></span>

<span data-ttu-id="4c8ba-125">**Pré-requisitos:**</span><span class="sxs-lookup"><span data-stu-id="4c8ba-125">**Prerequisites:**</span></span>

- <span data-ttu-id="4c8ba-126">Cliente contrata atual parceiro CSP na sua intenção de transição</span><span class="sxs-lookup"><span data-stu-id="4c8ba-126">Customer engages current CSP partner on their intent to transition</span></span>
- <span data-ttu-id="4c8ba-127">Futuro parceiro da CSP trabalha com o cliente para garantir que as necessidades dos clientes podem ser satisfeitas</span><span class="sxs-lookup"><span data-stu-id="4c8ba-127">Future CSP partner works with customer to ensure customer needs can be met</span></span>
- <span data-ttu-id="4c8ba-128">Futuro parceiro da CSP estabelece uma relação com o cliente e compra um plano Azure antes do início da transição</span><span class="sxs-lookup"><span data-stu-id="4c8ba-128">Future CSP partner establishes a relationship with customer and purchases an Azure plan before the transition begins</span></span>  
- <span data-ttu-id="4c8ba-129">Cliente deve assinar Acordo de Cliente da Microsoft com futuro parceiro CSP</span><span class="sxs-lookup"><span data-stu-id="4c8ba-129">Customer must sign Microsoft Customer Agreement with future CSP partner</span></span>
- <span data-ttu-id="4c8ba-130">O futuro parceiro da CSP deve ter assinado o Acordo de Parceiros da Microsoft para utilizar esta ferramenta</span><span class="sxs-lookup"><span data-stu-id="4c8ba-130">Future CSP partner must have signed the Microsoft Partner Agreement to use this tool</span></span>

## <a name="customer-tasks-to-be-completed"></a><span data-ttu-id="4c8ba-131">Tarefas do cliente a serem concluídas</span><span class="sxs-lookup"><span data-stu-id="4c8ba-131">Customer tasks to be completed</span></span>

<span data-ttu-id="4c8ba-132">Para transferir uma subscrição da Azure ao abrigo de um plano Azure, o cliente deve iniciar o processo contactando o seu parceiro atual.</span><span class="sxs-lookup"><span data-stu-id="4c8ba-132">To transfer an Azure subscription under an Azure plan, the customer must start the process by contacting their current partner.</span></span> <span data-ttu-id="4c8ba-133">Devem recolher o nome e o domínio da empresa do seu atual parceiro para que o seu futuro parceiro possa preencher o formulário de pedido de transferência em seu nome.</span><span class="sxs-lookup"><span data-stu-id="4c8ba-133">They should collect their current partner's company name and domain so their future partner can complete the transfer request form on their behalf.</span></span>

<span data-ttu-id="4c8ba-134">O cliente também deve identificar as subscrições que pretende transferir do seu parceiro atual.</span><span class="sxs-lookup"><span data-stu-id="4c8ba-134">The customer must also identify the subscriptions they wish to transfer from their current partner.</span></span> <span data-ttu-id="4c8ba-135">Não é possível alterar parceiros para as assinaturas Office 365, Enterprise Mobility Suite ou Microsoft Dynamics CRM.</span><span class="sxs-lookup"><span data-stu-id="4c8ba-135">You can't change partners for Office 365, Enterprise Mobility Suite, or Microsoft Dynamics CRM subscriptions.</span></span>

>[!Note]  
><span data-ttu-id="4c8ba-136">É da responsabilidade do futuro parceiro completar o formulário de pedido de transferência que inicia o processo de transferência.</span><span class="sxs-lookup"><span data-stu-id="4c8ba-136">It is the future partner's responsibility to complete the transfer request form that initiates the transfer process.</span></span> <span data-ttu-id="4c8ba-137">A Microsoft não pode intervir em nome do cliente ou do parceiro atual.</span><span class="sxs-lookup"><span data-stu-id="4c8ba-137">Microsoft cannot intervene on behalf of the customer or the current partner.</span></span> <span data-ttu-id="4c8ba-138">O cliente deve planear trabalhar em estreita colaboração com o seu futuro e atual parceiro para que a transição corra bem.</span><span class="sxs-lookup"><span data-stu-id="4c8ba-138">The customer should plan to work closely with their future and current partner to make the transition go smoothly.</span></span>

## <a name="future-partner-tasks-to-be-completed"></a><span data-ttu-id="4c8ba-139">Futuras tarefas parceiras a completar</span><span class="sxs-lookup"><span data-stu-id="4c8ba-139">Future partner tasks to be completed</span></span>

<span data-ttu-id="4c8ba-140">O futuro parceiro da subscrição precisa de preencher um formulário de pedido de transferência do Partner Center para solicitar uma transferência de assinatura:</span><span class="sxs-lookup"><span data-stu-id="4c8ba-140">The future partner of the subscription needs to complete a transfer request form from Partner Center to request a subscription transfer:</span></span>

1.  <span data-ttu-id="4c8ba-141">A partir do menu Partner Center, selecione **Clientes,** em seguida, selecione o cliente que deseja preencher um formulário de pedido de transferência em nome de.</span><span class="sxs-lookup"><span data-stu-id="4c8ba-141">From the Partner Center menu, select **Customers**, then select the customer you wish to complete a transfer request form on behalf of.</span></span>
2.  <span data-ttu-id="4c8ba-142">A partir do menu Cliente, **selecione Subscrições.**</span><span class="sxs-lookup"><span data-stu-id="4c8ba-142">From the Customer menu, select **Subscriptions**.</span></span>
3.  <span data-ttu-id="4c8ba-143">Selecione a secção **de pedido de Transferência.**</span><span class="sxs-lookup"><span data-stu-id="4c8ba-143">Select the **Transfer request** section.</span></span>
4.  <span data-ttu-id="4c8ba-144">A partir da **secção de pedido de transferência,** selecione Adicionar novo **pedido.**</span><span class="sxs-lookup"><span data-stu-id="4c8ba-144">From the **Transfer request section**, select **Add new request**.</span></span>

    :::image type="content" source="images/modernazuretransfers/Transferrequestheader.png" alt-text="Secção de transferências.":::

5.  <span data-ttu-id="4c8ba-146">Preencha o novo formulário **de pedido de transferência.**</span><span class="sxs-lookup"><span data-stu-id="4c8ba-146">Complete the **New transfer request** form.</span></span>

6.  <span data-ttu-id="4c8ba-147">Selecione **Enviar pedido de transferência**  >  **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="4c8ba-147">Select **Send transfer request** > **Send**.</span></span>

    :::image type="content" source="images/modernazuretransfers/CompleteTrnasferRequestForm.png" alt-text="Formulário completo de pedido de transferência.":::

7.  <span data-ttu-id="4c8ba-149">Confirmação do pedido de transferência de revisão</span><span class="sxs-lookup"><span data-stu-id="4c8ba-149">Review Transfer request confirmation</span></span>

    :::image type="content" source="images/modernazuretransfers/TransferPending.png" alt-text="Revisão pendente de transferência.":::

    >[!Note]
    ><span data-ttu-id="4c8ba-151">O futuro parceiro pode cancelar o pedido de transferência selecionando o pedido de **cancelamento** no canto superior direito apenas quando o estado do pedido de transferência estiver "pendente".</span><span class="sxs-lookup"><span data-stu-id="4c8ba-151">The future partner can cancel the transfer request by selecting **cancel request** in the upper right-hand corner only when the transfer request status is “pending”.</span></span> <span data-ttu-id="4c8ba-152">Uma vez que o estado do pedido de transferência esteja "em andamento" ou "completo", os cancelamentos não serão possíveis.</span><span class="sxs-lookup"><span data-stu-id="4c8ba-152">Once the transfer request status is “in progress” or “complete”, cancellations will not be possible.</span></span>

## <a name="current-partner-tasks-to-be-completed"></a><span data-ttu-id="4c8ba-153">Tarefas atuais do parceiro a completar</span><span class="sxs-lookup"><span data-stu-id="4c8ba-153">Current partner tasks to be completed</span></span>

<span data-ttu-id="4c8ba-154">O agente administrador do cliente do atual parceiro receberá um e-mail que o seu cliente está a solicitar uma transferência das suas subscrições:</span><span class="sxs-lookup"><span data-stu-id="4c8ba-154">The current partner's Admin Agent of the customer will receive an email that their customer is requesting a transfer of their subscriptions:</span></span>

:::image type="content" source="images/modernazuretransfers/SourceReviewEmail.png" alt-text="A revisão.":::

<span data-ttu-id="4c8ba-156">Reveja e aceite o formulário de pedido de transferência do Partner Center para completar a transferência de subscrição.</span><span class="sxs-lookup"><span data-stu-id="4c8ba-156">Review and accept the transfer request form from Partner Center to complete the subscription transfer.</span></span>

>[!Note]  
><span data-ttu-id="4c8ba-157">Se o atual parceiro não tomar medidas no prazo de 30 dias, o pedido expirará e o futuro parceiro terá de criar um novo pedido de transferência.</span><span class="sxs-lookup"><span data-stu-id="4c8ba-157">If no action is taken by the current partner within 30 days the request will expire and the future partner will have a to create a new transfer request.</span></span>

1.  <span data-ttu-id="4c8ba-158">Selecione Pedido de transferência de **Revisão** a partir do e-mail OR</span><span class="sxs-lookup"><span data-stu-id="4c8ba-158">Select **Review transfer Request** from the email OR</span></span>
1.  <span data-ttu-id="4c8ba-159">A partir do menu Partner Center, selecione **Clientes,** em seguida, selecione o cliente que um pedido de transferência foi submetido em nome de.</span><span class="sxs-lookup"><span data-stu-id="4c8ba-159">From the Partner Center menu, select **Customers**, then select the customer that a transfer request has been submitted on behalf of.</span></span>
2.  <span data-ttu-id="4c8ba-160">A partir do menu Cliente, **selecione Subscrições.**</span><span class="sxs-lookup"><span data-stu-id="4c8ba-160">From the Customer menu, select **Subscriptions**.</span></span>
3.  <span data-ttu-id="4c8ba-161">Selecione a secção **de pedido de Transferência.**</span><span class="sxs-lookup"><span data-stu-id="4c8ba-161">Select the **Transfer request** section.</span></span>
4.  <span data-ttu-id="4c8ba-162">Expandir as informações de transferência selecionando o **ID do pedido** de transferência escolhido nos **pedidos recebidos**</span><span class="sxs-lookup"><span data-stu-id="4c8ba-162">Expand transfer information by selecting the chosen **Transfer request ID** under **Received requests**</span></span>

:::image type="content" source="images/modernazuretransfers/ReviewRequest.png" alt-text="Fonte revê pedido de transferência.":::

5.  <span data-ttu-id="4c8ba-164">Reveja o pedido de transferência.</span><span class="sxs-lookup"><span data-stu-id="4c8ba-164">Review transfer request.</span></span> <span data-ttu-id="4c8ba-165">Selecione as subscrições solicitadas do Azure para transferir.</span><span class="sxs-lookup"><span data-stu-id="4c8ba-165">Select the requested Azure subscriptions to transfer.</span></span>

>[!Note]  
> <span data-ttu-id="4c8ba-166">Antes de prosseguir, note: Deixará de ter acesso às subscrições selecionadas.</span><span class="sxs-lookup"><span data-stu-id="4c8ba-166">Before proceeding please note: You will no longer have access to the selected subscriptions.</span></span>
> <span data-ttu-id="4c8ba-167">Não será faturado para posterior utilização.</span><span class="sxs-lookup"><span data-stu-id="4c8ba-167">You will not be invoiced for further usage.</span></span>
> <span data-ttu-id="4c8ba-168">As reservas da Azure não transferem com as assinaturas.</span><span class="sxs-lookup"><span data-stu-id="4c8ba-168">Azure reservations do not transfer with the subscriptions.</span></span>

6.  <span data-ttu-id="4c8ba-169">Em seguida, **selecione Aceitar e transferir** para concluir o processo de transferência.</span><span class="sxs-lookup"><span data-stu-id="4c8ba-169">Then select **Accept and transfer** to complete the transfer process.</span></span>

:::image type="content" source="images/modernazuretransfers/SelectSubs.png" alt-text="Selecione subscrições para serem transferidas ao abrigo dos seus planos Azure.":::

7.  <span data-ttu-id="4c8ba-171">Ver confirmação de aceitação de transferência.</span><span class="sxs-lookup"><span data-stu-id="4c8ba-171">View transfer acceptance confirmation.</span></span>

   <span data-ttu-id="4c8ba-172">Neste momento, o futuro parceiro, o cliente e atual parceiro será notificado do pedido de transferência aceite por e-mail.</span><span class="sxs-lookup"><span data-stu-id="4c8ba-172">At this point, the future partner, the customer, and current partner will be notified of the accepted transfer request via email.</span></span>

   <span data-ttu-id="4c8ba-173">Depois, a transição foi aceite, o estado de transferência pode permanecer pendente até 15 minutos enquanto o sistema é atualizado.</span><span class="sxs-lookup"><span data-stu-id="4c8ba-173">After, the transition has been accepted the transfer status might remain Pending for up to 15 minutes while the system is updated.</span></span> <span data-ttu-id="4c8ba-174">Se demorar mais, o sistema continuará a tentar durante três dias.</span><span class="sxs-lookup"><span data-stu-id="4c8ba-174">If it takes longer, the system will keep trying for three days.</span></span> <span data-ttu-id="4c8ba-175">Se o estado de transferência ainda estiver pendente, o parceiro deverá apresentar um pedido de serviço.</span><span class="sxs-lookup"><span data-stu-id="4c8ba-175">If the transfer status still remains Pending, the partner should submit a service request.</span></span>

   <span data-ttu-id="4c8ba-176">Uma vez concluída a transferência, as subscrições incluídas no pedido aparecerão no plano Azure do futuro parceiro, e deixarão de ser listadas consigo.</span><span class="sxs-lookup"><span data-stu-id="4c8ba-176">Once the transfer is complete, the subscriptions included within the request will appear in the Azure plan of the future partner, and no longer be listed with you.</span></span>

>[!Note]  
><span data-ttu-id="4c8ba-177">Para Fornecedores Indiretos: Informe o seu Revendedor Indireto de que o pedido de transferência foi aceite.</span><span class="sxs-lookup"><span data-stu-id="4c8ba-177">For Indirect Providers: Please inform your Indirect Reseller that the transfer request has been accepted.</span></span>

### <a name="managing-your-transferred-customer-subscriptions"></a><span data-ttu-id="4c8ba-178">Gerir as subscrições de clientes transferidas</span><span class="sxs-lookup"><span data-stu-id="4c8ba-178">Managing your transferred customer subscriptions</span></span>

- <span data-ttu-id="4c8ba-179">O acesso a utilizadores, grupos ou principais de serviço existentes que tenham sido atribuídos através do RBAC (controlo de acesso baseado em funções) do Azure, não é afetado durante a transição.</span><span class="sxs-lookup"><span data-stu-id="4c8ba-179">Access to existing users, groups, or service principals that were assigned using Azure role-based access control (RBAC) isn't affected during the transition.</span></span> <span data-ttu-id="4c8ba-180">O controlo de acesso baseado em funções [(Azure RBAC)](/azure/role-based-access-control/overview) ajuda o seu cliente a gerir quem tem acesso aos recursos Azure, o que pode fazer com esses recursos e a que áreas têm acesso.</span><span class="sxs-lookup"><span data-stu-id="4c8ba-180">Azure role-based access control [(Azure RBAC)](/azure/role-based-access-control/overview) helps your customer manage who has access to Azure resources, what they can do with those resources, and what areas they have access to.</span></span> <span data-ttu-id="4c8ba-181">Como novo parceiro, não lhe é dado qualquer acesso RBAC aos recursos do seu cliente após a transferência de subscrição.</span><span class="sxs-lookup"><span data-stu-id="4c8ba-181">As the new partner you aren't given any RBAC access to your customer’s resources after the subscription transfer.</span></span> <span data-ttu-id="4c8ba-182">O parceiro anterior do seu cliente mantém o seu acesso AO RBAC.</span><span class="sxs-lookup"><span data-stu-id="4c8ba-182">Your customer’s previous partner retains their RBAC access.</span></span> <span data-ttu-id="4c8ba-183">Trabalhe com o seu cliente para entender quem tem informações sobre as suas subscrições e como fazer quaisquer alterações desejadas.</span><span class="sxs-lookup"><span data-stu-id="4c8ba-183">Work with your customer to understand who has insight into their subscriptions and how to make any wanted changes.</span></span>

- <span data-ttu-id="4c8ba-184">Consequentemente, é importante que o seu cliente remova o acesso do Azure RBAC para o seu parceiro anterior e adicione acesso ao novo parceiro.</span><span class="sxs-lookup"><span data-stu-id="4c8ba-184">Consequently, it’s important that your customer removes Azure RBAC access for their previous partner and add access for the new partner.</span></span> <span data-ttu-id="4c8ba-185">Para obter mais informações sobre o seu cliente que dá novo acesso, consulte [o que é o controlo de acesso baseado em funções do Azure (Azure RBAC)?](/azure/role-based-access-control/overview)</span><span class="sxs-lookup"><span data-stu-id="4c8ba-185">For more information about your customer giving new access, see [What is Azure role-based access control (Azure RBAC)?](/azure/role-based-access-control/overview)</span></span> <span data-ttu-id="4c8ba-186">Para obter mais informações sobre o acesso do seu cliente ao RBAC do seu parceiro anterior, consulte [Remover uma atribuição de função](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment).</span><span class="sxs-lookup"><span data-stu-id="4c8ba-186">For more information about your customer removing your previous partner’s RBAC access, see [Remove a role assignment](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment).</span></span>

- <span data-ttu-id="4c8ba-187">Além disso, não obtém automaticamente acesso da [Administração em nome da (AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) às suas subscrições.</span><span class="sxs-lookup"><span data-stu-id="4c8ba-187">Additionally, you don’t automatically get [Admin on Behalf Of (AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) access to your subscriptions.</span></span> <span data-ttu-id="4c8ba-188">A AOBO é necessária para que os parceiros possam gerir as subscrições Azure dos seus clientes em seu nome.</span><span class="sxs-lookup"><span data-stu-id="4c8ba-188">AOBO is necessary for partner’s to manage their customer’s Azure subscriptions on their behalf.</span></span> <span data-ttu-id="4c8ba-189">Para obter mais informações sobre os privilégios Azure, consulte [Obter permissões para gerir o serviço ou subscrição de um cliente.](./customers-revoke-admin-privileges.md)</span><span class="sxs-lookup"><span data-stu-id="4c8ba-189">For more information about Azure privileges, see [Obtain permissions to manage a customer’s service or subscription.](./customers-revoke-admin-privileges.md)</span></span>

## <a name="next-steps"></a><span data-ttu-id="4c8ba-190">Passos seguintes:</span><span class="sxs-lookup"><span data-stu-id="4c8ba-190">Next steps:</span></span>

- [<span data-ttu-id="4c8ba-191">(Azure RBAC)</span><span class="sxs-lookup"><span data-stu-id="4c8ba-191">(Azure RBAC)</span></span>](/azure/role-based-access-control/overview)
- [<span data-ttu-id="4c8ba-192">Obtenha permissões para gerir o serviço ou subscrição de um cliente.</span><span class="sxs-lookup"><span data-stu-id="4c8ba-192">Obtain permissions to manage a customer’s service or subscription.</span></span>](./customers-revoke-admin-privileges.md)
