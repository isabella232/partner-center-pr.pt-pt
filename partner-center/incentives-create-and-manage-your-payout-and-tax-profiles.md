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
ms.openlocfilehash: 282fdacc8689ff71e885a2f0ea01ce9570611707
ms.sourcegitcommit: d37a3f353426e52dfbbac577b7576f9c3f6d2ddf
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/06/2021
ms.locfileid: "99624243"
---
# <a name="create-and-manage-incentives-payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="e4347-104">Criar e gerir incentivos no pagamento e perfis fiscais no Partner Center</span><span class="sxs-lookup"><span data-stu-id="e4347-104">Create and manage incentives payout and tax profiles in Partner Center</span></span>


<span data-ttu-id="e4347-105">**Funções adequadas:**</span><span class="sxs-lookup"><span data-stu-id="e4347-105">**Appropriate roles:**</span></span>

- <span data-ttu-id="e4347-106">Administradores de incentivos</span><span class="sxs-lookup"><span data-stu-id="e4347-106">Incentives admin</span></span>
- <span data-ttu-id="e4347-107">Administrador de conta</span><span class="sxs-lookup"><span data-stu-id="e4347-107">Account admin</span></span>
- <span data-ttu-id="e4347-108">Administrador global</span><span class="sxs-lookup"><span data-stu-id="e4347-108">Global admin</span></span>

<span data-ttu-id="e4347-109">Para receber o pagamento pelos seus programas de incentivos para uma determinada localização MPN, tem de completar a inscrição ao associar um perfil de pagamento e perfil fiscal válido ao programa e à localização MPN.</span><span class="sxs-lookup"><span data-stu-id="e4347-109">Before you can receive payment for your incentive programs for a particular MPN location, you must complete your enrollment by associating a valid payout and tax profile with the program and MPN location.</span></span> <span data-ttu-id="e4347-110">A Microsoft utilizará este perfil de pagamento e perfil fiscal para emitir os pagamentos.</span><span class="sxs-lookup"><span data-stu-id="e4347-110">Microsoft will use this payout and tax profile to issue payments.</span></span> <span data-ttu-id="e4347-111">Poderá ser permitida a utilização de transferências bancárias eletrónicas ou de notas de crédito para efeitos de pagamento, dependendo das regras do programa de incentivos.</span><span class="sxs-lookup"><span data-stu-id="e4347-111">You may be allowed to use electronic bank transfer or a credit note for payment, depending on the rules of the incentive program.</span></span> 

## <a name="roles-currencies-and-other-microsoft-programs"></a><span data-ttu-id="e4347-112">Funções, moedas e outros programas da Microsoft</span><span class="sxs-lookup"><span data-stu-id="e4347-112">Roles, currencies, and other Microsoft programs</span></span>

<span data-ttu-id="e4347-113">É importante entender a informação abaixo antes de começar com o seu pagamento e perfil fiscal.</span><span class="sxs-lookup"><span data-stu-id="e4347-113">It's important to understand the information below before you get started with your payout and tax profile.</span></span>

### <a name="roles-and-permissions"></a><span data-ttu-id="e4347-114">Funções e permissões</span><span class="sxs-lookup"><span data-stu-id="e4347-114">Roles and permissions</span></span>

<span data-ttu-id="e4347-115">Você deve ser um Incentivo Admin para inserir informação bancária e fiscal para pagamentos de incentivos.</span><span class="sxs-lookup"><span data-stu-id="e4347-115">You must be an Incentives Admin to enter bank and tax information for incentive payments.</span></span> <span data-ttu-id="e4347-116">Se for um ADMINISTRADOR MPN/Conta, pode atribuir-se a si próprio e/ou a um colega para ser o Administrador de Incentivos.</span><span class="sxs-lookup"><span data-stu-id="e4347-116">If you're an MPN/Account Admin, you can assign yourself and/or a colleague to be the Incentives Admin.</span></span>

<span data-ttu-id="e4347-117">Se precisar de solicitar permissões de Administração de Incentivos, contacte o seu MPN Admin ou a Global Admin. Pode descobrir quem na sua empresa tem estas funções ao inscrever-se no [painel de instrumentos](https://partner.microsoft.com/dashboard/)do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="e4347-117">If you need to request Incentives Admin permissions, contact your MPN Admin or Global Admin. You can find out who in your company has these roles by signing into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span> <span data-ttu-id="e4347-118">A partir do ícone **Definições** no topo direito, selecione **Gestão do Utilizador** e, em seguida, filtre no Administrador Global.</span><span class="sxs-lookup"><span data-stu-id="e4347-118">From the **Settings** icon at the top right, select **User Management** and then filter on Global Admin.</span></span>

<span data-ttu-id="e4347-119">Incentivos Os utilizadores podem ver os ganhos de incentivo e os detalhes e relatórios de pagamento, mas não podem editar detalhes bancários e fiscais.</span><span class="sxs-lookup"><span data-stu-id="e4347-119">Incentives Users can view Incentive earnings and payment details and reports, but can’t edit bank and tax details.</span></span>

### <a name="choose-your-disbursement-currency"></a><span data-ttu-id="e4347-120">Escolha a sua moeda de desembolso</span><span class="sxs-lookup"><span data-stu-id="e4347-120">Choose your disbursement currency</span></span>

<span data-ttu-id="e4347-121">Os pagamentos de incentivos são feitos na moeda que selecionou quando configura o seu perfil de pagamento.</span><span class="sxs-lookup"><span data-stu-id="e4347-121">Incentive payments are made in the currency you selected when you set up your payment profile.</span></span> <span data-ttu-id="e4347-122">Os pagamentos serão calculados usando uma taxa de câmbio definida mensalmente pela Microsoft.</span><span class="sxs-lookup"><span data-stu-id="e4347-122">Payments will be calculated using an exchange rate as set monthly by Microsoft.</span></span> <span data-ttu-id="e4347-123">Será responsável por quaisquer alterações de valor devido à moeda selecionada.</span><span class="sxs-lookup"><span data-stu-id="e4347-123">You’ll be responsible for any changes in value due to the currency selected.</span></span>

### <a name="using-different-profiles-for-different-microsoft-programs"></a><span data-ttu-id="e4347-124">Usando diferentes perfis para diferentes programas da Microsoft</span><span class="sxs-lookup"><span data-stu-id="e4347-124">Using different profiles for different Microsoft programs</span></span>

<span data-ttu-id="e4347-125">Se a sua empresa estiver matriculada em vários programas de incentivo, pode utilizar a mesma conta de pagamento para todos eles, ou optar por utilizar diferentes contas de pagamento para diferentes programas.</span><span class="sxs-lookup"><span data-stu-id="e4347-125">If your company is enrolled in multiple incentive programs, you can use the same payment account for all of them, or choose to use different payment accounts for different programs.</span></span>

## <a name="create-and-manage-payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="e4347-126">Criar e gerir perfis de pagamento e impostos no Partner Center</span><span class="sxs-lookup"><span data-stu-id="e4347-126">Create and manage payout and tax profiles in Partner Center</span></span>

<span data-ttu-id="e4347-127">As secções abaixo irão acompanhar-te através do processo de criação e gestão de perfis de pagamento e impostos no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="e4347-127">The sections below will walk you through the process of creating and managing payment and tax profiles in Partner Center.</span></span>

>[!IMPORTANT]
><span data-ttu-id="e4347-128">Deve ser um administrador de incentivo para criar ou gerir perfis de pagamento no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="e4347-128">You must be an Incentive admin to create or manage payment profiles in Partner Center.</span></span> <span data-ttu-id="e4347-129">As funções de incentivo devem ser atribuídas a cada localização MPN ao abrigo de cada programa de incentivo.</span><span class="sxs-lookup"><span data-stu-id="e4347-129">Incentive roles must be assigned to each MPN location under each incentive program.</span></span> <span data-ttu-id="e4347-130">Para obter mais informações sobre como adicionar administradores de incentivo no Partner Center, consulte [Criar contas de utilizador](create-user-accounts-and-set-permissions.md).</span><span class="sxs-lookup"><span data-stu-id="e4347-130">For more information on how to add Incentive admins in Partner Center, see [Create user accounts](create-user-accounts-and-set-permissions.md).</span></span>

## <a name="access-the-payout-and-tax-section-in-partner-center"></a><span data-ttu-id="e4347-131">Aceda à secção de pagamentos e impostos no Partner Center</span><span class="sxs-lookup"><span data-stu-id="e4347-131">Access the payout and tax section in Partner Center</span></span>

1. <span data-ttu-id="e4347-132">Inscreva-se no painel de [instrumentos](https://partner.microsoft.com/dashboard/) do Partner Center utilizando a sua conta Azure Ative (Azure AD) (conta da empresa) ou o endereço de e-mail apropriado se um for atribuído.</span><span class="sxs-lookup"><span data-stu-id="e4347-132">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/) using your Azure Active Directory (Azure AD) account (company account), or the appropriate email address if one was assigned.</span></span>

   - <span data-ttu-id="e4347-133">Vários domínios podem ser registados dentro de uma conta AD Azure.</span><span class="sxs-lookup"><span data-stu-id="e4347-133">Multiple domains can be registered within one Azure AD account.</span></span> <span data-ttu-id="e4347-134">Contacte o seu administrador Global para determinar quais os domínios associados.</span><span class="sxs-lookup"><span data-stu-id="e4347-134">Contact your Global admin to determine which domains are associated.</span></span>
   - <span data-ttu-id="e4347-135">Se só conseguir fazer login com o @onmicrosoft.com domínio, contacte o administrador da conta para adicionar domínios adicionais à conta Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e4347-135">If you're only able to log in with the @onmicrosoft.com domain, contact your Account admin to add additional domains to the Azure AD account.</span></span>
   - <span data-ttu-id="e4347-136">Se lhe for solicitado que selecione **conta de trabalho ou escola** ou conta **pessoal,** selecione **Trabalho ou conta escolar**.</span><span class="sxs-lookup"><span data-stu-id="e4347-136">If you're prompted to select **Work or school account** or **Personal Account**, select **Work or school account**.</span></span>

2. <span data-ttu-id="e4347-137">Selecione o ícone de engrenagem para abrir o menu **Definições** e, em seguida, selecione **as definições de Conta**.</span><span class="sxs-lookup"><span data-stu-id="e4347-137">Select the gear icon to open the **Settings** menu, and then select **Account settings**.</span></span>

3. <span data-ttu-id="e4347-138">No menu **de definições de conta,** selecione **Payout e tax**.</span><span class="sxs-lookup"><span data-stu-id="e4347-138">In the **Account settings** menu, select **Payout and tax**.</span></span> 

## <a name="assign-payout-and-tax-profiles-to-individual-programs"></a><span data-ttu-id="e4347-139">Atribuir perfis de pagamento e impostos a programas individuais</span><span class="sxs-lookup"><span data-stu-id="e4347-139">Assign payout and tax profiles to individual programs</span></span>

1. <span data-ttu-id="e4347-140">Inscreva-se no [painel de instrumentos Partner Center](https://partner.microsoft.com/dashboard/)e, em seguida, selecione o ícone de engrenagem para abrir o menu **Definições.**</span><span class="sxs-lookup"><span data-stu-id="e4347-140">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/), and then select the gear icon to open the **Settings** menu.</span></span> 

2. <span data-ttu-id="e4347-141">Selecione **as definições de Conta,** expanda a **secção de Pagamento e Imposto**, e, em seguida, selecione Payout e tax profile **assignment**.</span><span class="sxs-lookup"><span data-stu-id="e4347-141">Select **Account settings**, expand the **Payout and tax section**, and then select **Payout and tax profile assignment**.</span></span> 
   
   <span data-ttu-id="e4347-142">Será apresentada uma lista dos seus programas.</span><span class="sxs-lookup"><span data-stu-id="e4347-142">A list of your programs will be displayed.</span></span> <span data-ttu-id="e4347-143">Selecione a seta ao lado de um programa para ver os detalhes do perfil.</span><span class="sxs-lookup"><span data-stu-id="e4347-143">Select the arrow next to a program to see profile details.</span></span> 

3. <span data-ttu-id="e4347-144">No menu de entrega **do Perfil Fiscal,** selecione o perfil de imposto que deseja ou selecione a opção para criar um novo perfil.</span><span class="sxs-lookup"><span data-stu-id="e4347-144">In the **Tax Profile** dropdown menu, select the tax profile you want, or select the option to create a new profile.</span></span> <span data-ttu-id="e4347-145">Quando selecionar a opção para criar um novo perfil, será redirecionado adequadamente.</span><span class="sxs-lookup"><span data-stu-id="e4347-145">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span>  <span data-ttu-id="e4347-146">Selecione Continue na janela pop-up.</span><span class="sxs-lookup"><span data-stu-id="e4347-146">Select Continue in the pop-up window.</span></span> <span data-ttu-id="e4347-147">O processo de criação de um novo perfil fiscal foi apresentado abaixo.</span><span class="sxs-lookup"><span data-stu-id="e4347-147">The process for creating a new tax profile has been provided below.</span></span>

4. <span data-ttu-id="e4347-148">Selecione **o método de pagamento**.</span><span class="sxs-lookup"><span data-stu-id="e4347-148">Select **Payment method**.</span></span>

   - <span data-ttu-id="e4347-149">Se selecionou **a transferência bancária electrónica** como método de pagamento, selecione o perfil de pagamento que pretende ou selecione a opção de criar um novo perfil.</span><span class="sxs-lookup"><span data-stu-id="e4347-149">If you have selected **Electronic bank transfer** as your payment method, select the payment profile you want, or select the option to create a new profile.</span></span> <span data-ttu-id="e4347-150">Quando selecionar a opção para criar um novo perfil, será redirecionado adequadamente.</span><span class="sxs-lookup"><span data-stu-id="e4347-150">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span> <span data-ttu-id="e4347-151">Selecione Continue na janela pop-up.</span><span class="sxs-lookup"><span data-stu-id="e4347-151">Select Continue in the pop-up window.</span></span> <span data-ttu-id="e4347-152">O processo de criação de um novo perfil de pagamento foi fornecido abaixo.</span><span class="sxs-lookup"><span data-stu-id="e4347-152">The process for creating a new payment profile has been provided below.</span></span>

   - <span data-ttu-id="e4347-153">Se tiver selecionado **a Nota de Crédito** como método de pagamento, então complete a verificação.</span><span class="sxs-lookup"><span data-stu-id="e4347-153">If you have selected **Credit Note** as your payment method, then complete the verification.</span></span> <span data-ttu-id="e4347-154">Isto confirma que o número SAP referenciado pertence à sua organização.</span><span class="sxs-lookup"><span data-stu-id="e4347-154">This confirms that the referenced SAP number belongs to your organization.</span></span>

    >[!NOTE]
    ><span data-ttu-id="e4347-155">Se houver várias entidades empresariais da Microsoft listadas, deve selecionar um perfil de pagamento para cada entidade.</span><span class="sxs-lookup"><span data-stu-id="e4347-155">If there are multiple Microsoft business entities listed, you must select a payment profile for each entity.</span></span>

    >[!NOTE]
    ><span data-ttu-id="e4347-156">A disponibilidade do método de pagamento depende das regras do programa de incentivos.</span><span class="sxs-lookup"><span data-stu-id="e4347-156">The payment method availability is dependent on the rules of the incentive program.</span></span>
    
5. <span data-ttu-id="e4347-157">Selecione a **Moeda**.</span><span class="sxs-lookup"><span data-stu-id="e4347-157">Select the **Currency**.</span></span>

6. <span data-ttu-id="e4347-158">Quando tiver concluído todos os campos de pagamento, **selecione Enviar por isso.**</span><span class="sxs-lookup"><span data-stu-id="e4347-158">When you’ve completed all of the payment fields, select **Submit**.</span></span>

## <a name="create-your-bank-profile"></a><span data-ttu-id="e4347-159">Crie o seu perfil bancário</span><span class="sxs-lookup"><span data-stu-id="e4347-159">Create your bank profile</span></span>

<span data-ttu-id="e4347-160">Os perfis bancários são criados a nível de organização.</span><span class="sxs-lookup"><span data-stu-id="e4347-160">Bank profiles are created at an organization level.</span></span> <span data-ttu-id="e4347-161">Isto permite que um perfil bancário seja atribuído em vários programas de ID e incentivos de MPN dentro de uma organização.</span><span class="sxs-lookup"><span data-stu-id="e4347-161">This allows one bank profile to be assigned across multiple MPN ID’s and incentive programs within an organization.</span></span> <span data-ttu-id="e4347-162">Pode haver exceções na aplicação do perfil bancário a diferentes países, uma vez que podem ser aplicadas diferentes regras bancárias e fiscais.</span><span class="sxs-lookup"><span data-stu-id="e4347-162">There may be exceptions when applying the banking profile to different countries, as different banking and tax rules may apply.</span></span>

>[!NOTE]
><span data-ttu-id="e4347-163">Nas páginas seguintes, são necessários campos com asterisco.</span><span class="sxs-lookup"><span data-stu-id="e4347-163">On the following pages, fields with an asterisk are required.</span></span> <span data-ttu-id="e4347-164">Se não sabe o que é um campo, selecione o ícone da informação.</span><span class="sxs-lookup"><span data-stu-id="e4347-164">If you don’t know what a field is, select the information icon.</span></span> 

1. <span data-ttu-id="e4347-165">Na página **Detalhes,** preencha os seguintes campos: **Nome do perfil:** Introduza um nome único para identificar este perfil de pagamento.</span><span class="sxs-lookup"><span data-stu-id="e4347-165">On the **Details** page, complete the following fields: **Profile name:** Enter a unique name to identify this payment profile.</span></span>
    <span data-ttu-id="e4347-166">**Localização da conta bancária:** O país onde está localizado o banco da sua empresa.</span><span class="sxs-lookup"><span data-stu-id="e4347-166">**Bank account location:** The country in which your company’s bank is located.</span></span>
    <span data-ttu-id="e4347-167">**Método de pagamento:** O método de pagamento preferido para o Partner Center é a transferência bancária electrónica.</span><span class="sxs-lookup"><span data-stu-id="e4347-167">**Payment method:** The preferred payment method for Partner Center is electronic bank transfer.</span></span>

2. <span data-ttu-id="e4347-168">Selecione **Seguinte**.</span><span class="sxs-lookup"><span data-stu-id="e4347-168">Select **Next**.</span></span>

3. <span data-ttu-id="e4347-169">Na página da **conta Do Banco,** insira a sua informação.</span><span class="sxs-lookup"><span data-stu-id="e4347-169">On the **Bank account** page, enter your information.</span></span> <span data-ttu-id="e4347-170">Os campos mostrados nesta página variam de país para país.</span><span class="sxs-lookup"><span data-stu-id="e4347-170">Fields shown on this page will vary by country.</span></span> 

4. <span data-ttu-id="e4347-171">Selecione **Seguinte**.</span><span class="sxs-lookup"><span data-stu-id="e4347-171">Select **Next**.</span></span>

5. <span data-ttu-id="e4347-172">Na página **do Beneficiário,** insira as informações apropriadas.</span><span class="sxs-lookup"><span data-stu-id="e4347-172">On the **Beneficiary** page, enter the appropriate information.</span></span> <span data-ttu-id="e4347-173">O beneficiário é a pessoa na sua empresa que o banco entraria em contacto se precisasse de discutir a sua conta.</span><span class="sxs-lookup"><span data-stu-id="e4347-173">The beneficiary is the person in your company that the bank would contact if they need to discuss your account.</span></span>

6. <span data-ttu-id="e4347-174">Quando os campos estiverem concluídos, selecione **Terminar** e, em seguida, selecione **Confirmar** para criar o seu perfil bancário.</span><span class="sxs-lookup"><span data-stu-id="e4347-174">When the fields are completed, select **Finish**, and then select **Confirm** to create your bank profile.</span></span>

<span data-ttu-id="e4347-175">Será redirecionado para a página **de pagamentos e perfis fiscais.**</span><span class="sxs-lookup"><span data-stu-id="e4347-175">You’ll be redirected to the **Payout and tax profiles** page.</span></span> <span data-ttu-id="e4347-176">O estado do seu novo perfil refletirá **a validação pendente** da Microsoft até que a validação esteja concluída.</span><span class="sxs-lookup"><span data-stu-id="e4347-176">The status of your new profile will reflect **Pending Microsoft validation** until the validation has been completed.</span></span> <span data-ttu-id="e4347-177">Este processo pode demorar até 48 horas.</span><span class="sxs-lookup"><span data-stu-id="e4347-177">This process may take up to 48 hours.</span></span> <span data-ttu-id="e4347-178">Uma vez concluída a validação, o seu estado de perfil refletirá quer **aprovado** quer **ação necessária**.</span><span class="sxs-lookup"><span data-stu-id="e4347-178">Once validation has been completed, your profile status will reflect either **Approved** or **Action required**.</span></span> <span data-ttu-id="e4347-179">Se **for necessário** agir, repita os passos acima, fornecendo as informações necessárias.</span><span class="sxs-lookup"><span data-stu-id="e4347-179">If **Action Required**, repeat the steps above providing the necessary information.</span></span> 

## <a name="create-your-tax-profile"></a><span data-ttu-id="e4347-180">Crie o seu perfil fiscal</span><span class="sxs-lookup"><span data-stu-id="e4347-180">Create your tax profile</span></span>

<span data-ttu-id="e4347-181">Utilize o seguinte procedimento para fornecer à Microsoft as informações fiscais necessárias para a sua organização.</span><span class="sxs-lookup"><span data-stu-id="e4347-181">Use the following procedure to provide Microsoft with the tax information required for your organization.</span></span> <span data-ttu-id="e4347-182">As páginas desta secção são dinâmicas e variam de acordo com o seu país ou região.</span><span class="sxs-lookup"><span data-stu-id="e4347-182">The pages in this section are dynamic and will vary according to your country or region.</span></span> <span data-ttu-id="e4347-183">Se precisar de ajuda para identificar as informações fiscais corretas, contacte as fontes governamentais apropriadas no seu país.</span><span class="sxs-lookup"><span data-stu-id="e4347-183">If you need help with identifying the correct tax information, contact the appropriate government sources in your country.</span></span>

<span data-ttu-id="e4347-184">Para empresas parceiras nas Américas, se necessitar de informações sobre o preenchimento dos formulários W8 ou W9, os seguintes endereços levam-no ao site do IRS:</span><span class="sxs-lookup"><span data-stu-id="e4347-184">For partner companies in the Americas, if you require information on completing the W8 or W9 forms, the following addresses take you to the IRS site:</span></span>

- [http://www.irs.gov/pub/irs-pdf/iw8.pdf](http://www.irs.gov/pub/irs-pdf/iw8.pdf)
- [http://www.irs.gov/pub/irs-pdf/iw9.pdf](http://www.irs.gov/pub/irs-pdf/iw9.pdf)

>[!IMPORTANT]
> <span data-ttu-id="e4347-185">Insira apenas detalhes para a sua empresa.</span><span class="sxs-lookup"><span data-stu-id="e4347-185">Enter only details for your company.</span></span> <span data-ttu-id="e4347-186">Nunca introduza detalhes pessoais.</span><span class="sxs-lookup"><span data-stu-id="e4347-186">Never enter personal details.</span></span>

1. <span data-ttu-id="e4347-187">Na página **'Perfil de** Negócios', preencha os campos necessários e, em seguida, selecione **Seguinte**.</span><span class="sxs-lookup"><span data-stu-id="e4347-187">On the **Business Profile** page, complete the required fields and then select **Next**.</span></span> 

2. <span data-ttu-id="e4347-188">Na página **Configuração,** selecione a opção que se aplica à sua empresa.</span><span class="sxs-lookup"><span data-stu-id="e4347-188">On the **Setup** page, select the option that applies to your company.</span></span>

   - <span data-ttu-id="e4347-189">Selecione a opção à esquerda se a sua empresa for incorporada apenas nos Estados Unidos, ou se este perfil for para um indivíduo.</span><span class="sxs-lookup"><span data-stu-id="e4347-189">Select the option on the left if your company is incorporated in the United States only, or if this profile is for an individual.</span></span>
   - <span data-ttu-id="e4347-190">Selecione a opção à direita se a sua empresa estiver incorporada fora dos Estados Unidos e, em seguida, selecione o seu país/região da lista.</span><span class="sxs-lookup"><span data-stu-id="e4347-190">Select the option on the right if your company is incorporated outside of the United States, and then select your country/region from the list.</span></span>

3. <span data-ttu-id="e4347-191">Selecione **Seguinte**.</span><span class="sxs-lookup"><span data-stu-id="e4347-191">Select **Next**.</span></span> 

4. <span data-ttu-id="e4347-192">Na página de estado do **Imposto,** insira as informações necessárias e, em seguida, selecione **Seguinte**.</span><span class="sxs-lookup"><span data-stu-id="e4347-192">On the **Tax status** page, enter the required information, and then select **Next**.</span></span> <span data-ttu-id="e4347-193">Os campos nesta página variam por país.</span><span class="sxs-lookup"><span data-stu-id="e4347-193">Fields on this page will vary by country.</span></span> <span data-ttu-id="e4347-194">seus detalhes.</span><span class="sxs-lookup"><span data-stu-id="e4347-194">your details.</span></span> 

5. <span data-ttu-id="e4347-195">Na página **de documentação adicional,** os campos necessários e selecione **Seguinte**.</span><span class="sxs-lookup"><span data-stu-id="e4347-195">On the **Additional documentation** page, the required fields and select **Next**.</span></span> 

6. <span data-ttu-id="e4347-196">**Selecione Procurar** para carregar quaisquer documentos necessários pelo seu país ou região.</span><span class="sxs-lookup"><span data-stu-id="e4347-196">Select **Browse** to upload any documents required by your country or region.</span></span> <span data-ttu-id="e4347-197">Quando o nome do documento for mostrado, selecione **Upload**.</span><span class="sxs-lookup"><span data-stu-id="e4347-197">When the document name is shown, select **Upload**.</span></span> 

7. <span data-ttu-id="e4347-198">Se precisar de remover o documento, selecione **Remover**.</span><span class="sxs-lookup"><span data-stu-id="e4347-198">If you need to remove the document, select **Remove**.</span></span>

8. <span data-ttu-id="e4347-199">Para guardar e continuar, **selecione Terminar**.</span><span class="sxs-lookup"><span data-stu-id="e4347-199">To save and continue, select **Finish**.</span></span>

9. <span data-ttu-id="e4347-200">**Selecione Confirme** na mensagem pop-up.</span><span class="sxs-lookup"><span data-stu-id="e4347-200">Select **Confirm** on the pop-up message.</span></span> <span data-ttu-id="e4347-201">Você será levado de volta para a página **de pagamento e configuração de impostos.**</span><span class="sxs-lookup"><span data-stu-id="e4347-201">You’ll be taken back to the **Payout and tax setup** page.</span></span>

## <a name="next-steps"></a><span data-ttu-id="e4347-202">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="e4347-202">Next steps</span></span>

- [<span data-ttu-id="e4347-203">Questões comuns sobre pagamentos e impostos</span><span class="sxs-lookup"><span data-stu-id="e4347-203">Common questions about payouts and taxes</span></span>](payout-faq.md)
