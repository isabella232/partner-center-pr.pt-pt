---
title: Perfis fiscais e de pagamento no Centro de Parceiros
ms.topic: how-to
ms.date: 11/12/2020
description: Crie e gere o seu perfil de pagamento e impostos para que possa ser pago pelos seus incentivos. Inclui criar, gerir e usar perfis diferentes.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.openlocfilehash: 66177c6e3cd0091081866e1508d28346f49ec713
ms.sourcegitcommit: bfc9e6f6476766cf10ba714f03ca2e96560003b1
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/14/2020
ms.locfileid: "94626036"
---
# <a name="create-and-manage-incentives-payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="3d32c-104">Criar e gerir incentivos no pagamento e perfis fiscais no Partner Center</span><span class="sxs-lookup"><span data-stu-id="3d32c-104">Create and manage incentives payout and tax profiles in Partner Center</span></span>

<span data-ttu-id="3d32c-105">**Aplica-se a:**</span><span class="sxs-lookup"><span data-stu-id="3d32c-105">**Applies to:**</span></span>

- <span data-ttu-id="3d32c-106">Partner Center</span><span class="sxs-lookup"><span data-stu-id="3d32c-106">Partner Center</span></span>

<span data-ttu-id="3d32c-107">**Funções adequadas:**</span><span class="sxs-lookup"><span data-stu-id="3d32c-107">**Appropriate roles:**</span></span>

- <span data-ttu-id="3d32c-108">Administradores de incentivos</span><span class="sxs-lookup"><span data-stu-id="3d32c-108">Incentives admin</span></span>
- <span data-ttu-id="3d32c-109">Administrador de conta</span><span class="sxs-lookup"><span data-stu-id="3d32c-109">Account admin</span></span>
- <span data-ttu-id="3d32c-110">Administrador global</span><span class="sxs-lookup"><span data-stu-id="3d32c-110">Global admin</span></span>

<span data-ttu-id="3d32c-111">Para receber o pagamento pelos seus programas de incentivos para uma determinada localização MPN, tem de completar a inscrição ao associar um perfil de pagamento e perfil fiscal válido ao programa e à localização MPN.</span><span class="sxs-lookup"><span data-stu-id="3d32c-111">Before you can receive payment for your incentive programs for a particular MPN location, you must complete your enrollment by associating a valid payout and tax profile with the program and MPN location.</span></span> <span data-ttu-id="3d32c-112">A Microsoft utilizará este perfil de pagamento e perfil fiscal para emitir os pagamentos.</span><span class="sxs-lookup"><span data-stu-id="3d32c-112">Microsoft will use this payout and tax profile to issue payments.</span></span> <span data-ttu-id="3d32c-113">Poderá ser permitida a utilização de transferências bancárias eletrónicas ou de notas de crédito para efeitos de pagamento, dependendo das regras do programa de incentivos.</span><span class="sxs-lookup"><span data-stu-id="3d32c-113">You may be allowed to use electronic bank transfer or a credit note for payment, depending on the rules of the incentive program.</span></span> 

## <a name="roles-currencies-and-other-microsoft-programs"></a><span data-ttu-id="3d32c-114">Funções, moedas e outros programas da Microsoft</span><span class="sxs-lookup"><span data-stu-id="3d32c-114">Roles, currencies, and other Microsoft programs</span></span>

<span data-ttu-id="3d32c-115">É importante entender a informação abaixo antes de começar com o seu pagamento e perfil fiscal.</span><span class="sxs-lookup"><span data-stu-id="3d32c-115">It's important to understand the information below before you get started with your payout and tax profile.</span></span>

### <a name="roles-and-permissions"></a><span data-ttu-id="3d32c-116">Funções e permissões</span><span class="sxs-lookup"><span data-stu-id="3d32c-116">Roles and permissions</span></span>

<span data-ttu-id="3d32c-117">Você deve ser um Incentivo Admin para inserir informação bancária e fiscal para pagamentos de incentivos.</span><span class="sxs-lookup"><span data-stu-id="3d32c-117">You must be an Incentives Admin to enter bank and tax information for incentive payments.</span></span> <span data-ttu-id="3d32c-118">Se for um ADMINISTRADOR MPN/Conta, pode atribuir-se a si próprio e/ou a um colega para ser o Administrador de Incentivos.</span><span class="sxs-lookup"><span data-stu-id="3d32c-118">If you're an MPN/Account Admin, you can assign yourself and/or a colleague to be the Incentives Admin.</span></span>

<span data-ttu-id="3d32c-119">Se precisar de solicitar permissões de Administração de Incentivos, contacte o seu MPN Admin ou a Global Admin. Pode descobrir quem na sua empresa tem estas funções ao inscrever-se no [painel de instrumentos](https://partner.microsoft.com/dashboard/)do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="3d32c-119">If you need to request Incentives Admin permissions, contact your MPN Admin or Global Admin. You can find out who in your company has these roles by signing into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span> <span data-ttu-id="3d32c-120">A partir do ícone **Definições** no topo direito, selecione **Gestão do Utilizador** e, em seguida, filtre no Administrador Global.</span><span class="sxs-lookup"><span data-stu-id="3d32c-120">From the **Settings** icon at the top right, select **User Management** and then filter on Global Admin.</span></span>

<span data-ttu-id="3d32c-121">Incentivos Os utilizadores podem ver os ganhos de incentivo e os detalhes e relatórios de pagamento, mas não podem editar detalhes bancários e fiscais.</span><span class="sxs-lookup"><span data-stu-id="3d32c-121">Incentives Users can view Incentive earnings and payment details and reports, but can’t edit bank and tax details.</span></span>

### <a name="choose-your-disbursement-currency"></a><span data-ttu-id="3d32c-122">Escolha a sua moeda de desembolso</span><span class="sxs-lookup"><span data-stu-id="3d32c-122">Choose your disbursement currency</span></span>

<span data-ttu-id="3d32c-123">Os pagamentos de incentivos são feitos na moeda que selecionou quando configura o seu perfil de pagamento.</span><span class="sxs-lookup"><span data-stu-id="3d32c-123">Incentive payments are made in the currency you selected when you set up your payment profile.</span></span> <span data-ttu-id="3d32c-124">Os pagamentos serão calculados usando uma taxa de câmbio definida mensalmente pela Microsoft.</span><span class="sxs-lookup"><span data-stu-id="3d32c-124">Payments will be calculated using an exchange rate as set monthly by Microsoft.</span></span> <span data-ttu-id="3d32c-125">Será responsável por quaisquer alterações de valor devido à moeda selecionada.</span><span class="sxs-lookup"><span data-stu-id="3d32c-125">You’ll be responsible for any changes in value due to the currency selected.</span></span>

### <a name="using-different-profiles-for-different-microsoft-programs"></a><span data-ttu-id="3d32c-126">Usando diferentes perfis para diferentes programas da Microsoft</span><span class="sxs-lookup"><span data-stu-id="3d32c-126">Using different profiles for different Microsoft programs</span></span>

<span data-ttu-id="3d32c-127">Se a sua empresa estiver matriculada em vários programas de incentivo, pode utilizar a mesma conta de pagamento para todos eles, ou optar por utilizar diferentes contas de pagamento para diferentes programas.</span><span class="sxs-lookup"><span data-stu-id="3d32c-127">If your company is enrolled in multiple incentive programs, you can use the same payment account for all of them, or choose to use different payment accounts for different programs.</span></span>

## <a name="create-and-manage-payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="3d32c-128">Criar e gerir perfis de pagamento e impostos no Partner Center</span><span class="sxs-lookup"><span data-stu-id="3d32c-128">Create and manage payout and tax profiles in Partner Center</span></span>

<span data-ttu-id="3d32c-129">As secções abaixo irão acompanhar-te através do processo de criação e gestão de perfis de pagamento e impostos no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="3d32c-129">The sections below will walk you through the process of creating and managing payment and tax profiles in Partner Center.</span></span>

>[!IMPORTANT]
><span data-ttu-id="3d32c-130">Deve ser um administrador de incentivo para criar ou gerir perfis de pagamento no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="3d32c-130">You must be an Incentive admin to create or manage payment profiles in Partner Center.</span></span> <span data-ttu-id="3d32c-131">As funções de incentivo devem ser atribuídas a cada localização MPN ao abrigo de cada programa de incentivo.</span><span class="sxs-lookup"><span data-stu-id="3d32c-131">Incentive roles must be assigned to each MPN location under each incentive program.</span></span> <span data-ttu-id="3d32c-132">Para obter mais informações sobre como adicionar administradores de incentivo no Partner Center, consulte [Criar contas de utilizador](create-user-accounts-and-set-permissions.md).</span><span class="sxs-lookup"><span data-stu-id="3d32c-132">For more information on how to add Incentive admins in Partner Center, see [Create user accounts](create-user-accounts-and-set-permissions.md).</span></span>

## <a name="access-the-payout-and-tax-section-in-partner-center"></a><span data-ttu-id="3d32c-133">Aceda à secção de pagamentos e impostos no Partner Center</span><span class="sxs-lookup"><span data-stu-id="3d32c-133">Access the payout and tax section in Partner Center</span></span>

1. <span data-ttu-id="3d32c-134">Inscreva-se no painel de [instrumentos](https://partner.microsoft.com/dashboard/) do Partner Center utilizando a sua conta Azure Ative (Azure AD) (conta da empresa) ou o endereço de e-mail apropriado se um for atribuído.</span><span class="sxs-lookup"><span data-stu-id="3d32c-134">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/) using your Azure Active Directory (Azure AD) account (company account), or the appropriate email address if one was assigned.</span></span>

   - <span data-ttu-id="3d32c-135">Vários domínios podem ser registados dentro de uma conta AD Azure.</span><span class="sxs-lookup"><span data-stu-id="3d32c-135">Multiple domains can be registered within one Azure AD account.</span></span> <span data-ttu-id="3d32c-136">Contacte o seu administrador Global para determinar quais os domínios associados.</span><span class="sxs-lookup"><span data-stu-id="3d32c-136">Contact your Global admin to determine which domains are associated.</span></span>
   - <span data-ttu-id="3d32c-137">Se só conseguir fazer login com o @onmicrosoft.com domínio, contacte o administrador da conta para adicionar domínios adicionais à conta Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3d32c-137">If you're only able to log in with the @onmicrosoft.com domain, contact your Account admin to add additional domains to the Azure AD account.</span></span>
   - <span data-ttu-id="3d32c-138">Se lhe for solicitado que selecione **conta de trabalho ou escola** ou conta **pessoal,** selecione **Trabalho ou conta escolar**.</span><span class="sxs-lookup"><span data-stu-id="3d32c-138">If you're prompted to select **Work or school account** or **Personal Account** , select **Work or school account**.</span></span>

2. <span data-ttu-id="3d32c-139">Selecione o ícone de engrenagem para abrir o menu **Definições** e, em seguida, selecione **as definições de Parceiro**.</span><span class="sxs-lookup"><span data-stu-id="3d32c-139">Select the gear icon to open the **Settings** menu, and then select **Partner settings**.</span></span>

3. <span data-ttu-id="3d32c-140">No menu **de definições de conta,** selecione **Payout e tax**.</span><span class="sxs-lookup"><span data-stu-id="3d32c-140">In the **Account settings** menu, select **Payout and tax**.</span></span> 

## <a name="assign-payout-and-tax-profiles-to-individual-programs"></a><span data-ttu-id="3d32c-141">Atribuir perfis de pagamento e impostos a programas individuais</span><span class="sxs-lookup"><span data-stu-id="3d32c-141">Assign payout and tax profiles to individual programs</span></span>

1. <span data-ttu-id="3d32c-142">Inscreva-se no [painel de instrumentos Partner Center](https://partner.microsoft.com/dashboard/)e, em seguida, selecione o ícone de engrenagem para abrir o menu **Definições.**</span><span class="sxs-lookup"><span data-stu-id="3d32c-142">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/), and then select the gear icon to open the **Settings** menu.</span></span> 

2. <span data-ttu-id="3d32c-143">Selecione **as definições de Parceiro** , expanda a secção de Pagamento e **Imposto** , e, em seguida, selecione Payout e tax **profile assignment**.</span><span class="sxs-lookup"><span data-stu-id="3d32c-143">Select **Partner settings** , expand the **Payout and tax section** , and then select **Payout and tax profile assignment**.</span></span> 
   
   <span data-ttu-id="3d32c-144">Será apresentada uma lista dos seus programas.</span><span class="sxs-lookup"><span data-stu-id="3d32c-144">A list of your programs will be displayed.</span></span> <span data-ttu-id="3d32c-145">Selecione a seta ao lado de um programa para ver os detalhes do perfil.</span><span class="sxs-lookup"><span data-stu-id="3d32c-145">Select the arrow next to a program to see profile details.</span></span> 

3. <span data-ttu-id="3d32c-146">No menu de entrega **do Perfil Fiscal,** selecione o perfil de imposto que deseja ou selecione a opção para criar um novo perfil.</span><span class="sxs-lookup"><span data-stu-id="3d32c-146">In the **Tax Profile** dropdown menu, select the tax profile you want, or select the option to create a new profile.</span></span> <span data-ttu-id="3d32c-147">Quando selecionar a opção para criar um novo perfil, será redirecionado adequadamente.</span><span class="sxs-lookup"><span data-stu-id="3d32c-147">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span>  <span data-ttu-id="3d32c-148">Selecione Continue na janela pop-up.</span><span class="sxs-lookup"><span data-stu-id="3d32c-148">Select Continue in the pop-up window.</span></span> <span data-ttu-id="3d32c-149">O processo de criação de um novo perfil fiscal foi apresentado abaixo.</span><span class="sxs-lookup"><span data-stu-id="3d32c-149">The process for creating a new tax profile has been provided below.</span></span>

4. <span data-ttu-id="3d32c-150">Selecione **o método de pagamento**.</span><span class="sxs-lookup"><span data-stu-id="3d32c-150">Select **Payment method**.</span></span>

   - <span data-ttu-id="3d32c-151">Se selecionou **a transferência bancária electrónica** como método de pagamento, selecione o perfil de pagamento que pretende ou selecione a opção de criar um novo perfil.</span><span class="sxs-lookup"><span data-stu-id="3d32c-151">If you have selected **Electronic bank transfer** as your payment method, select the payment profile you want, or select the option to create a new profile.</span></span> <span data-ttu-id="3d32c-152">Quando selecionar a opção para criar um novo perfil, será redirecionado adequadamente.</span><span class="sxs-lookup"><span data-stu-id="3d32c-152">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span> <span data-ttu-id="3d32c-153">Selecione Continue na janela pop-up.</span><span class="sxs-lookup"><span data-stu-id="3d32c-153">Select Continue in the pop-up window.</span></span> <span data-ttu-id="3d32c-154">O processo de criação de um novo perfil de pagamento foi fornecido abaixo.</span><span class="sxs-lookup"><span data-stu-id="3d32c-154">The process for creating a new payment profile has been provided below.</span></span>

   - <span data-ttu-id="3d32c-155">Se tiver selecionado **a Nota de Crédito** como método de pagamento, então complete a verificação.</span><span class="sxs-lookup"><span data-stu-id="3d32c-155">If you have selected **Credit Note** as your payment method, then complete the verification.</span></span> <span data-ttu-id="3d32c-156">Isto confirma que o número SAP referenciado pertence à sua organização.</span><span class="sxs-lookup"><span data-stu-id="3d32c-156">This confirms that the referenced SAP number belongs to your organization.</span></span>

    >[!NOTE]
    ><span data-ttu-id="3d32c-157">Se houver várias entidades empresariais da Microsoft listadas, deve selecionar um perfil de pagamento para cada entidade.</span><span class="sxs-lookup"><span data-stu-id="3d32c-157">If there are multiple Microsoft business entities listed, you must select a payment profile for each entity.</span></span>

    >[!NOTE]
    ><span data-ttu-id="3d32c-158">A disponibilidade do método de pagamento depende das regras do programa de incentivos.</span><span class="sxs-lookup"><span data-stu-id="3d32c-158">The payment method availability is dependent on the rules of the incentive program.</span></span>
    
5. <span data-ttu-id="3d32c-159">Selecione a **Moeda**.</span><span class="sxs-lookup"><span data-stu-id="3d32c-159">Select the **Currency**.</span></span>

6. <span data-ttu-id="3d32c-160">Quando tiver concluído todos os campos de pagamento, **selecione Enviar por isso.**</span><span class="sxs-lookup"><span data-stu-id="3d32c-160">When you’ve completed all of the payment fields, select **Submit**.</span></span>

## <a name="create-your-bank-profile"></a><span data-ttu-id="3d32c-161">Crie o seu perfil bancário</span><span class="sxs-lookup"><span data-stu-id="3d32c-161">Create your bank profile</span></span>

<span data-ttu-id="3d32c-162">Os perfis bancários são criados a nível de organização.</span><span class="sxs-lookup"><span data-stu-id="3d32c-162">Bank profiles are created at an organization level.</span></span> <span data-ttu-id="3d32c-163">Isto permite que um perfil bancário seja atribuído em vários programas de ID e incentivos de MPN dentro de uma organização.</span><span class="sxs-lookup"><span data-stu-id="3d32c-163">This allows one bank profile to be assigned across multiple MPN ID’s and incentive programs within an organization.</span></span> <span data-ttu-id="3d32c-164">Pode haver exceções na aplicação do perfil bancário a diferentes países, uma vez que podem ser aplicadas diferentes regras bancárias e fiscais.</span><span class="sxs-lookup"><span data-stu-id="3d32c-164">There may be exceptions when applying the banking profile to different countries, as different banking and tax rules may apply.</span></span>

>[!NOTE]
><span data-ttu-id="3d32c-165">Nas páginas seguintes, são necessários campos com asterisco.</span><span class="sxs-lookup"><span data-stu-id="3d32c-165">On the following pages, fields with an asterisk are required.</span></span> <span data-ttu-id="3d32c-166">Se não sabe o que é um campo, selecione o ícone da informação.</span><span class="sxs-lookup"><span data-stu-id="3d32c-166">If you don’t know what a field is, select the information icon.</span></span> 

1. <span data-ttu-id="3d32c-167">Na página **Detalhes,** preencha os seguintes campos: **Nome do perfil:** Introduza um nome único para identificar este perfil de pagamento.</span><span class="sxs-lookup"><span data-stu-id="3d32c-167">On the **Details** page, complete the following fields: **Profile name:** Enter a unique name to identify this payment profile.</span></span>
    <span data-ttu-id="3d32c-168">**Localização da conta bancária:** O país onde está localizado o banco da sua empresa.</span><span class="sxs-lookup"><span data-stu-id="3d32c-168">**Bank account location:** The country in which your company’s bank is located.</span></span>
    <span data-ttu-id="3d32c-169">**Método de pagamento:** O método de pagamento preferido para o Partner Center é a transferência bancária electrónica.</span><span class="sxs-lookup"><span data-stu-id="3d32c-169">**Payment method:** The preferred payment method for Partner Center is electronic bank transfer.</span></span>

2. <span data-ttu-id="3d32c-170">Selecione **Seguinte**.</span><span class="sxs-lookup"><span data-stu-id="3d32c-170">Select **Next**.</span></span>

3. <span data-ttu-id="3d32c-171">Na página da **conta Do Banco,** insira a sua informação.</span><span class="sxs-lookup"><span data-stu-id="3d32c-171">On the **Bank account** page, enter your information.</span></span> <span data-ttu-id="3d32c-172">Os campos mostrados nesta página variam de país para país.</span><span class="sxs-lookup"><span data-stu-id="3d32c-172">Fields shown on this page will vary by country.</span></span> 

4. <span data-ttu-id="3d32c-173">Selecione **Seguinte**.</span><span class="sxs-lookup"><span data-stu-id="3d32c-173">Select **Next**.</span></span>

5. <span data-ttu-id="3d32c-174">Na página **do Beneficiário,** insira as informações apropriadas.</span><span class="sxs-lookup"><span data-stu-id="3d32c-174">On the **Beneficiary** page, enter the appropriate information.</span></span> <span data-ttu-id="3d32c-175">O beneficiário é a pessoa na sua empresa que o banco entraria em contacto se precisasse de discutir a sua conta.</span><span class="sxs-lookup"><span data-stu-id="3d32c-175">The beneficiary is the person in your company that the bank would contact if they need to discuss your account.</span></span>

6. <span data-ttu-id="3d32c-176">Quando os campos estiverem concluídos, selecione **Terminar** e, em seguida, selecione **Confirmar** para criar o seu perfil bancário.</span><span class="sxs-lookup"><span data-stu-id="3d32c-176">When the fields are completed, select **Finish** , and then select **Confirm** to create your bank profile.</span></span>

<span data-ttu-id="3d32c-177">Será redirecionado para a página **de pagamentos e perfis fiscais.**</span><span class="sxs-lookup"><span data-stu-id="3d32c-177">You’ll be redirected to the **Payout and tax profiles** page.</span></span> <span data-ttu-id="3d32c-178">O estado do seu novo perfil refletirá **a validação pendente** da Microsoft até que a validação esteja concluída.</span><span class="sxs-lookup"><span data-stu-id="3d32c-178">The status of your new profile will reflect **Pending Microsoft validation** until the validation has been completed.</span></span> <span data-ttu-id="3d32c-179">Este processo pode demorar até 48 horas.</span><span class="sxs-lookup"><span data-stu-id="3d32c-179">This process may take up to 48 hours.</span></span> <span data-ttu-id="3d32c-180">Uma vez concluída a validação, o seu estado de perfil refletirá quer **aprovado** quer **ação necessária**.</span><span class="sxs-lookup"><span data-stu-id="3d32c-180">Once validation has been completed, your profile status will reflect either **Approved** or **Action required**.</span></span> <span data-ttu-id="3d32c-181">Se **for necessário** agir, repita os passos acima, fornecendo as informações necessárias.</span><span class="sxs-lookup"><span data-stu-id="3d32c-181">If **Action Required** , repeat the steps above providing the necessary information.</span></span> 

## <a name="create-your-tax-profile"></a><span data-ttu-id="3d32c-182">Crie o seu perfil fiscal</span><span class="sxs-lookup"><span data-stu-id="3d32c-182">Create your tax profile</span></span>

<span data-ttu-id="3d32c-183">Utilize o seguinte procedimento para fornecer à Microsoft as informações fiscais necessárias para a sua organização.</span><span class="sxs-lookup"><span data-stu-id="3d32c-183">Use the following procedure to provide Microsoft with the tax information required for your organization.</span></span> <span data-ttu-id="3d32c-184">As páginas desta secção são dinâmicas e variam de acordo com o seu país ou região.</span><span class="sxs-lookup"><span data-stu-id="3d32c-184">The pages in this section are dynamic and will vary according to your country or region.</span></span> <span data-ttu-id="3d32c-185">Se precisar de ajuda para identificar as informações fiscais corretas, contacte as fontes governamentais apropriadas no seu país.</span><span class="sxs-lookup"><span data-stu-id="3d32c-185">If you need help with identifying the correct tax information, contact the appropriate government sources in your country.</span></span>

<span data-ttu-id="3d32c-186">Para empresas parceiras nas Américas, se necessitar de informações sobre o preenchimento dos formulários W8 ou W9, os seguintes endereços levam-no ao site do IRS:</span><span class="sxs-lookup"><span data-stu-id="3d32c-186">For partner companies in the Americas, if you require information on completing the W8 or W9 forms, the following addresses take you to the IRS site:</span></span>

- [http://www.irs.gov/pub/irs-pdf/iw8.pdf](http://www.irs.gov/pub/irs-pdf/iw8.pdf)
- [http://www.irs.gov/pub/irs-pdf/iw9.pdf](http://www.irs.gov/pub/irs-pdf/iw9.pdf)

>[!IMPORTANT]
> <span data-ttu-id="3d32c-187">Insira apenas detalhes para a sua empresa.</span><span class="sxs-lookup"><span data-stu-id="3d32c-187">Enter only details for your company.</span></span> <span data-ttu-id="3d32c-188">Nunca introduza detalhes pessoais.</span><span class="sxs-lookup"><span data-stu-id="3d32c-188">Never enter personal details.</span></span>

1. <span data-ttu-id="3d32c-189">Na página **'Perfil de** Negócios', preencha os campos necessários e, em seguida, selecione **Seguinte**.</span><span class="sxs-lookup"><span data-stu-id="3d32c-189">On the **Business Profile** page, complete the required fields and then select **Next**.</span></span> 

2. <span data-ttu-id="3d32c-190">Na página **Configuração,** selecione a opção que se aplica à sua empresa.</span><span class="sxs-lookup"><span data-stu-id="3d32c-190">On the **Setup** page, select the option that applies to your company.</span></span>

   - <span data-ttu-id="3d32c-191">Selecione a opção à esquerda se a sua empresa for incorporada apenas nos Estados Unidos, ou se este perfil for para um indivíduo.</span><span class="sxs-lookup"><span data-stu-id="3d32c-191">Select the option on the left if your company is incorporated in the United States only, or if this profile is for an individual.</span></span>
   - <span data-ttu-id="3d32c-192">Selecione a opção à direita se a sua empresa estiver incorporada fora dos Estados Unidos e, em seguida, selecione o seu país/região da lista.</span><span class="sxs-lookup"><span data-stu-id="3d32c-192">Select the option on the right if your company is incorporated outside of the United States, and then select your country/region from the list.</span></span>

3. <span data-ttu-id="3d32c-193">Selecione **Seguinte**.</span><span class="sxs-lookup"><span data-stu-id="3d32c-193">Select **Next**.</span></span> 

4. <span data-ttu-id="3d32c-194">Na página de estado do **Imposto,** insira as informações necessárias e, em seguida, selecione **Seguinte**.</span><span class="sxs-lookup"><span data-stu-id="3d32c-194">On the **Tax status** page, enter the required information, and then select **Next**.</span></span> <span data-ttu-id="3d32c-195">Os campos nesta página variam por país.</span><span class="sxs-lookup"><span data-stu-id="3d32c-195">Fields on this page will vary by country.</span></span> <span data-ttu-id="3d32c-196">seus detalhes.</span><span class="sxs-lookup"><span data-stu-id="3d32c-196">your details.</span></span> 

5. <span data-ttu-id="3d32c-197">Na página **de documentação adicional,** os campos necessários e selecione **Seguinte**.</span><span class="sxs-lookup"><span data-stu-id="3d32c-197">On the **Additional documentation** page, the required fields and select **Next**.</span></span> 

6. <span data-ttu-id="3d32c-198">**Selecione Procurar** para carregar quaisquer documentos necessários pelo seu país ou região.</span><span class="sxs-lookup"><span data-stu-id="3d32c-198">Select **Browse** to upload any documents required by your country or region.</span></span> <span data-ttu-id="3d32c-199">Quando o nome do documento for mostrado, selecione **Upload**.</span><span class="sxs-lookup"><span data-stu-id="3d32c-199">When the document name is shown, select **Upload**.</span></span> 

7. <span data-ttu-id="3d32c-200">Se precisar de remover o documento, selecione **Remover**.</span><span class="sxs-lookup"><span data-stu-id="3d32c-200">If you need to remove the document, select **Remove**.</span></span>

8. <span data-ttu-id="3d32c-201">Para guardar e continuar, **selecione Terminar**.</span><span class="sxs-lookup"><span data-stu-id="3d32c-201">To save and continue, select **Finish**.</span></span>

9. <span data-ttu-id="3d32c-202">**Selecione Confirme** na mensagem pop-up.</span><span class="sxs-lookup"><span data-stu-id="3d32c-202">Select **Confirm** on the pop-up message.</span></span> <span data-ttu-id="3d32c-203">Você será levado de volta para a página **de pagamento e configuração de impostos.**</span><span class="sxs-lookup"><span data-stu-id="3d32c-203">You’ll be taken back to the **Payout and tax setup** page.</span></span>

## <a name="next-steps"></a><span data-ttu-id="3d32c-204">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="3d32c-204">Next steps</span></span>

- [<span data-ttu-id="3d32c-205">Incentivos ao pagamento e ao perfil fiscal FAQs</span><span class="sxs-lookup"><span data-stu-id="3d32c-205">Incentives payout and tax profile FAQs</span></span>](incentives-payout-tax-profile-faqs.md)
