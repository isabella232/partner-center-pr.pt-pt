---
title: Mude o parceiro de conta direta para o revendedor indireto
ms.topic: how-to
ms.date: 06/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como um parceiro de programa CSP pode usar o Partner Center para transitar de parceiro de conta direta para revendedor indireto.
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e3cd791f5f9f781980d73c79f0ec18627585372a
ms.sourcegitcommit: b4771fd0781d95551e65baa481a572291c729d7d
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/28/2020
ms.locfileid: "92795870"
---
# <a name="transition-from-cloud-solution-provider-csp-direct-bill-partner-to-csp-indirect-reseller"></a><span data-ttu-id="e471f-103">Transição do parceiro de faturação direta do Fornecedor de Soluções Cloud para o revendedor indireto do CSP</span><span class="sxs-lookup"><span data-stu-id="e471f-103">Transition from Cloud Solution Provider (CSP) direct bill partner to CSP indirect reseller</span></span>

<span data-ttu-id="e471f-104">**Aplica-se a:**</span><span class="sxs-lookup"><span data-stu-id="e471f-104">**Applies to:**</span></span>
- <span data-ttu-id="e471f-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="e471f-105">Partner Center</span></span>

<span data-ttu-id="e471f-106">**Funções adequadas**</span><span class="sxs-lookup"><span data-stu-id="e471f-106">**Appropriate roles**</span></span>

- <span data-ttu-id="e471f-107">Todos os parceiros de conta direto cSP</span><span class="sxs-lookup"><span data-stu-id="e471f-107">All CSP direct bill partners</span></span>

>[!Note]
><span data-ttu-id="e471f-108">Este artigo destina-se a parceiros de conta direta que tenham decidido transitar para revendedores indiretos.</span><span class="sxs-lookup"><span data-stu-id="e471f-108">This article is intended for direct bill partners who have decided to transition to indirect resellers.</span></span> <span data-ttu-id="e471f-109">No entanto, mesmo que ainda não tenha tido uma decisão explícita de se inscrever como revendedor indireto, os parceiros de conta direto que não satisfaçam os novos requisitos para o programa de [parceiros](direct-partner-new-requirements.md) de conta direta CSP serão informados pela Microsoft quando as suas [capacidades de conta direta forem restringidas.](restricted-direct-bill-capabilities.md)</span><span class="sxs-lookup"><span data-stu-id="e471f-109">However, even if you have not made an explicit decision yet to enroll as an indirect reseller, direct bill partners who do not meet the new [requirements](direct-partner-new-requirements.md) for the CSP direct bill partner program will be informed by Microsoft when their [direct bill capabilities will be restricted](restricted-direct-bill-capabilities.md).</span></span>
<br><span data-ttu-id="e471f-110">A partir de janeiro de 2021, será adicionado um novo requisito de receita.</span><span class="sxs-lookup"><span data-stu-id="e471f-110">As of January 2021, a new revenue requirement will be added.</span></span> <span data-ttu-id="e471f-111">Os parceiros inscritos como parceiro de conta direta terão de ter transacionado pelo menos USD$300K em receitas do programa Cloud Solution Provider a um nível de Conta Global de Parceiros nos 12 meses anteriores.</span><span class="sxs-lookup"><span data-stu-id="e471f-111">Partners enrolled as a direct bill partner will need to have transacted at least USD$300K in Cloud Solution Provider program revenue at a Partner Global Account level over the previous 12 months.</span></span>

<span data-ttu-id="e471f-112">Poderá inscrever-se no programa de revenda indireto utilizando o seu inquilino de fatura direta existente.</span><span class="sxs-lookup"><span data-stu-id="e471f-112">You will be able to enroll in the indirect reseller program using your existing direct bill tenant.</span></span>

## <a name="get-started"></a><span data-ttu-id="e471f-113">Introdução</span><span class="sxs-lookup"><span data-stu-id="e471f-113">Get started</span></span>

1. <span data-ttu-id="e471f-114">Certifique-se de que o perfil do seu parceiro no Partner Center e no MPN ID estão em vigor.</span><span class="sxs-lookup"><span data-stu-id="e471f-114">Make sure your partner profile in Partner Center and MPN ID are current.</span></span>

2. <span data-ttu-id="e471f-115">Inscreva-se no Partner Center como administrador global para o inquilino de conta direta que está a transitar para o revendedor indireto.</span><span class="sxs-lookup"><span data-stu-id="e471f-115">Sign in to Partner Center as the global admin for the direct bill tenant you are transitioning to indirect reseller.</span></span>

   :::image type="content" source="images/direct/direct1.png" alt-text="Descrição geral":::

3. <span data-ttu-id="e471f-117">Reveja os detalhes do seu parceiro no formulário de inscrição.</span><span class="sxs-lookup"><span data-stu-id="e471f-117">Review your partner details on the enrollment form.</span></span>

   :::image type="content" source="images/direct/direct2a.png" alt-text="Inscreva-se agora":::

4. <span data-ttu-id="e471f-119">Selecione Matricular-se agora.</span><span class="sxs-lookup"><span data-stu-id="e471f-119">Select Enroll now.</span></span> <span data-ttu-id="e471f-120">O seu negócio de revendedor indireto usará o mesmo inquilino da AAD que usa para o seu negócio direto.</span><span class="sxs-lookup"><span data-stu-id="e471f-120">Your indirect reseller business will use the same AAD tenant you use for your direct business.</span></span>

    > [!NOTE]
    > <span data-ttu-id="e471f-121">Inicialmente, esta nova capacidade de transição estará disponível para parceiros com datas de aniversário de setembro a dezembro.</span><span class="sxs-lookup"><span data-stu-id="e471f-121">Initially, this new transition capability will be available for partners with September to December anniversary dates.</span></span> <span data-ttu-id="e471f-122">Se não tiver uma data de aniversário entre setembro e dezembro, não verá a capacidade neste momento.</span><span class="sxs-lookup"><span data-stu-id="e471f-122">If you don"t have an anniversary date between September and December, you won't see the capability at this time.</span></span> <span data-ttu-id="e471f-123">Os parceiros com datas de aniversário após dezembro de 2018 serão notificados mais tarde assim que a funcionalidade estiver ativada para os parceiros.</span><span class="sxs-lookup"><span data-stu-id="e471f-123">Partners with anniversary dates after December 2018 will be notified later once the feature is enabled for the partners.</span></span>

5. <span data-ttu-id="e471f-124">Quando a sua inscrição for aprovada, inscreva-se novamente no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="e471f-124">When your enrollment is approved, sign in to Partner Center again.</span></span>

    > [!NOTE]
    > <span data-ttu-id="e471f-125">Embora a aprovação seja geralmente imediata, pode levar até cinco dias úteis.</span><span class="sxs-lookup"><span data-stu-id="e471f-125">While approval is usually immediate, it can take up to five business days.</span></span> <span data-ttu-id="e471f-126">Uma vez aprovado, receberá uma notificação para o endereço de e-mail que especificou no contacto primário no formulário de inscrição.</span><span class="sxs-lookup"><span data-stu-id="e471f-126">Once approved, you will receive a notification to the email address you have specified under primary contact in the enrollment form.</span></span> <span data-ttu-id="e471f-127">Também pode verificar o **Settings** estado de inscrição nas  >  **definições de definições de parceiros**  >  **Partner Profile** > informações do Programa.</span><span class="sxs-lookup"><span data-stu-id="e471f-127">You can also check your enrollment status under **Settings** > **Partner Settings** > **Partner Profile** > Program info.</span></span>

6. <span data-ttu-id="e471f-128">Na sua página **de visão geral,** verá o acordo de revendedor indireto.</span><span class="sxs-lookup"><span data-stu-id="e471f-128">On your **Overview** page, you will see the indirect reseller agreement.</span></span> <span data-ttu-id="e471f-129">Selecione **Aceitar e continuar.**</span><span class="sxs-lookup"><span data-stu-id="e471f-129">Select **Accept and continue** .</span></span> <span data-ttu-id="e471f-130">Esta ação permite as capacidades de revendedor indiretos.</span><span class="sxs-lookup"><span data-stu-id="e471f-130">This action enables the indirect reseller capabilities.</span></span>

<span data-ttu-id="e471f-131">Quando aceitar o acordo de revendedor indireto, note que o seu perfil de Parceiro o identifica **como** uma fatura direta e um revendedor indireto.</span><span class="sxs-lookup"><span data-stu-id="e471f-131">When you have accepted the indirect reseller agreement, notice that your Partner profile identifies you as **both** a direct bill and indirect reseller.</span></span>

:::image type="content" source="images/direct/direct3.png" alt-text="Acordo de revendedor indireto":::

> [!IMPORTANT]
> <span data-ttu-id="e471f-133">Uma vez que você se inscreva como um revendedor indireto usando a nova capacidade, não há opção para reverter para um inquilino direto apenas.</span><span class="sxs-lookup"><span data-stu-id="e471f-133">Once you enroll as an indirect reseller using the new capability, there is no option to roll back to a direct bill- only tenant.</span></span> <span data-ttu-id="e471f-134">Por favor, certifique-se de que avalia totalmente as necessidades do seu negócio antes de se inscrever como revendedor indireto.</span><span class="sxs-lookup"><span data-stu-id="e471f-134">Please make sure that you fully evaluate your business needs before enrolling as an indirect reseller.</span></span>

## <a name="while-you-transition-from-direct-to-indirect-reseller"></a><span data-ttu-id="e471f-135">Enquanto faz a transição do revendedor direto para o revendedor indireto</span><span class="sxs-lookup"><span data-stu-id="e471f-135">While you transition from direct to indirect reseller</span></span>

<span data-ttu-id="e471f-136">Durante esta fase, continuará a gerir as necessidades de subscrição dos seus clientes diretos, incluindo o processo de faturação.</span><span class="sxs-lookup"><span data-stu-id="e471f-136">During this phase, you will continue to manage your direct customers' subscription needs including the billing process.</span></span> <span data-ttu-id="e471f-137">Também pode começar a aceitar clientes do seu fornecedor Indireto e a operar como revendedor indireto.</span><span class="sxs-lookup"><span data-stu-id="e471f-137">You can also begin accepting customers from your Indirect provider and operating as an indirect reseller.</span></span>

:::image type="content" source="images/direct/direct4.png" alt-text="Ambos são uma conta direta e um revendedor indireto":::

## <a name="find-an-indirect-provider"></a><span data-ttu-id="e471f-139">Localizar um fornecedor indireto</span><span class="sxs-lookup"><span data-stu-id="e471f-139">Find an indirect provider</span></span>

<span data-ttu-id="e471f-140">Após a inscrição, aparecerá um link para fornecedores indiretos no seu navegador esquerdo.</span><span class="sxs-lookup"><span data-stu-id="e471f-140">After enrolling, a link to Indirect providers will appear in your left nav.</span></span> <span data-ttu-id="e471f-141">Como revendedor indireto, estabelecerá uma relação com um fornecedor indireto que poderá então lidar com a sua faturação, comprar produtos para os seus clientes e apoiar a infraestrutura.</span><span class="sxs-lookup"><span data-stu-id="e471f-141">As an indirect reseller you will establish a relationship with an indirect provider who then can handle your billing, purchase products for your customers, and support infrastructure.</span></span>

<span data-ttu-id="e471f-142">Diferentes fornecedores indiretos oferecem diferentes suportes e serviços, por isso deve avaliar os fornecedores da sua área para determinar quais os que melhor satisfazem as suas necessidades.</span><span class="sxs-lookup"><span data-stu-id="e471f-142">Different indirect providers offer different support and services, so you should evaluate the providers in your area to determine which ones best meet your needs.</span></span> <span data-ttu-id="e471f-143">Geralmente, a maioria dos fornecedores:</span><span class="sxs-lookup"><span data-stu-id="e471f-143">Generally, most providers will:</span></span>

- <span data-ttu-id="e471f-144">Fornecer-lhe formação técnica e assistência</span><span class="sxs-lookup"><span data-stu-id="e471f-144">Provide you with technical training and assistance</span></span>
- <span data-ttu-id="e471f-145">Ajude-o a comercializar os seus produtos e serviços</span><span class="sxs-lookup"><span data-stu-id="e471f-145">Help you market your products and services</span></span>
- <span data-ttu-id="e471f-146">Gerir as suas condições de financiamento e crédito</span><span class="sxs-lookup"><span data-stu-id="e471f-146">Manage your financing and credit terms</span></span>

<span data-ttu-id="e471f-147">Pesse na lista de [fornecedores indiretos](https://partnercenter.microsoft.com/partner/find-a-provider)oficiais da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="e471f-147">Search the list of official [Microsoft indirect providers](https://partnercenter.microsoft.com/partner/find-a-provider).</span></span>

<span data-ttu-id="e471f-148">Saiba mais, leia  [Parceiro com fornecedores indiretos](indirect-reseller-tasks-in-partner-center.md)</span><span class="sxs-lookup"><span data-stu-id="e471f-148">Learn more, read  [Partner with indirect providers](indirect-reseller-tasks-in-partner-center.md)</span></span>

## <a name="accept-a-partnership-invitation-from-your-indirect-provider"></a><span data-ttu-id="e471f-149">Aceite um convite de parceria do seu fornecedor indireto</span><span class="sxs-lookup"><span data-stu-id="e471f-149">Accept a partnership invitation from your indirect provider</span></span>

<span data-ttu-id="e471f-150">Quando encontrar um fornecedor indireto para fazer parceria, estabeleça uma parceria com o fornecedor indireto no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="e471f-150">When you find an indirect provider to partner with, establish a partnership with the indirect provider in Partner Center.</span></span>

<span data-ttu-id="e471f-151">O fornecedor indireto que seleciona enviar-lhe-á por e-mail um link de convite de parceria que o levará ao seu convite no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="e471f-151">The indirect provider you select will send you in email a partnership invitation link that will take you to their invitation in Partner Center.</span></span> <span data-ttu-id="e471f-152">Certifique-se de que o seu administrador global assina no Partner Center e segue o link de convite.</span><span class="sxs-lookup"><span data-stu-id="e471f-152">Be sure your global admin signs in to Partner Center and follows the invitation link.</span></span> <span data-ttu-id="e471f-153">Quando aceitar o convite, o nome do fornecedor aparecerá na sua lista de fornecedores indiretos.</span><span class="sxs-lookup"><span data-stu-id="e471f-153">When you accept the invitation, the provider's name will appear in your indirect provider list.</span></span>

## <a name="acquire-new-customers-as-indirect-reseller"></a><span data-ttu-id="e471f-154">Adquirir novos clientes como revendedor indireto</span><span class="sxs-lookup"><span data-stu-id="e471f-154">Acquire new customers as indirect reseller</span></span>

<span data-ttu-id="e471f-155">Tanto você como o seu fornecedor indireto precisam de ter relações de revendedor com os clientes.</span><span class="sxs-lookup"><span data-stu-id="e471f-155">Both you and your indirect provider need to have reseller relationships with customers.</span></span> <span data-ttu-id="e471f-156">Estas relações de revendedor permitem-lhe gerir as subscrições e serviços de um cliente em seu nome.</span><span class="sxs-lookup"><span data-stu-id="e471f-156">These reseller relationships enable you to manage a customer's subscriptions and services on their behalf.</span></span> <span data-ttu-id="e471f-157">Para adquirir um novo cliente que tenha um inquilino Azure AD existente, pode convidar o cliente a estabelecer uma relação de revendedor tanto consigo como com o seu fornecedor ao mesmo tempo.</span><span class="sxs-lookup"><span data-stu-id="e471f-157">To acquire a new customer who has an existing Azure AD tenant, you can invite the customer to establish a reseller relationship with both you and your provider at the same time.</span></span>

<span data-ttu-id="e471f-158">Para criar um convite de revendedor indireto:</span><span class="sxs-lookup"><span data-stu-id="e471f-158">To create an indirect reseller invitation:</span></span>

1. <span data-ttu-id="e471f-159">Selecione **fornecedores indiretos** do seu navegador esquerdo Partner Center.</span><span class="sxs-lookup"><span data-stu-id="e471f-159">Select **Indirect providers** from your Partner Center left nav.</span></span>

2. <span data-ttu-id="e471f-160">Selecione **Convidar novos clientes** a convidar um cliente a estabelecer uma relação de revendedor tanto consigo como com o fornecedor indireto ao mesmo tempo.</span><span class="sxs-lookup"><span data-stu-id="e471f-160">Select **Invite new customers** to invite a customer to establish a reseller relationship with both you and the indirect provider at the same time.</span></span> <span data-ttu-id="e471f-161">O fornecedor precisa de ter uma relação de revendedor com o seu cliente, para que possa submeter encomendas em nome do seu cliente quando o cliente quiser comprar novas subscrições ou adicionar novas licenças às subscrições existentes.</span><span class="sxs-lookup"><span data-stu-id="e471f-161">The provider needs to have a reseller relationship with your customer, so they can submit orders on your customer's behalf when the customer wants to buy new subscriptions or add new licenses to existing subscriptions.</span></span>

3. <span data-ttu-id="e471f-162">Na página seguinte, analise a mensagem de e-mail de rascunho.</span><span class="sxs-lookup"><span data-stu-id="e471f-162">On the next page, review the draft email message.</span></span> <span data-ttu-id="e471f-163">Pode abrir a mensagem de rascunho por e-mail ou pode copiar a mensagem para a sua área de transferência e colá-la num e-mail.</span><span class="sxs-lookup"><span data-stu-id="e471f-163">You can open the draft message in email, or you can copy the message to your clipboard and paste it into an email.</span></span>

4. <span data-ttu-id="e471f-164">Edite o texto no e-mail para dizer o que precisa, mas certifique-se de incluir o link, uma vez que é personalizado para ligar o cliente diretamente à sua conta e à conta do seu fornecedor.</span><span class="sxs-lookup"><span data-stu-id="e471f-164">Edit the text in the email to say what you need but be sure to include the link as it is personalized to connect the customer directly to both your account and your provider's account.</span></span> <span data-ttu-id="e471f-165">Em seguida, selecione **Done** (Concluído).</span><span class="sxs-lookup"><span data-stu-id="e471f-165">Then select **Done** .</span></span>

5. <span data-ttu-id="e471f-166">Depois de o cliente o autorizar a si e ao seu fornecedor a serem os seus revendedores de registo, terá permissões de administrador para gerir as suas subscrições, licenças e utilizadores em seu nome, e o seu fornecedor indireto poderá submeter encomendas em seu nome.</span><span class="sxs-lookup"><span data-stu-id="e471f-166">After the customer authorizes you and your provider to be their resellers of record, you'll have administrator permissions to manage their subscriptions, licenses, and users on their behalf, and your indirect provider will be able to submit orders on their behalf.</span></span>
6. <span data-ttu-id="e471f-167">Para gerir a conta, serviços, utilizadores e licenças do cliente, expanda o registo do cliente selecionando a seta para baixo perto do seu nome.</span><span class="sxs-lookup"><span data-stu-id="e471f-167">To manage the customer's account, services, users, and licenses, expand the customer's record by selecting the down arrow near their name.</span></span>

<span data-ttu-id="e471f-168">Ao contrário dos parceiros de conta direta, os revendedores indiretos não podem criar inquilinos AZure AD para os seus novos clientes no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="e471f-168">Unlike direct bill partners, indirect resellers can't create Azure AD tenants for their new customers in Partner Center.</span></span> <span data-ttu-id="e471f-169">O seu fornecedor irá criar o inquilino e especificará-o como o revendedor indireto deste cliente.</span><span class="sxs-lookup"><span data-stu-id="e471f-169">Your provider will create the tenant and will specify you as the indirect reseller for this customer.</span></span> <span data-ttu-id="e471f-170">Isto garante que o cliente aparecerá na sua lista de clientes no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="e471f-170">This ensures that the customer will appear in your customer list in Partner Center.</span></span>

>[!Note]
><span data-ttu-id="e471f-171">Não poderá utilizar a sua capacidade de faturação direta para criar compras para clientes que adquire como revendedor indireto.</span><span class="sxs-lookup"><span data-stu-id="e471f-171">You will not be able to use your direct bill capability to create purchases for customers you acquire as an indirect reseller.</span></span>

## <a name="managing-your-direct-bill-customers-and-your-indirect-reseller-customers"></a><span data-ttu-id="e471f-172">Gerir os seus clientes de conta direta e os seus clientes revendedores indiretos</span><span class="sxs-lookup"><span data-stu-id="e471f-172">Managing your direct bill customers and your indirect reseller customers</span></span>

<span data-ttu-id="e471f-173">Gere os seus clientes de faturação direta e os seus clientes revendedores indiretos de forma diferente.</span><span class="sxs-lookup"><span data-stu-id="e471f-173">You manage your direct bill customers and your indirect reseller customers differently.</span></span>

### <a name="direct-bill-customers-things-you-wont-do-as-an-indirect-reseller"></a><span data-ttu-id="e471f-174">Clientes de faturação direta (coisas que não fará como revendedor indireto)</span><span class="sxs-lookup"><span data-stu-id="e471f-174">Direct bill customers (things you won't do as an indirect reseller)</span></span>

- <span data-ttu-id="e471f-175">Criar encomendas de produtos</span><span class="sxs-lookup"><span data-stu-id="e471f-175">Create orders for products</span></span>
- <span data-ttu-id="e471f-176">Gerir reservas do Azure</span><span class="sxs-lookup"><span data-stu-id="e471f-176">Manage Azure reservations</span></span>
- <span data-ttu-id="e471f-177">Gerir o histórico de encomendas</span><span class="sxs-lookup"><span data-stu-id="e471f-177">Manage their order history</span></span>
- <span data-ttu-id="e471f-178">Software de compra</span><span class="sxs-lookup"><span data-stu-id="e471f-178">Purchase software</span></span>
- <span data-ttu-id="e471f-179">Faturar diretamente os clientes</span><span class="sxs-lookup"><span data-stu-id="e471f-179">Bill customers directly</span></span>

### <a name="indirect-reseller-customers"></a><span data-ttu-id="e471f-180">Clientes revendedores indiretos</span><span class="sxs-lookup"><span data-stu-id="e471f-180">Indirect reseller customers</span></span>

- <span data-ttu-id="e471f-181">O seu fornecedor indireto encomenda produtos para os seus clientes</span><span class="sxs-lookup"><span data-stu-id="e471f-181">Your indirect provider orders products for your customers</span></span>
- <span data-ttu-id="e471f-182">Gerir as licenças e utilizadores dos clientes</span><span class="sxs-lookup"><span data-stu-id="e471f-182">Manage customers' licenses and users</span></span>
- <span data-ttu-id="e471f-183">Lidar com renovações de subscrição</span><span class="sxs-lookup"><span data-stu-id="e471f-183">Handle subscription renewals</span></span>

### <a name="to-identify-customers-that-you-acquired-as-a-direct-bill-partner"></a><span data-ttu-id="e471f-184">Para identificar clientes que adquiriu como parceiro de conta direta</span><span class="sxs-lookup"><span data-stu-id="e471f-184">To identify customers that you acquired as a direct bill partner</span></span>

1. <span data-ttu-id="e471f-185">Selecione **Clientes**</span><span class="sxs-lookup"><span data-stu-id="e471f-185">Select **Customers**</span></span>

2. <span data-ttu-id="e471f-186">Selecione um cliente para ver os seus detalhes</span><span class="sxs-lookup"><span data-stu-id="e471f-186">Select a customer to view their details</span></span>

3. <span data-ttu-id="e471f-187">Se este cliente for adquirido como parceiro de faturação direta, verá opções para **adicionar** ou **visualizar produtos** e verá as suas subscrições.</span><span class="sxs-lookup"><span data-stu-id="e471f-187">If this customer is one you acquired as a direct bill partner, you will see options to **add** or **view products** and you will see their subscriptions.</span></span>

4. <span data-ttu-id="e471f-188">Se o cliente tiver uma relação de revendedor indireto consigo, essas opções não estarão disponíveis.</span><span class="sxs-lookup"><span data-stu-id="e471f-188">If the customer has an indirect reseller relationship with you, those options will not be available.</span></span>

## <a name="move-your-direct-bill-customers-to-your-indirect-provider"></a><span data-ttu-id="e471f-189">Mova os seus clientes de faturação direta para o seu fornecedor indireto</span><span class="sxs-lookup"><span data-stu-id="e471f-189">Move your direct bill customers to your indirect provider</span></span>

<span data-ttu-id="e471f-190">O seu fornecedor indireto não pode submeter encomendas ou transferências de subscrição existentes para os seus clientes de fatura direta existentes até que tenham uma relação de revendedor com eles.</span><span class="sxs-lookup"><span data-stu-id="e471f-190">Your indirect provider cannot submit orders or existing subscription transfers for your existing direct bill customers until they have a reseller relationship with them.</span></span> <span data-ttu-id="e471f-191">Para estabelecer a relação de revendedor entre o seu fornecedor indireto e o seu cliente de conta direta existente, pode utilizar um dos seguintes métodos:</span><span class="sxs-lookup"><span data-stu-id="e471f-191">To establish the reseller relationship between your indirect provider and your existing direct bill customer, you can use one of the following methods:</span></span>

- [<span data-ttu-id="e471f-192">Extensão de relacionamento revendedor</span><span class="sxs-lookup"><span data-stu-id="e471f-192">Reseller relationship extension</span></span>](#reseller-relationship-extension)

- [<span data-ttu-id="e471f-193">Envie um convite de revendedor indireto ao cliente</span><span class="sxs-lookup"><span data-stu-id="e471f-193">Send an indirect reseller invitation to the customer</span></span>](#send-an-indirect-reseller-invitation-to-the-customer)

<span data-ttu-id="e471f-194">Pode encontrar uma visão geral detalhada do processo passo a passo no documento de [transição direto para indireto](https://partner.microsoft.com/resources/collection/Direct-Bill-transition-to-Indirect-reseller#/)</span><span class="sxs-lookup"><span data-stu-id="e471f-194">You can find a detailed overview of the step-by-step process in the [Direct to indirect transition document](https://partner.microsoft.com/resources/collection/Direct-Bill-transition-to-Indirect-reseller#/)</span></span>

### <a name="reseller-relationship-extension"></a><span data-ttu-id="e471f-195">Extensão de relacionamento revendedor</span><span class="sxs-lookup"><span data-stu-id="e471f-195">Reseller relationship extension</span></span>

<span data-ttu-id="e471f-196">Pode utilizar a funcionalidade de extensão de relacionamento do revendedor para estabelecer a relação de revendedor entre os clientes de faturação direta existentes e o seu fornecedor indireto utilizando o Partner Center Dashboard.</span><span class="sxs-lookup"><span data-stu-id="e471f-196">You can use the reseller relationship extension feature to establish reseller relationship between your existing direct bill customers and your indirect provider using Partner Center Dashboard.</span></span> <span data-ttu-id="e471f-197">Antes de utilizar a função, note o seguinte:</span><span class="sxs-lookup"><span data-stu-id="e471f-197">Before using the feature, note the following:</span></span>

- <span data-ttu-id="e471f-198">Esta funcionalidade só está disponível para os parceiros de faturação direto que estão em transição para se tornarem um revendedor indireto terem concluído a [inscrição do revendedor indireto](#get-started).</span><span class="sxs-lookup"><span data-stu-id="e471f-198">This feature is only available to direct bill partners who are transitioning to become an indirect reseller have completed the [indirect reseller enrollment](#get-started).</span></span>

- <span data-ttu-id="e471f-199">Só é possível aplicar esta funcionalidade aos clientes de faturação direta existentes.</span><span class="sxs-lookup"><span data-stu-id="e471f-199">You can only apply this feature to existing direct bill customers.</span></span> <span data-ttu-id="e471f-200">Não é aplicável aos [clientes revendedores indiretos.](#acquire-new-customers-as-indirect-reseller)</span><span class="sxs-lookup"><span data-stu-id="e471f-200">It is not applicable to [indirect reseller customers](#acquire-new-customers-as-indirect-reseller).</span></span>

- <span data-ttu-id="e471f-201">Só pode selecionar um fornecedor indireto para o qual [aceitou um convite de parceiro do seu fornecedor indireto.](#accept-a-partnership-invitation-from-your-indirect-provider)</span><span class="sxs-lookup"><span data-stu-id="e471f-201">You can only select an indirect provider for which you have [accepted a partner invitation from your indirect provider](#accept-a-partnership-invitation-from-your-indirect-provider).</span></span>

- <span data-ttu-id="e471f-202">Uma cópia da informação que tem para este cliente será disponibilizada ao fornecedor indireto.</span><span class="sxs-lookup"><span data-stu-id="e471f-202">A copy of the bill-to info you have for this customer will be made available to the indirect provider.</span></span> <span data-ttu-id="e471f-203">Pode aceder à informação da conta-a-lei acedendo à página conta deste cliente no Partner Center Dashboard.</span><span class="sxs-lookup"><span data-stu-id="e471f-203">You can access the bill-to info by accessing the Account page for this customer in Partner Center Dashboard.</span></span>

    > [!NOTE]
    > <span data-ttu-id="e471f-204">Ao utilizar a funcionalidade de extensão de relacionamento do revendedor, concorda em partilhar a informação que tem para este cliente com o fornecedor indireto.</span><span class="sxs-lookup"><span data-stu-id="e471f-204">By using the reseller relationship extension feature, you consent to sharing the bill-to info you have for this customer with the indirect provider.</span></span>

- <span data-ttu-id="e471f-205">O seu fornecedor indireto não será [dotando de privilégios administrativos delegados](customers-revoke-admin-privileges.md) ao cliente.</span><span class="sxs-lookup"><span data-stu-id="e471f-205">Your indirect provider will not be provided with [delegated administration privileges](customers-revoke-admin-privileges.md) to the customer tenant.</span></span> <span data-ttu-id="e471f-206">Se o seu fornecedor indireto necessitar de privilégios de administração delegados, deve enviar um convite de revendedor indireto ao cliente.</span><span class="sxs-lookup"><span data-stu-id="e471f-206">If your indirect provider requires delegated administration privileges, you must send an indirect reseller invitation to the customer instead.</span></span>

- <span data-ttu-id="e471f-207">Uma vez estabelecida a relação de revendedor, o fornecedor indireto aparecerá como parceiro CSP para o cliente na página Relações com Parceiros no [M365 Admin Center](https://admin.microsoft.com/AdminPortal/Home#/partners) e [Microsoft Store for Business](/microsoft-store/work-with-partner-microsoft-store-business).</span><span class="sxs-lookup"><span data-stu-id="e471f-207">Once the reseller relationship is established, the indirect provider will appear as a CSP partner to the customer under the Partner Relationships page in [M365 Admin Center](https://admin.microsoft.com/AdminPortal/Home#/partners) and [Microsoft Store for Business](/microsoft-store/work-with-partner-microsoft-store-business).</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="e471f-208">Para evitar confusões e mal-entendidos, é contratualmente obrigado pelo seu acordo de parceiro a informar e obter o consentimento do cliente de conta direta antes de utilizar a funcionalidade de extensão de relacionamento para estabelecer uma relação de revenda entre um cliente de conta direta existente e um fornecedor indireto.</span><span class="sxs-lookup"><span data-stu-id="e471f-208">To avoid confusion and misunderstanding, you are contractually obliged by your partner agreement to inform and obtain consent from the direct bill customer before you use the relationship extension feature to establish reseller relationship between an existing direct bill customer and an indirect provider.</span></span>

<span data-ttu-id="e471f-209">Para utilizar esta funcionalidade num inquilino de cliente existente:</span><span class="sxs-lookup"><span data-stu-id="e471f-209">To use this feature on an existing customer tenant:</span></span>

1. <span data-ttu-id="e471f-210">Faça login no Partner Center como **agente administrativo.**</span><span class="sxs-lookup"><span data-stu-id="e471f-210">Log in to Partner Center as an **Admin Agent** .</span></span>

2. <span data-ttu-id="e471f-211">Na **página Clientes,** selecione um cliente existente e clique no seu ícone **de links Rápidos** para expandir a visão sumária do cliente.</span><span class="sxs-lookup"><span data-stu-id="e471f-211">In the **Customers page** , select an existing customer and click on its **Quick links** icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="e471f-212">**No(s) fornecedor(s) indireto,** clique **em Transferir clientes num fornecedor indireto** .</span><span class="sxs-lookup"><span data-stu-id="e471f-212">Under **Indirect provider(s)** , click **Transfer customer on an indirect provider** .</span></span>

    :::image type="content" source="images/direct/direct5-1.png" alt-text="Transferir cliente para um fornecedor indireto":::

4. <span data-ttu-id="e471f-214">No diálogo pop-up, selecione o **Fornecedor Indireto** que pretende ter uma relação de revendedor com o cliente.</span><span class="sxs-lookup"><span data-stu-id="e471f-214">In the pop-up dialog, select the **Indirect Provider** you would like to have reseller relationship with the customer.</span></span>

5. <span data-ttu-id="e471f-215">Clique **em Guardar e continuar.**</span><span class="sxs-lookup"><span data-stu-id="e471f-215">Click **Save and continue** .</span></span>

6. <span data-ttu-id="e471f-216">Verifique se o fornecedor indireto selecionado aparece no **ou nos fornecedores indiretos.**</span><span class="sxs-lookup"><span data-stu-id="e471f-216">Verify the selected indirect provider shows up under **Indirect provider(s)** .</span></span>

    :::image type="content" source="images/direct/direct5-2.png" alt-text="Fornecedor indireto listado":::

### <a name="send-an-indirect-reseller-invitation-to-the-customer"></a><span data-ttu-id="e471f-218">Envie um convite de revendedor indireto ao cliente</span><span class="sxs-lookup"><span data-stu-id="e471f-218">Send an indirect reseller invitation to the customer</span></span>

<span data-ttu-id="e471f-219">O seu fornecedor indireto não pode submeter encomendas para os seus clientes de faturação direta existentes até que tenham uma relação de revendedor com eles.</span><span class="sxs-lookup"><span data-stu-id="e471f-219">Your indirect provider cannot submit orders for your existing direct bill customers until they have a reseller relationship with them.</span></span> <span data-ttu-id="e471f-220">Para estabelecer a relação de revendedor entre os seus clientes existentes e o seu fornecedor indireto, convide o cliente usando um convite de revendedor indireto.</span><span class="sxs-lookup"><span data-stu-id="e471f-220">To establish the reseller relationship between your existing customers and your indirect provider, invite the customer using an indirect reseller invitation.</span></span>

1. <span data-ttu-id="e471f-221">Selecione **fornecedores indiretos** do seu navegador esquerdo Partner Center.</span><span class="sxs-lookup"><span data-stu-id="e471f-221">Select **Indirect providers** from your Partner Center left nav.</span></span>

2. <span data-ttu-id="e471f-222">Selecione **Convidar novos clientes** a convidar um cliente a estabelecer uma relação de revendedor tanto consigo como com o fornecedor indireto ao mesmo tempo.</span><span class="sxs-lookup"><span data-stu-id="e471f-222">Select **Invite new customers** to invite a customer to establish a reseller relationship with both you and the indirect provider at the same time.</span></span> <span data-ttu-id="e471f-223">O fornecedor precisa de ter uma relação de revendedor com o seu cliente, para que possa submeter encomendas em nome do seu cliente quando o cliente quiser comprar novas subscrições ou adicionar novas licenças às subscrições existentes.</span><span class="sxs-lookup"><span data-stu-id="e471f-223">The provider needs to have a reseller relationship with your customer, so they can submit orders on your customer's behalf when the customer wants to buy new subscriptions or add new licenses to existing subscriptions.</span></span>

    :::image type="content" source="images/direct/direct6.png" alt-text="Convidar novos clientes":::

3. <span data-ttu-id="e471f-225">Na página seguinte, analise a mensagem de e-mail de rascunho.</span><span class="sxs-lookup"><span data-stu-id="e471f-225">On the next page, review the draft email message.</span></span> <span data-ttu-id="e471f-226">Pode abrir a mensagem de rascunho por e-mail ou pode copiar a mensagem para a sua área de transferência e colá-la num e-mail.</span><span class="sxs-lookup"><span data-stu-id="e471f-226">You can open the draft message in email, or you can copy the message to your clipboard and paste it into an email.</span></span>

4. <span data-ttu-id="e471f-227">Edite o texto no e-mail para dizer o que precisa, mas certifique-se de incluir o link, uma vez que é personalizado para ligar o cliente diretamente à sua conta e à conta do seu fornecedor.</span><span class="sxs-lookup"><span data-stu-id="e471f-227">Edit the text in the email to say what you need but be sure to include the link as it is personalized to connect the customer directly to both your account and your provider's account.</span></span> <span data-ttu-id="e471f-228">Em seguida, selecione **Done** (Concluído).</span><span class="sxs-lookup"><span data-stu-id="e471f-228">Then select **Done** .</span></span>

5. <span data-ttu-id="e471f-229">Depois de o cliente o autorizar a si e ao seu fornecedor a serem os seus revendedores de registo, terá permissões de administrador para gerir as suas subscrições, licenças e utilizadores em seu nome, e o seu fornecedor indireto poderá submeter encomendas em seu nome.</span><span class="sxs-lookup"><span data-stu-id="e471f-229">After the customer authorizes you and your provider to be their resellers of record, you'll have administrator permissions to manage their subscriptions, licenses, and users on their behalf, and your indirect provider will be able to submit orders on their behalf.</span></span>

6. <span data-ttu-id="e471f-230">Para gerir a conta, serviços, utilizadores e licenças do cliente, expanda o registo do cliente selecionando a seta para baixo perto do seu nome.</span><span class="sxs-lookup"><span data-stu-id="e471f-230">To manage the customer's account, services, users, and licenses, expand the customer's record by selecting the down arrow near their name.</span></span>

### <a name="microsoft-customer-agreement-acceptance"></a><span data-ttu-id="e471f-231">Aceitação do Acordo de Cliente da Microsoft</span><span class="sxs-lookup"><span data-stu-id="e471f-231">Microsoft Customer Agreement acceptance</span></span>

<span data-ttu-id="e471f-232">O Microsoft Cloud Agreement é válido até 31 de janeiro de 2020.</span><span class="sxs-lookup"><span data-stu-id="e471f-232">Microsoft Cloud Agreement is valid until January 31, 2020.</span></span> <span data-ttu-id="e471f-233">Após essa data, todos os clientes, existentes e novos, devem assinar o novo [Acordo de Cliente da Microsoft.](confirm-customer-agreement.md)</span><span class="sxs-lookup"><span data-stu-id="e471f-233">After that date, all customers, existing and new, must sign the new [Microsoft Customer Agreement](confirm-customer-agreement.md).</span></span> <span data-ttu-id="e471f-234">Para clientes em transição, se:</span><span class="sxs-lookup"><span data-stu-id="e471f-234">For transitioning customers, if:</span></span>

- <span data-ttu-id="e471f-235">**O cliente ainda não aceitou o Acordo de Cliente da Microsoft**</span><span class="sxs-lookup"><span data-stu-id="e471f-235">**Customer has not accepted Microsoft Customer Agreement yet**</span></span>

   <span data-ttu-id="e471f-236">Por favor, trabalhe com o Fornecedor Indireto para que o cliente [aceite o Acordo de Cliente da Microsoft.](confirm-customer-agreement.md)</span><span class="sxs-lookup"><span data-stu-id="e471f-236">Please work with Indirect Provider to have customer [accept the Microsoft Customer Agreement](confirm-customer-agreement.md).</span></span>

- <span data-ttu-id="e471f-237">**O Cliente aceitou o Microsoft Customer Agreement consigo através do Microsoft 365 Admin Center**</span><span class="sxs-lookup"><span data-stu-id="e471f-237">**Customer has accepted Microsoft Customer Agreement with you through the Microsoft 365 Admin Center**</span></span>

   <span data-ttu-id="e471f-238">A aceitação será mantida assim que a relação do revendedor for estabelecida com o Fornecedor Indireto.</span><span class="sxs-lookup"><span data-stu-id="e471f-238">The acceptance will be retained once the reseller relationship is established with the Indirect Provider.</span></span> <span data-ttu-id="e471f-239">Não há nada que precises de fazer.</span><span class="sxs-lookup"><span data-stu-id="e471f-239">There is nothing you need to do.</span></span>

- <span data-ttu-id="e471f-240">**O Cliente aceitou o Microsoft Customer Agreement consigo através da atestado de parceiros**</span><span class="sxs-lookup"><span data-stu-id="e471f-240">**Customer has accepted Microsoft Customer Agreement with you through partner attestation**</span></span>

   <span data-ttu-id="e471f-241">A aceitação não será mantida.</span><span class="sxs-lookup"><span data-stu-id="e471f-241">The acceptance will not be retained.</span></span> <span data-ttu-id="e471f-242">Por favor, trabalhe com o Fornecedor Indireto para [atualizar a aceitação do cliente no Partner Center.](confirm-customer-agreement.md#confirm-customer-acceptance-for-existing-customers)</span><span class="sxs-lookup"><span data-stu-id="e471f-242">Please work with Indirect Provider to [update the customer's acceptance in Partner Center](confirm-customer-agreement.md#confirm-customer-acceptance-for-existing-customers).</span></span>

## <a name="transfer-existing-direct-bill-subscriptions-to-indirect-provider"></a><span data-ttu-id="e471f-243">Transferir assinaturas de conta direta existentes para fornecedor indireto</span><span class="sxs-lookup"><span data-stu-id="e471f-243">Transfer existing direct bill subscriptions to indirect provider</span></span>

<span data-ttu-id="e471f-244">De acordo com o modelo indireto da CSP, os revendedores indiretos não têm relações de faturação com a Microsoft.</span><span class="sxs-lookup"><span data-stu-id="e471f-244">Under CSP indirect model, indirect resellers do not have billing relationships with Microsoft.</span></span> <span data-ttu-id="e471f-245">Em vez disso, os revendedores indiretos obtêm subscrições para os seus clientes através dos seus fornecedores indiretos.</span><span class="sxs-lookup"><span data-stu-id="e471f-245">Instead, indirect resellers obtain subscriptions for their customers through their indirect providers.</span></span> <span data-ttu-id="e471f-246">Durante a transição de parceiro de conta direta para revendedor indireto, precisa transferir as subscrições existentes que tem como parceiro de conta direta para o seu fornecedor indireto.</span><span class="sxs-lookup"><span data-stu-id="e471f-246">While transitioning from direct bill partner to indirect reseller, you need to transfer the existing subscriptions you have as the direct bill partner to your indirect provider.</span></span> <span data-ttu-id="e471f-247">Pode utilizar a função de transferência de subscrição auto-servida no Partner Center Dashboard para o fazer.</span><span class="sxs-lookup"><span data-stu-id="e471f-247">You can use the self-served subscription transfer feature in Partner Center Dashboard to do so.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="e471f-248">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e471f-248">Pre-requisites</span></span>

- <span data-ttu-id="e471f-249">Esta funcionalidade só está disponível para parceiros em transição que tenham concluído a inscrição do revendedor indireto utilizando os inquilinos parceiros de conta direto existentes</span><span class="sxs-lookup"><span data-stu-id="e471f-249">This feature is only available to transitioning partners who have completed the indirect reseller enrollment using their existing direct bill partner tenants</span></span>

- <span data-ttu-id="e471f-250">Antes de transferir as subscrições associadas a um determinado cliente, o parceiro de transição deve mover o cliente para um fornecedor indireto.</span><span class="sxs-lookup"><span data-stu-id="e471f-250">Before transferring subscriptions associated with a given customer, the transitioning partner must move the customer to an indirect provider.</span></span>

- <span data-ttu-id="e471f-251">O cliente deve ter [aceitado o Acordo de Cliente da Microsoft através do Fornecedor Indireto.](#microsoft-customer-agreement-acceptance)</span><span class="sxs-lookup"><span data-stu-id="e471f-251">Customer must have [accepted Microsoft Customer Agreement through the Indirect Provider](#microsoft-customer-agreement-acceptance).</span></span>

### <a name="how-to-transition-to-indirect-reseller-status"></a><span data-ttu-id="e471f-252">Como transitar para o estatuto de revendedor indireto</span><span class="sxs-lookup"><span data-stu-id="e471f-252">How to transition to indirect reseller status</span></span>

<span data-ttu-id="e471f-253">A funcionalidade é um processo de 4 etapas, onde:</span><span class="sxs-lookup"><span data-stu-id="e471f-253">The feature is a 4-step process, where:</span></span>

- <span data-ttu-id="e471f-254">O parceiro de transição cria um pedido de transferência de assinatura.</span><span class="sxs-lookup"><span data-stu-id="e471f-254">The transitioning partner creates a subscription transfer request.</span></span> <span data-ttu-id="e471f-255">O pedido contém uma ou mais subscrições existentes associadas ao mesmo cliente e é endereçado a um fornecedor indireto.</span><span class="sxs-lookup"><span data-stu-id="e471f-255">The request contains one or more existing subscriptions associated with the same customer and is addressed to an indirect provider.</span></span>

- <span data-ttu-id="e471f-256">O fornecedor indireto revê e aceita (ou rejeita) o pedido de transferência.</span><span class="sxs-lookup"><span data-stu-id="e471f-256">The indirect provider reviews and accepts (or reject) the transfer request.</span></span>

- <span data-ttu-id="e471f-257">O prestador indireto verifica que o pedido de transferência está completo.</span><span class="sxs-lookup"><span data-stu-id="e471f-257">The indirect provider verifies that the transfer request is complete.</span></span>

- <span data-ttu-id="e471f-258">O parceiro de transição verifica que o pedido de transferência está completo.</span><span class="sxs-lookup"><span data-stu-id="e471f-258">The transitioning partner verifies that the transfer request is complete.</span></span>

### <a name="transitioning-partner"></a><span data-ttu-id="e471f-259">Parceiro de transição</span><span class="sxs-lookup"><span data-stu-id="e471f-259">Transitioning partner</span></span>

> [!NOTE]
> <span data-ttu-id="e471f-260">Também pode utilizar [a API/SDK do Partner Center](/partner-center/develop/manage-customers) para transferir as subscrições existentes para o seu fornecedor indireto.</span><span class="sxs-lookup"><span data-stu-id="e471f-260">You can also use [Partner Center API/SDK](/partner-center/develop/manage-customers) to transfer the existing subscriptions to your indirect provider.</span></span>
>
> - [<span data-ttu-id="e471f-261">Obtenha a elegibilidade de transferência de subscrições de um cliente</span><span class="sxs-lookup"><span data-stu-id="e471f-261">Get a customer's subscriptions transfer eligibility</span></span>](/partner-center/develop/get-customer-s-subscriptions-transfer-eligibility)
> - [<span data-ttu-id="e471f-262">Criar transferência de um cliente</span><span class="sxs-lookup"><span data-stu-id="e471f-262">Create a customer's transfer</span></span>](/partner-center/develop/create-a-transfer)
> - [<span data-ttu-id="e471f-263">Retirar a transferência de um cliente</span><span class="sxs-lookup"><span data-stu-id="e471f-263">Withdraw a customer's transfer</span></span>](/partner-center/develop/withdraw-a-transfer)
> - [<span data-ttu-id="e471f-264">Aceitar a transferência de um cliente</span><span class="sxs-lookup"><span data-stu-id="e471f-264">Accept a customer's transfer</span></span>](/partner-center/develop/accept-a-transfer)
> - [<span data-ttu-id="e471f-265">Rejeitar a transferência de um Cliente</span><span class="sxs-lookup"><span data-stu-id="e471f-265">Reject a Customer's transfer</span></span>](/partner-center/develop/reject-a-transfer)
> - [<span data-ttu-id="e471f-266">Obter transferências de um cliente</span><span class="sxs-lookup"><span data-stu-id="e471f-266">Get a customer's transfers</span></span>](/partner-center/develop/get-all-of-a-customer-s-transfers)
> - [<span data-ttu-id="e471f-267">Obtenha detalhes de transferência por id</span><span class="sxs-lookup"><span data-stu-id="e471f-267">Get transfer details by id</span></span>](/partner-center/develop/get-transfer-by-id)

### <a name="transitioning-partner---create-transfer-request"></a><span data-ttu-id="e471f-268">Parceiro de transição - crie pedido de transferência</span><span class="sxs-lookup"><span data-stu-id="e471f-268">Transitioning partner - create transfer request</span></span>

<span data-ttu-id="e471f-269">Para criar um pedido de transferência como parceiro de transição:</span><span class="sxs-lookup"><span data-stu-id="e471f-269">To create a transfer request as the transitioning partner:</span></span>

1. <span data-ttu-id="e471f-270">Faça login no Partner Center como **agente administrativo.**</span><span class="sxs-lookup"><span data-stu-id="e471f-270">Log in to Partner Center as an **Admin Agent** .</span></span>

2. <span data-ttu-id="e471f-271">Na página **Clientes,** selecione o cliente pretendido e clique no ícone links Rápidos para expandir a visão sumária do cliente.</span><span class="sxs-lookup"><span data-stu-id="e471f-271">In the **Customers** page, select the intended customer and click on the Quick links icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="e471f-272">Ao abrigo **do ou dos fornecedores indiretos,** confirme que o fornecedor indireto pretendido está listado.</span><span class="sxs-lookup"><span data-stu-id="e471f-272">Under **Indirect provider(s)** , confirm that the intended indirect provider is listed.</span></span>

4. <span data-ttu-id="e471f-273">Clique **em Ver Assinaturas** .</span><span class="sxs-lookup"><span data-stu-id="e471f-273">Click **View Subscriptions** .</span></span>

5. <span data-ttu-id="e471f-274">Na página **subscrições,** procure **a Transferência de Assinaturas.**</span><span class="sxs-lookup"><span data-stu-id="e471f-274">In the **Subscriptions** page, look for **Subscription Transfer** .</span></span>

6. <span data-ttu-id="e471f-275">Em **Transferência de Assinatura** , clique em Solicitar transferência de **subscrição.**</span><span class="sxs-lookup"><span data-stu-id="e471f-275">Under **Subscription Transfer** , click **Request subscription transfer** .</span></span>

    :::image type="content" source="images/direct/direct8.png" alt-text="Solicitar transferência de assinatura":::

7. <span data-ttu-id="e471f-277">No diálogo do pedido de transferência, selecione uma ou mais subscrições a serem transferidas.</span><span class="sxs-lookup"><span data-stu-id="e471f-277">In the transfer request dialog, select one or more subscriptions to be transferred.</span></span>

    :::image type="content" source="images/direct/direct9.png" alt-text="Criar Pedido de Transferência":::

8. <span data-ttu-id="e471f-279">Clique em **Criar** .</span><span class="sxs-lookup"><span data-stu-id="e471f-279">Click **Create** .</span></span>

9. <span data-ttu-id="e471f-280">Um pedido de transferência de assinatura ativo será apresentado no âmbito **da Transferência de Assinaturas.**</span><span class="sxs-lookup"><span data-stu-id="e471f-280">An active subscription transfer request will appear under **Subscription Transfer** .</span></span>

    :::image type="content" source="images/direct/direct10.png" alt-text="Lista de pedidos de transferência":::

10. <span data-ttu-id="e471f-282">Informe o seu fornecedor indireto de que criou um pedido de transferência de assinatura para eles.</span><span class="sxs-lookup"><span data-stu-id="e471f-282">Inform your indirect provider that you have created a subscription transfer request to them.</span></span>

### <a name="indirect-provider---accept-transfer-request"></a><span data-ttu-id="e471f-283">Fornecedor indireto - aceite pedido de transferência</span><span class="sxs-lookup"><span data-stu-id="e471f-283">Indirect provider - accept transfer request</span></span>

<span data-ttu-id="e471f-284">Rever e aceitar um pedido de transferência como fornecedor indireto:</span><span class="sxs-lookup"><span data-stu-id="e471f-284">To review and accept a transfer request as the indirect provider:</span></span>

1. <span data-ttu-id="e471f-285">Inicie sessão no Partner Center como **Agente** Administrativo ou Agente **de Vendas.**</span><span class="sxs-lookup"><span data-stu-id="e471f-285">Log in to Partner Center as an **Admin** Agent or **Sales Agent** .</span></span>

2. <span data-ttu-id="e471f-286">Na página **Clientes,** selecione o cliente pretendido e clique no ícone de links Rápidos para expandir a visão sumária do cliente.</span><span class="sxs-lookup"><span data-stu-id="e471f-286">In the **Customers** page, select the intended customer and click on its Quick links icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="e471f-287">**No(s) Revendedor indireto,** confirme que o parceiro de transição está listado.</span><span class="sxs-lookup"><span data-stu-id="e471f-287">Under **Indirect reseller(s)** , confirm the transitioning partner is listed.</span></span>

4. <span data-ttu-id="e471f-288">Clique **em Ver Assinaturas** .</span><span class="sxs-lookup"><span data-stu-id="e471f-288">Click **View Subscriptions** .</span></span>

5. <span data-ttu-id="e471f-289">Na página **subscrições,** procure **a Transferência de Assinaturas.**</span><span class="sxs-lookup"><span data-stu-id="e471f-289">In the **Subscriptions** page, look for **Subscription Transfer** .</span></span>

    :::image type="content" source="images/direct/direct11.png" alt-text="Ver pedido de transferência":::

6. <span data-ttu-id="e471f-291">No Âmbito **da Transferência de Assinaturas,** clique no pedido de transferência a rever.</span><span class="sxs-lookup"><span data-stu-id="e471f-291">Under **Subscription Transfer** , click on the transfer request to review.</span></span>

7. <span data-ttu-id="e471f-292">Clique **em Aceitar** (ou **Rejeitar)** conforme apropriado.</span><span class="sxs-lookup"><span data-stu-id="e471f-292">Click **Accept** (or **Reject** ) as appropriate.</span></span>

    :::image type="content" source="images/direct/direct12.png" alt-text="Aceite o pedido de transferência":::

8. <span data-ttu-id="e471f-294">Aguarde que o pedido de transferência esteja concluído.</span><span class="sxs-lookup"><span data-stu-id="e471f-294">Wait for the transfer request to complete.</span></span>

### <a name="indirect-provider---verify-transfer-request-is-complete"></a><span data-ttu-id="e471f-295">Fornecedor indireto - verifique se o pedido de transferência está completo</span><span class="sxs-lookup"><span data-stu-id="e471f-295">Indirect provider - verify transfer request is complete</span></span>

1. <span data-ttu-id="e471f-296">Após o pedido de transferência ter sido concluído com sucesso, verifique se pode ver as subscrições aparecerem em **Subscrições** .</span><span class="sxs-lookup"><span data-stu-id="e471f-296">After the transfer request is completed successfully, verify that you can see the subscriptions appear under **Subscriptions** .</span></span>

2. <span data-ttu-id="e471f-297">Informe o parceiro de transição.</span><span class="sxs-lookup"><span data-stu-id="e471f-297">Inform the transitioning partner.</span></span>

### <a name="transitioning-partner---verify-transfer-request-is-complete"></a><span data-ttu-id="e471f-298">Parceiro de transição - verifique se o pedido de transferência está completo</span><span class="sxs-lookup"><span data-stu-id="e471f-298">Transitioning partner - verify transfer request is complete</span></span>

<span data-ttu-id="e471f-299">O parceiro de transição deve fazer o seguinte:</span><span class="sxs-lookup"><span data-stu-id="e471f-299">The transitioning partner should do the following:</span></span>

1. <span data-ttu-id="e471f-300">Inscreva-se no Partner Center como **Agente Administrativo** ou **Agente comercial.**</span><span class="sxs-lookup"><span data-stu-id="e471f-300">Sign into Partner Center as an **Admin Agent** or **Sales Agent** .</span></span>

2. <span data-ttu-id="e471f-301">Na página **Clientes,** selecione o cliente pretendido e clique no ícone **links Rápidos** para expandir a visão sumária do cliente.</span><span class="sxs-lookup"><span data-stu-id="e471f-301">In the **Customers** page, select the intended customer and click on the **Quick links** icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="e471f-302">Clique **em Ver Assinaturas** .</span><span class="sxs-lookup"><span data-stu-id="e471f-302">Click **View Subscriptions** .</span></span>

4. <span data-ttu-id="e471f-303">Na página **subscrições,** procure **a Transferência de Assinaturas.**</span><span class="sxs-lookup"><span data-stu-id="e471f-303">In the **Subscriptions** page, look for **Subscription Transfer** .</span></span>

5. <span data-ttu-id="e471f-304">Verifique se o pedido de transferência está marcado como **Completo** .</span><span class="sxs-lookup"><span data-stu-id="e471f-304">Verify that the transfer request is marked as **Complete** .</span></span>

6. <span data-ttu-id="e471f-305">Verifique se as subscrições deixaram de aparecer como ativas na página **de Subscrições:**</span><span class="sxs-lookup"><span data-stu-id="e471f-305">Verify that the subscription(s) no longer appear as active in the **Subscriptions** page:</span></span>

   1. <span data-ttu-id="e471f-306">Se se trata de uma subscrição do Azure (MS-AZR-0145P), deixará de ser listada.</span><span class="sxs-lookup"><span data-stu-id="e471f-306">If this is an Azure subscription (MS-AZR-0145P), it will no longer be listed.</span></span>

   2. <span data-ttu-id="e471f-307">Se se trata de uma subscrição baseada em licença (Office 365, Dynamics, Intune), será listada com o estado como **Suspenso.**</span><span class="sxs-lookup"><span data-stu-id="e471f-307">If this is a license-based subscription (Office 365, Dynamics, Intune), it will be listed with state as **Suspended** .</span></span>

   :::image type="content" source="images/direct/direct13.png" alt-text="Assinatura suspensa":::

### <a name="considerations"></a><span data-ttu-id="e471f-309">Considerações</span><span class="sxs-lookup"><span data-stu-id="e471f-309">Considerations</span></span>

- <span data-ttu-id="e471f-310">**O ID da subscrição será diferente após a transferência.**</span><span class="sxs-lookup"><span data-stu-id="e471f-310">**Subscription ID will be different after transfer.**</span></span> <span data-ttu-id="e471f-311">Se for uma subscrição da Azure (MS-AZR-0145P), além disso, terá um ID de assinatura Azure, que é retido do anterior proprietário, e aparecerá no portal de gestão Azure.</span><span class="sxs-lookup"><span data-stu-id="e471f-311">If it is an Azure subscription (MS-AZR-0145P), additionally, it will have an Azure Subscription ID, which is retained from the previous owner, and will appear in the Azure management portal.</span></span>

- <span data-ttu-id="e471f-312">**A mesma subscrição não pode ser referenciada por múltiplos pedidos de transferência.**</span><span class="sxs-lookup"><span data-stu-id="e471f-312">**The same subscription cannot be referenced by multiple transfer requests.**</span></span> <span data-ttu-id="e471f-313">Depois de ter criado um pedido de transferência, que inclui uma subscrição existente, não é possível criar pedidos de transferência adicionais, incluindo a mesma subscrição, até que o primeiro pedido de transferência seja cancelado.</span><span class="sxs-lookup"><span data-stu-id="e471f-313">After you have created a transfer request, which includes an existing subscription, you cannot create additional transfer requests including the same subscription, until the first transfer request is canceled.</span></span>

- <span data-ttu-id="e471f-314">**Os complementos para assinaturas baseadas em licenças devem ser transferidos juntamente com a sua subscrição base.**</span><span class="sxs-lookup"><span data-stu-id="e471f-314">**Add-ons for license-based subscriptions must be transferred along with their base subscription.**</span></span> <span data-ttu-id="e471f-315">Ao criar um pedido de transferência, se escolher uma subscrição existente com um ou mais addons, os addons serão automaticamente incluídos no pedido de transferência.</span><span class="sxs-lookup"><span data-stu-id="e471f-315">When creating a transfer request, if you pick an existing subscription with one or more add-ons, the add-ons will automatically be included in the transfer request.</span></span>

- <span data-ttu-id="e471f-316">**As alterações na contagem de licenças para uma subscrição não serão refletidas no pedido de transferência existente.**</span><span class="sxs-lookup"><span data-stu-id="e471f-316">**License count changes to a subscription will not be reflected in existing transfer request.**</span></span> <span data-ttu-id="e471f-317">Depois de ter criado um pedido de transferência que inclua uma subscrição existente, deve evitar atualizar a quantidade de licença da subscrição (ou addons associados).</span><span class="sxs-lookup"><span data-stu-id="e471f-317">After you have created a transfer request which includes an existing subscription, you should avoid updating the license quantity of the subscription (or associated addons).</span></span> <span data-ttu-id="e471f-318">Se o fizer, a nova quantidade não se refletirá no pedido de transferência.</span><span class="sxs-lookup"><span data-stu-id="e471f-318">If you do so, the new quantity will not be reflected in the transfer request.</span></span> <span data-ttu-id="e471f-319">Após o prestador indireto aceitar o pedido de transferência, a subscrição resultante terá a quantidade antiga.</span><span class="sxs-lookup"><span data-stu-id="e471f-319">After the indirect provider accepts the transfer request, the resultant subscription will have the old quantity.</span></span> <span data-ttu-id="e471f-320">Se desejar que a nova quantidade seja transferida para o fornecedor indireto, deve cancelar o pedido de transferência existente e recriar uma nova.</span><span class="sxs-lookup"><span data-stu-id="e471f-320">If you wish for the new quantity to be transferred to the indirect provider, you must cancel the existing transfer request and recreate a new one.</span></span>

- <span data-ttu-id="e471f-321">**Nem todas as compras podem ser transferidas usando transferência de assinatura auto-servida.**</span><span class="sxs-lookup"><span data-stu-id="e471f-321">**Not all purchases can be transferred using self-served subscription transfer.**</span></span> <span data-ttu-id="e471f-322">Atualmente, só é possível transferir subscrições O365 e subscrições Azure PAYG (MS-AZR-0145P) utilizando esta funcionalidade.</span><span class="sxs-lookup"><span data-stu-id="e471f-322">Currently, you can only transfer O365 subscriptions and Azure PAYG subscriptions (MS-AZR-0145P) using this feature.</span></span> <span data-ttu-id="e471f-323">Outras compras, incluindo planos Azure, Azure Reserved Instances, Subscrições baseadas em prazos e subscrições SaaS para o Azure Marketplace não são suportadas.</span><span class="sxs-lookup"><span data-stu-id="e471f-323">Other purchases including Azure Plans, Azure Reserved Instances, Term-based Subscriptions and SaaS subscriptions for Azure Marketplace are not supported.</span></span> <span data-ttu-id="e471f-324">Verá uma razão pela qual uma subscrição não pode ser transferida na página de pedido de transferência de envio.</span><span class="sxs-lookup"><span data-stu-id="e471f-324">You will see a reason why a subscription cannot be transferred in the submit transfer request page.</span></span> <span data-ttu-id="e471f-325">Para transferir estas subscrições, terá de [cancelar a subscrição existente](create-a-new-subscription.md#suspend-or-cancel-a-subscription) e adquirir uma nova oferta para o cliente através do Fornecedor Indireto.</span><span class="sxs-lookup"><span data-stu-id="e471f-325">To transfer these subscriptions, you will need to [cancel the existing subscription](create-a-new-subscription.md#suspend-or-cancel-a-subscription) and purchase new offer for customer through Indirect Provider.</span></span>

- <span data-ttu-id="e471f-326">**Não é possível testar utilizando o ambiente da caixa de areia.**</span><span class="sxs-lookup"><span data-stu-id="e471f-326">**Cannot be tested using sandbox environment.**</span></span>

## <a name="enroll-for-indirect-reseller-incentives"></a><span data-ttu-id="e471f-327">Inscreva-se para incentivos indiretos do revendedor</span><span class="sxs-lookup"><span data-stu-id="e471f-327">Enroll for indirect reseller incentives</span></span>

<span data-ttu-id="e471f-328">Depois de se ter inscrito com sucesso como revendedor indireto no seu inquilino parceiro de conta direta existente, receberá um convite para se inscrever para o incentivo de revendedor indireto no prazo de 30 dias.</span><span class="sxs-lookup"><span data-stu-id="e471f-328">After you have successfully enrolled as an indirect reseller on your existing direct bill partner tenant, you will receive an invitation to enroll for indirect reseller incentive within 30 days.</span></span> <span data-ttu-id="e471f-329">O convite baseia-se na conta MPN parceira que está atualmente associada ao seu inquilino parceiro da CSP.</span><span class="sxs-lookup"><span data-stu-id="e471f-329">The invitation is based on the partner MPN account that is currently associated with your CSP partner tenant.</span></span> <span data-ttu-id="e471f-330">O convite será enviado para o endereço de e-mail associado à conta MPN do parceiro.</span><span class="sxs-lookup"><span data-stu-id="e471f-330">The invitation will be sent to the email address associated with the partner MPN account.</span></span>

<span data-ttu-id="e471f-331">Você também é elegível para se inscrever para programas de incentivo de conta direta com o mesmo inquilino parceiro.</span><span class="sxs-lookup"><span data-stu-id="e471f-331">You are also eligible to enroll for direct bill incentive programs with that same partner tenant.</span></span> <span data-ttu-id="e471f-332">Tem de gerir os programas separadamente.</span><span class="sxs-lookup"><span data-stu-id="e471f-332">You must manage the programs separately.</span></span>

## <a name="next-steps"></a><span data-ttu-id="e471f-333">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="e471f-333">Next steps</span></span>

- [<span data-ttu-id="e471f-334">Informações adicionais sobre se tornar um revendedor indireto</span><span class="sxs-lookup"><span data-stu-id="e471f-334">Additional information on becoming an indirect reseller</span></span>](https://assetsprod.microsoft.com/csp-directbill-to-indirect-transition.pdf)
- [<span data-ttu-id="e471f-335">CSP parceiro direto novos requisitos</span><span class="sxs-lookup"><span data-stu-id="e471f-335">CSP direct partner new requirements</span></span>](direct-partner-new-requirements.md)
- [<span data-ttu-id="e471f-336">Capacidades de conta direta restritas</span><span class="sxs-lookup"><span data-stu-id="e471f-336">Restricted direct bill capabilities</span></span>](restricted-direct-bill-capabilities.md)