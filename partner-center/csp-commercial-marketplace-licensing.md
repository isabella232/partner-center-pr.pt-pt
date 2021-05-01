---
title: Gerir licenciamento em ofertas de marketplace
ms.topic: how-to
ms.date: 04/29/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como configurar e gerir o licenciamento para as suas ofertas de mercado comercial ISV.
author: petand123
ms.author: v-petand
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f049ffda4c3d9476c09257fc814e5acac393cb54
ms.sourcegitcommit: 6c20c3cc4a226cada70c56df295966696affcec8
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/30/2021
ms.locfileid: "108328020"
---
# <a name="manage-licensing-in-marketplace-offers"></a><span data-ttu-id="8cfd5-103">Gerir licenciamento em ofertas de marketplace</span><span class="sxs-lookup"><span data-stu-id="8cfd5-103">Manage licensing in marketplace offers</span></span>

<span data-ttu-id="8cfd5-104">**Funções adequadas**</span><span class="sxs-lookup"><span data-stu-id="8cfd5-104">**Appropriate roles**</span></span>

- <span data-ttu-id="8cfd5-105">Administrador global</span><span class="sxs-lookup"><span data-stu-id="8cfd5-105">Global admin</span></span>
- <span data-ttu-id="8cfd5-106">Administrador de conta</span><span class="sxs-lookup"><span data-stu-id="8cfd5-106">Account admin</span></span>

<span data-ttu-id="8cfd5-107">Este artigo acompanha-o através do processo de criação de uma oferta no Partner Center, disponibilizando-a no Microsoft AppSource e, em seguida, gerindo licenças para essa oferta.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-107">This article walks you through the process of setting up an offer in Partner Center, making it available in Microsoft AppSource, and then managing licenses for that offer.</span></span>  

>[!IMPORTANT]
><span data-ttu-id="8cfd5-108">As capacidades deste artigo estão atualmente em Visualização Pública.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-108">The capabilities in this article are currently in Public Preview.</span></span>

## <a name="before-you-begin"></a><span data-ttu-id="8cfd5-109">Antes de começar</span><span class="sxs-lookup"><span data-stu-id="8cfd5-109">Before you begin</span></span>

### <a name="commercial-marketplace-basics"></a><span data-ttu-id="8cfd5-110">Básicos do mercado comercial</span><span class="sxs-lookup"><span data-stu-id="8cfd5-110">Commercial marketplace basics</span></span>

<span data-ttu-id="8cfd5-111">Antes de iniciar este processo, deve familiarizar-se com o básico do mercado comercial.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-111">Before you begin this process, you should familiarize yourself with the basics of the commercial marketplace.</span></span> <span data-ttu-id="8cfd5-112">Os artigos na tabela abaixo ajudarão a começar.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-112">The articles in the table below will help get you started.</span></span> 

| <span data-ttu-id="8cfd5-113">Tópico</span><span class="sxs-lookup"><span data-stu-id="8cfd5-113">Topic</span></span>  | <span data-ttu-id="8cfd5-114">Artigo</span><span class="sxs-lookup"><span data-stu-id="8cfd5-114">Article</span></span>  |
|-------|--------|
|<span data-ttu-id="8cfd5-115">Planos de mercado comercial</span><span class="sxs-lookup"><span data-stu-id="8cfd5-115">Commercial marketplace plans</span></span> | [<span data-ttu-id="8cfd5-116">Planos e preços para ofertas de mercado comercial</span><span class="sxs-lookup"><span data-stu-id="8cfd5-116">Plans and pricing for commercial marketplace offers</span></span>](/azure/marketplace/plans-pricing)    |
|<span data-ttu-id="8cfd5-117">Ofertas de mercado comercial</span><span class="sxs-lookup"><span data-stu-id="8cfd5-117">Commercial marketplace offers</span></span>  | [<span data-ttu-id="8cfd5-118">Tipos de listagem</span><span class="sxs-lookup"><span data-stu-id="8cfd5-118">Listing types</span></span>](/azure/marketplace/determine-your-listing-type)    |
|<span data-ttu-id="8cfd5-119">Contas de mercado comercial</span><span class="sxs-lookup"><span data-stu-id="8cfd5-119">Commercial marketplace accounts</span></span> |  [<span data-ttu-id="8cfd5-120">Criar uma conta de mercado comercial no Partner Center</span><span class="sxs-lookup"><span data-stu-id="8cfd5-120">Create a commercial marketplace account in Partner Center</span></span>](/azure/marketplace/create-account) |

### <a name="determine-your-offer-id"></a><span data-ttu-id="8cfd5-121">Determine o seu ID de oferta</span><span class="sxs-lookup"><span data-stu-id="8cfd5-121">Determine your Offer ID</span></span>

<span data-ttu-id="8cfd5-122">Nos procedimentos abaixo, você será solicitado para introduzir um ID de oferta.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-122">In the procedures below, you’ll be prompted to enter an Offer ID.</span></span> <span data-ttu-id="8cfd5-123">Dedem um pouco para chegar a um ID de oferta adequado, tendo em conta os seguintes pontos:</span><span class="sxs-lookup"><span data-stu-id="8cfd5-123">Take some time now to come up with a suitable Offer ID, keeping in mind the following points:</span></span>

- <span data-ttu-id="8cfd5-124">Este ID é visível para os clientes no endereço web para a oferta de mercado e modelos de Gestor de Recursos Azure, se aplicável.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-124">This ID is visible to customers in the web address for the marketplace offer and Azure Resource Manager templates, if applicable.</span></span>
- <span data-ttu-id="8cfd5-125">O ID da oferta combinado com o ID da Editora deve ter menos de 40 caracteres de comprimento.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-125">The Offer ID combined with the Publisher ID must be under 40 characters in length.</span></span>
- <span data-ttu-id="8cfd5-126">Utilize apenas letras minúsculas e números.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-126">Use only lowercase letters and numbers.</span></span> <span data-ttu-id="8cfd5-127">O ID da Oferta pode incluir hífens e sublinhados, mas sem espaços.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-127">The Offer ID can include hyphens and underscores, but no spaces.</span></span> <span data-ttu-id="8cfd5-128">Por exemplo, se o seu ID de editor estiver `testpublisherid` e `test-offer-1` introduzir, o endereço web da oferta será `https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1` .</span><span class="sxs-lookup"><span data-stu-id="8cfd5-128">For example, if your Publisher ID is `testpublisherid` and you enter `test-offer-1`, the offer web address will be `https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1`.</span></span>
- <span data-ttu-id="8cfd5-129">Este ID não pode ser alterado depois de selecionar **Criar**.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-129">This ID can't be changed after you select **Create**.</span></span>

### <a name="determine-your-offer-alias"></a><span data-ttu-id="8cfd5-130">Determine o seu pseudónimo oferta</span><span class="sxs-lookup"><span data-stu-id="8cfd5-130">Determine your Offer alias</span></span>

<span data-ttu-id="8cfd5-131">O pseudónimo Offer é o nome usado para a oferta no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-131">The Offer alias is the name used for the offer in Partner Center.</span></span> <span data-ttu-id="8cfd5-132">Você também precisará de um pseudónimo de Oferta apropriado que siga as diretrizes abaixo:</span><span class="sxs-lookup"><span data-stu-id="8cfd5-132">You’ll also need an appropriate Offer alias that follows the guidelines below:</span></span>

- <span data-ttu-id="8cfd5-133">Este nome não é usado no mercado e é diferente do nome da oferta e outros valores mostrados aos clientes.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-133">This name isn't used in the marketplace and is different from the offer name and other values shown to customers.</span></span>
- <span data-ttu-id="8cfd5-134">Este nome não pode ser alterado depois de selecionar Criar.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-134">This name can't be changed after you select Create.</span></span>

## <a name="create-your-offer"></a><span data-ttu-id="8cfd5-135">Crie a sua oferta</span><span class="sxs-lookup"><span data-stu-id="8cfd5-135">Create your offer</span></span>

<span data-ttu-id="8cfd5-136">O primeiro passo no processo de licenciamento é criar a sua oferta de mercado comercial.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-136">The first step in the licensing process is to create your commercial marketplace offer.</span></span> 

1. <span data-ttu-id="8cfd5-137">Inicie sessão no [dashboard do Centro de Parceiros](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="8cfd5-137">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="8cfd5-138">No menu de navegação à esquerda, selecione **Commercial Marketplace/Overview**.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-138">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="8cfd5-139">No topo da página 'Overview', selecione **Nova oferta** e, em seguida, selecione **Dynamics 365 para Customer Engagement & PowerApps**.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-139">At the top of the Overview page, select **New offer**, and then select **Dynamics 365 for Customer Engagement & PowerApps**.</span></span>
4. <span data-ttu-id="8cfd5-140">Insira o **ID da Oferta** e **ofereça o pseudónimo** que criou anteriormente.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-140">Enter the **Offer ID** and **Offer alias** you created earlier.</span></span>
5. <span data-ttu-id="8cfd5-141">Selecione **Criar** para gerar a oferta e continuar.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-141">Select **Create** to generate the offer and continue.</span></span>
6. <span data-ttu-id="8cfd5-142">Escolha as suas opções de licenciamento.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-142">Choose your licensing options.</span></span>

    - <span data-ttu-id="8cfd5-143">Para ativar a gestão da licença para a sua oferta, selecione **Ative a gestão da licença de aplicações através da Microsoft.**</span><span class="sxs-lookup"><span data-stu-id="8cfd5-143">To enable license management for your offer, select **Enable app license management through Microsoft**.</span></span> <span data-ttu-id="8cfd5-144">Este é um cenário único, e não pode mudá-lo uma vez que a sua oferta é publicada.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-144">This is a one-time setting, and you can’t change it once your offer is published.</span></span>

    - <span data-ttu-id="8cfd5-145">Também pode permitir que os clientes executem a funcionalidade base da sua aplicação sem licença e executem funcionalidades premium uma vez que tenham adquirido uma licença.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-145">You can also enable customers to run your app’s base functionality without a license, and run premium features once they’ve purchased a license.</span></span> <span data-ttu-id="8cfd5-146">Para isso, selecione **Permitir que os clientes instalem a minha aplicação mesmo que as licenças não sejam atribuídas.**</span><span class="sxs-lookup"><span data-stu-id="8cfd5-146">To do this, select **Allow customers to install my app even if licenses are not assigned**.</span></span>

    - <span data-ttu-id="8cfd5-147">Se não quiser que a sua oferta tenha a gestão da licença ativada, selecione **Get it now (Free)**, **Free trial**, ou **Contacte-me**.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-147">If you don’t want your offer to have license management enabled, select **Get it now (Free)**, **Free trial**, or **Contact me**.</span></span>

## <a name="create-your-plan"></a><span data-ttu-id="8cfd5-148">Criar o plano</span><span class="sxs-lookup"><span data-stu-id="8cfd5-148">Create your plan</span></span>

<span data-ttu-id="8cfd5-149">Nestes passos definirá o plano ou planos que deseja ativar para a sua oferta.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-149">In these steps you’ll define the plan or plans you want to enable for your offer.</span></span>

1. <span data-ttu-id="8cfd5-150">No menu de navegação à esquerda, selecione **Plan overview** e, em seguida, selecione **Criar novo plano**.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-150">On the left navigation menu, select **Plan overview**, and then select **Create new plan**.</span></span>
2. <span data-ttu-id="8cfd5-151">Introduza o nome **de identificação** e **plano do** plano e, em seguida, selecione **Criar**.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-151">Enter a **Plan ID** and **Plan name**, and then select **Create**.</span></span>
3. <span data-ttu-id="8cfd5-152">Na página de listagem do **Plano,** insira a **descrição do seu Plano.**</span><span class="sxs-lookup"><span data-stu-id="8cfd5-152">On the **Plan listing** page, enter your **Plan description**.</span></span>
4. <span data-ttu-id="8cfd5-153">Para guardar a descrição e terminar mais tarde, **selecione Guardar o rascunho**.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-153">To save the description and finish later, select **Save draft**.</span></span>

5. <span data-ttu-id="8cfd5-154">Quando terminar, selecione **'Rever' e publicar.**</span><span class="sxs-lookup"><span data-stu-id="8cfd5-154">When you’re finished, select **Review and publish**.</span></span> <span data-ttu-id="8cfd5-155">A informação do plano será agora exibida no appsource.microsoft.com em lista de ofertas (secção de planos).</span><span class="sxs-lookup"><span data-stu-id="8cfd5-155">The plan information will now be displayed on appsource.microsoft.com under offer listing (plans section).</span></span>

6. <span data-ttu-id="8cfd5-156">Depois de ter criado todos os planos para esta oferta, terá de copiar o ID de serviço de cada plano.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-156">After you’ve created all of the plans for this offer, you’ll need to copy each plan’s Service ID.</span></span> <span data-ttu-id="8cfd5-157">Selecione **a visão geral** do plano no topo da página de listagem do Plano.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-157">Select **Plan overview** at the top of the Plan listing page.</span></span> <span data-ttu-id="8cfd5-158">Copie o ID de serviço para cada plano para um local seguro.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-158">Copy the Service ID for each plan to a safe location.</span></span>

## <a name="add-service-ids-to-your-solution"></a><span data-ttu-id="8cfd5-159">Adicione IDs de serviço à sua solução</span><span class="sxs-lookup"><span data-stu-id="8cfd5-159">Add Service IDs to your solution</span></span>

<span data-ttu-id="8cfd5-160">O próximo passo é atualizar a sua solução adicionando os IDs de serviço para cada plano que acabou de copiar.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-160">The next step is to update your solution by adding the Service IDs for each plan that you just copied.</span></span> <span data-ttu-id="8cfd5-161">Para obter orientações sobre este ponto, consulte [Criar um Pacote AppSource para a sua solução.](https://docs.microsoft.com/powerapps/developer/data-platform/create-package-app-appsource)</span><span class="sxs-lookup"><span data-stu-id="8cfd5-161">For guidance on this, see [Create an AppSource Package for your solution](https://docs.microsoft.com/powerapps/developer/data-platform/create-package-app-appsource).</span></span>

## <a name="upload-your-package-and-publish-your-offer"></a><span data-ttu-id="8cfd5-162">Faça upload do seu pacote e publique a sua oferta</span><span class="sxs-lookup"><span data-stu-id="8cfd5-162">Upload your package and publish your offer</span></span>

1. <span data-ttu-id="8cfd5-163">No painel de navegação à esquerda, selecione **Mercado Comercial** e, em seguida, selecione **configuração técnica**.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-163">On the left navigation pane, select **Commercial Marketplace**, and then select **Technical configuration**.</span></span>
2. <span data-ttu-id="8cfd5-164">Sob **o Modelo base de licença,** selecione **Utilizador.**</span><span class="sxs-lookup"><span data-stu-id="8cfd5-164">Under **Base License Model**, select **User**.</span></span>
3. <span data-ttu-id="8cfd5-165">No **pacote CRM,** insira o URL da sua localização do pacote.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-165">Under **CRM Package**, enter the URL of your package location.</span></span>
4. <span data-ttu-id="8cfd5-166">Utilize os outros separadores no painel de navegação esquerdo para introduzir qualquer outra informação necessária.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-166">Use the other tabs on the left navigation pane to enter any other required information.</span></span> <span data-ttu-id="8cfd5-167">Quando terminar, selecione **'Rever' e publicar**.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-167">When you’re done, select **Review and publish**.</span></span>

<span data-ttu-id="8cfd5-168">Depois de publicar a oferta, vamos rever e verificar as suas informações.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-168">After you publish the offer, we’ll review and verify your information.</span></span> <span data-ttu-id="8cfd5-169">Se houver algum problema com este processo, vamos notificá-lo.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-169">If there are any issues with this process, we’ll notify you.</span></span> <span data-ttu-id="8cfd5-170">Quando todos os problemas tiverem sido resolvidos, receberá uma notificação de que a sua oferta está disponível no AppSource.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-170">When all issues have been resolved, you’ll get a notification that your offer is available in AppSource.</span></span> <span data-ttu-id="8cfd5-171">Nessa altura, podes fazê-lo viver.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-171">At that point you can make it live.</span></span>

## <a name="make-your-offer-live-in-partner-center"></a><span data-ttu-id="8cfd5-172">Faça a sua oferta ao vivo no Partner Center</span><span class="sxs-lookup"><span data-stu-id="8cfd5-172">Make your offer live in Partner Center</span></span>

<span data-ttu-id="8cfd5-173">O procedimento abaixo acompanha-o através do processo de fazer a sua oferta ao vivo no AppSource.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-173">The procedure below walks you through the process of making your offer live in AppSource.</span></span> <span data-ttu-id="8cfd5-174">Para saber mais sobre este processo, consulte [Introdução às opções de listagem.](https://docs.microsoft.com/azure/marketplace/determine-your-listing-type)</span><span class="sxs-lookup"><span data-stu-id="8cfd5-174">To learn more about this process, see [Introduction to listing options](https://docs.microsoft.com/azure/marketplace/determine-your-listing-type).</span></span>

>[!NOTE]
><span data-ttu-id="8cfd5-175">Uma vez publicada a sua oferta, levará 4 a 6 horas para ir ao vivo.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-175">Once you publish your offer, it will take 4-6 hours to go live.</span></span>

1. <span data-ttu-id="8cfd5-176">Inicie sessão no [dashboard do Centro de Parceiros](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="8cfd5-176">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="8cfd5-177">No menu de navegação à esquerda, selecione **Commercial Marketplace/Overview**.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-177">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="8cfd5-178">Na página **geral,** encontre a oferta que procura.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-178">On the **Overview** page, find the offer you’re looking for.</span></span> <span data-ttu-id="8cfd5-179">As ofertas prontas a serem publicadas terão um estatuto de **Pré-visualização**.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-179">Offers ready to be published will have a status of **Preview**.</span></span> <span data-ttu-id="8cfd5-180">Selecione a oferta.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-180">Select the offer.</span></span>
4. <span data-ttu-id="8cfd5-181">Na página geral da **Oferta,** selecione **Go live**.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-181">On the **Offer overview** page, select **Go live**.</span></span>
<span data-ttu-id="8cfd5-182">A oferta será ao vivo em 4-6 horas.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-182">The offer will be live in 4-6 hours.</span></span>
5. <span data-ttu-id="8cfd5-183">Para ver a sua lista de ofertas no AppSource, selecione o link **AppSource** na parte inferior da página geral da **Oferta.**</span><span class="sxs-lookup"><span data-stu-id="8cfd5-183">To see your offer listing on AppSource, select the **AppSource** link at the bottom of the **Offer overview** page.</span></span>

    - <span data-ttu-id="8cfd5-184">**Para ofertas habilitados a licença :** Se a sua oferta necessitar de uma verificação de licença, os utilizadores só poderão introduzir uma pista clicando **em Contato comigo**, para que possa comunicar com eles.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-184">**For license-enabled offers**: If your offer requires a license check, users will only be able to enter a lead by clicking **Contact Me**, so that you can communicate with them.</span></span>

    - <span data-ttu-id="8cfd5-185">**Para ofertas habilitados a licenças com opção de instalação gratuita**: Se a sua oferta não necessitar de uma verificação de licença, os utilizadores administrativos verão um botão **Get It Now** para além do Contact **Me**.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-185">**For license-enabled offers with free installation option**: If your offer does not require a license check, admin users will see a **Get It Now** button in addition to **Contact Me**.</span></span> <span data-ttu-id="8cfd5-186">Os utilizadores que pretendam experimentar a sua opção de instalação gratuita devem clicar em **Get It Now**, o que os levará a instalar a oferta no Power Platform Admin Center.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-186">Users who want to try your free installation option should click **Get It Now**, which will bring them to install the offer on Power Platform Admin Center.</span></span> <span data-ttu-id="8cfd5-187">Os utilizadores ainda podem utilizar **o Contato Me** se tiverem alguma dúvida, ou se quiserem fazer upgrade para um plano pago.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-187">Users can still use **Contact Me** if they have any questions, or if they want to upgrade to a paid plan.</span></span>

## <a name="register-isv-connect-deal-in-deal-registration"></a><span data-ttu-id="8cfd5-188">Registre o negócio ISV Connect no Registo de Negócios</span><span class="sxs-lookup"><span data-stu-id="8cfd5-188">Register ISV Connect deal in Deal Registration</span></span>

<span data-ttu-id="8cfd5-189">Antes de poder atribuir licenças a um cliente, cada venda tem de ser registada no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-189">Before you can assign licenses to a customer, each sale needs to be registered in Partner Center.</span></span> <span data-ttu-id="8cfd5-190">Para isso, consulte [registar as suas ofertas.](register-deals.md)</span><span class="sxs-lookup"><span data-stu-id="8cfd5-190">To do this, see [Register your deals](register-deals.md).</span></span>

## <a name="invite-the-customer"></a><span data-ttu-id="8cfd5-191">Convide o cliente</span><span class="sxs-lookup"><span data-stu-id="8cfd5-191">Invite the customer</span></span>

<span data-ttu-id="8cfd5-192">Utilize o seguinte procedimento para convidar o cliente a participar neste negócio.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-192">Use the following procedure to invite the customer to participate in this deal.</span></span>  

1. <span data-ttu-id="8cfd5-193">Inicie sessão no [dashboard do Centro de Parceiros](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="8cfd5-193">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="8cfd5-194">No menu de navegação à esquerda, selecione **Commercial Marketplace/Overview**.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-194">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="8cfd5-195">No menu de navegação à esquerda, selecione **Referências** e, em seguida, selecione **'Registar negócios'.**</span><span class="sxs-lookup"><span data-stu-id="8cfd5-195">On the left navigation menu, select **Referrals**, and then select **Deal Registration**.</span></span>
4. <span data-ttu-id="8cfd5-196">Filtrar para **ofertas submetidas,** selecione o separador **Em Progresso** e, em seguida, selecione o negócio que deseja.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-196">Filter for **Submitted** deals, select the **In Progress** tab, and then select the deal you want.</span></span>
5. <span data-ttu-id="8cfd5-197">Na página geral para este negócio, selecione **Gerir licenças**.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-197">On the overview page for this deal, select **Manage licenses**.</span></span>
6. <span data-ttu-id="8cfd5-198">Na janela **de licenças 'Gerir',** selecione o cliente da lista de dados do **Cliente.**</span><span class="sxs-lookup"><span data-stu-id="8cfd5-198">In the **Manage licenses** window, select the customer from the **Customer details** dropdown list.</span></span> <span data-ttu-id="8cfd5-199">Se a relação com o cliente ainda não existir, selecione **+Convide um novo cliente a consentir.**</span><span class="sxs-lookup"><span data-stu-id="8cfd5-199">If the customer relationship does not exist yet, select **+Invite a new customer to consent**.</span></span>
7. <span data-ttu-id="8cfd5-200">Copie o link que é apresentado.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-200">Copy the link that is displayed.</span></span>
8. <span data-ttu-id="8cfd5-201">Envie este link por e-mail para a administração de faturação ou administração global do seu cliente, e faça-os usar este link para aceder a admin.microsoft.com e aceitar e autorizar a relação que está a estabelecer.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-201">Email this link to your customer’s billing admin or global admin, and have them use this link to access admin.microsoft.com and accept and authorize the relationship you’re establishing.</span></span>

    >[!NOTE]
    ><span data-ttu-id="8cfd5-202">A relação não será estabelecida até que o cliente realize este passo.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-202">The relationship will not be established until the customer performs this step.</span></span>

## <a name="activate-manage-and-remove-your-licenses"></a><span data-ttu-id="8cfd5-203">Ativar, gerir e remover as suas licenças</span><span class="sxs-lookup"><span data-stu-id="8cfd5-203">Activate, manage, and remove your licenses</span></span>

<span data-ttu-id="8cfd5-204">Uma vez que o seu cliente tenha autorizado a relação consigo, pode começar a adicionar planos da sua oferta e a atribuir licenças a cada plano.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-204">Once your customer has authorized the relationship with you, you can start adding plans from your offer and assigning licenses to each plan.</span></span>

1. <span data-ttu-id="8cfd5-205">Na janela de licenças Manage para este negócio, selecione **+Adicione um plano**.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-205">In the Manage licenses window for this deal, select **+Add a plan**.</span></span>
2. <span data-ttu-id="8cfd5-206">Preencha os **Planos para esta solução** e número de campos **de licenças** e, em seguida, selecione **licenças de Atualização**.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-206">Complete the **Plans for this solution** and **Number of licenses** fields, and then select **Update licenses**.</span></span> <span data-ttu-id="8cfd5-207">As licenças estarão disponíveis em admin.microsoft.com para os clientes gerirem e atribuíram aos colaboradores.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-207">The licenses will be available at admin.microsoft.com for customers to manage and assign to employees.</span></span>

    - <span data-ttu-id="8cfd5-208">Para alterar o número de licenças para um plano existente, insira o novo número no campo **Número de licenças** e, em seguida, selecione **Licenças de Atualização**.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-208">To change the number of licenses for an existing plan, enter the new number in the **Number of licenses** field and then select **Update licenses**.</span></span>

    - <span data-ttu-id="8cfd5-209">Para desativar ou remover licenças para uma oferta, selecione o ícone do caixote do lixo no campo Ações e, em seguida, selecione **'Update licenses'** **(Atualização).**</span><span class="sxs-lookup"><span data-stu-id="8cfd5-209">To deactivate or remove licenses for a deal, select the trash can icon in the **Actions** field and then select **Update licenses**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="8cfd5-210">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="8cfd5-210">Next steps</span></span>

[<span data-ttu-id="8cfd5-211">Recursos de licenças</span><span class="sxs-lookup"><span data-stu-id="8cfd5-211">Licensing resources</span></span>](support-resources-licensing.md)
