---
title: Criar subscrições de clientes no Partner Center
ms.topic: how-to
ms.date: 05/19/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como vender subscrições aos seus clientes por produtos publicados pela Microsoft, bem como produtos SaaS publicados por ISVs de terceiros.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: 9052954c81ef55a2bfa06778ace651c9d0f9b26f
ms.sourcegitcommit: e0444145d7720df948b9d02ae2469206db48dba5
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110201413"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a><span data-ttu-id="f37cf-103">Create, suspend, or cancel customer subscriptions (Criar, suspender ou cancelar subscrições de clientes)</span><span class="sxs-lookup"><span data-stu-id="f37cf-103">Create, suspend, or cancel customer subscriptions</span></span>

<span data-ttu-id="f37cf-104">**Aplica-se a**: Partner Center | Centro de Parceiros para Microsoft Cloud para governo dos EUA</span><span class="sxs-lookup"><span data-stu-id="f37cf-104">**Applies to**: Partner Center | Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="f37cf-105">**Funções adequadas**: Agente administrador | Administrador de faturação | Administração global | Agente helpdesk | Agente comercial</span><span class="sxs-lookup"><span data-stu-id="f37cf-105">**Appropriate roles**: Admin agent | Billing admin | Global admin | Helpdesk agent | Sales agent</span></span>

<span data-ttu-id="f37cf-106">Depois de ter criado um registo do seu cliente no Partner Center, pode vendê-los subscrições a produtos do catálogo.</span><span class="sxs-lookup"><span data-stu-id="f37cf-106">After you've created a record of your customer in the Partner Center, you can sell them subscriptions to products in the catalog.</span></span> <span data-ttu-id="f37cf-107">Isto inclui produtos publicados pela Microsoft e software como um serviço (SaaS) produtos publicados por fornecedores de software independentes de terceiros (ISVs) para o [mercado comercial.](https://azuremarketplace.microsoft.com/marketplace)</span><span class="sxs-lookup"><span data-stu-id="f37cf-107">This includes products published by Microsoft and Software as a Service (SaaS) products published by third-party Independent Software Vendors (ISVs) to the [commercial marketplace](https://azuremarketplace.microsoft.com/marketplace).</span></span>

<span data-ttu-id="f37cf-108">Algumas ofertas são limitadas a uma subscrição por cliente.</span><span class="sxs-lookup"><span data-stu-id="f37cf-108">Some offers are limited to one subscription per customer.</span></span> <span data-ttu-id="f37cf-109">Para ver uma lista das ofertas restritas, visite a página de Preços e Ofertas do Centro de Parceiros.</span><span class="sxs-lookup"><span data-stu-id="f37cf-109">To see a list of which offers are restricted, visit the Partner Center Pricing and Offers page.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="f37cf-110">Como parceiro no programa CSP, pode adquirir assinaturas SaaS **baseadas em licenças** ou **medidos** a editores da ISV dentro do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="f37cf-110">As a partner in the CSP program, you can purchase **license-based** or **metered** SaaS subscriptions from ISV publishers within Partner Center.</span></span> <span data-ttu-id="f37cf-111">Isto significa que pode adquirir qualquer oferta SaaS **baseada em licença** ou **medido** que o editor ISV lhe tenha disponibilizado, incluindo [ofertas exclusivas](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) às quais tem acesso.</span><span class="sxs-lookup"><span data-stu-id="f37cf-111">This means you can purchase any **license-based** or **metered** SaaS offer the ISV publisher has made available to you, including [exclusive offers](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to which you have access.</span></span> <span data-ttu-id="f37cf-112">Para comprar ou gerir outras ofertas comerciais de marketplace a partir de ISVs (tais como ofertas baseadas em uso envolvendo aplicações Azure, Contentores ou VMs), você deve ir ao [portal Azure.](https://portal.azure.com/)</span><span class="sxs-lookup"><span data-stu-id="f37cf-112">To purchase or manage other, commercial marketplace offers from ISVs (such as usage-based offers involving Azure applications, Containers or VMs), you must go to the [Azure portal](https://portal.azure.com/).</span></span>

>[!NOTE]
><span data-ttu-id="f37cf-113">Todas as datas e horários no Partner Center são dadas na norma de tempo coordenada (UTC) do tempo universal.</span><span class="sxs-lookup"><span data-stu-id="f37cf-113">All dates and times in Partner Center are given in the Universal Time Coordinated (UTC) time standard.</span></span> <span data-ttu-id="f37cf-114">Isto pode diferir até 24 horas a partir da sua hora local.</span><span class="sxs-lookup"><span data-stu-id="f37cf-114">This can differ by up to 24 hours from your local time.</span></span>

## <a name="create-a-new-subscription"></a><span data-ttu-id="f37cf-115">Criar uma nova subscrição</span><span class="sxs-lookup"><span data-stu-id="f37cf-115">Create a new subscription</span></span>

1. <span data-ttu-id="f37cf-116">Inicie sessão no [dashboard do Centro de Parceiros](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="f37cf-116">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="f37cf-117">No menu Partner Center, selecione **Clientes,** em seguida, escolha um cliente da lista.</span><span class="sxs-lookup"><span data-stu-id="f37cf-117">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="f37cf-118">Selecione **Adicionar subscrição**.</span><span class="sxs-lookup"><span data-stu-id="f37cf-118">Select **Add subscription**.</span></span> <span data-ttu-id="f37cf-119">O separador **Serviços Online** mostrará todas as ofertas disponíveis do Marketplace SaaS.</span><span class="sxs-lookup"><span data-stu-id="f37cf-119">The **Online Services** tab will show all available Marketplace SaaS offers.</span></span>

4. <span data-ttu-id="f37cf-120">Para ver apenas certos tipos de subscrições, faça seleções nos filtros disponíveis:</span><span class="sxs-lookup"><span data-stu-id="f37cf-120">To see only certain types of subscriptions, make selections in the available filters:</span></span>
   - <span data-ttu-id="f37cf-121">**Editor**: Escolha a **Microsoft** para ver apenas ofertas da Microsoft, ou **Partner** para ver produtos de mercado comercial publicados por ISVs.</span><span class="sxs-lookup"><span data-stu-id="f37cf-121">**Publisher**: Choose **Microsoft** to see only offers from Microsoft, or **Partner** to see commercial marketplace products published by ISVs.</span></span>
   - <span data-ttu-id="f37cf-122">**Tipo de faturação**: Selecione o tipo de faturação de subscrição que pretende utilizar: **Licença** ou **Utilização**.</span><span class="sxs-lookup"><span data-stu-id="f37cf-122">**Billing type**: Select the type of subscription billing you want to use: **License** or **Usage**.</span></span> <span data-ttu-id="f37cf-123">Consulte [a faturação baseada em licença](license-based-billing.md) para obter informações que o ajudarão a decidir entre a frequência de faturação mensal e anual.</span><span class="sxs-lookup"><span data-stu-id="f37cf-123">See [License-based billing](license-based-billing.md) for information that will help you decide between the monthly and annual billing frequency.</span></span>
   - <span data-ttu-id="f37cf-124">**Categoria**: Escolha **Empresa,** **Pequenas empresas,** ou **Trial.**</span><span class="sxs-lookup"><span data-stu-id="f37cf-124">**Category**: Choose **Enterprise**, **Small business**, or **Trial**.</span></span> <span data-ttu-id="f37cf-125">Para obter informações sobre subscrições de teste, consulte [Oferecer aos seus clientes testes de produtos microsoft.](offer-your-customers-trials-of-microsoft-products.md)</span><span class="sxs-lookup"><span data-stu-id="f37cf-125">For info about trial subscriptions, see [Offer your customers trials of Microsoft products](offer-your-customers-trials-of-microsoft-products.md).</span></span>

5. <span data-ttu-id="f37cf-126">Selecione as subscrições de produto que pretende comprar para o seu cliente.</span><span class="sxs-lookup"><span data-stu-id="f37cf-126">Select the product subscriptions you want to purchase for your customer.</span></span> <span data-ttu-id="f37cf-127">Os produtos que vê dependem do tipo de segmento de cliente (educação, governo, etc.) e dos filtros que aplicou.</span><span class="sxs-lookup"><span data-stu-id="f37cf-127">The products you see depend on the type of customer segment (education, government, etc.) and the filters you have applied.</span></span> <span data-ttu-id="f37cf-128">Algumas ofertas apresentadas no Mercado podem nem sempre estar disponíveis para um cliente específico ou um parceiro CSP específico.</span><span class="sxs-lookup"><span data-stu-id="f37cf-128">Some offers shown on the Marketplace may not always be available to a specific customer or a specific CSP partner.</span></span> <span data-ttu-id="f37cf-129">Isto pode ser porque:</span><span class="sxs-lookup"><span data-stu-id="f37cf-129">This can be because:</span></span>

   - <span data-ttu-id="f37cf-130">O cliente já tem uma subscrição desse produto e só é permitido um</span><span class="sxs-lookup"><span data-stu-id="f37cf-130">The customer already has a subscription to that product and is only allowed one</span></span>

   - <span data-ttu-id="f37cf-131">A subscrição do cliente pode ter sido suspensa (neste caso, pode reativar a subscrição em vez de comprar uma nova.)</span><span class="sxs-lookup"><span data-stu-id="f37cf-131">The customer's subscription may have been suspended (In this case, you can reactivate the subscription rather than purchase a new one.)</span></span>

   - <span data-ttu-id="f37cf-132">Para as ofertas isv SaaS, pode haver algumas razões pelas quais a oferta não está disponível para compra: O ISV pode não suportar o país ou região de faturação do cliente; o ISV pode ter optado por não disponibilizar a oferta através do programa CSP; ou, o ISV pode ter feito a oferta [exclusiva](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) a apenas alguns parceiros da CSP.</span><span class="sxs-lookup"><span data-stu-id="f37cf-132">For ISV SaaS offers, there may be a few reasons why the offer is not available to purchase: The ISV may not support the customer's billing country or region; the ISV may have chosen not to make the offer available through the CSP program; or, the ISV may have made the offer [exclusive](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to only certain CSP partners.</span></span> <span data-ttu-id="f37cf-133">A oferta ISV também pode não ser transacionável através do Partner Center (por exemplo, contentores ou algumas ofertas baseadas em uso).</span><span class="sxs-lookup"><span data-stu-id="f37cf-133">The ISV offer may also not be transactable through the Partner Center (for example, containers or some usage-based offers).</span></span>  

6. <span data-ttu-id="f37cf-134">Para cada subscrição que pretende adicionar, insira o número de licenças (se necessário) e selecione **Adicionar ao carrinho**.</span><span class="sxs-lookup"><span data-stu-id="f37cf-134">For each subscription you want to add, enter the number of licenses (if needed) and select **Add to cart**.</span></span>

7. <span data-ttu-id="f37cf-135">Quando terminar de adicionar subscrições, selecione **'Rever'** e reveja a sua encomenda.</span><span class="sxs-lookup"><span data-stu-id="f37cf-135">When you are finished adding subscriptions, select **Review** and review your order.</span></span>

8. <span data-ttu-id="f37cf-136">Depois de rever as suas encomendas e estiver pronto para comprar estas subscrições, selecione **Comprar**.</span><span class="sxs-lookup"><span data-stu-id="f37cf-136">Once you've reviewed your orders and are ready to purchase these subscriptions, select **Buy**.</span></span>

9. <span data-ttu-id="f37cf-137">Depois de comprar uma subscrição para um cliente, ocorrerá o seguinte:</span><span class="sxs-lookup"><span data-stu-id="f37cf-137">After you buy a subscription for a customer, the following will occur:</span></span>

    - <span data-ttu-id="f37cf-138">Pode rever ou editar a subscrição selecionando o nome de subscrição na página de **Subscrições** desse cliente.</span><span class="sxs-lookup"><span data-stu-id="f37cf-138">You can review or edit the subscription by selecting the subscription name from that customer's **Subscriptions** page.</span></span> <span data-ttu-id="f37cf-139">A partir daqui, pode selecionar licenças adicionais se alguma estiver disponível, alterar a quantidade de licenças ou suspender a subscrição.</span><span class="sxs-lookup"><span data-stu-id="f37cf-139">From here, you can select add-on licenses if any are available, change the quantity of licenses, or suspend the subscription.</span></span>

    <span data-ttu-id="f37cf-140">**Para assinaturas ISV SaaS (baseadas em licenças e contadores):**</span><span class="sxs-lookup"><span data-stu-id="f37cf-140">**For ISV SaaS (license-based and metered) subscriptions:**</span></span>
    - <span data-ttu-id="f37cf-141">Receberá um link para o site da editora ISV.</span><span class="sxs-lookup"><span data-stu-id="f37cf-141">You will receive a link to the ISV publisher's site.</span></span> <span data-ttu-id="f37cf-142">Este link deve ajudá-lo a completar a implementação ou configuração da conta da subscrição do cliente.</span><span class="sxs-lookup"><span data-stu-id="f37cf-142">This link should help you complete the deployment or account setup of the customer's subscription.</span></span>
      
    >[!NOTE]
    > <span data-ttu-id="f37cf-143">Nem você nem o seu cliente receberão um e-mail com instruções para completar a configuração/provisionamento da conta para este tipo de subscrição ISV.)</span><span class="sxs-lookup"><span data-stu-id="f37cf-143">Neither you nor your customer will receive an email with instructions to complete account set up/provisioning for this type of ISV subscription.)</span></span>

    - <span data-ttu-id="f37cf-144">Se a sua subscrição vier com um teste gratuito de 30 dias, o período experimental gratuito será aplicado automaticamente.</span><span class="sxs-lookup"><span data-stu-id="f37cf-144">If your subscription comes with a 30-day free trial, the free trial period will be applied automatically.</span></span> <span data-ttu-id="f37cf-145">Como parceiro no programa CSP, não pode renunciar ao período experimental gratuito nas ofertas que compra para os clientes.</span><span class="sxs-lookup"><span data-stu-id="f37cf-145">As a partner in the CSP program, you cannot waive the free trial period on offers you purchase for customers.</span></span> <span data-ttu-id="f37cf-146">Uma vez terminada a duração do período experimental gratuito, o prazo de subscrição começará e a subscrição converter-se-á em estatuto pago.</span><span class="sxs-lookup"><span data-stu-id="f37cf-146">Once the free trial period ends, the subscription term will begin and the subscription will convert to paid status.</span></span> <span data-ttu-id="f37cf-147">A subscrição irá então renovar automaticamente de acordo com o mesmo horário.</span><span class="sxs-lookup"><span data-stu-id="f37cf-147">The subscription will then auto-renew according to the same schedule.</span></span>
   
## <a name="update-subscriptions-with-add-ons"></a><span data-ttu-id="f37cf-148">Atualizar subscrições com suplementos</span><span class="sxs-lookup"><span data-stu-id="f37cf-148">Update subscriptions with add-ons</span></span> 

<span data-ttu-id="f37cf-149">Para adquirir um addon, o cliente deve primeiro ter uma subscrição base ativa.</span><span class="sxs-lookup"><span data-stu-id="f37cf-149">To purchase an add-on, the customer must first have an active base subscription.</span></span>  <span data-ttu-id="f37cf-150">Não pode comprar suplementos através do catálogo.</span><span class="sxs-lookup"><span data-stu-id="f37cf-150">You can't purchase add-ons through the catalog.</span></span>

1. <span data-ttu-id="f37cf-151">Inscreva-se no painel do Centro [de Parceiros](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="f37cf-151">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="f37cf-152">No menu Partner Center, selecione **Clientes,** em seguida, escolha um cliente da lista.</span><span class="sxs-lookup"><span data-stu-id="f37cf-152">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="f37cf-153">Escolha a subscrição que pretende gerir.</span><span class="sxs-lookup"><span data-stu-id="f37cf-153">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="f37cf-154">Abaixo da secção **'Estado',** encontram-se uma lista de Add-ons disponíveis para a subscrição.</span><span class="sxs-lookup"><span data-stu-id="f37cf-154">Below the **Status** section, are a list of available Add-ons for the subscription.</span></span>  

5. <span data-ttu-id="f37cf-155">Atualize a quantidade de licenças para cada Add-on necessário.</span><span class="sxs-lookup"><span data-stu-id="f37cf-155">Update the quantity of licenses for each required Add-on.</span></span> <span data-ttu-id="f37cf-156">Em seguida, **submeta** as alterações.</span><span class="sxs-lookup"><span data-stu-id="f37cf-156">Then **Submit** your changes.</span></span>

<span data-ttu-id="f37cf-157">A capacidade de adquirir addons através do Partner Center só está disponível para faturas diretas e fornecedores indiretos.</span><span class="sxs-lookup"><span data-stu-id="f37cf-157">The ability to purchase add-ons through Partner Center is only available to direct bill and indirect providers.</span></span>
<span data-ttu-id="f37cf-158">Apenas os complementos elegíveis são apresentados com base nos requisitos de base e na disponibilidade regional.</span><span class="sxs-lookup"><span data-stu-id="f37cf-158">Only eligible add-ons are displayed based on the base requirements and regional availability.</span></span> <span data-ttu-id="f37cf-159">Para obter mais informações sobre preços e ofertas, consulte a matriz de oferta de Cloud Reseller.</span><span class="sxs-lookup"><span data-stu-id="f37cf-159">For more information about pricing and offers, refer to the Cloud Reseller offer matrix.</span></span> <span data-ttu-id="f37cf-160">A suspensão da subscrição base suspenderá também todos os suplementos associados.</span><span class="sxs-lookup"><span data-stu-id="f37cf-160">Suspending the base subscription will also suspend any associated add-ons.</span></span>

<span data-ttu-id="f37cf-161">As datas de início dos suplementos alinham-se com a subscrição base e os custos são calculados a partir da Data de início dos custos e da Data de fim dos custos, com os custos numa base pro-rata na primeira fatura.</span><span class="sxs-lookup"><span data-stu-id="f37cf-161">Start dates for add-ons align to the base subscription and charges are calculated from the Charge start date and Charge end date with pro-rata charges in the first invoice.</span></span> <span data-ttu-id="f37cf-162">Para obter informações adicionais consulte, [faturação baseada em licença.](license-based-billing.md)</span><span class="sxs-lookup"><span data-stu-id="f37cf-162">For additional information see, [License-based billing](license-based-billing.md).</span></span>


## <a name="suspend-or-cancel-a-subscription"></a><span data-ttu-id="f37cf-163">Suspender ou cancelar uma subscrição</span><span class="sxs-lookup"><span data-stu-id="f37cf-163">Suspend or cancel a subscription</span></span>

<span data-ttu-id="f37cf-164">Os parceiros podem suspender ou cancelar uma subscrição se solicitado pelo cliente, ou em casos de não pagamento ou fraude.</span><span class="sxs-lookup"><span data-stu-id="f37cf-164">Partners can suspend or cancel a subscription if requested by the customer, or in cases of nonpayment or fraud.</span></span>

### <a name="suspend-a-subscription"></a><span data-ttu-id="f37cf-165">Suspender uma subscrição</span><span class="sxs-lookup"><span data-stu-id="f37cf-165">Suspend a subscription</span></span>

<span data-ttu-id="f37cf-166">Quando altera o estado de uma subscrição de **Suspenso,** os utilizadores não podem iniciar sôms ou aceder a serviços.</span><span class="sxs-lookup"><span data-stu-id="f37cf-166">When you change the status of a subscription to **Suspended**, users are not able to sign in or access services.</span></span>

1. <span data-ttu-id="f37cf-167">Inscreva-se no painel do Centro [de Parceiros](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="f37cf-167">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="f37cf-168">No menu Partner Center, selecione **Clientes,** em seguida, escolha um cliente da lista.</span><span class="sxs-lookup"><span data-stu-id="f37cf-168">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="f37cf-169">Escolha a subscrição que pretende gerir.</span><span class="sxs-lookup"><span data-stu-id="f37cf-169">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="f37cf-170">Na secção **Estado**, escolha **Suspenso**.</span><span class="sxs-lookup"><span data-stu-id="f37cf-170">In the **Status** section, choose **Suspended**.</span></span> <span data-ttu-id="f37cf-171">Em seguida, **submeta** as alterações.</span><span class="sxs-lookup"><span data-stu-id="f37cf-171">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="f37cf-172">Todos os dados serão eliminados a menos que a subscrição seja reativada no prazo de 90 dias, ou 90 dias mais o número de dias entre o momento em que a conta foi aberta e o primeiro período de faturação (máximo de 120 dias).</span><span class="sxs-lookup"><span data-stu-id="f37cf-172">All data will be deleted unless the subscription is reactivated within 90 days, or 90 days plus the number of days between the time the account was opened and the first billing period (maximum 120 days).</span></span>

<span data-ttu-id="f37cf-173">Quando suspende uma subscrição, a data que vê abaixo do botão **Suspenso** indica quando a subscrição expirará automaticamente se não a reativar.</span><span class="sxs-lookup"><span data-stu-id="f37cf-173">When you suspend a subscription, the date you see below the **Suspended** button indicates when the subscription would automatically expire if you don't reactivate it.</span></span> 

>[!NOTE]
><span data-ttu-id="f37cf-174">As subscrições da CSP não têm um período de validade (como fazem as subscrições diretas da Web) durante o qual os serviços ainda funcionam, mas a subscrição não gera quaisquer encargos de faturação.</span><span class="sxs-lookup"><span data-stu-id="f37cf-174">CSP subscriptions don't have an expired period (the way web-direct subscriptions do) during which the services are still working but the subscription doesn't generate any billing charges.</span></span> <span data-ttu-id="f37cf-175">As assinaturas CSP estão ativas ou suspensas (ou totalmente eliminadas).</span><span class="sxs-lookup"><span data-stu-id="f37cf-175">CSP subscriptions are either active or suspended (or fully deleted).</span></span>

### <a name="cancel-a-subscription"></a><span data-ttu-id="f37cf-176">Cancelar uma subscrição</span><span class="sxs-lookup"><span data-stu-id="f37cf-176">Cancel a subscription</span></span>

<span data-ttu-id="f37cf-177">Pode cancelar subscrições saaS baseadas em licenças de editores ISV de terceiros no [mercado comercial](csp-commercial-marketplace-overview.md)partner Center .</span><span class="sxs-lookup"><span data-stu-id="f37cf-177">You can cancel license-based SaaS subscriptions from third-party ISV publishers within the Partner Center [commercial marketplace](csp-commercial-marketplace-overview.md).</span></span> <span data-ttu-id="f37cf-178">Desde que cancele dentro do período de cancelamento, receberá um reembolso total.</span><span class="sxs-lookup"><span data-stu-id="f37cf-178">As long as you cancel within the cancellation period, you will receive a full refund.</span></span>

<span data-ttu-id="f37cf-179">Para ofertas ISV faturadas mensalmente:</span><span class="sxs-lookup"><span data-stu-id="f37cf-179">For ISV offers billed monthly:</span></span>

- <span data-ttu-id="f37cf-180">Se cancelar menos de 24 horas após a encomenda, receberá um crédito total na próxima fatura.</span><span class="sxs-lookup"><span data-stu-id="f37cf-180">If you cancel less than 24 hours after you placed the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="f37cf-181">Se cancelar mais de 24 horas após a encomenda, o cancelamento será agendado para a renovação.</span><span class="sxs-lookup"><span data-stu-id="f37cf-181">If you cancel later than 24 hours after you placed the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="f37cf-182">Para ofertas faturadas anualmente:</span><span class="sxs-lookup"><span data-stu-id="f37cf-182">For offers billed annually:</span></span>

- <span data-ttu-id="f37cf-183">Se cancelar menos de 14 dias após a e realização do pedido, receberá um crédito total na próxima fatura.</span><span class="sxs-lookup"><span data-stu-id="f37cf-183">If you cancel less than 14 days after you place the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="f37cf-184">Se cancelar mais de 14 dias após a e realização da encomenda, o cancelamento será agendado para a renovação.</span><span class="sxs-lookup"><span data-stu-id="f37cf-184">If you cancel later than 14 days after you place the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="f37cf-185">Depois destes períodos terminados, deixará de ver a opção de cancelar a subscrição.</span><span class="sxs-lookup"><span data-stu-id="f37cf-185">After these periods are over, you will no longer see the option to cancel the subscription.</span></span>

> [!NOTE]
> <span data-ttu-id="f37cf-186">Os serviços ISV baseados e medidos em uso (que utilizam máquinas virtuais ou contentores, por exemplo) não são elegíveis para devolução.</span><span class="sxs-lookup"><span data-stu-id="f37cf-186">Usage-based and metered, third-party ISV services (that use virtual machines or containers, for example) are not eligible for return.</span></span> <span data-ttu-id="f37cf-187">Os serviços baseados na utilização podem ser desavisionados como um método de cancelamento.</span><span class="sxs-lookup"><span data-stu-id="f37cf-187">Usage-based services can be de-provisioned as a cancellation method.</span></span> <span data-ttu-id="f37cf-188">Uma vez que os encargos são cobrados após a utilização, estes serviços não são elegíveis para reembolso.</span><span class="sxs-lookup"><span data-stu-id="f37cf-188">Since charges are billed after use, these services are not eligible for a refund.</span></span>

<span data-ttu-id="f37cf-189">Para cancelar uma subscrição SaaS com base numa licença num editor do ISV, faça o seguinte:</span><span class="sxs-lookup"><span data-stu-id="f37cf-189">To cancel a license-based SaaS subscription from an ISV publisher, do the following:</span></span>

1. <span data-ttu-id="f37cf-190">Inscreva-se no painel do Centro [de Parceiros](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="f37cf-190">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="f37cf-191">No menu Partner Center, selecione **Clientes,** em seguida, escolha um cliente da lista.</span><span class="sxs-lookup"><span data-stu-id="f37cf-191">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="f37cf-192">Localize a subscrição que pretende cancelar.</span><span class="sxs-lookup"><span data-stu-id="f37cf-192">Locate the subscription you want to cancel.</span></span>

4. <span data-ttu-id="f37cf-193">Na coluna **'Estado',** **selecione Cancelar**.</span><span class="sxs-lookup"><span data-stu-id="f37cf-193">In the **Status** column, select **Cancel**.</span></span> <span data-ttu-id="f37cf-194">Em seguida, **submeta** as alterações.</span><span class="sxs-lookup"><span data-stu-id="f37cf-194">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="f37cf-195">Se aparecer uma caixa de diálogo, preencha os detalhes relevantes e, em seguida, **selecione Enviar por isso**.</span><span class="sxs-lookup"><span data-stu-id="f37cf-195">If a dialog box appears, fill out any relevant details then select **Submit**.</span></span>

6. <span data-ttu-id="f37cf-196">Para confirmar o cancelamento, selecione **Sim, cancele**.</span><span class="sxs-lookup"><span data-stu-id="f37cf-196">To confirm the cancellation, select **Yes, cancel**.</span></span>

> [!NOTE]
> <span data-ttu-id="f37cf-197">Também pode optar por cancelar uma subscrição do Azure Marketplace utilizando APIs.</span><span class="sxs-lookup"><span data-stu-id="f37cf-197">You can also choose to cancel an Azure Marketplace subscription using APIs.</span></span> <span data-ttu-id="f37cf-198">Para tal, consulte [cancelar uma subscrição do Azure Marketplace](/partner-center/develop/cancel-an-azure-marketplace-subscription).</span><span class="sxs-lookup"><span data-stu-id="f37cf-198">To do so, see [Cancel an Azure Marketplace subscription](/partner-center/develop/cancel-an-azure-marketplace-subscription).</span></span>

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a><span data-ttu-id="f37cf-199">Escolha se renova automaticamente uma subscrição de mercado comercial</span><span class="sxs-lookup"><span data-stu-id="f37cf-199">Choose whether to automatically renew a commercial marketplace subscription</span></span>

<span data-ttu-id="f37cf-200">Por predefinição, as subscrições ativas estão definidas para se renovarem automaticamente quando o período de subscrição terminar.</span><span class="sxs-lookup"><span data-stu-id="f37cf-200">By default, active subscriptions are set to automatically renew when the subscription period expires.</span></span> <span data-ttu-id="f37cf-201">Para [subscrições de produtos de mercado comercial,](csp-commercial-marketplace-overview.md)pode optar opcionalmente por não renovar automaticamente a subscrição.</span><span class="sxs-lookup"><span data-stu-id="f37cf-201">For [subscriptions to commercial marketplace products](csp-commercial-marketplace-overview.md), you can optionally choose not to automatically renew the subscription.</span></span>

<span data-ttu-id="f37cf-202">Para impedir que uma subscrição de mercado comercial ativo renove automaticamente:</span><span class="sxs-lookup"><span data-stu-id="f37cf-202">To stop an active commercial marketplace subscription from automatically renewing:</span></span>

1. <span data-ttu-id="f37cf-203">Inscreva-se no painel do Centro [de Parceiros](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="f37cf-203">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="f37cf-204">No menu Partner Center, selecione **Clientes,** em seguida, escolha um cliente da lista.</span><span class="sxs-lookup"><span data-stu-id="f37cf-204">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="f37cf-205">Selecione **Subscrições**.</span><span class="sxs-lookup"><span data-stu-id="f37cf-205">Select **Subscriptions**.</span></span> <span data-ttu-id="f37cf-206">Isto lista quaisquer subscrições baseadas em licença que tenha comprado para o cliente.</span><span class="sxs-lookup"><span data-stu-id="f37cf-206">This lists any license-based subscriptions you have purchased for the customer.</span></span>

4. <span data-ttu-id="f37cf-207">Na coluna **Subscrição,** selecione a subscrição que pretende modificar.</span><span class="sxs-lookup"><span data-stu-id="f37cf-207">In the **Subscription** column, select the subscription you want to modify.</span></span>

5. <span data-ttu-id="f37cf-208">Na página de detalhes da subscrição, localize a secção **'Estado'** e desmarque a caixa **de renovação automática.**</span><span class="sxs-lookup"><span data-stu-id="f37cf-208">In the subscription details page, locate the **Status** section and uncheck the **Auto-renew** box.</span></span>

6. <span data-ttu-id="f37cf-209">Selecione **Submeter**.</span><span class="sxs-lookup"><span data-stu-id="f37cf-209">Select **Submit**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="f37cf-210">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="f37cf-210">Next steps</span></span>

- [<span data-ttu-id="f37cf-211">Compre produtos de mercado comercial para os seus clientes</span><span class="sxs-lookup"><span data-stu-id="f37cf-211">Purchase commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-purchase.md)

- [<span data-ttu-id="f37cf-212">Gerir produtos de mercado comercial para os seus clientes</span><span class="sxs-lookup"><span data-stu-id="f37cf-212">Manage commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-manage.md)

- [<span data-ttu-id="f37cf-213">Descrição geral do marketplace comercial</span><span class="sxs-lookup"><span data-stu-id="f37cf-213">Commercial marketplace overview</span></span>](csp-commercial-marketplace-overview.md)