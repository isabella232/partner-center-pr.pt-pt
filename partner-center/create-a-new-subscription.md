---
title: Criar subscrições de clientes no Partner Center
ms.topic: how-to
ms.date: 07/22/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como vender subscrições dos seus clientes a produtos publicados pela Microsoft, bem como produtos SaaS publicados por ISVs de terceiros.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: 85a40974557817825d58246c2c010c7cf8a6a5e1
ms.sourcegitcommit: f34f2f69e6df4f260479a205d94010cf47987ff2
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/25/2020
ms.locfileid: "96038885"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a><span data-ttu-id="c5c1c-103">Create, suspend, or cancel customer subscriptions (Criar, suspender ou cancelar subscrições de clientes)</span><span class="sxs-lookup"><span data-stu-id="c5c1c-103">Create, suspend, or cancel customer subscriptions</span></span>

<span data-ttu-id="c5c1c-104">**Aplica-se a**</span><span class="sxs-lookup"><span data-stu-id="c5c1c-104">**Applies to**</span></span>

- <span data-ttu-id="c5c1c-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="c5c1c-105">Partner Center</span></span>
- <span data-ttu-id="c5c1c-106">Centro de Parceiros do Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="c5c1c-106">Partner Center for Microsoft Cloud for US Government</span></span>
- <span data-ttu-id="c5c1c-107">Parceiros CSP</span><span class="sxs-lookup"><span data-stu-id="c5c1c-107">CSP partners</span></span>

<span data-ttu-id="c5c1c-108">**Funções adequadas**</span><span class="sxs-lookup"><span data-stu-id="c5c1c-108">**Appropriate roles**</span></span>

- <span data-ttu-id="c5c1c-109">Agente administrativo</span><span class="sxs-lookup"><span data-stu-id="c5c1c-109">Admin agent</span></span>
- <span data-ttu-id="c5c1c-110">Administrador de faturação</span><span class="sxs-lookup"><span data-stu-id="c5c1c-110">Billing admin</span></span>
- <span data-ttu-id="c5c1c-111">Administrador global</span><span class="sxs-lookup"><span data-stu-id="c5c1c-111">Global admin</span></span>
- <span data-ttu-id="c5c1c-112">Agente helpdesk</span><span class="sxs-lookup"><span data-stu-id="c5c1c-112">Helpdesk agent</span></span>
- <span data-ttu-id="c5c1c-113">Agente comercial</span><span class="sxs-lookup"><span data-stu-id="c5c1c-113">Sales agent</span></span>

<span data-ttu-id="c5c1c-114">Depois de ter criado um registo do seu cliente no Partner Center, pode vendê-los subscrições a produtos do catálogo.</span><span class="sxs-lookup"><span data-stu-id="c5c1c-114">After you've created a record of your customer in the Partner Center, you can sell them subscriptions to products in the catalog.</span></span> <span data-ttu-id="c5c1c-115">Isto inclui produtos publicados pela Microsoft, bem como produtos de Software como um Serviço (SaaS) publicados por fornecedores de software independentes de terceiros (ISVs) para o [mercado comercial.](https://azuremarketplace.microsoft.com/marketplace)</span><span class="sxs-lookup"><span data-stu-id="c5c1c-115">This includes products published by Microsoft as well as Software as a Service (SaaS) products published by third-party Independent Software Vendors (ISVs) to the [commercial marketplace](https://azuremarketplace.microsoft.com/marketplace).</span></span>

<span data-ttu-id="c5c1c-116">Algumas ofertas são limitadas a uma subscrição por cliente.</span><span class="sxs-lookup"><span data-stu-id="c5c1c-116">Some offers are limited to one subscription per customer.</span></span> <span data-ttu-id="c5c1c-117">Para ver uma lista das ofertas restritas, visite a página de Preços e Ofertas do Centro de Parceiros.</span><span class="sxs-lookup"><span data-stu-id="c5c1c-117">To see a list of which offers are restricted, visit the Partner Center Pricing and Offers page.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="c5c1c-118">Como parceiro no programa CSP, pode adquirir assinaturas SaaS **baseadas em licenças** ou **medidos** a editores da ISV dentro do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="c5c1c-118">As a partner in the CSP program, you can purchase **license-based** or **metered** SaaS subscriptions from ISV publishers within Partner Center.</span></span> <span data-ttu-id="c5c1c-119">Isto significa que pode adquirir qualquer oferta SaaS **baseada em licença** ou **medido** que o editor ISV lhe tenha disponibilizado, incluindo [ofertas exclusivas](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) às quais tem acesso.</span><span class="sxs-lookup"><span data-stu-id="c5c1c-119">This means you can purchase any **license-based** or **metered** SaaS offer the ISV publisher has made available to you, including [exclusive offers](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to which you have access.</span></span> <span data-ttu-id="c5c1c-120">Para comprar ou gerir outras ofertas comerciais de marketplace a partir de ISVs (tais como ofertas baseadas em uso envolvendo aplicações Azure, Contentores ou VMs), você deve ir ao [portal Azure.](https://portal.azure.com/)</span><span class="sxs-lookup"><span data-stu-id="c5c1c-120">To purchase or manage other, commercial marketplace offers from ISVs (such as usage-based offers involving Azure applications, Containers or VMs), you must go to the [Azure portal](https://portal.azure.com/).</span></span>

## <a name="create-a-new-subscription"></a><span data-ttu-id="c5c1c-121">Criar uma nova subscrição</span><span class="sxs-lookup"><span data-stu-id="c5c1c-121">Create a new subscription</span></span>

1. <span data-ttu-id="c5c1c-122">Inicie sessão no [dashboard do Centro de Parceiros](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="c5c1c-122">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="c5c1c-123">No menu Partner Center, selecione **Clientes,** em seguida, escolha um cliente da lista.</span><span class="sxs-lookup"><span data-stu-id="c5c1c-123">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="c5c1c-124">Selecione **Adicionar subscrição**.</span><span class="sxs-lookup"><span data-stu-id="c5c1c-124">Select **Add subscription**.</span></span> <span data-ttu-id="c5c1c-125">O separador **Serviços Online** mostrará todas as ofertas disponíveis do Marketplace SaaS.</span><span class="sxs-lookup"><span data-stu-id="c5c1c-125">The **Online Services** tab will show all available Marketplace SaaS offers.</span></span>

4. <span data-ttu-id="c5c1c-126">Para ver apenas certos tipos de subscrições, faça seleções nos filtros disponíveis:</span><span class="sxs-lookup"><span data-stu-id="c5c1c-126">To see only certain types of subscriptions, make selections in the available filters:</span></span>
   - <span data-ttu-id="c5c1c-127">**Editor**: Escolha a **Microsoft** para ver apenas ofertas da Microsoft, ou **Partner** para ver produtos de mercado comercial publicados por ISVs.</span><span class="sxs-lookup"><span data-stu-id="c5c1c-127">**Publisher**: Choose **Microsoft** to see only offers from Microsoft, or **Partner** to see commercial marketplace products published by ISVs.</span></span>
   - <span data-ttu-id="c5c1c-128">**Tipo de faturação**: Selecione o tipo de faturação de subscrição que pretende utilizar: **Licença** ou **Utilização**.</span><span class="sxs-lookup"><span data-stu-id="c5c1c-128">**Billing type**: Select the type of subscription billing you want to use: **License** or **Usage**.</span></span> <span data-ttu-id="c5c1c-129">Consulte [a faturação baseada em licença](license-based-billing.md) para obter informações que o ajudarão a decidir entre a frequência de faturação mensal e anual.</span><span class="sxs-lookup"><span data-stu-id="c5c1c-129">See [License-based billing](license-based-billing.md) for information that will help you decide between the monthly and annual billing frequency.</span></span>
   - <span data-ttu-id="c5c1c-130">**Categoria**: Escolha **Empresa,** **Pequenas empresas,** ou **Trial.**</span><span class="sxs-lookup"><span data-stu-id="c5c1c-130">**Category**: Choose **Enterprise**, **Small business**, or **Trial**.</span></span> <span data-ttu-id="c5c1c-131">Para obter informações sobre subscrições de teste, consulte [Oferecer aos seus clientes testes de produtos microsoft.](offer-your-customers-trials-of-microsoft-products.md)</span><span class="sxs-lookup"><span data-stu-id="c5c1c-131">For info about trial subscriptions, see [Offer your customers trials of Microsoft products](offer-your-customers-trials-of-microsoft-products.md).</span></span>

5. <span data-ttu-id="c5c1c-132">Selecione as subscrições de produto que pretende comprar para o seu cliente.</span><span class="sxs-lookup"><span data-stu-id="c5c1c-132">Select the product subscriptions you want to purchase for your customer.</span></span> <span data-ttu-id="c5c1c-133">Os produtos que vê dependem do tipo de segmento de cliente (educação, governo, etc.) e dos filtros que aplicou.</span><span class="sxs-lookup"><span data-stu-id="c5c1c-133">The products you see depend on the type of customer segment (education, government, etc.) and the filters you have applied.</span></span> <span data-ttu-id="c5c1c-134">Algumas ofertas apresentadas no Mercado podem nem sempre estar disponíveis para um cliente específico ou um parceiro CSP específico.</span><span class="sxs-lookup"><span data-stu-id="c5c1c-134">Some offers shown on the Marketplace may not always be available to a specific customer or a specific CSP partner.</span></span> <span data-ttu-id="c5c1c-135">Isto pode ser porque:</span><span class="sxs-lookup"><span data-stu-id="c5c1c-135">This can be because:</span></span>

   - <span data-ttu-id="c5c1c-136">O cliente já tem uma subscrição desse produto e só é permitido um</span><span class="sxs-lookup"><span data-stu-id="c5c1c-136">The customer already has a subscription to that product and is only allowed one</span></span>

   - <span data-ttu-id="c5c1c-137">A subscrição do cliente pode ter sido suspensa (neste caso, pode reativar a subscrição em vez de comprar uma nova.)</span><span class="sxs-lookup"><span data-stu-id="c5c1c-137">The customer's subscription may have been suspended (In this case, you can reactivate the subscription rather than purchase a new one.)</span></span>

   - <span data-ttu-id="c5c1c-138">Para as ofertas isv SaaS, pode haver algumas razões pelas quais a oferta não está disponível para compra: O ISV pode não suportar o país ou região de faturação do cliente; o ISV pode ter optado por não disponibilizar a oferta através do programa CSP; ou, o ISV pode ter feito a oferta [exclusiva](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) a apenas alguns parceiros da CSP.</span><span class="sxs-lookup"><span data-stu-id="c5c1c-138">For ISV SaaS offers, there may be a few reasons why the offer is not available to purchase: The ISV may not support the customer's billing country or region; the ISV may have chosen not to make the offer available through the CSP program; or, the ISV may have made the offer [exclusive](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to only certain CSP partners.</span></span> <span data-ttu-id="c5c1c-139">A oferta ISV também pode não ser transacionável através do Partner Center (por exemplo, contentores ou algumas ofertas baseadas em uso).</span><span class="sxs-lookup"><span data-stu-id="c5c1c-139">The ISV offer may also not be transactable through the Partner Center (for example, containers or some usage-based offers).</span></span>  

6. <span data-ttu-id="c5c1c-140">Para cada subscrição que pretende adicionar, insira o número de licenças (se necessário) e selecione **Adicionar ao carrinho**.</span><span class="sxs-lookup"><span data-stu-id="c5c1c-140">For each subscription you want to add, enter the number of licenses (if needed) and select **Add to cart**.</span></span>

7. <span data-ttu-id="c5c1c-141">Quando terminar de adicionar subscrições, selecione **'Rever'** e reveja a sua encomenda.</span><span class="sxs-lookup"><span data-stu-id="c5c1c-141">When you are finished adding subscriptions, select **Review** and review your order.</span></span>

8. <span data-ttu-id="c5c1c-142">Depois de rever as suas encomendas e estiver pronto para comprar estas subscrições, selecione **Comprar**.</span><span class="sxs-lookup"><span data-stu-id="c5c1c-142">Once you've reviewed your orders and are ready to purchase these subscriptions, select **Buy**.</span></span>

9. <span data-ttu-id="c5c1c-143">Depois de comprar uma subscrição para um cliente, ocorrerá o seguinte:</span><span class="sxs-lookup"><span data-stu-id="c5c1c-143">After you buy a subscription for a customer, the following will occur:</span></span>

    - <span data-ttu-id="c5c1c-144">Pode rever ou editar a subscrição selecionando o nome de subscrição na página de **Subscrições** desse cliente.</span><span class="sxs-lookup"><span data-stu-id="c5c1c-144">You can review or edit the subscription by selecting the subscription name from that customer's **Subscriptions** page.</span></span> <span data-ttu-id="c5c1c-145">A partir daqui, pode selecionar licenças adicionais se alguma estiver disponível, alterar a quantidade de licenças ou suspender a subscrição.</span><span class="sxs-lookup"><span data-stu-id="c5c1c-145">From here, you can select add-on licenses if any are available, change the quantity of licenses, or suspend the subscription.</span></span>

    <span data-ttu-id="c5c1c-146">**Para assinaturas ISV SaaS (baseadas em licenças e contadores):**</span><span class="sxs-lookup"><span data-stu-id="c5c1c-146">**For ISV SaaS (license-based and metered) subscriptions:**</span></span>
    - <span data-ttu-id="c5c1c-147">Receberá um link para o site da editora ISV.</span><span class="sxs-lookup"><span data-stu-id="c5c1c-147">You will receive a link to the ISV publisher's site.</span></span> <span data-ttu-id="c5c1c-148">Este link deve ajudá-lo a completar a implementação ou configuração da conta da subscrição do cliente.</span><span class="sxs-lookup"><span data-stu-id="c5c1c-148">This link should help you complete the deployment or account setup of the customer's subscription.</span></span>
      
    >[!NOTE]
    > <span data-ttu-id="c5c1c-149">Nem você nem o seu cliente receberão um e-mail com instruções para completar a configuração/provisionamento da conta para este tipo de subscrição ISV.)</span><span class="sxs-lookup"><span data-stu-id="c5c1c-149">Neither you nor your customer will receive an email with instructions to complete account set up/provisioning for this type of ISV subscription.)</span></span>

    - <span data-ttu-id="c5c1c-150">Se a sua subscrição vier com um teste gratuito de 30 dias, o período experimental gratuito será aplicado automaticamente.</span><span class="sxs-lookup"><span data-stu-id="c5c1c-150">If your subscription comes with a 30-day free trial, the free trial period will be applied automatically.</span></span> <span data-ttu-id="c5c1c-151">Como parceiro no programa CSP, não pode renunciar ao período experimental gratuito nas ofertas que compra para os clientes.</span><span class="sxs-lookup"><span data-stu-id="c5c1c-151">As a partner in the CSP program, you cannot waive the free trial period on offers you purchase for customers.</span></span> <span data-ttu-id="c5c1c-152">Uma vez terminada a duração do período experimental gratuito, o prazo de subscrição começará e a subscrição converter-se-á em estatuto pago.</span><span class="sxs-lookup"><span data-stu-id="c5c1c-152">Once the free trial period ends, the subscription term will begin and the subscription will convert to paid status.</span></span> <span data-ttu-id="c5c1c-153">A subscrição irá então renovar automaticamente de acordo com o mesmo horário.</span><span class="sxs-lookup"><span data-stu-id="c5c1c-153">The subscription will then auto-renew according to the same schedule.</span></span>
   
## <a name="update-subscriptions-with-add-ons"></a><span data-ttu-id="c5c1c-154">Atualizar subscrições com suplementos</span><span class="sxs-lookup"><span data-stu-id="c5c1c-154">Update subscriptions with add-ons</span></span> 

<span data-ttu-id="c5c1c-155">Para comprar um suplemento, o cliente deve ter uma subscrição base ativa.</span><span class="sxs-lookup"><span data-stu-id="c5c1c-155">To purchase an add-on the customer must first have an active base subscription.</span></span>  <span data-ttu-id="c5c1c-156">Não pode comprar suplementos através do catálogo.</span><span class="sxs-lookup"><span data-stu-id="c5c1c-156">You can't purchase add-ons through the catalog.</span></span>

1. <span data-ttu-id="c5c1c-157">Inscreva-se no painel do Centro [de Parceiros](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="c5c1c-157">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="c5c1c-158">No menu Partner Center, selecione **Clientes,** em seguida, escolha um cliente da lista.</span><span class="sxs-lookup"><span data-stu-id="c5c1c-158">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="c5c1c-159">Escolha a subscrição que pretende gerir.</span><span class="sxs-lookup"><span data-stu-id="c5c1c-159">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="c5c1c-160">Abaixo da secção **'Estado',** encontram-se uma lista de Add-ons disponíveis para a subscrição.</span><span class="sxs-lookup"><span data-stu-id="c5c1c-160">Below the **Status** section, are a list of available Add-ons for the subscription.</span></span>  

5. <span data-ttu-id="c5c1c-161">Atualize a quantidade de licenças para cada Add-on necessário.</span><span class="sxs-lookup"><span data-stu-id="c5c1c-161">Update the quantity of licenses for each required Add-on.</span></span> <span data-ttu-id="c5c1c-162">Em seguida, **submeta** as alterações.</span><span class="sxs-lookup"><span data-stu-id="c5c1c-162">Then **Submit** your changes.</span></span>

<span data-ttu-id="c5c1c-163">A capacidade de adquirir addons através do Partner Center só está disponível para faturas diretas e fornecedores indiretos.</span><span class="sxs-lookup"><span data-stu-id="c5c1c-163">The ability to purchase add-ons through Partner Center is only available to direct bill and indirect providers.</span></span>
<span data-ttu-id="c5c1c-164">Apenas os complementos elegíveis são apresentados com base nos requisitos de base e na disponibilidade regional.</span><span class="sxs-lookup"><span data-stu-id="c5c1c-164">Only eligible add-ons are displayed based on the base requirements and regional availability.</span></span> <span data-ttu-id="c5c1c-165">Veja a matriz da oferta Revendedor de Soluções Cloud para obter mais informações sobre preços e ofertas.</span><span class="sxs-lookup"><span data-stu-id="c5c1c-165">Refer to the Cloud Reseller offer matrix for more information about pricing and offers.</span></span>  <span data-ttu-id="c5c1c-166">A suspensão da subscrição base suspenderá também todos os suplementos associados.</span><span class="sxs-lookup"><span data-stu-id="c5c1c-166">Suspending the base subscription will also suspend any associated add-ons.</span></span>

<span data-ttu-id="c5c1c-167">As datas de início dos suplementos alinham-se com a subscrição base e os custos são calculados a partir da Data de início dos custos e da Data de fim dos custos, com os custos numa base pro-rata na primeira fatura.</span><span class="sxs-lookup"><span data-stu-id="c5c1c-167">Start dates for add-ons align to the base subscription and charges are calculated from the Charge start date and Charge end date with pro-rata charges in the first invoice.</span></span> <span data-ttu-id="c5c1c-168">Para obter informações adicionais consulte, [faturação baseada em licença.](license-based-billing.md)</span><span class="sxs-lookup"><span data-stu-id="c5c1c-168">For additional information see, [License-based billing](license-based-billing.md).</span></span>


## <a name="suspend-or-cancel-a-subscription"></a><span data-ttu-id="c5c1c-169">Suspender ou cancelar uma subscrição</span><span class="sxs-lookup"><span data-stu-id="c5c1c-169">Suspend or cancel a subscription</span></span>

<span data-ttu-id="c5c1c-170">Os parceiros podem suspender ou cancelar uma subscrição se solicitado pelo cliente, ou em casos de não pagamento ou fraude.</span><span class="sxs-lookup"><span data-stu-id="c5c1c-170">Partners can suspend or cancel a subscription if requested by the customer, or in cases of nonpayment or fraud.</span></span>

### <a name="suspend-a-subscription"></a><span data-ttu-id="c5c1c-171">Suspender uma subscrição</span><span class="sxs-lookup"><span data-stu-id="c5c1c-171">Suspend a subscription</span></span>

<span data-ttu-id="c5c1c-172">Quando altera o estado de uma subscrição de **Suspenso,** os utilizadores não podem iniciar sôms ou aceder a serviços.</span><span class="sxs-lookup"><span data-stu-id="c5c1c-172">When you change the status of a subscription to **Suspended**, users are not able to sign in or access services.</span></span>

1. <span data-ttu-id="c5c1c-173">Inscreva-se no painel do Centro [de Parceiros](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="c5c1c-173">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="c5c1c-174">No menu Partner Center, selecione **Clientes,** em seguida, escolha um cliente da lista.</span><span class="sxs-lookup"><span data-stu-id="c5c1c-174">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="c5c1c-175">Escolha a subscrição que pretende gerir.</span><span class="sxs-lookup"><span data-stu-id="c5c1c-175">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="c5c1c-176">Na secção **Estado**, escolha **Suspenso**.</span><span class="sxs-lookup"><span data-stu-id="c5c1c-176">In the **Status** section, choose **Suspended**.</span></span> <span data-ttu-id="c5c1c-177">Em seguida, **submeta** as alterações.</span><span class="sxs-lookup"><span data-stu-id="c5c1c-177">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="c5c1c-178">Todos os dados serão eliminados a menos que a subscrição seja reativada no prazo de 90 dias, ou 90 dias mais o número de dias entre o momento em que a conta foi aberta e o primeiro período de faturação (máximo de 120 dias).</span><span class="sxs-lookup"><span data-stu-id="c5c1c-178">All data will be deleted unless the subscription is reactivated within 90 days, or 90 days plus the number of days between the time the account was opened and the first billing period (maximum 120 days).</span></span>

<span data-ttu-id="c5c1c-179">Quando suspende uma subscrição, a data que vê abaixo do botão **Suspenso** indica quando a subscrição expirará automaticamente se não a reativar.</span><span class="sxs-lookup"><span data-stu-id="c5c1c-179">When you suspend a subscription, the date you see below the **Suspended** button indicates when the subscription would automatically expire if you don't reactivate it.</span></span> 

### <a name="cancel-a-subscription"></a><span data-ttu-id="c5c1c-180">Cancelar uma subscrição</span><span class="sxs-lookup"><span data-stu-id="c5c1c-180">Cancel a subscription</span></span>

<span data-ttu-id="c5c1c-181">Tem a opção de cancelar subscrições SaaS baseadas em licenças de editores ISV de terceiros dentro do [mercado comercial](csp-commercial-marketplace-overview.md)partner Center .</span><span class="sxs-lookup"><span data-stu-id="c5c1c-181">You have the option to cancel license-based SaaS subscriptions from third-party ISV publishers within the Partner Center [commercial marketplace](csp-commercial-marketplace-overview.md).</span></span> <span data-ttu-id="c5c1c-182">Desde que cancele dentro do período de cancelamento, receberá um reembolso total.</span><span class="sxs-lookup"><span data-stu-id="c5c1c-182">As long as you cancel within the cancellation period, you will receive a full refund.</span></span>

<span data-ttu-id="c5c1c-183">Para ofertas ISV faturadas mensalmente:</span><span class="sxs-lookup"><span data-stu-id="c5c1c-183">For ISV offers billed monthly:</span></span>

- <span data-ttu-id="c5c1c-184">Se cancelar menos de 24 horas após a encomenda, receberá um crédito total na próxima fatura.</span><span class="sxs-lookup"><span data-stu-id="c5c1c-184">If you cancel less than 24 hours after you placed the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="c5c1c-185">Se cancelar mais de 24 horas após a encomenda, o cancelamento será agendado para a renovação.</span><span class="sxs-lookup"><span data-stu-id="c5c1c-185">If you cancel later than 24 hours after you placed the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="c5c1c-186">Para ofertas faturadas anualmente:</span><span class="sxs-lookup"><span data-stu-id="c5c1c-186">For offers billed annually:</span></span>

- <span data-ttu-id="c5c1c-187">Se cancelar menos de 14 dias após a e realização do pedido, receberá um crédito total na próxima fatura.</span><span class="sxs-lookup"><span data-stu-id="c5c1c-187">If you cancel less than 14 days after you place the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="c5c1c-188">Se cancelar mais de 14 dias após a e realização da encomenda, o cancelamento será agendado para a renovação.</span><span class="sxs-lookup"><span data-stu-id="c5c1c-188">If you cancel later than 14 days after you place the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="c5c1c-189">Depois destes períodos terminados, deixará de ver a opção de cancelar a subscrição.</span><span class="sxs-lookup"><span data-stu-id="c5c1c-189">After these periods are over, you will no longer see the option to cancel the subscription.</span></span>

> [!NOTE]
> <span data-ttu-id="c5c1c-190">Os serviços ISV baseados e medidos em uso (que utilizam máquinas virtuais ou contentores, por exemplo) não são elegíveis para devolução.</span><span class="sxs-lookup"><span data-stu-id="c5c1c-190">Usage-based and metered, third-party ISV services (that use virtual machines or containers, for example) are not eligible for return.</span></span> <span data-ttu-id="c5c1c-191">Os serviços baseados na utilização podem ser desavisionados como um método de cancelamento.</span><span class="sxs-lookup"><span data-stu-id="c5c1c-191">Usage-based services can be de-provisioned as a cancellation method.</span></span> <span data-ttu-id="c5c1c-192">Uma vez que os encargos são cobrados após a utilização, estes serviços não são elegíveis para reembolso.</span><span class="sxs-lookup"><span data-stu-id="c5c1c-192">Since charges are billed after use, these services are not eligible for a refund.</span></span>

<span data-ttu-id="c5c1c-193">Para cancelar uma subscrição SaaS com base numa licença num editor do ISV, faça o seguinte:</span><span class="sxs-lookup"><span data-stu-id="c5c1c-193">To cancel a license-based SaaS subscription from an ISV publisher, do the following:</span></span>

1. <span data-ttu-id="c5c1c-194">Inscreva-se no painel do Centro [de Parceiros](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="c5c1c-194">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="c5c1c-195">No menu Partner Center, selecione **Clientes,** em seguida, escolha um cliente da lista.</span><span class="sxs-lookup"><span data-stu-id="c5c1c-195">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="c5c1c-196">Localize a subscrição que pretende cancelar.</span><span class="sxs-lookup"><span data-stu-id="c5c1c-196">Locate the subscription you want to cancel.</span></span>

4. <span data-ttu-id="c5c1c-197">Na coluna **'Estado',** **selecione Cancelar**.</span><span class="sxs-lookup"><span data-stu-id="c5c1c-197">In the **Status** column, select **Cancel**.</span></span> <span data-ttu-id="c5c1c-198">Em seguida, **submeta** as alterações.</span><span class="sxs-lookup"><span data-stu-id="c5c1c-198">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="c5c1c-199">Se aparecer uma caixa de diálogo, preencha os detalhes relevantes e, em seguida, **selecione Enviar por isso**.</span><span class="sxs-lookup"><span data-stu-id="c5c1c-199">If a dialog box appears, fill out any relevant details then select **Submit**.</span></span>

6. <span data-ttu-id="c5c1c-200">Para confirmar o cancelamento, selecione **Sim, cancele**.</span><span class="sxs-lookup"><span data-stu-id="c5c1c-200">To confirm the cancellation, select **Yes, cancel**.</span></span>

> [!NOTE]
> <span data-ttu-id="c5c1c-201">Também pode optar por cancelar uma subscrição do Azure Marketplace utilizando APIs.</span><span class="sxs-lookup"><span data-stu-id="c5c1c-201">You can also choose to cancel an Azure Marketplace subscription using APIs.</span></span> <span data-ttu-id="c5c1c-202">Para tal, consulte [cancelar uma subscrição do Azure Marketplace](/partner-center/develop/cancel-an-azure-marketplace-subscription).</span><span class="sxs-lookup"><span data-stu-id="c5c1c-202">To do so, see [Cancel an Azure Marketplace subscription](/partner-center/develop/cancel-an-azure-marketplace-subscription).</span></span>

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a><span data-ttu-id="c5c1c-203">Escolha se renova automaticamente uma subscrição de mercado comercial</span><span class="sxs-lookup"><span data-stu-id="c5c1c-203">Choose whether to automatically renew a commercial marketplace subscription</span></span>

<span data-ttu-id="c5c1c-204">Por predefinição, as subscrições ativas estão definidas para se renovarem automaticamente quando o período de subscrição terminar.</span><span class="sxs-lookup"><span data-stu-id="c5c1c-204">By default, active subscriptions are set to automatically renew when the subscription period expires.</span></span> <span data-ttu-id="c5c1c-205">Para [subscrições de produtos de mercado comercial,](csp-commercial-marketplace-overview.md)pode optar opcionalmente por não renovar automaticamente a subscrição.</span><span class="sxs-lookup"><span data-stu-id="c5c1c-205">For [subscriptions to commercial marketplace products](csp-commercial-marketplace-overview.md), you can optionally choose not to automatically renew the subscription.</span></span>

<span data-ttu-id="c5c1c-206">Para impedir que uma subscrição de mercado comercial ativo renove automaticamente:</span><span class="sxs-lookup"><span data-stu-id="c5c1c-206">To stop an active commercial marketplace subscription from automatically renewing:</span></span>

1. <span data-ttu-id="c5c1c-207">Inscreva-se no painel do Centro [de Parceiros](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="c5c1c-207">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="c5c1c-208">No menu Partner Center, selecione **Clientes,** em seguida, escolha um cliente da lista.</span><span class="sxs-lookup"><span data-stu-id="c5c1c-208">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="c5c1c-209">Selecione **Subscrições**.</span><span class="sxs-lookup"><span data-stu-id="c5c1c-209">Select **Subscriptions**.</span></span> <span data-ttu-id="c5c1c-210">Isto lista quaisquer subscrições baseadas em licença que tenha comprado para o cliente.</span><span class="sxs-lookup"><span data-stu-id="c5c1c-210">This lists any license-based subscriptions you have purchased for the customer.</span></span>

4. <span data-ttu-id="c5c1c-211">Na coluna **Subscrição,** selecione a subscrição que pretende modificar.</span><span class="sxs-lookup"><span data-stu-id="c5c1c-211">In the **Subscription** column, select the subscription you want to modify.</span></span>

5. <span data-ttu-id="c5c1c-212">Na página de detalhes da subscrição, localize a secção **'Estado'** e desmarque a caixa **de renovação automática.**</span><span class="sxs-lookup"><span data-stu-id="c5c1c-212">In the subscription details page, locate the **Status** section and uncheck the **Auto-renew** box.</span></span>

6. <span data-ttu-id="c5c1c-213">Selecione **Submeter**.</span><span class="sxs-lookup"><span data-stu-id="c5c1c-213">Select **Submit**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="c5c1c-214">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="c5c1c-214">Next steps</span></span>

- [<span data-ttu-id="c5c1c-215">Compre produtos de mercado comercial para os seus clientes</span><span class="sxs-lookup"><span data-stu-id="c5c1c-215">Purchase commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-purchase.md)

- [<span data-ttu-id="c5c1c-216">Gerir produtos de mercado comercial para os seus clientes</span><span class="sxs-lookup"><span data-stu-id="c5c1c-216">Manage commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-manage.md)

- [<span data-ttu-id="c5c1c-217">Descrição geral do marketplace comercial</span><span class="sxs-lookup"><span data-stu-id="c5c1c-217">Commercial marketplace overview</span></span>](csp-commercial-marketplace-overview.md)