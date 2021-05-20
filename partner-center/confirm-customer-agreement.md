---
title: Como confirmar que o seu cliente aceitou o Acordo de Cliente da Microsoft para o programa CSP
description: Os parceiros do Cloud Solution Provider (CSP) precisam confirmar a aceitação do cliente do Microsoft Customer Agreement antes de encomendar os serviços da Microsoft aos clientes.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 03/24/2021
ms.openlocfilehash: c75f129ae5a0755833462138f60901cc7ff36732
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148521"
---
# <a name="how-to-confirm-that-your-customer-has-accepted-the-microsoft-customer-agreement-to-the-csp-program"></a><span data-ttu-id="264f6-103">Como confirmar que o seu cliente aceitou o Acordo de Cliente da Microsoft para o programa CSP</span><span class="sxs-lookup"><span data-stu-id="264f6-103">How to confirm that your customer has accepted the Microsoft Customer Agreement to the CSP program</span></span>

<span data-ttu-id="264f6-104">**Funções adequadas**: Agente administrador | Agente comercial</span><span class="sxs-lookup"><span data-stu-id="264f6-104">**Appropriate roles**: Admin agent | Sales agent</span></span>


<span data-ttu-id="264f6-105">Os clientes têm duas opções para a forma como aceitam o Acordo de Cliente da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="264f6-105">Customers have two options for how they accept the Microsoft Customer Agreement.</span></span>

<span data-ttu-id="264f6-106">**Opção 1**: Atestado parceiro de aceitação do cliente - O Parceiro pode confirmar a aceitação do cliente utilizando o Partner Center API/SDK ou através do painel partner Center.</span><span class="sxs-lookup"><span data-stu-id="264f6-106">**Option 1**: Partner attestation of customer acceptance - Partner can confirm customer acceptance using Partner Center API/SDK or through the Partner Center dashboard.</span></span>

<span data-ttu-id="264f6-107">**Opção 2**: Aceitação direta do cliente - O parceiro pode convidar o cliente através de um URL para rever e aceitar o acordo no Microsoft 365 Admin Center.</span><span class="sxs-lookup"><span data-stu-id="264f6-107">**Option 2**: Customer direct acceptance - Partner can invite the customer via a URL to review and accept the agreement in the Microsoft 365 Admin Center.</span></span>

## <a name="access-microsoft-customer-agreement-template"></a><span data-ttu-id="264f6-108">Aceder ao modelo de Acordo de Cliente da Microsoft</span><span class="sxs-lookup"><span data-stu-id="264f6-108">Access Microsoft Customer Agreement template</span></span>

<span data-ttu-id="264f6-109">Pode descarregar manualmente a versão mais recente do modelo do Microsoft Customer Agreement a partir [daqui.](https://aka.ms/customeragreement)</span><span class="sxs-lookup"><span data-stu-id="264f6-109">You can manually download the latest version of the Microsoft Customer Agreement template from [here](https://aka.ms/customeragreement).</span></span> <span data-ttu-id="264f6-110">O Microsoft Customer Agreement é específico por país.</span><span class="sxs-lookup"><span data-stu-id="264f6-110">The Microsoft Customer Agreement is country-specific.</span></span> <span data-ttu-id="264f6-111">Ao solicitar o modelo do Contrato de Cliente da Microsoft, certifique-se de selecionar o país correto com base na localização do cliente.</span><span class="sxs-lookup"><span data-stu-id="264f6-111">When requesting the Microsoft Customer Agreement template, be sure to select the correct country based on the customer's location.</span></span>

## <a name="option-1-confirm-customer-acceptance-in-partner-center"></a><span data-ttu-id="264f6-112">Opção 1: Confirmar a aceitação do cliente no Partner Center</span><span class="sxs-lookup"><span data-stu-id="264f6-112">Option 1: Confirm customer acceptance in Partner Center</span></span>

<span data-ttu-id="264f6-113">Os parceiros de conta direta podem confirmar a aceitação do Cliente do Microsoft Customer Agreement no Partner Center para clientes novos e existentes.</span><span class="sxs-lookup"><span data-stu-id="264f6-113">Direct bill partners can confirm customer acceptance of the Microsoft Customer Agreement in Partner Center for new and existing customers.</span></span> <span data-ttu-id="264f6-114">Os revendedores indiretos não podem atestar em nome dos seus clientes e precisam de trabalhar com o seu Fornecedor Indireto para obter o atestado concluído.</span><span class="sxs-lookup"><span data-stu-id="264f6-114">Indirect resellers cannot attest on behalf of their customers and need to work with their Indirect Provider to get attestation completed.</span></span>

### <a name="confirm-customer-acceptance-for-new-customers"></a><span data-ttu-id="264f6-115">Confirme a aceitação do cliente para novos clientes</span><span class="sxs-lookup"><span data-stu-id="264f6-115">Confirm customer acceptance for new customers</span></span>

<span data-ttu-id="264f6-116">Quando criar um novo inquilino de clientes no Partner Center, utilize os seguintes passos para confirmar a aceitação do Cliente do Microsoft Customer Agreement.</span><span class="sxs-lookup"><span data-stu-id="264f6-116">When you create a new customer tenant in Partner Center, use the following steps to confirm the customer's acceptance of the Microsoft Customer Agreement.</span></span> <span data-ttu-id="264f6-117">Deve ser um agente administrativo ou agente comercial para executar estes passos.</span><span class="sxs-lookup"><span data-stu-id="264f6-117">You must be an Admin agent or Sales agent to perform these steps.</span></span>

1. <span data-ttu-id="264f6-118">Selecione **Clientes**, e depois **Novo cliente**.</span><span class="sxs-lookup"><span data-stu-id="264f6-118">Select **Customers**, and then **New customer**.</span></span>

2. <span data-ttu-id="264f6-119">Informação em **Conta,** introduza informação para a empresa e o seu contacto principal.</span><span class="sxs-lookup"><span data-stu-id="264f6-119">Under **Account info**, enter information for the company and its primary contact.</span></span>

3. <span data-ttu-id="264f6-120">De acordo com o **acordo da Microsoft,** selecione a caixa para atestar que o cliente aceitou o Acordo de Cliente da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="264f6-120">Under **Microsoft agreement**, select the box to attest that the customer has accepted the Microsoft Customer Agreement.</span></span>

4. <span data-ttu-id="264f6-121">Nos termos **da data de aceitação** do Acordo, insira a data adequada.</span><span class="sxs-lookup"><span data-stu-id="264f6-121">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="264f6-122">Não pode marcar isto para uma data futura.</span><span class="sxs-lookup"><span data-stu-id="264f6-122">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="264f6-123">Certifique-se de que as informações de contacto do utilizador primário apresentadas estão corretas.</span><span class="sxs-lookup"><span data-stu-id="264f6-123">Make sure that the primary user contact information displayed is correct.</span></span> <span data-ttu-id="264f6-124">Se estiver incorreto, selecione **Update** e introduza as informações precisas para a pessoa que aceitou o acordo.</span><span class="sxs-lookup"><span data-stu-id="264f6-124">If it's incorrect, select **Update** and enter the accurate information for the person who accepted the agreement.</span></span>

6. <span data-ttu-id="264f6-125">Selecione **Next** para continuar a criar o inquilino do cliente.</span><span class="sxs-lookup"><span data-stu-id="264f6-125">Select **Next** to continue creating the customer tenant.</span></span>

   :::image type="content" source="images/mca/newcustomeragreement.jpg" alt-text="Novo cliente":::  

### <a name="confirm-customer-acceptance-for-existing-customers"></a><span data-ttu-id="264f6-127">Confirme a aceitação do cliente para os clientes existentes</span><span class="sxs-lookup"><span data-stu-id="264f6-127">Confirm customer acceptance for existing customers</span></span>

<span data-ttu-id="264f6-128">Deve ser um agente administrativo ou agente comercial para fazer isto:</span><span class="sxs-lookup"><span data-stu-id="264f6-128">You must be an Admin agent or Sales agent to do this:</span></span>

1. <span data-ttu-id="264f6-129">Selecione **Clientes**.</span><span class="sxs-lookup"><span data-stu-id="264f6-129">Select **Customers**.</span></span> <span data-ttu-id="264f6-130">Encontre e selecione o cliente.</span><span class="sxs-lookup"><span data-stu-id="264f6-130">Find and select the customer.</span></span>

2. <span data-ttu-id="264f6-131">Selecione **informação de Conta**.</span><span class="sxs-lookup"><span data-stu-id="264f6-131">Select **Account info**.</span></span>

3. <span data-ttu-id="264f6-132">Ao abrigo **do Microsoft Customer Agreement**, selecione **Update**.</span><span class="sxs-lookup"><span data-stu-id="264f6-132">Under **Microsoft Customer Agreement**, select **Update**.</span></span>

4. <span data-ttu-id="264f6-133">Introduza o **Nome Próprio**, **Apelido,** **endereço de e-mail** e número de **telefone** (opcional) da pessoa que aceitou o acordo.</span><span class="sxs-lookup"><span data-stu-id="264f6-133">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the person who accepted the agreement.</span></span> <span data-ttu-id="264f6-134">Nos termos **da data de aceitação** do Acordo, insira a data adequada.</span><span class="sxs-lookup"><span data-stu-id="264f6-134">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="264f6-135">Não pode marcar isto para uma data futura.</span><span class="sxs-lookup"><span data-stu-id="264f6-135">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="264f6-136">**Selecione Save** e continue.</span><span class="sxs-lookup"><span data-stu-id="264f6-136">Select **Save** and continue.</span></span>

   :::image type="content" source="images/mcua2-update2.png" alt-text="Cliente existente":::

### <a name="retrieve-confirmation-of-customer-acceptance"></a><span data-ttu-id="264f6-138">Recuperar a confirmação da aceitação do cliente</span><span class="sxs-lookup"><span data-stu-id="264f6-138">Retrieve confirmation of customer acceptance</span></span>

<span data-ttu-id="264f6-139">Para obter a confirmação de que um cliente existente aceitou o Acordo de Cliente da Microsoft, utilize os seguintes passos.</span><span class="sxs-lookup"><span data-stu-id="264f6-139">To retrieve confirmation that an existing customer has accepted the Microsoft Customer Agreement, use the following steps.</span></span> <span data-ttu-id="264f6-140">Deves ser um agente administrativo ou agente comercial para fazer isto.</span><span class="sxs-lookup"><span data-stu-id="264f6-140">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="264f6-141">Selecione **Clientes** e, em seguida, encontre e selecione o cliente que deseja ver.</span><span class="sxs-lookup"><span data-stu-id="264f6-141">Select **Customers**, and then find and select the customer you want to see.</span></span>

2. <span data-ttu-id="264f6-142">Selecione **informação de Conta**.</span><span class="sxs-lookup"><span data-stu-id="264f6-142">Select **Account info**.</span></span>

3. <span data-ttu-id="264f6-143">De acordo com **o contrato de cliente da Microsoft,** consulte se a confirmação foi ou não fornecida por este cliente.</span><span class="sxs-lookup"><span data-stu-id="264f6-143">Under **Microsoft customer agreement**, view if confirmation has or hasn't been provided by this customer.</span></span>

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a><span data-ttu-id="264f6-144">Confirme a aceitação do cliente usando Partner Center API/SDK</span><span class="sxs-lookup"><span data-stu-id="264f6-144">Confirm customer acceptance using Partner Center API/SDK</span></span>

<span data-ttu-id="264f6-145">Pode utilizar a API/SDK do Partner Center para confirmar a aceitação do cliente do Microsoft Customer Agreement.</span><span class="sxs-lookup"><span data-stu-id="264f6-145">You can use Partner Center API/SDK to confirm customer acceptance of the Microsoft Customer Agreement.</span></span> <span data-ttu-id="264f6-146">Para mais informações sobre a API/SDK, consulte:</span><span class="sxs-lookup"><span data-stu-id="264f6-146">For details on the API/SDK, refer to:</span></span>

- [<span data-ttu-id="264f6-147">Obter metadados de contrato para o Contrato de Cliente Microsoft</span><span class="sxs-lookup"><span data-stu-id="264f6-147">Get agreement metadata for the Microsoft Customer Agreement</span></span>](/partner-center/develop/get-customer-agreement-metadata)

- [<span data-ttu-id="264f6-148">Confirmar aceitação do cliente do Contrato de Cliente Microsoft</span><span class="sxs-lookup"><span data-stu-id="264f6-148">Confirm customer acceptance of Microsoft Customer Agreement</span></span>](/partner-center/develop/confirm-customer-consent-customer-agreement)

- [<span data-ttu-id="264f6-149">Obter confirmação da aceitação do cliente do Contrato de Cliente Microsoft</span><span class="sxs-lookup"><span data-stu-id="264f6-149">Get confirmation of customer acceptance of Microsoft Customer Agreement</span></span>](/partner-center/develop/get-confirmation-of-customer-agreement)

- [<span data-ttu-id="264f6-150">Obtenha um link de descarregamento para o modelo do Contrato de Cliente da Microsoft</span><span class="sxs-lookup"><span data-stu-id="264f6-150">Get a download link for the Microsoft Customer Agreement template</span></span>](/partner-center/develop/download-customer-agreement-template)

## <a name="option-2-customer-acceptance-in-microsoft-365-admin-center"></a><span data-ttu-id="264f6-151">Opção 2: Aceitação do cliente no Microsoft 365 Admin Center</span><span class="sxs-lookup"><span data-stu-id="264f6-151">Option 2: Customer acceptance in Microsoft 365 Admin Center</span></span>

<span data-ttu-id="264f6-152">Os parceiros podem convidar clientes novos e existentes, através de um URL, a rever e aceitar o acordo dentro do Microsoft 365 Admin Center.</span><span class="sxs-lookup"><span data-stu-id="264f6-152">Partners can invite new and existing customers, via a URL, to review and accept the agreement within the Microsoft 365 Admin Center.</span></span> <span data-ttu-id="264f6-153">As próximas secções mostram-lhe como:</span><span class="sxs-lookup"><span data-stu-id="264f6-153">The next few sections show you how to:</span></span>

- <span data-ttu-id="264f6-154">Crie um novo cliente e convide o cliente a rever e aceitar o acordo.</span><span class="sxs-lookup"><span data-stu-id="264f6-154">Create a new customer and invite the customer to review and accept the agreement.</span></span>

- <span data-ttu-id="264f6-155">Convide um novo cliente a rever e a aceitar a relação e o acordo do revendedor.</span><span class="sxs-lookup"><span data-stu-id="264f6-155">Invite a new customer to review and accept the reseller relationship and agreement.</span></span>

- <span data-ttu-id="264f6-156">Convide um cliente existente a rever e a aceitar o acordo.</span><span class="sxs-lookup"><span data-stu-id="264f6-156">Invite an existing customer to review and accept the agreement.</span></span>

>[!NOTE]
> <span data-ttu-id="264f6-157">Pode utilizar [a API/SDK do Partner Center](/partner-center/develop/get-direct-sign-status-of-customer-agreement) para obter o estado da aceitação direta de um cliente do Acordo de Cliente da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="264f6-157">You can use [Partner Center API/SDK](/partner-center/develop/get-direct-sign-status-of-customer-agreement) to get the status of a customer's direct acceptance of the Microsoft Customer Agreement.</span></span>  

## <a name="create-a-new-customer-and-invite-the-customer-to-review-and-accept-the-agreement"></a><span data-ttu-id="264f6-158">Crie um novo cliente e convide o cliente a rever e aceitar o acordo</span><span class="sxs-lookup"><span data-stu-id="264f6-158">Create a new customer and invite the customer to review and accept the agreement</span></span>

<span data-ttu-id="264f6-159">Use os seguintes passos para criar um novo cliente no Partner Center e, em seguida, convidá-los a rever e aceitar o Acordo de Cliente da Microsoft dentro do Microsoft 365 Admin Center.</span><span class="sxs-lookup"><span data-stu-id="264f6-159">Use the following steps to create a new customer in Partner Center then invite them to review and accept the Microsoft Customer Agreement within Microsoft 365 Admin Center.</span></span>

1. <span data-ttu-id="264f6-160">A partir do separador **Clientes** dentro do Partner Center, **selecione Adicionar cliente.**</span><span class="sxs-lookup"><span data-stu-id="264f6-160">From the **Customers** tab within Partner Center, select **Add customer**.</span></span>

2. <span data-ttu-id="264f6-161">Informação **em Conta**, introduza informações sobre o novo cliente em todas as áreas requeridas, incluindo o nome da empresa do cliente e o contacto primário.</span><span class="sxs-lookup"><span data-stu-id="264f6-161">Under **Account Info**, enter information about the new customer in all required fields, including the customer's company name and primary contact.</span></span>

3. <span data-ttu-id="264f6-162">De acordo com **o Cliente,** será solicitado ao Cliente que **aceite o Acordo de Cliente da Microsoft no Microsoft 365 Admin Center**.</span><span class="sxs-lookup"><span data-stu-id="264f6-162">Under **Customer Agreement**, select **Customer will be asked to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center**.</span></span> <span data-ttu-id="264f6-163">Preencha todos os outros campos necessários na página.</span><span class="sxs-lookup"><span data-stu-id="264f6-163">Complete any other required fields on the page.</span></span>

4. <span data-ttu-id="264f6-164">Selecione **Seguinte: Reveja** então continue os passos para criar o inquilino do cliente.</span><span class="sxs-lookup"><span data-stu-id="264f6-164">Select **Next: Review** then continue the steps to create the customer tenant.</span></span> 

>[!NOTE] 
><span data-ttu-id="264f6-165">Os novos clientes não podem fazer uma compra até aceitarem o Acordo de Cliente da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="264f6-165">New customers cannot make a purchase until they accept the Microsoft Customer Agreement.</span></span>  

   :::image type="content" source="images/mca/create-new-customer.jpg" alt-text="Criar novo cliente":::

5. <span data-ttu-id="264f6-167">Quando chegar ao ecrã **de Confirmação** no novo fluxo de trabalho do cliente, guarde as credenciais do cliente.</span><span class="sxs-lookup"><span data-stu-id="264f6-167">When you reach the **Confirmation** screen in the new customer workflow, save the customer credentials.</span></span> <span data-ttu-id="264f6-168">Terá de dar estas credenciais ao seu cliente mais tarde.</span><span class="sxs-lookup"><span data-stu-id="264f6-168">You will need to give these credentials to your customer later.</span></span>

6. <span data-ttu-id="264f6-169">Fora do Partner Center, crie e envie um e-mail que convida o cliente a aceitar o Acordo de Cliente da Microsoft no Microsoft 365 Admin Center.</span><span class="sxs-lookup"><span data-stu-id="264f6-169">Outside of Partner Center, create and send an email that invites the customer to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center.</span></span> <span data-ttu-id="264f6-170">Certifique-se de incluir estes itens no e-mail:</span><span class="sxs-lookup"><span data-stu-id="264f6-170">Make sure to include these items in the email:</span></span>

   - <span data-ttu-id="264f6-171">Um link para este [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (Inscrição obrigatória)</span><span class="sxs-lookup"><span data-stu-id="264f6-171">A link to this [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (Sign-in required)</span></span>

   - <span data-ttu-id="264f6-172">As credenciais do cliente que guardou no passo 5.</span><span class="sxs-lookup"><span data-stu-id="264f6-172">The customer's credentials that you saved in Step 5.</span></span>

7. <span data-ttu-id="264f6-173">O cliente receberá então o convite de e-mail do parceiro e selecionará o [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span><span class="sxs-lookup"><span data-stu-id="264f6-173">The customer will then receive the email invite from the partner and select the [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span></span>

8. <span data-ttu-id="264f6-174">O cliente assina no Microsoft 365 Admin Center utilizando as credenciais de cliente que forneceu.</span><span class="sxs-lookup"><span data-stu-id="264f6-174">The customer signs into Microsoft 365 Admin Center using the customer credentials you provided.</span></span>

9. <span data-ttu-id="264f6-175">O cliente verifica a caixa para aceitar o acordo de Cliente da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="264f6-175">The customer checks the box to accept the Microsoft Customer agreement.</span></span>

## <a name="invite-a-new-customer-to-review-and-accept-the-reseller-relationship-and-microsoft-customer-agreement"></a><span data-ttu-id="264f6-176">Convide um novo cliente a rever e aceitar a relação de revendedor e o Acordo de Cliente da Microsoft</span><span class="sxs-lookup"><span data-stu-id="264f6-176">Invite a new customer to review and accept the reseller relationship and Microsoft Customer Agreement</span></span> 

<span data-ttu-id="264f6-177">Utilize os seguintes passos para convidar um novo cliente a rever e aceitar a relação de revendedor e o Acordo de Cliente da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="264f6-177">Use the following steps to invite a new customer to review and accept the reseller relationship and the Microsoft Customer Agreement.</span></span> 

1. <span data-ttu-id="264f6-178">A partir do separador **Clientes** dentro do Partner Center, selecione Solicite um link **de relacionamento revendedor.**</span><span class="sxs-lookup"><span data-stu-id="264f6-178">From the **Customers** tab within Partner Center, select **Request a reseller relationship** link.</span></span> 

2. <span data-ttu-id="264f6-179">Será gerado um modelo de e-mail automático, incluindo texto e um URL parametrizado que direciona o cliente para o Microsoft 365 Admin Center.</span><span class="sxs-lookup"><span data-stu-id="264f6-179">An automatic email template will be generated, including text and a parameterized URL that directs the customer to the Microsoft 365 Admin Center.</span></span>

3. <span data-ttu-id="264f6-180">Pode personalizar o modelo de e-mail gerado automaticamente e, em seguida, selecionar **Copy para clipboard** ou **Abrir no e-mail**.</span><span class="sxs-lookup"><span data-stu-id="264f6-180">You can customize the automatically generated email template and then select **Copy to clipboard** or **Open in email**.</span></span>

4. <span data-ttu-id="264f6-181">Utilize este modelo de e-mail para convidar o cliente a aceitar o pedido **de relacionamento do revendedor** e o **Acordo de Cliente da Microsoft.**</span><span class="sxs-lookup"><span data-stu-id="264f6-181">Use this email template to invite the customer to accept **reseller relationship** request and the **Microsoft Customer Agreement**.</span></span> <span data-ttu-id="264f6-182">(Nota: No convite por e-mail, certifique-se de que o parceiro também inclui o URL que foi fornecido automaticamente, bem como as credenciais de cliente que foram criadas recentemente.)</span><span class="sxs-lookup"><span data-stu-id="264f6-182">(Note: In the email invite, make sure the partner also includes the URL that was automatically provided as well as the customer credentials that were recently created.)</span></span>

   :::image type="content" source="images/mca/createrelationship.png" alt-text="criar uma relação":::

5. <span data-ttu-id="264f6-184">O cliente recebe convite via e-mail e clica no URL parametrizado.</span><span class="sxs-lookup"><span data-stu-id="264f6-184">Customer receives invite via email and clicks on the parameterized URL.</span></span> 

6. <span data-ttu-id="264f6-185">O cliente utiliza credenciais que fornece dentro de e-mail para assinar no Microsoft 365 Admin Center.</span><span class="sxs-lookup"><span data-stu-id="264f6-185">Customer uses credentials you provide within email to sign into Microsoft 365 Admin Center.</span></span>

7. <span data-ttu-id="264f6-186">O cliente verifica a caixa para aceitar a relação de **revendedor** e **o Acordo de Cliente da Microsoft.**</span><span class="sxs-lookup"><span data-stu-id="264f6-186">Customer checks the box to accept the **reseller relationship** and **Microsoft Customer Agreement**.</span></span> 

8. <span data-ttu-id="264f6-187">Dentro do mesmo URL, o cliente é capaz de ver uma lista consolidada de diferentes parceiros com os quais está a trabalhar.</span><span class="sxs-lookup"><span data-stu-id="264f6-187">Within the same URL, the customer is able to see a consolidated list of different partners they are working with.</span></span> <span data-ttu-id="264f6-188">Podem selecionar um parceiro para ver detalhes.</span><span class="sxs-lookup"><span data-stu-id="264f6-188">They can select a partner to see details.</span></span>

   :::image type="content" source="images/mca/accept.jpg" alt-text="Aceitar o contrato":::


## <a name="invite-an-existing-customer-to-review-and-accept-the-agreement"></a><span data-ttu-id="264f6-190">Convide um cliente existente a rever e aceitar o acordo</span><span class="sxs-lookup"><span data-stu-id="264f6-190">Invite an existing customer to review and accept the agreement</span></span>

<span data-ttu-id="264f6-191">Utilize os seguintes passos para convidar um cliente existente a rever e aceitar o Acordo de Cliente da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="264f6-191">Use the following steps to invite an existing customer to review and accept the Microsoft Customer Agreement.</span></span> 

1. <span data-ttu-id="264f6-192">Crie o e-mail do cliente com o URL incorporado convidando o seu cliente a aceitar o Acordo de Cliente da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="264f6-192">Create the customer email with the embedded URL inviting your customer to accept the Microsoft Customer Agreement.</span></span>

2. <span data-ttu-id="264f6-193">O seu cliente recebe o convite por e-mail e clica no [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span><span class="sxs-lookup"><span data-stu-id="264f6-193">Your customer receives the invitation via email and clicks the [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span></span> 

3. <span data-ttu-id="264f6-194">O cliente introduz as suas credenciais no Microsoft 365 Admin Center.</span><span class="sxs-lookup"><span data-stu-id="264f6-194">The customer enters their credentials into Microsoft 365 Admin Center.</span></span>

4. <span data-ttu-id="264f6-195">O seu cliente verifica a caixa para aceitar o Acordo de Cliente da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="264f6-195">Your customer checks the box to accept the Microsoft Customer Agreement.</span></span> 

5. <span data-ttu-id="264f6-196">Dentro do mesmo URL, o cliente pode ver a lista consolidada de diferentes parceiros com quem está a trabalhar.</span><span class="sxs-lookup"><span data-stu-id="264f6-196">Within the same URL, the customer can see the consolidated list of different partners they are working with.</span></span> <span data-ttu-id="264f6-197">Podem selecionar um parceiro para ver detalhes.</span><span class="sxs-lookup"><span data-stu-id="264f6-197">They can select a partner to see details.</span></span>

   :::image type="content" source="images/mca/customeraccept.png" alt-text="cliente":::

>[!NOTE]
><span data-ttu-id="264f6-199">Em certos cenários, os clientes podem não ser capazes de aceitar diretamente o Acordo de Cliente da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="264f6-199">In certain scenarios, customers may not be able to directly accept the Microsoft Customer Agreement.</span></span> <span data-ttu-id="264f6-200">Para saber mais sobre estas situações, leia Dois cenários onde precisa de atestar em nome do seu cliente, abaixo.</span><span class="sxs-lookup"><span data-stu-id="264f6-200">To learn more about these situations, read Two scenarios where you need to attest on behalf of your customer, below.</span></span>

## <a name="two-scenarios-where-you-need-to-attest-on-behalf-of-your-customer"></a><span data-ttu-id="264f6-201">Dois cenários em que precisa de atestar em nome do seu cliente</span><span class="sxs-lookup"><span data-stu-id="264f6-201">Two scenarios where you need to attest on behalf of your customer</span></span>

<span data-ttu-id="264f6-202">Existem dois cenários em que os clientes podem não ser capazes de aceitar diretamente o Acordo de Cliente da Microsoft dentro do Microsoft 365 Admin Center.</span><span class="sxs-lookup"><span data-stu-id="264f6-202">There are two scenarios where customers may not be able to directly accept the Microsoft Customer Agreement within the Microsoft 365 Admin Center.</span></span>

<span data-ttu-id="264f6-203">**Cenário 1**: Um cliente existente adquiriu qualquer um dos seguintes através de uma relação de parceiro existente: ofertas, subscrições de software ou software, Instâncias Reservadas ou Plano Azure.</span><span class="sxs-lookup"><span data-stu-id="264f6-203">**Scenario 1**: An existing customer has purchased any of the following through an existing partner relationship: offers, software or software subscriptions, Reserved Instances, or Azure Plan.</span></span> <span data-ttu-id="264f6-204">O cliente está agora a tentar fazer qualquer nova compra (excluindo a renovação automática).</span><span class="sxs-lookup"><span data-stu-id="264f6-204">The customer is now attempting to make any new purchase (excluding auto renewal).</span></span> <span data-ttu-id="264f6-205">Quando esse cliente clicar no URL, receberão a mensagem "Por favor contacte o seu Parceiro para confirmar a sua aceitação do Acordo de Cliente da Microsoft."</span><span class="sxs-lookup"><span data-stu-id="264f6-205">When that customer clicks the URL, they will receive the message "Please reach out to your Partner to confirm your acceptance of the Microsoft Customer Agreement."</span></span>  

<span data-ttu-id="264f6-206">**Para resolver:** Tem de atestar em nome do cliente.</span><span class="sxs-lookup"><span data-stu-id="264f6-206">**To resolve**: You must attest on behalf of the customer.</span></span>

:::image type="content" source="images/mca/accept-scenario-1.png" alt-text="Screenshot da página do Microsoft 365 Admin Center pedindo-lhe que contacte o seu parceiro para confirmar a aceitação do Acordo de Cliente da Microsoft.":::

<span data-ttu-id="264f6-208">**Cenário 2**: Um cliente existente adquiriu qualquer uma das seguintes ofertas, subscrições de software e software, Instâncias Reservadas e Plano Azure.</span><span class="sxs-lookup"><span data-stu-id="264f6-208">**Scenario 2**: An existing customer has purchased any of the following offers, software and software subscriptions, Reserved Instances, and Azure Plan.</span></span> <span data-ttu-id="264f6-209">O cliente está agora a tentar fazer qualquer nova compra com um novo parceiro.</span><span class="sxs-lookup"><span data-stu-id="264f6-209">The customer is now attempting to make any new purchase with a new partner.</span></span>

<span data-ttu-id="264f6-210">Quando o cliente clicar no URL para o Microsoft 365 Admin Center para aceitar a nova relação de parceiro e o acordo, eles receberão a mensagem "Por favor contacte o seu Parceiro para confirmar a sua aceitação do Acordo de Cliente da Microsoft."</span><span class="sxs-lookup"><span data-stu-id="264f6-210">When the customer clicks the URL to Microsoft 365 Admin Center to accept the new partner relationship and the agreement, they will receive the message "Please reach out to your Partner to confirm your acceptance of the Microsoft Customer Agreement."</span></span>  

<span data-ttu-id="264f6-211">**Para resolver:** Tem de atestar em nome do cliente.</span><span class="sxs-lookup"><span data-stu-id="264f6-211">**To resolve**: You must attest on behalf of the customer.</span></span>  

## <a name="confirm-that-a-customer-has-accepted-the-agreement"></a><span data-ttu-id="264f6-212">Confirme que um cliente aceitou o acordo</span><span class="sxs-lookup"><span data-stu-id="264f6-212">Confirm that a customer has accepted the agreement</span></span>

<span data-ttu-id="264f6-213">Se tentar criar uma nova encomenda para um cliente existente que não tenha confirmado antes, receberá um pedido para completar a confirmação.</span><span class="sxs-lookup"><span data-stu-id="264f6-213">If you try to create a new order for an existing customer who you have not confirmed before, you'll receive a prompt to complete the confirmation.</span></span> <span data-ttu-id="264f6-214">Utilize o seguinte procedimento para o fazer.</span><span class="sxs-lookup"><span data-stu-id="264f6-214">Use the following procedure to do this.</span></span>

1. <span data-ttu-id="264f6-215">Introduza o **Nome Próprio**, **Apelido,** **endereço de e-mail** e número de **telefone** (opcional) do utilizador que aceitou o acordo.</span><span class="sxs-lookup"><span data-stu-id="264f6-215">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the user who accepted the agreement.</span></span>

2. <span data-ttu-id="264f6-216">Nos termos **da data de aceitação** do Acordo, insira a data adequada.</span><span class="sxs-lookup"><span data-stu-id="264f6-216">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="264f6-217">Não pode marcar isto para uma data futura.</span><span class="sxs-lookup"><span data-stu-id="264f6-217">You cannot set this to a future date.</span></span>

3. <span data-ttu-id="264f6-218">Selecione **Guardar e continuar**.</span><span class="sxs-lookup"><span data-stu-id="264f6-218">Select **Save and continue**.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="264f6-219">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="264f6-219">Next steps</span></span>

- [<span data-ttu-id="264f6-220">Verifique ou atualize as informações do perfil da empresa</span><span class="sxs-lookup"><span data-stu-id="264f6-220">Verify or update your company profile information</span></span>](update-your-partner-profile.md)
- [<span data-ttu-id="264f6-221">Contratos de Cliente Microsoft (por região, idioma)</span><span class="sxs-lookup"><span data-stu-id="264f6-221">Microsoft Customer Agreements (by region, language)</span></span>](Agreements.md)
