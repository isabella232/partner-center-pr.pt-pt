---
title: Anúncios de março de 2021
description: Março de 2021 anúncios para o Microsoft Partner Center, incluindo novas capacidades, promoções, ofertas, mercados ou alterações às ofertas existentes.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.custom: announcement
ms.localizationpriority: high
ms.date: 04/02/2021
ms.openlocfilehash: 12954a5f7eafb138794de879a41026ef54c65da7
ms.sourcegitcommit: c6c741475604b8daf386fb54bb2795a6445ac887
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/05/2021
ms.locfileid: "106374396"
---
# <a name="march-2021-announcements"></a><span data-ttu-id="a77c5-103">Anúncios de março de 2021</span><span class="sxs-lookup"><span data-stu-id="a77c5-103">March 2021 announcements</span></span>

<span data-ttu-id="a77c5-104">Esta página fornece os anúncios para o Microsoft Partner Center para março de 2021.</span><span class="sxs-lookup"><span data-stu-id="a77c5-104">This page provides the announcements for Microsoft Partner Center for March 2021.</span></span>

________________
## <a name="updated-csp-customer-address-validation-api-now-available-for-testing"></a><a name="18"></a><span data-ttu-id="a77c5-105">A API de validação de endereços de cliente csp atualizada já disponível para testes</span><span class="sxs-lookup"><span data-stu-id="a77c5-105">Updated CSP customer address validation API now available for testing</span></span>

### <a name="categories"></a><span data-ttu-id="a77c5-106">Categorias</span><span class="sxs-lookup"><span data-stu-id="a77c5-106">Categories</span></span>

- <span data-ttu-id="a77c5-107">Data: 2021-03-31</span><span class="sxs-lookup"><span data-stu-id="a77c5-107">Date: 2021-03-31</span></span>
- <span data-ttu-id="a77c5-108">Capacidades</span><span class="sxs-lookup"><span data-stu-id="a77c5-108">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="a77c5-109">Resumo</span><span class="sxs-lookup"><span data-stu-id="a77c5-109">Summary</span></span>

<span data-ttu-id="a77c5-110">Como parte do nosso compromisso de ajudar parceiros e clientes a gerir o seu negócio com base na confiança, estaremos convidando parceiros de todo o mundo para testar as alterações à API ValidadaAddress.</span><span class="sxs-lookup"><span data-stu-id="a77c5-110">As part of our commitment to help partners and customers run their business based on trust, we will be inviting partners worldwide to test the changes to the ValidateAddress API.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="a77c5-111">Audiência impactada</span><span class="sxs-lookup"><span data-stu-id="a77c5-111">Impacted audience</span></span>

<span data-ttu-id="a77c5-112">Todos os parceiros de conta direta da CSP e fornecedores indiretos que criam novos ou atualizaram os detalhes do endereço do cliente existentes</span><span class="sxs-lookup"><span data-stu-id="a77c5-112">All CSP direct bill partners and indirect providers who create new or update existing customer address details</span></span>

### <a name="details"></a><span data-ttu-id="a77c5-113">Detalhes</span><span class="sxs-lookup"><span data-stu-id="a77c5-113">Details</span></span>

<span data-ttu-id="a77c5-114">A Microsoft tem confiança.</span><span class="sxs-lookup"><span data-stu-id="a77c5-114">Microsoft runs on trust.</span></span> <span data-ttu-id="a77c5-115">Estamos empenhados em fornecer um método compatível, seguro e seguro de submeter a validação do endereço do cliente para transação de subscrições de clientes no programa CSP.</span><span class="sxs-lookup"><span data-stu-id="a77c5-115">We’re committed to providing a compliant, safe, and secure method of submitting customer address validation for transacting customer subscriptions in the CSP program.</span></span> <span data-ttu-id="a77c5-116">Hoje, 31 de março de 2021, introduzimos alterações na API ValidadaAddress que gostaríamos de convidá-lo a testar, antes de ir ao vivo com as mudanças em junho de 2021.</span><span class="sxs-lookup"><span data-stu-id="a77c5-116">Today, March 31, 2021, we have introduced changes to the ValidateAddress API that we’d like to invite you to test, prior to going live with the changes in June 2021.</span></span> 

<span data-ttu-id="a77c5-117">Note que estas alterações afetam apenas a API validadora.</span><span class="sxs-lookup"><span data-stu-id="a77c5-117">Note that these changes affect the ValidateAddress API only.</span></span> <span data-ttu-id="a77c5-118">CreateCustomer e UpdateBillingProfile APIs não são afetados.</span><span class="sxs-lookup"><span data-stu-id="a77c5-118">CreateCustomer and UpdateBillingProfile APIs are not affected.</span></span>

<span data-ttu-id="a77c5-119">A resposta devolverá uma das seguintes mensagens de estado:</span><span class="sxs-lookup"><span data-stu-id="a77c5-119">The response will return one of the following status messages:</span></span>

| <span data-ttu-id="a77c5-120">Estado</span><span class="sxs-lookup"><span data-stu-id="a77c5-120">Status</span></span> | <span data-ttu-id="a77c5-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="a77c5-121">Description</span></span> | <span data-ttu-id="a77c5-122">Número de endereços sugeridos devolvidos</span><span class="sxs-lookup"><span data-stu-id="a77c5-122">Number of suggested addresses returned</span></span> |
|----------|-------------|-------------------|
| <span data-ttu-id="a77c5-123">VerificadoShippable</span><span class="sxs-lookup"><span data-stu-id="a77c5-123">VerifiedShippable</span></span> | <span data-ttu-id="a77c5-124">O endereço é verificado e pode ser enviado para.</span><span class="sxs-lookup"><span data-stu-id="a77c5-124">Address is verified and can be shipped to.</span></span> | <span data-ttu-id="a77c5-125">Único</span><span class="sxs-lookup"><span data-stu-id="a77c5-125">Single</span></span> |
| <span data-ttu-id="a77c5-126">Verificado</span><span class="sxs-lookup"><span data-stu-id="a77c5-126">Verified</span></span> | <span data-ttu-id="a77c5-127">O endereço está verificado.</span><span class="sxs-lookup"><span data-stu-id="a77c5-127">Address is verified.</span></span> | <span data-ttu-id="a77c5-128">Único</span><span class="sxs-lookup"><span data-stu-id="a77c5-128">Single</span></span> |
| <span data-ttu-id="a77c5-129">InteracçãoRequired</span><span class="sxs-lookup"><span data-stu-id="a77c5-129">InteractionRequired</span></span> | <span data-ttu-id="a77c5-130">O endereço sugerido foi alterado significativamente e precisa de confirmação do utilizador.</span><span class="sxs-lookup"><span data-stu-id="a77c5-130">Suggested address(es) has been changed significantly and needs user confirmation.</span></span> | <span data-ttu-id="a77c5-131">Único</span><span class="sxs-lookup"><span data-stu-id="a77c5-131">Single</span></span> |
| <span data-ttu-id="a77c5-132">StreetPartial</span><span class="sxs-lookup"><span data-stu-id="a77c5-132">StreetPartial</span></span> | <span data-ttu-id="a77c5-133">A rua dada no endereço é parcial e precisa de mais informações.</span><span class="sxs-lookup"><span data-stu-id="a77c5-133">The given street in the address is partial and needs more info.</span></span> | <span data-ttu-id="a77c5-134">Múltiplos — máximo de três</span><span class="sxs-lookup"><span data-stu-id="a77c5-134">Multiple—maximum of three</span></span>|
| <span data-ttu-id="a77c5-135">InstalaçõesPartial</span><span class="sxs-lookup"><span data-stu-id="a77c5-135">PremisesPartial</span></span> | <span data-ttu-id="a77c5-136">As instalações dadas (número de construção, número de suite, etc.) são parciais e precisam de mais informações.</span><span class="sxs-lookup"><span data-stu-id="a77c5-136">The given premises (building number, suite number, etc.) is partial and needs more info.</span></span> | <span data-ttu-id="a77c5-137">Múltiplos — máximo de três</span><span class="sxs-lookup"><span data-stu-id="a77c5-137">Multiple—maximum of three</span></span> |
| <span data-ttu-id="a77c5-138">Vários</span><span class="sxs-lookup"><span data-stu-id="a77c5-138">Multiple</span></span> | <span data-ttu-id="a77c5-139">Existem vários campos que são parciais no endereço (potencialmente também incluindo o StreetPartial e o PremisesPartial).</span><span class="sxs-lookup"><span data-stu-id="a77c5-139">There are multiple fields that are partial in the address (potentially also including StreetPartial and PremisesPartial).</span></span> | <span data-ttu-id="a77c5-140">Múltiplos — máximo de três</span><span class="sxs-lookup"><span data-stu-id="a77c5-140">Multiple—maximum of three</span></span> |
| <span data-ttu-id="a77c5-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a77c5-141">None</span></span> | <span data-ttu-id="a77c5-142">O endereço está incorreto.</span><span class="sxs-lookup"><span data-stu-id="a77c5-142">Address is incorrect.</span></span> | <span data-ttu-id="a77c5-143">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a77c5-143">None</span></span> |
| <span data-ttu-id="a77c5-144">Não ÉDoida</span><span class="sxs-lookup"><span data-stu-id="a77c5-144">NotValidated</span></span> | <span data-ttu-id="a77c5-145">O endereço não pôde ser enviado através do processo de validação.</span><span class="sxs-lookup"><span data-stu-id="a77c5-145">Address was not able to be sent through the validation process.</span></span>  | <span data-ttu-id="a77c5-146">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a77c5-146">None</span></span> |

<span data-ttu-id="a77c5-147">Uma vez que um endereço tenha sido submetido a ser validado através da API ValidadaAddress, será devolvido o seguinte esquema de resposta:</span><span class="sxs-lookup"><span data-stu-id="a77c5-147">Once an address has been submitted to be validated via the ValidateAddress API, the following response schema will be returned:</span></span>

```csharp

// <summary>
/// Object represents the address validation response.
/// </summary>

public class AddressValidationResponse
{
   /// <summary>
   /// Gets or sets the original address
   /// </summary>
   /// <value>
   /// Original Address
   /// </value>
   public Address OriginalAddress { get; set; }

   /// <summary>
   /// Gets or sets the suggested addresses
   /// </summary>
   /// <value>
   /// Suggested Addresses
   /// </value>
   public List<Address> SuggestedAddresses { get; set; }

   /// <summary>
   /// Gets or sets the validation status
   /// </summary>
   /// <value>
   /// Status
   /// </value>
   public string Status { get; set; }

   /// <summary>
   /// Gets or sets the validation message
   /// </summary>
   /// <value>
   /// Validation Message
   /// </value>
   public string ValidationMessage { get; set; }
   ```

<span data-ttu-id="a77c5-148">Dê uma olhada nesta resposta da amostra.</span><span class="sxs-lookup"><span data-stu-id="a77c5-148">Take a look at this sample response.</span></span> <span data-ttu-id="a77c5-149">Note que para os EUA, a resposta devolverá um sufixo adicional de quatro dígitos para a linha de código postal se introduzir apenas cinco dígitos para o código postal.</span><span class="sxs-lookup"><span data-stu-id="a77c5-149">Note that for the US, the response will return an additional four-digit suffix for the postal code line if you only enter five digits for the zip code.</span></span>

```csharp

"suggested_address": {
    "Country": "US",
    "region": "WA",
    "city": "Redmond",
    "address_line1": "1 Microsoft Way",
    "postal_Code": "98052-8300"
},
"original_address": {
    "Country": "US",
    "region": "WA",
    "city": "Redmond",
    "address_line1": "1 Micro Way",
    "postal_Code": "98052"
},
"status":  "InteractionRequired",
"validation_message": "Address field invalid for property: ‘Street’"
}
```

### <a name="next-steps"></a><span data-ttu-id="a77c5-150">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="a77c5-150">Next steps</span></span>

- <span data-ttu-id="a77c5-151">Partilhe o seu ID de inquilino de sandbox com o nosso especialista em assuntos (PME), Ali Khaki, a ser incluído no voo de teste, para que possa começar a preparar-se para a atualização.</span><span class="sxs-lookup"><span data-stu-id="a77c5-151">Share your sandbox tenant ID with our subject matter expert (SME), Ali Khaki, to be included in the test flight, so that you can begin preparing for the update.</span></span>

- <span data-ttu-id="a77c5-152">Se estiver a utilizar uma solução de fornecedor de painéis de controlo (CPV), consulte o seu CPV.</span><span class="sxs-lookup"><span data-stu-id="a77c5-152">If you’re using a control panel vendor (CPV) solution, consult your CPV.</span></span>

### <a name="questions"></a><span data-ttu-id="a77c5-153">Perguntas?</span><span class="sxs-lookup"><span data-stu-id="a77c5-153">Questions?</span></span>

<span data-ttu-id="a77c5-154">Se tiver alguma dúvida ou precisar de apoio para as suas operações com a Microsoft, contacte o grupo Yammer de suporte ao seu parceiro.</span><span class="sxs-lookup"><span data-stu-id="a77c5-154">If you have any questions or need support for your operations with Microsoft, reach out to your partner support Yammer group.</span></span>

________________
## <a name="new-exchange-admin-center-eac-experience"></a><a name="17"></a><span data-ttu-id="a77c5-155">Experiência do Centro de Administração new exchange (EAC)</span><span class="sxs-lookup"><span data-stu-id="a77c5-155">New Exchange admin center (EAC) experience</span></span>

### <a name="categories"></a><span data-ttu-id="a77c5-156">Categorias</span><span class="sxs-lookup"><span data-stu-id="a77c5-156">Categories</span></span>

- <span data-ttu-id="a77c5-157">Data: 2021-03-29</span><span class="sxs-lookup"><span data-stu-id="a77c5-157">Date: 2021-03-29</span></span>
- <span data-ttu-id="a77c5-158">Capacidades</span><span class="sxs-lookup"><span data-stu-id="a77c5-158">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="a77c5-159">Resumo</span><span class="sxs-lookup"><span data-stu-id="a77c5-159">Summary</span></span>

<span data-ttu-id="a77c5-160">A partir de 27 de abril de 2021, o Centro de Administração exchange (EAC) lançará uma nova experiência que melhorará a eficiência do dia-a-dia para os utilizadores.</span><span class="sxs-lookup"><span data-stu-id="a77c5-160">Starting April 27, 2021, the Exchange admin center (EAC) will roll out a new experience that will improve day-to-day efficiency for users.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="a77c5-161">Audiência impactada</span><span class="sxs-lookup"><span data-stu-id="a77c5-161">Impacted audience</span></span>

<span data-ttu-id="a77c5-162">Administradores delegados que acedem ao Exchange através do Partner Center</span><span class="sxs-lookup"><span data-stu-id="a77c5-162">Delegated admins accessing Exchange through Partner Center</span></span>

### <a name="details"></a><span data-ttu-id="a77c5-163">Detalhes</span><span class="sxs-lookup"><span data-stu-id="a77c5-163">Details</span></span>

<span data-ttu-id="a77c5-164">A partir de 27 de abril de 2021, os parceiros que navegarem para o Exchange através do Partner Center serão redirecionados para o novo EAC.</span><span class="sxs-lookup"><span data-stu-id="a77c5-164">Starting April 27, 2021, partners who navigate to Exchange through Partner Center will be redirected to the new EAC.</span></span>

<span data-ttu-id="a77c5-165">Esta nova experiência está atualmente disponível como pré-visualização, e os administradores podem ativar esta experiência selecionando o toggle no canto superior direito dentro do clássico EAC.</span><span class="sxs-lookup"><span data-stu-id="a77c5-165">This new experience is currently available as a preview, and admins can activate this experience by selecting the toggle on the top right corner within the classic EAC.</span></span> <span data-ttu-id="a77c5-166">Também podem navegar para o novo EAC selecionando o banner "Experimente agora" que é exibido em todas as páginas.</span><span class="sxs-lookup"><span data-stu-id="a77c5-166">They can also navigate to the new EAC by selecting the “Try it now” banner that’s displayed on all the pages.</span></span>

<span data-ttu-id="a77c5-167">Os benefícios do novo CEA incluem:</span><span class="sxs-lookup"><span data-stu-id="a77c5-167">Benefits of the new EAC include:</span></span>

- <span data-ttu-id="a77c5-168">Informações adicionadas, relatórios e mecanismos de alerta para problemas relacionados com o fluxo de correio.</span><span class="sxs-lookup"><span data-stu-id="a77c5-168">Added insights, reports, and alert mechanisms for mail flow–related issues.</span></span> 

- <span data-ttu-id="a77c5-169">Dashboards personalizados para aumentar a produtividade.</span><span class="sxs-lookup"><span data-stu-id="a77c5-169">Personalized dashboards to increase productivity.</span></span>

<span data-ttu-id="a77c5-170">Para ajudá-lo a navegar através da nova experiência, os vídeos estão disponíveis na secção **Guia de & formação** sobre a nova experiência EAC.</span><span class="sxs-lookup"><span data-stu-id="a77c5-170">To help you navigate through the new experience, videos are available within the **Training & Guide** section on the new EAC experience.</span></span> <span data-ttu-id="a77c5-171">Estes dar-lhe-ão uma visão geral de como pode utilizar melhor o novo portal.</span><span class="sxs-lookup"><span data-stu-id="a77c5-171">These will give you an overview of how you can best use the new portal.</span></span>

>[!NOTE]
><span data-ttu-id="a77c5-172">Com esta mudança, a experiência clássica da EAC não será depreciada.</span><span class="sxs-lookup"><span data-stu-id="a77c5-172">With this change, the classic EAC experience will not be deprecated.</span></span> <span data-ttu-id="a77c5-173">Será notificado com muita antecedência antes de qualquer alteração ser implementada.</span><span class="sxs-lookup"><span data-stu-id="a77c5-173">You will be notified well in advance before any change is implemented.</span></span>

### <a name="next-steps"></a><span data-ttu-id="a77c5-174">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="a77c5-174">Next steps</span></span>

- <span data-ttu-id="a77c5-175">Confira os [recursos sobre este tema,](https://partner.microsoft.com/resources/collection/new-exchange-admin-center-experience#/)onde pode ver imagens da nova experiência.</span><span class="sxs-lookup"><span data-stu-id="a77c5-175">Check out the [resources about this topic](https://partner.microsoft.com/resources/collection/new-exchange-admin-center-experience#/), where you can view screenshots of the new experience.</span></span>

- <span data-ttu-id="a77c5-176">Partilhe esta informação com as partes interessadas apropriadas na sua organização.</span><span class="sxs-lookup"><span data-stu-id="a77c5-176">Share this information with the appropriate stakeholders in your organization.</span></span> 

### <a name="questions"></a><span data-ttu-id="a77c5-177">Perguntas?</span><span class="sxs-lookup"><span data-stu-id="a77c5-177">Questions?</span></span>

<span data-ttu-id="a77c5-178">Para quaisquer questões sobre estas alterações, consulte as suas comunidades Yammer relevantes.</span><span class="sxs-lookup"><span data-stu-id="a77c5-178">For any questions about these changes, check your relevant Yammer communities.</span></span>

________________
## <a name="microsoft-operations-introducing-the-product-launch-calendar"></a><a name="16"></a><span data-ttu-id="a77c5-179">Microsoft Operations: Introdução do calendário de lançamento do produto</span><span class="sxs-lookup"><span data-stu-id="a77c5-179">Microsoft Operations: Introducing the product launch calendar</span></span>

### <a name="categories"></a><span data-ttu-id="a77c5-180">Categorias</span><span class="sxs-lookup"><span data-stu-id="a77c5-180">Categories</span></span>

- <span data-ttu-id="a77c5-181">Data: 2021-03-25</span><span class="sxs-lookup"><span data-stu-id="a77c5-181">Date: 2021-03-25</span></span>
- <span data-ttu-id="a77c5-182">Ofertas | Local de trabalho moderno</span><span class="sxs-lookup"><span data-stu-id="a77c5-182">Offers | Modern Workplace</span></span>

### <a name="summary"></a><span data-ttu-id="a77c5-183">Resumo</span><span class="sxs-lookup"><span data-stu-id="a77c5-183">Summary</span></span>

<span data-ttu-id="a77c5-184">Em resposta ao feedback dos parceiros, a Microsoft Operations irá agilizar as comunicações para lançamentos de produtos.</span><span class="sxs-lookup"><span data-stu-id="a77c5-184">In response to partner feedback, Microsoft Operations will streamline communications for product launches.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="a77c5-185">Audiência impactada</span><span class="sxs-lookup"><span data-stu-id="a77c5-185">Impacted audience</span></span>

<span data-ttu-id="a77c5-186">Parceiros do Cloud Solution Provider (CSP)</span><span class="sxs-lookup"><span data-stu-id="a77c5-186">Cloud Solution Provider (CSP) partners</span></span>

### <a name="details"></a><span data-ttu-id="a77c5-187">Detalhes</span><span class="sxs-lookup"><span data-stu-id="a77c5-187">Details</span></span>

<span data-ttu-id="a77c5-188">A Microsoft está empenhada em melhorar continuamente as experiências dos parceiros.</span><span class="sxs-lookup"><span data-stu-id="a77c5-188">Microsoft is committed to continually improving partner experiences.</span></span> <span data-ttu-id="a77c5-189">Recebemos comentários seus de que tem recebido demasiadas comunicações da Microsoft, incluindo anúncios duplicados para lançamentos de produtos.</span><span class="sxs-lookup"><span data-stu-id="a77c5-189">We’ve had feedback from you that you’ve been receiving too many communications from Microsoft, including duplicate announcements for product launches.</span></span>

<span data-ttu-id="a77c5-190">Em resposta ao seu feedback, a Microsoft dinamizou a experiência de prontidão para lançamentos de produtos para novas ofertas existentes.</span><span class="sxs-lookup"><span data-stu-id="a77c5-190">In response to your feedback, Microsoft has streamlined the readiness experience for product launches for new and existing offers.</span></span>

<span data-ttu-id="a77c5-191">Disponibilizamos-lhe agora uma única visão mensal dos lançamentos de produtos, publicada na galeria de recursos de prontidão operações.</span><span class="sxs-lookup"><span data-stu-id="a77c5-191">We now provide you with a single monthly view of product launches, published in the Operations readiness resource gallery.</span></span> <span data-ttu-id="a77c5-192">Esta [visão](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) mensal do calendário de lançamento do produto substituirá as comunicações individuais de lançamento de produtos na galeria de recursos de prontidão de Operações e nos anúncios do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="a77c5-192">This monthly [product launch calendar view](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) will replace individual product launch communications in the Operations readiness resource gallery and in Partner Center announcements.</span></span>

<span data-ttu-id="a77c5-193">Você também pode acessá-lo calendário de [lançamento](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) de produtos a partir de [coleções comunitárias, vistas](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) [de calendário](https://partner.microsoft.com/resources/assets#/?type=collection&search=Calendar&sort=updated)e [newsletters CSP.](https://partner.microsoft.com/resources/collection/csp-monthly-update#/)</span><span class="sxs-lookup"><span data-stu-id="a77c5-193">You can also access this [product launch calendar](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) from [community collections](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/), [calendar views](https://partner.microsoft.com/resources/assets#/?type=collection&search=Calendar&sort=updated), and [CSP newsletters](https://partner.microsoft.com/resources/collection/csp-monthly-update#/).</span></span> <span data-ttu-id="a77c5-194">Iremos notificá-lo quando publicarmos o calendário de lançamento de produtos de cada mês com um anúncio na galeria de recursos de prontidão opera.</span><span class="sxs-lookup"><span data-stu-id="a77c5-194">We’ll notify you when we publish each month’s product launch calendar with an announcement in the Operations readiness resource gallery.</span></span>

<span data-ttu-id="a77c5-195">Você ainda pode encontrar informações sobre ofertas novas e existentes na lista de preços pré-visualização e registos de alteração de lista de preços, bem como em blogs de produtos, guias de licenciamento e páginas de marketing de produtos.</span><span class="sxs-lookup"><span data-stu-id="a77c5-195">You can still find information regarding new and existing offers in the price list preview and price list change logs, as well as in product blogs, licensing guides, and product marketing pages.</span></span>

<span data-ttu-id="a77c5-196">A alteração aplicar-se-á aos lançamentos para os seguintes produtos:</span><span class="sxs-lookup"><span data-stu-id="a77c5-196">The change will apply to launches for the following products:</span></span>

- <span data-ttu-id="a77c5-197">Dinâmica no local</span><span class="sxs-lookup"><span data-stu-id="a77c5-197">Dynamics on-premises</span></span>
- <span data-ttu-id="a77c5-198">Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="a77c5-198">Microsoft 365</span></span>
- <span data-ttu-id="a77c5-199">Microsoft Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="a77c5-199">Microsoft Dynamics 365</span></span>
- <span data-ttu-id="a77c5-200">Windows</span><span class="sxs-lookup"><span data-stu-id="a77c5-200">Windows</span></span>
- <span data-ttu-id="a77c5-201">Servidor</span><span class="sxs-lookup"><span data-stu-id="a77c5-201">Server</span></span>  
- <span data-ttu-id="a77c5-202">Ferramentas</span><span class="sxs-lookup"><span data-stu-id="a77c5-202">Tools</span></span>
- <span data-ttu-id="a77c5-203">Equipas e Telco</span><span class="sxs-lookup"><span data-stu-id="a77c5-203">Teams and Telco</span></span>

<span data-ttu-id="a77c5-204">Continuaremos a enviar anúncios específicos para lançamentos de produtos que requerem detalhes de prontidão das operações.</span><span class="sxs-lookup"><span data-stu-id="a77c5-204">We’ll continue to send specific announcements for product launches that require Operations readiness details.</span></span>

### <a name="next-steps"></a><span data-ttu-id="a77c5-205">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="a77c5-205">Next steps</span></span>

<span data-ttu-id="a77c5-206">Reveja os recursos sobre este tema e partilhe esta informação com as partes interessadas apropriadas na sua organização.</span><span class="sxs-lookup"><span data-stu-id="a77c5-206">Review the resources about this topic and share this information with the appropriate stakeholders in your organization.</span></span>

### <a name="questions"></a><span data-ttu-id="a77c5-207">Perguntas?</span><span class="sxs-lookup"><span data-stu-id="a77c5-207">Questions?</span></span>

<span data-ttu-id="a77c5-208">Para mais perguntas sobre estas ofertas, consulte as suas comunidades Yammer relevantes.</span><span class="sxs-lookup"><span data-stu-id="a77c5-208">For any further questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="changes-to-csp-customer-onboarding-requirements"></a><a name="15"></a><span data-ttu-id="a77c5-209">Alterações aos requisitos de embarque do cliente CSP</span><span class="sxs-lookup"><span data-stu-id="a77c5-209">Changes to CSP customer onboarding requirements</span></span>

### <a name="categories"></a><span data-ttu-id="a77c5-210">Categorias</span><span class="sxs-lookup"><span data-stu-id="a77c5-210">Categories</span></span>

- <span data-ttu-id="a77c5-211">Data: 2021-03-25</span><span class="sxs-lookup"><span data-stu-id="a77c5-211">Date: 2021-03-25</span></span>
- <span data-ttu-id="a77c5-212">Capacidades</span><span class="sxs-lookup"><span data-stu-id="a77c5-212">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="a77c5-213">Resumo</span><span class="sxs-lookup"><span data-stu-id="a77c5-213">Summary</span></span>

<span data-ttu-id="a77c5-214">Como parte do nosso compromisso de ajudar parceiros e clientes a gerir o seu negócio com base na confiança, vamos solicitar informações adicionais ao cliente, a partir de 25 de março de 2021.</span><span class="sxs-lookup"><span data-stu-id="a77c5-214">As part of our commitment to help partners and customers run their business based on trust, we will request additional customer information, effective March 25, 2021.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="a77c5-215">Audiência impactada</span><span class="sxs-lookup"><span data-stu-id="a77c5-215">Impacted audience</span></span>

<span data-ttu-id="a77c5-216">Cloud Solution Provider (CSP) parceiros de conta direta e fornecedores indiretos que têm clientes novos ou existentes nos países listados na secção seguinte</span><span class="sxs-lookup"><span data-stu-id="a77c5-216">Cloud Solution Provider (CSP) direct bill partners and indirect providers who have new or existing customers in the countries listed in the next section</span></span>

### <a name="details"></a><span data-ttu-id="a77c5-217">Detalhes</span><span class="sxs-lookup"><span data-stu-id="a77c5-217">Details</span></span>

<span data-ttu-id="a77c5-218">A Microsoft tem confiança.</span><span class="sxs-lookup"><span data-stu-id="a77c5-218">Microsoft runs on trust.</span></span> <span data-ttu-id="a77c5-219">Estamos empenhados em fornecer um método de validação de clientes conforme, seguro e seguro para a transação de subscrições de clientes no programa CSP.</span><span class="sxs-lookup"><span data-stu-id="a77c5-219">We’re committed to providing a compliant, safe, and secure method of customer validation for transacting customer subscriptions in the CSP program.</span></span> <span data-ttu-id="a77c5-220">No dia 25 de março de 2021, apresentaremos melhorias no Partner Center API e na interface de utilizador (UI) que afetarão os parceiros que cumprem ambos os seguintes critérios:</span><span class="sxs-lookup"><span data-stu-id="a77c5-220">On March 25, 2021, we will be introducing Partner Center API and user interface (UI) enhancements that will affect partners who meet both of the following criteria:</span></span>

1. <span data-ttu-id="a77c5-221">O parceiro tem uma relação de faturação direta com a Microsoft (o que significa que o parceiro é ou um parceiro de conta direta ou um fornecedor indireto).</span><span class="sxs-lookup"><span data-stu-id="a77c5-221">The partner has a direct billing relationship with Microsoft (which means that the partner is either a direct bill partner or an indirect provider).</span></span>

2. <span data-ttu-id="a77c5-222">O parceiro negoceia com clientes novos ou existentes nos seguintes países:</span><span class="sxs-lookup"><span data-stu-id="a77c5-222">The partner does business with new or existing customers in the following countries:</span></span>

    - <span data-ttu-id="a77c5-223">Tailândia</span><span class="sxs-lookup"><span data-stu-id="a77c5-223">Thailand</span></span>
    - <span data-ttu-id="a77c5-224">Vietname</span><span class="sxs-lookup"><span data-stu-id="a77c5-224">Vietnam</span></span>
    - <span data-ttu-id="a77c5-225">Turquia</span><span class="sxs-lookup"><span data-stu-id="a77c5-225">Turkey</span></span>
    - <span data-ttu-id="a77c5-226">Polónia</span><span class="sxs-lookup"><span data-stu-id="a77c5-226">Poland</span></span>
    - <span data-ttu-id="a77c5-227">África do Sul</span><span class="sxs-lookup"><span data-stu-id="a77c5-227">South Africa</span></span>
    - <span data-ttu-id="a77c5-228">Índia</span><span class="sxs-lookup"><span data-stu-id="a77c5-228">India</span></span>
    - <span data-ttu-id="a77c5-229">Brasil</span><span class="sxs-lookup"><span data-stu-id="a77c5-229">Brazil</span></span>
    - <span data-ttu-id="a77c5-230">Iraque</span><span class="sxs-lookup"><span data-stu-id="a77c5-230">Iraq</span></span>
    - <span data-ttu-id="a77c5-231">Mianmar</span><span class="sxs-lookup"><span data-stu-id="a77c5-231">Myanmar</span></span>
    - <span data-ttu-id="a77c5-232">Sudão do Sul</span><span class="sxs-lookup"><span data-stu-id="a77c5-232">South Sudan</span></span>
    - <span data-ttu-id="a77c5-233">Arábia Saudita</span><span class="sxs-lookup"><span data-stu-id="a77c5-233">Saudi Arabia</span></span>
    - <span data-ttu-id="a77c5-234">Emirados Árabes Unidos</span><span class="sxs-lookup"><span data-stu-id="a77c5-234">United Arab Emirates</span></span>
    - <span data-ttu-id="a77c5-235">Venezuela</span><span class="sxs-lookup"><span data-stu-id="a77c5-235">Venezuela</span></span>

<span data-ttu-id="a77c5-236">Os parceiros que satisfaçam os critérios terão de submeter o **ID** de registo da empresa de um cliente (também conhecido como organização do cliente **INN)** e o número de **telefone** quando estiverem a bordo de novos clientes ou modificar os dados do cliente existentes.</span><span class="sxs-lookup"><span data-stu-id="a77c5-236">Partners who meet the criteria will have to submit a customer's **company registration ID** (also known as the customer's **organization INN**) and **phone number** when they onboard new customers or modify existing customer details.</span></span> <span data-ttu-id="a77c5-237">Estes parceiros também podem introduzir um **nome do meio** opcional para o cliente.</span><span class="sxs-lookup"><span data-stu-id="a77c5-237">These partners can also enter an optional **middle name** for the customer.</span></span>

<span data-ttu-id="a77c5-238">Note que quando adicionar o ID de registo da sua empresa deve usar o seu ID de imposto de negócio e não o ID pessoal do cliente.</span><span class="sxs-lookup"><span data-stu-id="a77c5-238">Note that when you add your company registration ID you should use your business tax ID and not the customer personal ID.</span></span>

<span data-ttu-id="a77c5-239">Os parceiros que fazem negócios com clientes novos ou já existentes nos seguintes países já foram a bordo com um lançamento anterior em novembro de 2020.</span><span class="sxs-lookup"><span data-stu-id="a77c5-239">Partners who do business with new or existing customers in the following countries have already been onboarded with a previous release in November 2020.</span></span>

- <span data-ttu-id="a77c5-240">Arménia</span><span class="sxs-lookup"><span data-stu-id="a77c5-240">Armenia</span></span>
- <span data-ttu-id="a77c5-241">Azerbaijão</span><span class="sxs-lookup"><span data-stu-id="a77c5-241">Azerbaijan</span></span>
- <span data-ttu-id="a77c5-242">Bielorrússia</span><span class="sxs-lookup"><span data-stu-id="a77c5-242">Belarus</span></span>
- <span data-ttu-id="a77c5-243">Hungria</span><span class="sxs-lookup"><span data-stu-id="a77c5-243">Hungary</span></span>
- <span data-ttu-id="a77c5-244">Cazaquistão</span><span class="sxs-lookup"><span data-stu-id="a77c5-244">Kazakhstan</span></span>
- <span data-ttu-id="a77c5-245">Quirguistão</span><span class="sxs-lookup"><span data-stu-id="a77c5-245">Kyrgyzstan</span></span>
- <span data-ttu-id="a77c5-246">Moldávia</span><span class="sxs-lookup"><span data-stu-id="a77c5-246">Moldova</span></span>
- <span data-ttu-id="a77c5-247">Rússia</span><span class="sxs-lookup"><span data-stu-id="a77c5-247">Russia</span></span>
- <span data-ttu-id="a77c5-248">Tajiquistão</span><span class="sxs-lookup"><span data-stu-id="a77c5-248">Tajikistan</span></span>
- <span data-ttu-id="a77c5-249">Ucrânia</span><span class="sxs-lookup"><span data-stu-id="a77c5-249">Ukraine</span></span>
- <span data-ttu-id="a77c5-250">Usbequistão</span><span class="sxs-lookup"><span data-stu-id="a77c5-250">Uzbekistan</span></span>

<span data-ttu-id="a77c5-251">Os parceiros com clientes no resto do mundo terão a capacidade, no dia 25 de março de 2021, de introduzir o ID de registo da **empresa,** **número de telefone** e nome do **meio** para os clientes como detalhes opcionais.</span><span class="sxs-lookup"><span data-stu-id="a77c5-251">Partners with customers in the rest of the world will have the ability on March 25, 2021 to enter the **company registration ID**, **phone number**, and **middle name** for customers as optional details.</span></span>

### <a name="next-steps"></a><span data-ttu-id="a77c5-252">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="a77c5-252">Next steps</span></span>

- <span data-ttu-id="a77c5-253">Reveja a documentação técnica e questione frequentemente na [coleção de parceiros dedicados](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) para obter uma orientação mais detalhada.</span><span class="sxs-lookup"><span data-stu-id="a77c5-253">Review the technical documentation and frequently asked questions in the [dedicated partner collection](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) for more detailed guidance.</span></span>

- <span data-ttu-id="a77c5-254">Prepare-se para incorporar as alterações utilizando a API do Partner Center e a experiência do utilizador web.</span><span class="sxs-lookup"><span data-stu-id="a77c5-254">Prepare to incorporate the changes using the Partner Center API and web user experience.</span></span> <span data-ttu-id="a77c5-255">A API/SDKs estará disponível para testes.</span><span class="sxs-lookup"><span data-stu-id="a77c5-255">API/SDKs will be available for testing.</span></span>

- <span data-ttu-id="a77c5-256">Certifique-se de submeter os dados adicionais ao embarcar em novos clientes ou modificar os dados do cliente existentes.</span><span class="sxs-lookup"><span data-stu-id="a77c5-256">Make sure to submit the additional data when onboarding new customers or modifying existing customer details.</span></span>

- <span data-ttu-id="a77c5-257">Se estiver a utilizar uma solução de fornecedor de painéis de controlo (CPV), consulte o seu CPV.</span><span class="sxs-lookup"><span data-stu-id="a77c5-257">If you’re using a control panel vendor (CPV) solution, consult your CPV.</span></span>

### <a name="questions"></a><span data-ttu-id="a77c5-258">Perguntas?</span><span class="sxs-lookup"><span data-stu-id="a77c5-258">Questions?</span></span>

<span data-ttu-id="a77c5-259">Contacte o seu consultor fiscal ou o fisco local se tiver alguma questão relacionada com o identificador legal (também chamado INN ou TIN).</span><span class="sxs-lookup"><span data-stu-id="a77c5-259">Contact your tax advisor or local tax office if you have any questions related to the legal identifier (also called INN or TIN).</span></span> <span data-ttu-id="a77c5-260">A Microsoft não pode fornecer orientações sobre questões fiscais.</span><span class="sxs-lookup"><span data-stu-id="a77c5-260">Microsoft cannot provide guidance on tax matters.</span></span>

<span data-ttu-id="a77c5-261">Se precisar de apoio nas suas operações com a Microsoft, [abra um pedido de serviço](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span><span class="sxs-lookup"><span data-stu-id="a77c5-261">If you need support in your operations with Microsoft, [open a service request](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span></span>

________________
## <a name="corrections-made-to-march-1-2021-perpetual-software-price-list"></a><a name="14"></a><span data-ttu-id="a77c5-262">Correções feitas até 1 de março de 2021 lista de preços perpétuos de software</span><span class="sxs-lookup"><span data-stu-id="a77c5-262">Corrections made to March 1, 2021 perpetual software price list</span></span>

### <a name="categories"></a><span data-ttu-id="a77c5-263">Categorias</span><span class="sxs-lookup"><span data-stu-id="a77c5-263">Categories</span></span>

- <span data-ttu-id="a77c5-264">Data: 2021-03-23</span><span class="sxs-lookup"><span data-stu-id="a77c5-264">Date: 2021-03-23</span></span>
- <span data-ttu-id="a77c5-265">Ofertas/Mercados</span><span class="sxs-lookup"><span data-stu-id="a77c5-265">Offers/Markets</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="a77c5-266">Audiência impactada</span><span class="sxs-lookup"><span data-stu-id="a77c5-266">Impacted audience</span></span>

<span data-ttu-id="a77c5-267">Fornecedores indiretos e parceiros de conta direto que transfiram software perpétuo no programa Cloud Solution Provider</span><span class="sxs-lookup"><span data-stu-id="a77c5-267">Indirect providers and direct bill partners transacting perpetual software in the Cloud Solution Provider program</span></span> 

### <a name="details"></a><span data-ttu-id="a77c5-268">Detalhes</span><span class="sxs-lookup"><span data-stu-id="a77c5-268">Details</span></span>

<span data-ttu-id="a77c5-269">A lista de preços do software perpétuo publicada a 1 de março de 2021 incluía mercados que não deveriam ter estado lá.</span><span class="sxs-lookup"><span data-stu-id="a77c5-269">The price list for perpetual software posted on March 1, 2021 included markets that should not have been there.</span></span> <span data-ttu-id="a77c5-270">A lista de preços perpétuos de software foi atualizada em 17 de março de 2021 com as correções.</span><span class="sxs-lookup"><span data-stu-id="a77c5-270">The perpetual software price list was updated on March 17, 2021 with the corrections.</span></span> <span data-ttu-id="a77c5-271">Estas correções só se aplicavam:</span><span class="sxs-lookup"><span data-stu-id="a77c5-271">These corrections were only applicable to:</span></span>

- <span data-ttu-id="a77c5-272">ID do produto: DF77X4D43RKT</span><span class="sxs-lookup"><span data-stu-id="a77c5-272">Product ID: DF77X4D43RKT</span></span> 
- <span data-ttu-id="a77c5-273">Nome do produto: Windows 10 Home to Pro Upgrade para o Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="a77c5-273">Product name: Windows 10 Home to Pro Upgrade for Microsoft 365 Business</span></span>
- <span data-ttu-id="a77c5-274">Mercados removidos ou não apoiados: AE, AF, AL, AM, AO, BA, BB, BD, BH, BM, BN, BO, BR, BS, BW, BY, BZ, CI, CL, CM, CO, CR, CW, CW, DO, DZ, EC, EG, ET, FJ, FO, GE, GH, GT, HN, IL, IN, IQ, JM, JO, KE, KG, KN, KW, KY, KZ, LB, LK, LY, MA, MC, MD, ME, MN, MN, , NI, NP, OM, PA, PE, PH, PK, PR, PY, QA, RS, RU, RW, SG, SN, SV, TH, TJ, TM, TN, TT, TZ, UA, UG, UY, UZ, VE, VN, YE, ZM, ZW</span><span class="sxs-lookup"><span data-stu-id="a77c5-274">Removed or unsupported markets: AE, AF, AL, AM, AO, BA, BB, BD, BH, BM, BN, BO, BR, BS, BW, BY, BZ, CI, CL, CM, CO, CR, CW, DO, DZ, EC, EG, ET, FJ, FO, GE, GH, GT, HN, IL, IN, IQ, JM, JO, KE, KG, KN, KW, KY, KZ, LB, LK, LY, MA, MC, MD, ME, MN, MO, MU, NA, NG, NI, NP, OM, PA, PE, PH, PK, PR, PY, QA, RS, RU, RW, SG, SN, SV, TH, TJ, TM, TN, TT, TZ, UA, UG, UY, UZ, VE, VN, YE, ZM, ZW</span></span>

<span data-ttu-id="a77c5-275">Estas alterações aplicam-se apenas ao produto acima referido.</span><span class="sxs-lookup"><span data-stu-id="a77c5-275">These changes only apply to the above product.</span></span> <span data-ttu-id="a77c5-276">Outros produtos não tinham correções.</span><span class="sxs-lookup"><span data-stu-id="a77c5-276">Other products had no corrections.</span></span> 

### <a name="next-steps-and-resources"></a><span data-ttu-id="a77c5-277">Próximos passos e recursos</span><span class="sxs-lookup"><span data-stu-id="a77c5-277">Next steps and resources</span></span>

- <span data-ttu-id="a77c5-278">Os parceiros que transacionam software perpétuo devem descarregar a mais recente lista de preços perpétuos de software.</span><span class="sxs-lookup"><span data-stu-id="a77c5-278">Partners who transact perpetual software should download the latest perpetual software price list.</span></span>
- <span data-ttu-id="a77c5-279">Consulte os [códigos dos países](https://docs.microsoft.com/azure/marketplace/commercial-marketplace-co-sell-countries) da região para um mapeamento amigável da abreviatura de duas letras para os países.</span><span class="sxs-lookup"><span data-stu-id="a77c5-279">Consult the [region country codes](https://docs.microsoft.com/azure/marketplace/commercial-marketplace-co-sell-countries) for a friendly mapping of the two letter abbreviation to countries.</span></span>
________________
## <a name="sdk-release-on-net-standard-v1170"></a><a name="13"></a> <span data-ttu-id="a77c5-280">Lançamento SDK em .NET Standard (v1.17.0)</span><span class="sxs-lookup"><span data-stu-id="a77c5-280">SDK Release on .NET Standard (v1.17.0)</span></span>

### <a name="categories"></a><span data-ttu-id="a77c5-281">Categorias</span><span class="sxs-lookup"><span data-stu-id="a77c5-281">Categories</span></span>

- <span data-ttu-id="a77c5-282">Data: 2021-03-23</span><span class="sxs-lookup"><span data-stu-id="a77c5-282">Date: 2021-03-23</span></span>

- <span data-ttu-id="a77c5-283">Capacidades</span><span class="sxs-lookup"><span data-stu-id="a77c5-283">Capabilities</span></span>
 
### <a name="impacted-audience"></a><span data-ttu-id="a77c5-284">Audiência impactada</span><span class="sxs-lookup"><span data-stu-id="a77c5-284">Impacted audience</span></span>

<span data-ttu-id="a77c5-285">Parceiros Direct Bill e Fornecedores Indiretos que participam no programa CSP que estão a utilizar o Partner Center .NET SDK.</span><span class="sxs-lookup"><span data-stu-id="a77c5-285">Direct Bill partners and Indirect Providers participating in the CSP program who are using the Partner Center .NET SDK.</span></span>

### <a name="details"></a><span data-ttu-id="a77c5-286">Detalhes</span><span class="sxs-lookup"><span data-stu-id="a77c5-286">Details</span></span>

<span data-ttu-id="a77c5-287">A partir de 23 de março de 2020, os Parceiros podem começar a descarregar a versão do [MicrosoftPartnerCenter.NETSDK (NuGet Gallery | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0), juntamente com [amostras atualizadas](https://github.com/Microsoft/Partner-Center-DotNet-Samples)do Centro De Parceiros Públicos SDK GitHub .</span><span class="sxs-lookup"><span data-stu-id="a77c5-287">As of March 23 2020, Partners can start downloading the version of [MicrosoftPartnerCenter.NETSDK (NuGet Gallery | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0), along with updated public Partner Center SDK [GitHub samples](https://github.com/Microsoft/Partner-Center-DotNet-Samples).</span></span> <span data-ttu-id="a77c5-288">Esta versão inclui atualizações aos seguintes métodos:</span><span class="sxs-lookup"><span data-stu-id="a77c5-288">This version includes updates to the following methods:</span></span>

#### <a name="audit-updated-new-operation-types"></a><span data-ttu-id="a77c5-289">Auditoria Atualizada: Novos tipos de operação</span><span class="sxs-lookup"><span data-stu-id="a77c5-289">Audit Updated: New operation types</span></span>

<span data-ttu-id="a77c5-290">Adicione novos [tipos de operação](https://docs.microsoft.com/partner-center/develop/auditing-resources) para saber quando o cliente aprovou e encerrou o DAP.</span><span class="sxs-lookup"><span data-stu-id="a77c5-290">Added new [operation types](https://docs.microsoft.com/partner-center/develop/auditing-resources) for knowing when the customer approved and terminated DAP.</span></span>

- <span data-ttu-id="a77c5-291">DapAdminRelationshipApproved</span><span class="sxs-lookup"><span data-stu-id="a77c5-291">DapAdminRelationshipApproved</span></span>

- <span data-ttu-id="a77c5-292">DapAdminRelationshipTerminated</span><span class="sxs-lookup"><span data-stu-id="a77c5-292">DapAdminRelationshipTerminated</span></span>

#### <a name="audit-updated-new-resource-and-operation-types"></a><span data-ttu-id="a77c5-293">Auditoria Atualizada: Novos tipos de recursos e de operação</span><span class="sxs-lookup"><span data-stu-id="a77c5-293">Audit Updated: New resource and operation types</span></span>

<span data-ttu-id="a77c5-294">Adicionou novos [tipos de recursos e de operação](https://docs.microsoft.com/partner-center/develop/auditing-resources) para apoiar o cenário de função do diretório do cliente.</span><span class="sxs-lookup"><span data-stu-id="a77c5-294">Added new [resource and operation types](https://docs.microsoft.com/partner-center/develop/auditing-resources) for supporting the customer directory role scenario.</span></span>

- <span data-ttu-id="a77c5-295">Novo tipo de recurso "CustomerDirectoryRole"</span><span class="sxs-lookup"><span data-stu-id="a77c5-295">New resource type “CustomerDirectoryRole”</span></span>

- <span data-ttu-id="a77c5-296">Tipos de operação "AddUserMember" e "RemoveUserMember"</span><span class="sxs-lookup"><span data-stu-id="a77c5-296">Operation types “AddUserMember” and “RemoveUserMember”</span></span>

#### <a name="sdk-updates-to-customer-accounts"></a><span data-ttu-id="a77c5-297">Atualizações SDK para contas de clientes</span><span class="sxs-lookup"><span data-stu-id="a77c5-297">SDK Updates to customer accounts</span></span>

- <span data-ttu-id="a77c5-298">Suporte para GET /clientes/{customer-tenant-id}/directSignedMicrosoftCustomerAgreementStatus</span><span class="sxs-lookup"><span data-stu-id="a77c5-298">Support for GET /customers/{customer-tenant-id}/directSignedMicrosoftCustomerAgreementStatus</span></span>

- <span data-ttu-id="a77c5-299">GET /clientes/{cliente-inquilino-id}/qualificações</span><span class="sxs-lookup"><span data-stu-id="a77c5-299">GET /customers/{customer-tenant-id}/qualifications</span></span>

- <span data-ttu-id="a77c5-300">POST /clientes/{customer_id}/qualificações?código={validação Código}</span><span class="sxs-lookup"><span data-stu-id="a77c5-300">POST /customers/{customer_id}/qualifications?code={validationCode}</span></span>

#### <a name="additional-changes"></a><span data-ttu-id="a77c5-301">Alterações adicionais</span><span class="sxs-lookup"><span data-stu-id="a77c5-301">Additional changes</span></span>

<span data-ttu-id="a77c5-302">As seguintes alterações são introduzidas como parte do Novo Comércio, e estão atualmente disponíveis apenas por convite para parceiros que fazem parte da experiência técnica M365/D365 New Commerce.</span><span class="sxs-lookup"><span data-stu-id="a77c5-302">The following changes are introduced as part of New Commerce, and are currently available by invitation only to partners who are part of the M365/D365 New Commerce experience technical preview.</span></span> <span data-ttu-id="a77c5-303">Os parceiros que não fazem parte da pré-visualização técnica do Novo Comércio não devem notar impactos e devem ser compatíveis com retroparos.</span><span class="sxs-lookup"><span data-stu-id="a77c5-303">Partners who are not part of the New Commerce technical preview should not notice impacts and should be backward compatible.</span></span>

- <span data-ttu-id="a77c5-304">Alterações no catálogo:</span><span class="sxs-lookup"><span data-stu-id="a77c5-304">Catalog Changes:</span></span>

  - <span data-ttu-id="a77c5-305">GET /products/{product-id}/skus/{sku-id}</span><span class="sxs-lookup"><span data-stu-id="a77c5-305">GET /products/{product-id}/skus/{sku-id}</span></span>

- <span data-ttu-id="a77c5-306">Compra e Gestão:</span><span class="sxs-lookup"><span data-stu-id="a77c5-306">Purchase and Manage:</span></span>
  - <span data-ttu-id="a77c5-307">GET /clientes/{clienteId}/subscrições</span><span class="sxs-lookup"><span data-stu-id="a77c5-307">GET /customers/{customerId}/subscriptions</span></span>
  - <span data-ttu-id="a77c5-308">GET /clientes/{customerId}/subscrições/{subscriçãoD}</span><span class="sxs-lookup"><span data-stu-id="a77c5-308">GET /customers/{customerId}/subscriptions/{subscriptionId}</span></span>
  - <span data-ttu-id="a77c5-309">PATCH /clientes/{customerId}/subscrições/{subscriçãoD}</span><span class="sxs-lookup"><span data-stu-id="a77c5-309">PATCH /customers/{customerId}/subscriptions/{subscriptionId}</span></span>
  - <span data-ttu-id="a77c5-310">GET /clientes/{customerId}/subscrições/{subscriçãoD}/transitioneligibilities</span><span class="sxs-lookup"><span data-stu-id="a77c5-310">GET /customers/{customerId}/subscriptions/{subscriptionId}/transitioneligibilities</span></span>
  - <span data-ttu-id="a77c5-311">GET /clientes/{customerId}/subscrições/{subscriçãoId}/transições</span><span class="sxs-lookup"><span data-stu-id="a77c5-311">GET /customers/{customerId}/subscriptions/{subscriptionId}/transitions</span></span>
  - <span data-ttu-id="a77c5-312">POST /clientes/{customerId}/subscrições/{subscriçãoD}/transições</span><span class="sxs-lookup"><span data-stu-id="a77c5-312">POST /customers/{customerId}/subscriptions/{subscriptionId}/transitions</span></span>

### <a name="next-steps"></a><span data-ttu-id="a77c5-313">Passos Seguintes</span><span class="sxs-lookup"><span data-stu-id="a77c5-313">Next Steps</span></span>

- <span data-ttu-id="a77c5-314">Descarregue a versão mais recente [do MicrosoftPartnerCenter.NETSDK (NuGet Gallery | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0)</span><span class="sxs-lookup"><span data-stu-id="a77c5-314">Download the latest version [MicrosoftPartnerCenter.NETSDK (NuGet Gallery | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0)</span></span>
- <span data-ttu-id="a77c5-315">Faça o download e reveja as amostras do [GitHub](https://github.com/Microsoft/Partner-Center-DotNet-Samples)</span><span class="sxs-lookup"><span data-stu-id="a77c5-315">Download and review the [GitHub samples](https://github.com/Microsoft/Partner-Center-DotNet-Samples)</span></span>

________________
## <a name="csp-commercial-marketplace-offer-and-fy21-csp-incentives-for-eligible-offers"></a><a name="12"></a><span data-ttu-id="a77c5-316">Oferta de mercado comercial da CSP e incentivos ao CDS para ofertas elegíveis</span><span class="sxs-lookup"><span data-stu-id="a77c5-316">CSP commercial marketplace offer and FY21 CSP incentives for eligible offers</span></span>

### <a name="categories"></a><span data-ttu-id="a77c5-317">Categorias</span><span class="sxs-lookup"><span data-stu-id="a77c5-317">Categories</span></span>

- <span data-ttu-id="a77c5-318">Data: 2021-03-18</span><span class="sxs-lookup"><span data-stu-id="a77c5-318">Date: 2021-03-18</span></span>
- <span data-ttu-id="a77c5-319">Capacidades</span><span class="sxs-lookup"><span data-stu-id="a77c5-319">Capabilities</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="a77c5-320">Audiência impactada</span><span class="sxs-lookup"><span data-stu-id="a77c5-320">Impacted audience</span></span>

<span data-ttu-id="a77c5-321">Fornecedores indiretos e parceiros de conta direta no programa Cloud Solution Provider</span><span class="sxs-lookup"><span data-stu-id="a77c5-321">Indirect providers and direct bill partners in the Cloud Solution Provider program</span></span> 

### <a name="details"></a><span data-ttu-id="a77c5-322">Detalhes</span><span class="sxs-lookup"><span data-stu-id="a77c5-322">Details</span></span>

<span data-ttu-id="a77c5-323">Os fornecedores indiretos e parceiros de conta direta no programa Cloud Solution Provider podem vender ofertas de terceiros e ganhar um incentivo de desconto para cada oferta de terceiros elegível transacionada no Partner Center ou no portal Azure.</span><span class="sxs-lookup"><span data-stu-id="a77c5-323">Indirect providers and direct bill partners in the Cloud Solution Provider program can sell third party offers and earn a rebate incentive for each eligible third-party offer transacted in Partner Center or the Azure portal.</span></span> <span data-ttu-id="a77c5-324">O incentivo será sob a forma de um desconto nas vendas faturadas para as ofertas elegíveis e está **disponível até 30 de junho de 2021**.</span><span class="sxs-lookup"><span data-stu-id="a77c5-324">The incentive will be in the form of a rebate on billed sales for the eligible offers and is **available until June 30, 2021**.</span></span>  

<span data-ttu-id="a77c5-325">Continue a aprender sobre este incentivo CSP Commercial Marketplace Offer abaixo e contacte os seus clientes hoje para identificar as ofertas certas para permitir o seu sucesso contínuo e transformação digital.</span><span class="sxs-lookup"><span data-stu-id="a77c5-325">Continue learning about this CSP Commercial Marketplace Offer incentive below and contact your customers today to identify the right offers to enable their continued success and digital transformation.</span></span>

<span data-ttu-id="a77c5-326">Fazemos parcerias com fornecedores de software independentes (ISVs) para trazer as mais recentes soluções IaaS e SaaS para o mercado para os clientes da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="a77c5-326">We partner with Independent Software Vendors (ISVs) to bring the latest IaaS and SaaS solutions to market for Microsoft customers.</span></span> <span data-ttu-id="a77c5-327">Os editores da ISV têm a opção de permitir a venda das suas ofertas através do canal parceiro da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="a77c5-327">ISV publishers have the option of enabling sales of their offers through the Microsoft partner channel.</span></span> <span data-ttu-id="a77c5-328">As nossas ofertas elegíveis para incentivos enquadram-se em duas categorias:</span><span class="sxs-lookup"><span data-stu-id="a77c5-328">Our incentive-eligible offers fall into two categories:</span></span>

- <span data-ttu-id="a77c5-329">Selecione ofertas de terceiros SaaS e IaaS com o estado de co-venda do Azure IP.</span><span class="sxs-lookup"><span data-stu-id="a77c5-329">Select SaaS and IaaS third-party offers with Azure IP co-sell incentivized status.</span></span> 

- <span data-ttu-id="a77c5-330">Aplicações SaaS integradas com Equipas ou pelo menos duas aplicações de produtividade Microsoft 365, tais como PowerPoint, Word, Excel, Outlook ou SharePoint.</span><span class="sxs-lookup"><span data-stu-id="a77c5-330">SaaS applications integrated with Teams or at least two Microsoft 365 productivity apps, such as PowerPoint, Word, Excel, Outlook, or SharePoint.</span></span>

### <a name="next-steps-and-resources"></a><span data-ttu-id="a77c5-331">Próximos passos e recursos</span><span class="sxs-lookup"><span data-stu-id="a77c5-331">Next steps and resources</span></span>

- <span data-ttu-id="a77c5-332">Saiba mais sobre o ganho [de Incentivos a Parceiros](https://partner.microsoft.com/membership/partner-incentives) para a venda de aplicações elegíveis para o mercado, as aplicações elegíveis para incentivos.</span><span class="sxs-lookup"><span data-stu-id="a77c5-332">Learn about earning [Partner Incentives](https://partner.microsoft.com/membership/partner-incentives) for selling eligible marketplace apps the incentive eligible apps.</span></span> <span data-ttu-id="a77c5-333">Novas ofertas são adicionadas mensalmente.</span><span class="sxs-lookup"><span data-stu-id="a77c5-333">New offers are added monthly.</span></span>  
- [<span data-ttu-id="a77c5-334">Cloud Solution Provider recursos de incentivo de parceiro de conta direta</span><span class="sxs-lookup"><span data-stu-id="a77c5-334">Cloud Solution Provider direct bill partner incentive resources</span></span>](https://partner.microsoft.com/asset/collection/cloud-solution-provider-direct-partner-incentive-resources#/)
- [<span data-ttu-id="a77c5-335">Recursos de incentivo indiretos do Fornecedor de Soluções Cloud</span><span class="sxs-lookup"><span data-stu-id="a77c5-335">Cloud Solution Provider indirect provider incentive resources</span></span>](https://partner.microsoft.com/asset/collection/cloud-solution-provider-indirect-provider-incentive-resources#/)
- <span data-ttu-id="a77c5-336">Reveja esta [apresentação](https://partner.microsoft.com/resources/detail/partner-center-cm-for-csp-overview-pdf) para saber mais sobre a venda das aplicações de marketplace comercial.</span><span class="sxs-lookup"><span data-stu-id="a77c5-336">Review this [presentation](https://partner.microsoft.com/resources/detail/partner-center-cm-for-csp-overview-pdf) to learn more about selling the commercial marketplace apps.</span></span> <span data-ttu-id="a77c5-337">Confira os recursos adicionais [aqui.](https://partner.microsoft.com/resources/collection/partner-center-cm-for-csp-collection#/)</span><span class="sxs-lookup"><span data-stu-id="a77c5-337">Check out additional resources [here](https://partner.microsoft.com/resources/collection/partner-center-cm-for-csp-collection#/).</span></span> 
- <span data-ttu-id="a77c5-338">Explore o catálogo de marketplace comercial no [Partner Center](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-discover) ou no [portal Azure](https://ms.portal.azure.com/#home)</span><span class="sxs-lookup"><span data-stu-id="a77c5-338">Explore the commercial marketplace catalog in [Partner Center](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-discover) or [Azure portal](https://ms.portal.azure.com/#home)</span></span>
- <span data-ttu-id="a77c5-339">Utilize [APIs](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market) para integrar apps no mercado da sua empresa</span><span class="sxs-lookup"><span data-stu-id="a77c5-339">Use [APIs](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market) to integrate apps into your company’s marketplace</span></span>
- <span data-ttu-id="a77c5-340">Contacte os ISVs com os que está interessado em fazer negócios</span><span class="sxs-lookup"><span data-stu-id="a77c5-340">Reach out to ISVs you are interested in doing business with</span></span>
- <span data-ttu-id="a77c5-341">Os fornecedores indiretos precisam de integrar usando APIs e guiar revendedores em que apps vender</span><span class="sxs-lookup"><span data-stu-id="a77c5-341">Indirect providers need to integrate using APIs and guide resellers on which apps to sell</span></span>

### <a name="questions"></a><span data-ttu-id="a77c5-342">Perguntas?</span><span class="sxs-lookup"><span data-stu-id="a77c5-342">Questions?</span></span>  

<span data-ttu-id="a77c5-343">Consulte [este artigo](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-overview) para obter uma visão geral do mercado comercial no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="a77c5-343">Refer to [this article](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-overview) for an overview of the commercial marketplace in Partner Center.</span></span>

<span data-ttu-id="a77c5-344">Se precisar de assistência adicional, pode criar um pedido de apoio no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="a77c5-344">If you need additional assistance you can create a support request in Partner Center.</span></span> <span data-ttu-id="a77c5-345">Saiba mais em [https://aka.ms/IncentivesSupport](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=1) .</span><span class="sxs-lookup"><span data-stu-id="a77c5-345">Learn more at [https://aka.ms/IncentivesSupport](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=1).</span></span>

________________
## <a name="power-bi-premium-offer-naming-and-prerequisite-update"></a><a name="11"></a><span data-ttu-id="a77c5-346">Power BI Premium oferece nomeação e atualização pré-requisito</span><span class="sxs-lookup"><span data-stu-id="a77c5-346">Power BI Premium offer naming and prerequisite update</span></span>

### <a name="categories"></a><span data-ttu-id="a77c5-347">Categorias</span><span class="sxs-lookup"><span data-stu-id="a77c5-347">Categories</span></span>

- <span data-ttu-id="a77c5-348">Data: 2021-03-18</span><span class="sxs-lookup"><span data-stu-id="a77c5-348">Date: 2021-03-18</span></span>
- <span data-ttu-id="a77c5-349">Capacidades</span><span class="sxs-lookup"><span data-stu-id="a77c5-349">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="a77c5-350">Resumo</span><span class="sxs-lookup"><span data-stu-id="a77c5-350">Summary</span></span>

<span data-ttu-id="a77c5-351">A lista final de preços de 1 de abril de 2021 será atualizada para adicionar clareza ao nome e/ou informação pré-requisito para ofertas de Power BI Premium Per User.</span><span class="sxs-lookup"><span data-stu-id="a77c5-351">The April 1, 2021 final price list will be updated to add clarity to the naming and/or prerequisite information for Power BI Premium Per User offers.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="a77c5-352">Audiência impactada</span><span class="sxs-lookup"><span data-stu-id="a77c5-352">Impacted audience</span></span>

<span data-ttu-id="a77c5-353">Cloud Solution Provider (CSP) parceiros diretos e indiretos</span><span class="sxs-lookup"><span data-stu-id="a77c5-353">Cloud Solution Provider (CSP) direct and indirect partners</span></span>

### <a name="details"></a><span data-ttu-id="a77c5-354">Detalhes</span><span class="sxs-lookup"><span data-stu-id="a77c5-354">Details</span></span>

<span data-ttu-id="a77c5-355">A lista final de preços de 1 de abril de 2021 será atualizada para adicionar clareza ao nome e/ou informação pré-requisito para ofertas de Power BI Premium Per User.</span><span class="sxs-lookup"><span data-stu-id="a77c5-355">The April 1, 2021 final price list will be updated to add clarity to the naming and/or prerequisite information for Power BI Premium Per User offers.</span></span>

<span data-ttu-id="a77c5-356">Até que a lista final de preços seja atualizada, utilize as informações nesta secção para garantir que o produto correto é encomendado.</span><span class="sxs-lookup"><span data-stu-id="a77c5-356">Until the final price list is updated, use the information in this section to ensure that the correct product is ordered.</span></span>

<span data-ttu-id="a77c5-357">Os seguintes detalhes mostram o SKU afetado e os detalhes pré-requisitos.</span><span class="sxs-lookup"><span data-stu-id="a77c5-357">The following details show the affected SKU and prerequisite details.</span></span>

| <span data-ttu-id="a77c5-358">Oferta nome de exibição na pré-visualização da lista de preços de 1 de março</span><span class="sxs-lookup"><span data-stu-id="a77c5-358">Offer display name on March 1 price list preview</span></span> |  <span data-ttu-id="a77c5-359">Nome de exibição de oferta atualizado na lista final de preços de 1 de abril</span><span class="sxs-lookup"><span data-stu-id="a77c5-359">Updated offer display name on April 1 final price list</span></span>| <span data-ttu-id="a77c5-360">ID da oferta</span><span class="sxs-lookup"><span data-stu-id="a77c5-360">Offer ID</span></span> |
| ------ | ----------- | ----------- |
| <span data-ttu-id="a77c5-361">Power BI Premium por utilizador Add-On (Preços de Pessoal sem fins lucrativos)</span><span class="sxs-lookup"><span data-stu-id="a77c5-361">Power BI Premium Per User Add-On (Nonprofit Staff Pricing)</span></span>  |  <span data-ttu-id="a77c5-362">Power BI Premium por utilizador Add-On **(Office)** (Preço do Pessoal sem fins lucrativos)</span><span class="sxs-lookup"><span data-stu-id="a77c5-362">Power BI Premium Per User Add-On **(Office)** (Nonprofit Staff Pricing)</span></span>   | <span data-ttu-id="a77c5-363">31c03289-47ab-4ab0-8df1-03742c127ac6</span><span class="sxs-lookup"><span data-stu-id="a77c5-363">31c03289-47ab-4ab0-8df1-03742c127ac6</span></span>   |

<span data-ttu-id="a77c5-364">Os clientes são obrigados a ter qualquer um dos seguintes pré-requisitos para comprar esta oferta:</span><span class="sxs-lookup"><span data-stu-id="a77c5-364">Customers are required to have any one of the following prerequisites to purchase this offer:</span></span>

| <span data-ttu-id="a77c5-365">Oferta nome de exibição</span><span class="sxs-lookup"><span data-stu-id="a77c5-365">Offer display name</span></span> | <span data-ttu-id="a77c5-366">ID da oferta</span><span class="sxs-lookup"><span data-stu-id="a77c5-366">Offer ID</span></span> |
| ------ | ----------- |
| <span data-ttu-id="a77c5-367">Microsoft 365 E5 (Preços do Pessoal sem fins lucrativos)</span><span class="sxs-lookup"><span data-stu-id="a77c5-367">Microsoft 365 E5 (Nonprofit Staff Pricing)</span></span>  |  <span data-ttu-id="a77c5-368">31bedf01-9e57-4ece-a53a-d3656a563931</span><span class="sxs-lookup"><span data-stu-id="a77c5-368">31bedf01-9e57-4ece-a53a-d3656a563931</span></span>   |
|   <span data-ttu-id="a77c5-369">Microsoft 365 E5 sem Audio Conferencing (Preços de Pessoal sem fins lucrativos)</span><span class="sxs-lookup"><span data-stu-id="a77c5-369">Microsoft 365 E5 without Audio Conferencing (Nonprofit Staff Pricing)</span></span>|  <span data-ttu-id="a77c5-370">b456810a-c414-4e07-98fc-ef74e8175a09</span><span class="sxs-lookup"><span data-stu-id="a77c5-370">b456810a-c414-4e07-98fc-ef74e8175a09</span></span>|
|   <span data-ttu-id="a77c5-371">Escritório 365 E5 (Preços do Pessoal sem fins lucrativos)</span><span class="sxs-lookup"><span data-stu-id="a77c5-371">Office 365 E5 (Nonprofit Staff Pricing)</span></span>| <span data-ttu-id="a77c5-372">ce139fe5-8bd5-47ed-a5be-07c286f8b9e</span><span class="sxs-lookup"><span data-stu-id="a77c5-372">ce139fe5-8bd5-47ed-a5be-07c286f8b9e</span></span>    |
|   <span data-ttu-id="a77c5-373">Julgamento do Escritório 365 E5 (Preço do Pessoal Sem Fins Lucrativos)</span><span class="sxs-lookup"><span data-stu-id="a77c5-373">Office 365 E5 (Nonprofit Staff Pricing) Trial</span></span>|  <span data-ttu-id="a77c5-374">2f192efe-608a-4c9c-9d19-2b0b70b0962e</span><span class="sxs-lookup"><span data-stu-id="a77c5-374">2f192efe-608a-4c9c-9d19-2b0b70b0962e</span></span>|
|   <span data-ttu-id="a77c5-375">Escritório 365 E5 sem Audio Conferencing (Preços do Pessoal Sem Fins Lucrativos)</span><span class="sxs-lookup"><span data-stu-id="a77c5-375">Office 365 E5 without Audio Conferencing (Nonprofit Staff Pricing)</span></span>|  <span data-ttu-id="a77c5-376">c3897426-9f49-4eaf-9b4d-7d9a1c72aef7</span><span class="sxs-lookup"><span data-stu-id="a77c5-376">c3897426-9f49-4eaf-9b4d-7d9a1c72aef7</span></span>|

<span data-ttu-id="a77c5-377">A seguinte oferta Power BI Premium tem um pré-requisito necessário para a compra:</span><span class="sxs-lookup"><span data-stu-id="a77c5-377">The following Power BI Premium offer has a prerequisite required for purchase:</span></span>

| <span data-ttu-id="a77c5-378">Oferta nome de exibição</span><span class="sxs-lookup"><span data-stu-id="a77c5-378">Offer display name</span></span> | <span data-ttu-id="a77c5-379">ID da oferta</span><span class="sxs-lookup"><span data-stu-id="a77c5-379">Offer ID</span></span> |
| ------ | ----------- |
|   <span data-ttu-id="a77c5-380">Power BI Premium por utilizador Add-On (Preços de Pessoal sem fins lucrativos)</span><span class="sxs-lookup"><span data-stu-id="a77c5-380">Power BI Premium Per User Add-On (Nonprofit Staff Pricing)</span></span>|  <span data-ttu-id="a77c5-381">ef0b895b-681b-4026-a5b1-dda182a57d40</span><span class="sxs-lookup"><span data-stu-id="a77c5-381">ef0b895b-681b-4026-a5b1-dda182a57d40</span></span> |

<span data-ttu-id="a77c5-382">Os clientes são obrigados a ter este pré-requisito para a compra desta oferta:</span><span class="sxs-lookup"><span data-stu-id="a77c5-382">Customers are required to have this prerequisite to purchase this offer:</span></span>

| <span data-ttu-id="a77c5-383">Oferta nome de exibição</span><span class="sxs-lookup"><span data-stu-id="a77c5-383">Offer display name</span></span> | <span data-ttu-id="a77c5-384">ID da oferta</span><span class="sxs-lookup"><span data-stu-id="a77c5-384">Offer ID</span></span> |
| ------ |----------|
| <span data-ttu-id="a77c5-385">Power BI Pro (Preços do Pessoal Sem Fins Lucrativos)</span><span class="sxs-lookup"><span data-stu-id="a77c5-385">Power BI Pro (Nonprofit Staff Pricing)</span></span>  |   <span data-ttu-id="a77c5-386">cabdfc93-5786-4224-bfd3-35d58f833b35</span><span class="sxs-lookup"><span data-stu-id="a77c5-386">cabdfc93-5786-4224-bfd3-35d58f833b35</span></span> |

### <a name="next-steps"></a><span data-ttu-id="a77c5-387">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="a77c5-387">Next steps</span></span>

<span data-ttu-id="a77c5-388">Reveja os recursos sobre este tema e partilhe esta informação com as partes interessadas apropriadas na sua organização.</span><span class="sxs-lookup"><span data-stu-id="a77c5-388">Review the resources about this topic, and share this information with the appropriate stakeholders in your organization.</span></span>  

### <a name="questions"></a><span data-ttu-id="a77c5-389">Perguntas?</span><span class="sxs-lookup"><span data-stu-id="a77c5-389">Questions?</span></span>

<span data-ttu-id="a77c5-390">Para quaisquer questões sobre estas ofertas, consulte as suas comunidades Yammer relevantes.</span><span class="sxs-lookup"><span data-stu-id="a77c5-390">For any questions about these offers, check your relevant Yammer communities.</span></span> 

## <a name="march-price-updates-for-microsoft-365-f3"></a><a name="10"></a> <span data-ttu-id="a77c5-391">Atualizações de preços de março para o Microsoft 365 F3</span><span class="sxs-lookup"><span data-stu-id="a77c5-391">March price updates for Microsoft 365 F3</span></span>

### <a name="categories"></a><span data-ttu-id="a77c5-392">Categorias</span><span class="sxs-lookup"><span data-stu-id="a77c5-392">Categories</span></span>

- <span data-ttu-id="a77c5-393">Data: 2021-03-16</span><span class="sxs-lookup"><span data-stu-id="a77c5-393">Date: 2021-03-16</span></span>
- <span data-ttu-id="a77c5-394">Ofertas/Mercados</span><span class="sxs-lookup"><span data-stu-id="a77c5-394">Offers/Markets</span></span>

### <a name="summary"></a><span data-ttu-id="a77c5-395">Resumo</span><span class="sxs-lookup"><span data-stu-id="a77c5-395">Summary</span></span>

<span data-ttu-id="a77c5-396">Os preços incorretos de março de 2021 foram corrigidos para a Microsoft 365 F3 British Pound (GBP) e Euro (EUR).</span><span class="sxs-lookup"><span data-stu-id="a77c5-396">Incorrect March 2021 pricing has been corrected for Microsoft 365 F3 British Pound (GBP) and Euro (EUR).</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="a77c5-397">Audiência impactada</span><span class="sxs-lookup"><span data-stu-id="a77c5-397">Impacted audience</span></span>

<span data-ttu-id="a77c5-398">Parceiros que compram o Microsoft 365 F3 em GBP ou EUR entre 1 de março e 17 de março de 2021 através do programa Cloud Solution Provider (CSP).</span><span class="sxs-lookup"><span data-stu-id="a77c5-398">Partners purchasing Microsoft 365 F3 in GBP or EUR between March 1 and March 17, 2021 through the Cloud Solution Provider (CSP) program.</span></span>

### <a name="details"></a><span data-ttu-id="a77c5-399">Detalhes</span><span class="sxs-lookup"><span data-stu-id="a77c5-399">Details</span></span>

<span data-ttu-id="a77c5-400">A Microsoft resolveu preços incorretos para o Microsoft 365 F3.</span><span class="sxs-lookup"><span data-stu-id="a77c5-400">Microsoft has resolved incorrect pricing for Microsoft 365 F3.</span></span> <span data-ttu-id="a77c5-401">Os preços incorretos foram para GBP e EUR e apenas para ofertas adquiridas entre 1 de março e 17 de março de 2021.</span><span class="sxs-lookup"><span data-stu-id="a77c5-401">The incorrect prices were for GBP and EUR and only for offers purchased between March 1 and March 17, 2021.</span></span> <span data-ttu-id="a77c5-402">As ofertas e moedas impactadas estão listadas abaixo.</span><span class="sxs-lookup"><span data-stu-id="a77c5-402">The impacted offers and currencies are listed below.</span></span> 

| <span data-ttu-id="a77c5-403">Nome da oferta</span><span class="sxs-lookup"><span data-stu-id="a77c5-403">Offer name</span></span> | <span data-ttu-id="a77c5-404">Moeda</span><span class="sxs-lookup"><span data-stu-id="a77c5-404">Currency</span></span> | <span data-ttu-id="a77c5-405">ID da oferta</span><span class="sxs-lookup"><span data-stu-id="a77c5-405">Offer ID</span></span> | <span data-ttu-id="a77c5-406">Material ID</span><span class="sxs-lookup"><span data-stu-id="a77c5-406">Material ID</span></span> |
| ------ |----------- |----------- |----------- |
| <span data-ttu-id="a77c5-407">Microsoft 365 F3 (Caridade)</span><span class="sxs-lookup"><span data-stu-id="a77c5-407">Microsoft 365 F3 (Charity)</span></span> | <span data-ttu-id="a77c5-408">GBP</span><span class="sxs-lookup"><span data-stu-id="a77c5-408">GBP</span></span> | <span data-ttu-id="a77c5-409">57b722c2-c435-4bfb-9bc8-80509213a13a</span><span class="sxs-lookup"><span data-stu-id="a77c5-409">57b722c2-c435-4bfb-9bc8-80509213a13a</span></span> | <span data-ttu-id="a77c5-410">AAD-11626</span><span class="sxs-lookup"><span data-stu-id="a77c5-410">AAD-11626</span></span> |
| <span data-ttu-id="a77c5-411">Microsoft 365 F3 (Comercial)</span><span class="sxs-lookup"><span data-stu-id="a77c5-411">Microsoft 365 F3 (Commercial)</span></span> | <span data-ttu-id="a77c5-412">EUR</span><span class="sxs-lookup"><span data-stu-id="a77c5-412">EUR</span></span>| <span data-ttu-id="a77c5-413">3451a3b0-8cda-44a7-bad7-c30be81c4aaa</span><span class="sxs-lookup"><span data-stu-id="a77c5-413">3451a3b0-8cda-44a7-bad7-c30be81c4aaa</span></span> | <span data-ttu-id="a77c5-414">AAA-89898</span><span class="sxs-lookup"><span data-stu-id="a77c5-414">AAA-89898</span></span> |
 
<span data-ttu-id="a77c5-415">As listas de preços base de licença de março e abril foram atualizadas a 16 de março, 17:00 horas.</span><span class="sxs-lookup"><span data-stu-id="a77c5-415">The March and April preview license-base price lists were updated March 16, 5PM pacific standard time.</span></span>

### <a name="next-steps"></a><span data-ttu-id="a77c5-416">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="a77c5-416">Next steps</span></span>

- <span data-ttu-id="a77c5-417">Os parceiros devem reencaitar as atuais listas de preços baseadas em licenças, tanto em março como na pré-visualização de abril, com estas correções de preços, se aplicável.</span><span class="sxs-lookup"><span data-stu-id="a77c5-417">Partners should redownload the current license-based price lists, both March and the April preview, with these price corrections if applicable.</span></span>  
- <span data-ttu-id="a77c5-418">A Microsoft entrará em contacto com parceiros impactados nas próximas semanas por e-mail para os informar dos próximos passos relacionados com a correção das transações afetadas.</span><span class="sxs-lookup"><span data-stu-id="a77c5-418">Microsoft will be contacting impacted partners in the coming weeks via email to inform them of next steps related to correcting affected transactions.</span></span>

### <a name="questions"></a><span data-ttu-id="a77c5-419">Perguntas?</span><span class="sxs-lookup"><span data-stu-id="a77c5-419">Questions?</span></span>

<span data-ttu-id="a77c5-420">Para mais perguntas, verifique as suas comunidades CSP Yammer relevantes.</span><span class="sxs-lookup"><span data-stu-id="a77c5-420">For any further questions please check your relevant CSP Yammer communities.</span></span>

________________

## <a name="update-a-legal-company-name-through-partner-center"></a><a name="9"></a> <span data-ttu-id="a77c5-421">Atualize um nome legal da empresa através do Partner Center</span><span class="sxs-lookup"><span data-stu-id="a77c5-421">Update a legal company name through Partner Center</span></span>

### <a name="categories"></a><span data-ttu-id="a77c5-422">Categorias</span><span class="sxs-lookup"><span data-stu-id="a77c5-422">Categories</span></span>

- <span data-ttu-id="a77c5-423">Data: 2021-03-16</span><span class="sxs-lookup"><span data-stu-id="a77c5-423">Date: 2021-03-16</span></span>
- <span data-ttu-id="a77c5-424">Escala de & de eficiência de unidade</span><span class="sxs-lookup"><span data-stu-id="a77c5-424">Drive Efficiency & Scale</span></span>

### <a name="summary"></a><span data-ttu-id="a77c5-425">Resumo</span><span class="sxs-lookup"><span data-stu-id="a77c5-425">Summary</span></span>

<span data-ttu-id="a77c5-426">A partir de março de 2021, os parceiros da Microsoft Partner Network (MPN) e os revendedores indiretos cloud Solution Provider (CSP) podem atualizar o nome da empresa legal através do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="a77c5-426">Starting March 2021, Microsoft Partner Network (MPN) partners and Cloud Solution Provider (CSP) indirect resellers can update their legal company name through Partner Center.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="a77c5-427">Audiência impactada</span><span class="sxs-lookup"><span data-stu-id="a77c5-427">Impacted audience</span></span>

<span data-ttu-id="a77c5-428">Parceiros MPN e revendedores indiretos CSP (não aplicáveis aos parceiros de conta direta da CSP)</span><span class="sxs-lookup"><span data-stu-id="a77c5-428">MPN partners and CSP indirect resellers (not applicable to CSP direct bill partners)</span></span>

### <a name="details"></a><span data-ttu-id="a77c5-429">Detalhes</span><span class="sxs-lookup"><span data-stu-id="a77c5-429">Details</span></span>

<span data-ttu-id="a77c5-430">A partir de março de 2021, os parceiros mpn e revendedores indiretos da CSP podem atualizar o nome da sua empresa legal através do Partner Center de forma compatível e self-serve.</span><span class="sxs-lookup"><span data-stu-id="a77c5-430">Starting March 2021, MPN partners and CSP indirect resellers can update their legal company name through Partner Center in a compliant, self-serve manner.</span></span> <span data-ttu-id="a77c5-431">Com esta nova funcionalidade, os parceiros deixarão de precisar de submeter um bilhete de suporte do Partner Center para atualizar o nome da empresa.</span><span class="sxs-lookup"><span data-stu-id="a77c5-431">With this new feature, partners will no longer need to submit a Partner Center support ticket to update their company name.</span></span> <span data-ttu-id="a77c5-432">Isto poupará um tempo significativo para os parceiros na realização destas atividades.</span><span class="sxs-lookup"><span data-stu-id="a77c5-432">This will save a significant amount of time for partners when performing these activities.</span></span> 

<span data-ttu-id="a77c5-433">Para saber mais, consulte [Atualizar o seu perfil de negócio legal.](../update-your-partner-profile.md#update-your-legal-business-profile)</span><span class="sxs-lookup"><span data-stu-id="a77c5-433">To learn more, see [Update your legal business profile](../update-your-partner-profile.md#update-your-legal-business-profile).</span></span>

>[!NOTE]
><span data-ttu-id="a77c5-434">Certifique-se de que o nome da empresa no seu perfil de negócio legal está livre de erros ortográficos e abreviaturas, e corresponde exatamente aos seus registos formais de registo comercial da empresa.</span><span class="sxs-lookup"><span data-stu-id="a77c5-434">Ensure that the company name in your legal business profile is free of spelling errors and abbreviations, and exactly matches your formal company business registration records.</span></span> <span data-ttu-id="a77c5-435">Para obter mais informações sobre a atualização do seu perfil de organização, consulte para [verificar o seu perfil de organização.](../update-your-partner-profile.md#update-your-legal-business-profile)</span><span class="sxs-lookup"><span data-stu-id="a77c5-435">For more information on updating your organization profile, refer to [Verify your organization profile](../update-your-partner-profile.md#update-your-legal-business-profile).</span></span>

### <a name="next-steps"></a><span data-ttu-id="a77c5-436">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="a77c5-436">Next steps</span></span>

<span data-ttu-id="a77c5-437">Partilhe esta informação dentro da sua organização para que a equipa adequada possa rever e atualizar os seus processos.</span><span class="sxs-lookup"><span data-stu-id="a77c5-437">Share this information within your organization so that the appropriate team can review and update their processes.</span></span>

### <a name="questions"></a><span data-ttu-id="a77c5-438">Perguntas?</span><span class="sxs-lookup"><span data-stu-id="a77c5-438">Questions?</span></span>

<span data-ttu-id="a77c5-439">Para mais perguntas, verifique as suas comunidades CSP Yammer relevantes.</span><span class="sxs-lookup"><span data-stu-id="a77c5-439">For any further questions please check your relevant CSP Yammer communities.</span></span>

________________
## <a name="update-to-cloud-solution-provider-csp-program-evolution-and-open-license-program-changes"></a><a name="8"></a> <span data-ttu-id="a77c5-440">Atualização para a evolução do programa do Fornecedor de Soluções de Nuvem (CSP) e alterações do programa Open License</span><span class="sxs-lookup"><span data-stu-id="a77c5-440">Update to Cloud Solution Provider (CSP) program evolution and Open License program changes</span></span>

### <a name="categories"></a><span data-ttu-id="a77c5-441">Categorias</span><span class="sxs-lookup"><span data-stu-id="a77c5-441">Categories</span></span>

- <span data-ttu-id="a77c5-442">Data: 2021-03-15</span><span class="sxs-lookup"><span data-stu-id="a77c5-442">Date: 2021-03-15</span></span>
- <span data-ttu-id="a77c5-443">Capacidades</span><span class="sxs-lookup"><span data-stu-id="a77c5-443">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="a77c5-444">Resumo</span><span class="sxs-lookup"><span data-stu-id="a77c5-444">Summary</span></span>

<span data-ttu-id="a77c5-445">Novas ofertas de software perpétuo do sector comercial e público estão a chegar ao programa Cloud Solution Provider (CSP), juntamente com alterações ao programa open licensing.</span><span class="sxs-lookup"><span data-stu-id="a77c5-445">New commercial and public sector perpetual software offers are coming to the Cloud Solution Provider (CSP) program along with changes to the Open Licensing program.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="a77c5-446">Audiência impactada</span><span class="sxs-lookup"><span data-stu-id="a77c5-446">Impacted audience</span></span>

<span data-ttu-id="a77c5-447">Distribuidores comerciais e revendedores geridos que vendem através do programa Open License, bem como todos os parceiros da CSP que transacionam software perpétuo</span><span class="sxs-lookup"><span data-stu-id="a77c5-447">Commercial distributors and managed resellers selling through the Open License program, as well as all CSP partners transacting perpetual software</span></span>

### <a name="details"></a><span data-ttu-id="a77c5-448">Detalhes</span><span class="sxs-lookup"><span data-stu-id="a77c5-448">Details</span></span>

<span data-ttu-id="a77c5-449">Em setembro de 2020, a Microsoft [anunciou](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) uma série de passos na nossa jornada de transformação digital para expandir oportunidades aos parceiros no programa CSP, incluindo a disponibilidade de software no local para parceiros.</span><span class="sxs-lookup"><span data-stu-id="a77c5-449">In September 2020, Microsoft [announced](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) a series of steps in our digital transformation journey to expand opportunities to partners in the CSP program, including the availability of on-premises software for partners.</span></span> <span data-ttu-id="a77c5-450">Estas mudanças permitem que os parceiros cresçam o seu negócio e aumentem o seu alcance, aproveitando as licenças de software na CSP, posicionando-as para o sucesso no mundo atual em nuvem.</span><span class="sxs-lookup"><span data-stu-id="a77c5-450">These changes enable partners to grow their business and extend their reach by leveraging software licenses in CSP, positioning them for success in today’s cloud-first world.</span></span> <span data-ttu-id="a77c5-451">Também capacitam as transições dos clientes para a nuvem e dão aos parceiros a flexibilidade necessária para ambientes de nuvem híbrida do cliente.</span><span class="sxs-lookup"><span data-stu-id="a77c5-451">They also empower customers’ transitions to the cloud and give partners the flexibility needed for customer hybrid cloud environments.</span></span>

<span data-ttu-id="a77c5-452">Na continuação desta transformação digital, anunciamos as seguintes alterações:</span><span class="sxs-lookup"><span data-stu-id="a77c5-452">In continuation of this digital transformation, we are announcing the following changes:</span></span>

- <span data-ttu-id="a77c5-453">1 de julho de 2021: Não serão adicionados novos SKUs, produtos ou promoções à lista de preços do programa Open License.</span><span class="sxs-lookup"><span data-stu-id="a77c5-453">July 1, 2021:  No new SKUs, products, or promotions will be added to the Open License program price list.</span></span>

- <span data-ttu-id="a77c5-454">7 de julho de 2021: Duas ofertas comerciais, Get Genuine Windows e Visual Studio Professional, e ofertas do setor público (governo, educação e sem fins lucrativos – ver [anúncio](./2020-december.md#9)) serão adicionadas à lista de preços perpétuos de software da CSP.</span><span class="sxs-lookup"><span data-stu-id="a77c5-454">July 7, 2021:  Two commercial offers, Get Genuine Windows and Visual Studio Professional, and public sector offers (government, education and nonprofit – see [announcement](./2020-december.md#9)) will be added to the CSP perpetual software price list.</span></span>  <span data-ttu-id="a77c5-455">A lista de preços pode ser encontrada na secção de Software da página [de venda > de preços & Ofertas](https://partnercenter.microsoft.com/pcv/sales) no Partner Center e será republica nesta data.</span><span class="sxs-lookup"><span data-stu-id="a77c5-455">The price list can be found in the Software section of the [Sell > Pricing & Offers](https://partnercenter.microsoft.com/pcv/sales) page in Partner Center and will be republished on this date.</span></span>

<span data-ttu-id="a77c5-456">Para obter detalhes completos sobre a evolução do programa CSP e alterações no programa Open License, consulte os **Próximos Passos** abaixo.</span><span class="sxs-lookup"><span data-stu-id="a77c5-456">For full details regarding the CSP program evolution and Open License program changes, please see **Next Steps** below.</span></span>

### <a name="next-steps"></a><span data-ttu-id="a77c5-457">Passos Seguintes:</span><span class="sxs-lookup"><span data-stu-id="a77c5-457">Next Steps:</span></span>

- <span data-ttu-id="a77c5-458">Evolução do Programa CSP: Reveja o [software perpétuo nos](https://partner.microsoft.com/resources/collection/software-in-csp#/) materiais de prontidão do programa Cloud Solution Provider.</span><span class="sxs-lookup"><span data-stu-id="a77c5-458">CSP Program evolution:  Review the [Perpetual software in the Cloud Solution Provider program](https://partner.microsoft.com/resources/collection/software-in-csp#/) readiness materials.</span></span> <span data-ttu-id="a77c5-459">Use este [mapa de prontidão](https://partner.microsoft.com/resources/detail/software-in-csp-readiness-map-pdf) para localizar rapidamente as informações certas para o seu papel.</span><span class="sxs-lookup"><span data-stu-id="a77c5-459">Use this [readiness map](https://partner.microsoft.com/resources/detail/software-in-csp-readiness-map-pdf) to quickly locate the right information for your role.</span></span>

- <span data-ttu-id="a77c5-460">Alterações no programa De Licença Aberta: Rever a evolução do [programa CSP e o programa Open License altera os](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/) materiais de prontidão.</span><span class="sxs-lookup"><span data-stu-id="a77c5-460">Open License program changes:  Review the [CSP program evolution and Open License program changes](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/) readiness materials.</span></span> <span data-ttu-id="a77c5-461">Use este [mapa de prontidão](https://partner.microsoft.com/resources/detail/csp-open-evolution-to-a-better-experience-readiness-map-pdf) para localizar rapidamente as informações certas para o seu papel.</span><span class="sxs-lookup"><span data-stu-id="a77c5-461">Use this [readiness map](https://partner.microsoft.com/resources/detail/csp-open-evolution-to-a-better-experience-readiness-map-pdf) to quickly locate the right information for your role.</span></span>

### <a name="questions"></a><span data-ttu-id="a77c5-462">Perguntas</span><span class="sxs-lookup"><span data-stu-id="a77c5-462">Questions</span></span>

<span data-ttu-id="a77c5-463">Para mais perguntas, verifique as suas comunidades CSP Yammer relevantes.</span><span class="sxs-lookup"><span data-stu-id="a77c5-463">For any further questions please check your relevant CSP Yammer communities.</span></span>

_______________
## <a name="update-to-a-previous-announcement-premium-assessments-an-add-on-to-compliance-manager"></a><a name="7"></a><span data-ttu-id="a77c5-464">Atualização para um anúncio anterior: Avaliações Premium, um add-on ao Compliance Manager</span><span class="sxs-lookup"><span data-stu-id="a77c5-464">Update to a previous announcement: Premium Assessments, an add-on to Compliance Manager</span></span>

### <a name="categories"></a><span data-ttu-id="a77c5-465">Categorias</span><span class="sxs-lookup"><span data-stu-id="a77c5-465">Categories</span></span>

- <span data-ttu-id="a77c5-466">Data: 2021-03-15</span><span class="sxs-lookup"><span data-stu-id="a77c5-466">Date: 2021-03-15</span></span>
- <span data-ttu-id="a77c5-467">Expandir o seu negócio</span><span class="sxs-lookup"><span data-stu-id="a77c5-467">Grow your business</span></span>

### <a name="summary"></a><span data-ttu-id="a77c5-468">Resumo</span><span class="sxs-lookup"><span data-stu-id="a77c5-468">Summary</span></span>

<span data-ttu-id="a77c5-469">As ofertas de julgamento não deveriam ter sido listadas na lista de preços e serão removidas.</span><span class="sxs-lookup"><span data-stu-id="a77c5-469">The trial offers shouldn’t have been listed on the price list and will be removed.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="a77c5-470">Audiência impactada</span><span class="sxs-lookup"><span data-stu-id="a77c5-470">Impacted audience</span></span>

<span data-ttu-id="a77c5-471">Parceiros transacionando através do Cloud Solution Provider</span><span class="sxs-lookup"><span data-stu-id="a77c5-471">Partners transacting through Cloud Solution Provider</span></span>

### <a name="details"></a><span data-ttu-id="a77c5-472">Detalhes</span><span class="sxs-lookup"><span data-stu-id="a77c5-472">Details</span></span>

<span data-ttu-id="a77c5-473">As ofertas de julgamento não deviam ter sido incluídas na lista de preços.</span><span class="sxs-lookup"><span data-stu-id="a77c5-473">The trial offers shouldn’t have been included in the price list.</span></span> <span data-ttu-id="a77c5-474">Estes serão removidos da lista de preços de 1 de maio de 2021.</span><span class="sxs-lookup"><span data-stu-id="a77c5-474">These will be removed from the May 1, 2021 price list.</span></span>

<span data-ttu-id="a77c5-475">O anúncio original está [aqui.](./2021-february.md#4)</span><span class="sxs-lookup"><span data-stu-id="a77c5-475">The original announcement is [here](./2021-february.md#4).</span></span>

### <a name="additional-resources"></a><span data-ttu-id="a77c5-476">Recursos adicionais</span><span class="sxs-lookup"><span data-stu-id="a77c5-476">Additional resources</span></span>

- [<span data-ttu-id="a77c5-477">Segurança e conformidade microsoft 365 E5</span><span class="sxs-lookup"><span data-stu-id="a77c5-477">Microsoft 365 E5 security and compliance</span></span>](https://www.microsoft.com/licensing/product-licensing/microsoft-365-enterprise?activetab=m365-enterprise:primaryr5)

- [<span data-ttu-id="a77c5-478">Construir e gerir avaliações no Microsoft Compliance Manager - Microsoft 365 Compliance</span><span class="sxs-lookup"><span data-stu-id="a77c5-478">Build and manage assessments in Microsoft Compliance Manager - Microsoft 365 Compliance</span></span>](/microsoft-365/compliance/compliance-manager-assessments)

### <a name="next-steps"></a><span data-ttu-id="a77c5-479">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="a77c5-479">Next steps</span></span>

<span data-ttu-id="a77c5-480">Reveja os recursos sobre este tema e partilhe esta informação com as partes interessadas apropriadas na sua organização.</span><span class="sxs-lookup"><span data-stu-id="a77c5-480">Review the resources about this topic, and share this information with the appropriate stakeholders in your organization.</span></span>

### <a name="questions"></a><span data-ttu-id="a77c5-481">Perguntas?</span><span class="sxs-lookup"><span data-stu-id="a77c5-481">Questions?</span></span>

<span data-ttu-id="a77c5-482">Para questões sobre estas ofertas, consulte as suas comunidades Yammer relevantes.</span><span class="sxs-lookup"><span data-stu-id="a77c5-482">For questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="migrate-your-solutions-from-one-commercial-partner-ocp-go-to-market-gtm-to-the-microsoft-commercial-marketplace"></a><a name="6"></a> <span data-ttu-id="a77c5-483">Migrar as suas soluções de One Commercial Partner (OCP) go-to market (GTM) para o mercado comercial da Microsoft</span><span class="sxs-lookup"><span data-stu-id="a77c5-483">Migrate your solutions from One Commercial Partner (OCP) go-to market (GTM) to the Microsoft commercial marketplace</span></span>

### <a name="categories"></a><span data-ttu-id="a77c5-484">Categorias</span><span class="sxs-lookup"><span data-stu-id="a77c5-484">Categories</span></span>

- <span data-ttu-id="a77c5-485">Data: 2021-03-12</span><span class="sxs-lookup"><span data-stu-id="a77c5-485">Date: 2021-03-12</span></span>
- <span data-ttu-id="a77c5-486">Capacidades</span><span class="sxs-lookup"><span data-stu-id="a77c5-486">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="a77c5-487">Resumo</span><span class="sxs-lookup"><span data-stu-id="a77c5-487">Summary</span></span>

<span data-ttu-id="a77c5-488">A partir de 29 de março de 2021, começará a experimentar capacidades limitadas de um Parceiro Comercial (OCP) no mercado (GTM).</span><span class="sxs-lookup"><span data-stu-id="a77c5-488">From March 29, 2021, you will begin to experience limited One Commercial Partner (OCP) go-to market (GTM) capabilities.</span></span> <span data-ttu-id="a77c5-489">Encorajamo-lo a migrar as suas soluções para o mercado comercial no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="a77c5-489">We encourage you to migrate your solutions to the commercial marketplace in Partner Center.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="a77c5-490">Audiência impactada</span><span class="sxs-lookup"><span data-stu-id="a77c5-490">Impacted audience</span></span>

<span data-ttu-id="a77c5-491">Organizações co-vendem com soluções no OCP GTM</span><span class="sxs-lookup"><span data-stu-id="a77c5-491">Organizations co-selling with solutions in OCP GTM</span></span>

### <a name="details"></a><span data-ttu-id="a77c5-492">Detalhes</span><span class="sxs-lookup"><span data-stu-id="a77c5-492">Details</span></span>

<span data-ttu-id="a77c5-493">Em dezembro de 2020, iniciámos a nossa viagem desde a ferramenta Microsoft OCP GTM até ao mercado comercial da Microsoft no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="a77c5-493">In December 2020, we started our journey from the Microsoft OCP GTM tool to the Microsoft commercial marketplace in Partner Center.</span></span> <span data-ttu-id="a77c5-494">Esta transição expande as capacidades do mercado comercial onde pode mostrar as suas soluções a milhões de clientes, partilhar oportunidades bidirecionalmente com outros vendedores da Microsoft e parceiros e vender soluções inovadoras em conjunto.</span><span class="sxs-lookup"><span data-stu-id="a77c5-494">This transition expands the capabilities of the commercial marketplace where you can showcase your solutions to millions of customers, bidirectionally share opportunities with other Microsoft and partner sellers, and jointly sell innovative solutions.</span></span>

<span data-ttu-id="a77c5-495">O próximo marco na transição terá lugar no dia 29 de março de 2021.</span><span class="sxs-lookup"><span data-stu-id="a77c5-495">The next milestone in the transition will take place on March 29, 2021.</span></span> <span data-ttu-id="a77c5-496">É aí que começará a experimentar capacidades limitadas de OCP GTM, com alguns campos a tornarem-se apenas para ler.</span><span class="sxs-lookup"><span data-stu-id="a77c5-496">That’s when you’ll begin to experience limited OCP GTM capabilities, with some fields becoming read-only.</span></span> <span data-ttu-id="a77c5-497">Se está atualmente a co-vender com soluções no OCP GTM, encorajamo-lo a migrar as suas soluções para o mercado comercial para tirar partido das suas capacidades e simplificar a sua experiência de publicação.</span><span class="sxs-lookup"><span data-stu-id="a77c5-497">If you’re currently co-selling with solutions in OCP GTM, we encourage you to migrate your solutions to the commercial marketplace to take advantage of its capabilities and simplify your publishing experience.</span></span> 

<span data-ttu-id="a77c5-498">Mudar-se para o mercado comercial faz do Partner Center o principal destino da experiência de co-venda.</span><span class="sxs-lookup"><span data-stu-id="a77c5-498">Moving to the commercial marketplace makes Partner Center the primary destination for the co-sell publishing experience.</span></span> <span data-ttu-id="a77c5-499">É onde pode continuar a crescer o seu negócio ligando as suas soluções aos nossos clientes partilhados através dos mesmos canais e experiências no produto que usamos para produtos da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="a77c5-499">It’s where you can continue to grow your business by connecting your solutions with our shared customers through the same channels and in-product experiences that we use for Microsoft products.</span></span> <span data-ttu-id="a77c5-500">[Saiba mais sobre o mercado comercial.](https://blogs.partner.microsoft.com/mpn/getting-started-with-the-microsoft-commercial-marketplace/)</span><span class="sxs-lookup"><span data-stu-id="a77c5-500">[Learn more about the commercial marketplace](https://blogs.partner.microsoft.com/mpn/getting-started-with-the-microsoft-commercial-marketplace/).</span></span>

### <a name="next-steps"></a><span data-ttu-id="a77c5-501">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="a77c5-501">Next steps</span></span>

- <span data-ttu-id="a77c5-502">Se ainda não mexeu nas suas soluções, siga as instruções detalhadas no guia de [transição](/azure/marketplace/co-sell-solution-migration) ou veja o [tutorial de vídeo passo a passo](https://partner.microsoft.com/asset/detail/ocp-gtm-to-the-microsoft-commercial-marketplace-mp4) para completar todas as atividades de migração e começar a publicar as suas soluçãos no mercado comercial.</span><span class="sxs-lookup"><span data-stu-id="a77c5-502">If you have not yet moved your solutions, follow the instructions detailed in the [transition guide](/azure/marketplace/co-sell-solution-migration) or view the [step-by-step video tutorial](https://partner.microsoft.com/asset/detail/ocp-gtm-to-the-microsoft-commercial-marketplace-mp4) to complete all migration activities and start publishing your solution(s) in the commercial marketplace.</span></span>

- <span data-ttu-id="a77c5-503">Para questões relacionadas com a experiência de capacidade limitada no OCP GTM, consulte os [requisitos de Co-venda para publicar no mercado comercial da Microsoft FAQ](https://partner.microsoft.com/resources/detail/co-sell-requirements-publish-commercial-marketplace-faq-pdf).</span><span class="sxs-lookup"><span data-stu-id="a77c5-503">For questions regarding the limited capability experience in OCP GTM, view the [Co-sell requirements to publish in the Microsoft commercial marketplace FAQ](https://partner.microsoft.com/resources/detail/co-sell-requirements-publish-commercial-marketplace-faq-pdf).</span></span> <span data-ttu-id="a77c5-504">(Ver a secção "OCP GTM limited capabilities starting March 29, 2021.")</span><span class="sxs-lookup"><span data-stu-id="a77c5-504">(See the section “OCP GTM limited capabilities starting March 29, 2021.”)</span></span>

### <a name="questions"></a><span data-ttu-id="a77c5-505">Perguntas?</span><span class="sxs-lookup"><span data-stu-id="a77c5-505">Questions?</span></span>

<span data-ttu-id="a77c5-506">[Contacte o Suporte](https://partner.microsoft.com/support/?stage=1) se tiver alguma dúvida ou precisar de mais informações.</span><span class="sxs-lookup"><span data-stu-id="a77c5-506">Contact [Support](https://partner.microsoft.com/support/?stage=1) if you have any questions or need more information.</span></span>

________________
## <a name="expanding-the-new-commerce-experience-in-the-cloud-solution-provider-csp-program-for-azure-to-russia"></a><a name="5"></a><span data-ttu-id="a77c5-507">Expandir a nova experiência de comércio no programa Cloud Solution Provider (CSP) para o Azure à Rússia</span><span class="sxs-lookup"><span data-stu-id="a77c5-507">Expanding the new commerce experience in the Cloud Solution Provider (CSP) program for Azure to Russia</span></span>

### <a name="categories"></a><span data-ttu-id="a77c5-508">Categorias</span><span class="sxs-lookup"><span data-stu-id="a77c5-508">Categories</span></span>

- <span data-ttu-id="a77c5-509">Data: 2021-03-10</span><span class="sxs-lookup"><span data-stu-id="a77c5-509">Date: 2021-03-10</span></span>
- <span data-ttu-id="a77c5-510">Capacidades</span><span class="sxs-lookup"><span data-stu-id="a77c5-510">Capabilities</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="a77c5-511">Audiência impactada</span><span class="sxs-lookup"><span data-stu-id="a77c5-511">Impacted audience</span></span>

<span data-ttu-id="a77c5-512">Todos os parceiros na Rússia transacionam através do programa Cloud Solution Provider (CSP).</span><span class="sxs-lookup"><span data-stu-id="a77c5-512">All partners in Russia transacting through the Cloud Solution Provider (CSP) program.</span></span>

### <a name="details"></a><span data-ttu-id="a77c5-513">Detalhes</span><span class="sxs-lookup"><span data-stu-id="a77c5-513">Details</span></span>

<span data-ttu-id="a77c5-514">A partir de 10 de março de 2021, estamos entusiasmados por anunciar a disponibilidade da nova experiência de **comércio na CSP para o Azure na Rússia.**</span><span class="sxs-lookup"><span data-stu-id="a77c5-514">Starting March 10 2021, we’re excited to announce the availability of the **new commerce experience in CSP for Azure in Russia**.</span></span> <span data-ttu-id="a77c5-515">Esta experiência irá dinamizar e melhorar a forma como os clientes compram e consomem serviços Azure.</span><span class="sxs-lookup"><span data-stu-id="a77c5-515">This experience will streamline and improve the way customers buy and consume Azure services.</span></span> <span data-ttu-id="a77c5-516">Também dará aos parceiros do programa CSP uma visão consistente dos preços do Azure através de moções de vendas, preços USD para consistência global, alinhamento de datas de faturação e acesso à Azure Cost Management.</span><span class="sxs-lookup"><span data-stu-id="a77c5-516">It will also give partners in the CSP program a consistent view of Azure pricing across sales motions, USD pricing for global consistency, billing date alignment, and access to Azure Cost Management.</span></span>

### <a name="next-steps"></a><span data-ttu-id="a77c5-517">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="a77c5-517">Next steps</span></span>

<span data-ttu-id="a77c5-518">Existem vários recursos disponíveis introduzindo a nova experiência de comércio Azure e fornecendo informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="a77c5-518">There are several resources available introducing the new Azure commerce experience and providing additional information.</span></span> <span data-ttu-id="a77c5-519">Encontre as últimas FAQs, decks, vídeo e muito mais na Galeria de [Recursos de Atualizações do Programa CSP.](https://partner.microsoft.com/resources/collection/new-azure-experience-in-csp#/)</span><span class="sxs-lookup"><span data-stu-id="a77c5-519">Find the latest FAQs, decks, video and more in the [CSP Program Updates Resource Gallery](https://partner.microsoft.com/resources/collection/new-azure-experience-in-csp#/).</span></span>

________________
## <a name="partner-center-software-license-key-and-download-fulfillment"></a><a name="4"></a><span data-ttu-id="a77c5-520">Chave de licença de software Partner Center e cumprimento de descarregamento</span><span class="sxs-lookup"><span data-stu-id="a77c5-520">Partner Center software license key and download fulfillment</span></span>

### <a name="categories"></a><span data-ttu-id="a77c5-521">Categorias</span><span class="sxs-lookup"><span data-stu-id="a77c5-521">Categories</span></span>

- <span data-ttu-id="a77c5-522">Data: 2021-03-04</span><span class="sxs-lookup"><span data-stu-id="a77c5-522">Date: 2021-03-04</span></span>
- <span data-ttu-id="a77c5-523">Capacidades</span><span class="sxs-lookup"><span data-stu-id="a77c5-523">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="a77c5-524">Resumo</span><span class="sxs-lookup"><span data-stu-id="a77c5-524">Summary</span></span>

<span data-ttu-id="a77c5-525">O software Partner Center descarregamento e capacidade de cumprimento da chave da licença foi reintegrado.</span><span class="sxs-lookup"><span data-stu-id="a77c5-525">The Partner Center software download and license key fulfillment capability has been reinstated.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="a77c5-526">Audiência impactada</span><span class="sxs-lookup"><span data-stu-id="a77c5-526">Impacted audience</span></span>

<span data-ttu-id="a77c5-527">Todos os parceiros do Cloud Solution Provider (CSP) transacionando encomendas de software de subscrição perpétua e servidor através do Partner Center</span><span class="sxs-lookup"><span data-stu-id="a77c5-527">All Cloud Solution Provider (CSP) partners transacting perpetual and server subscription software orders through Partner Center</span></span>

### <a name="details"></a><span data-ttu-id="a77c5-528">Detalhes</span><span class="sxs-lookup"><span data-stu-id="a77c5-528">Details</span></span>

<span data-ttu-id="a77c5-529">Em resposta ao feedback do parceiro, estamos a reinstaurar a capacidade de cumprimento do Partner Center para obter chaves de software e licença para ordens de software de subscrição perpétua e servidor.</span><span class="sxs-lookup"><span data-stu-id="a77c5-529">In response to partner feedback, we’re reinstating the Partner Center fulfillment capability to obtain software and license keys for perpetual and server subscription software orders.</span></span> <span data-ttu-id="a77c5-530">Será restaurado ao seu estado anterior antes de ser removido em 19 de janeiro de 2021.</span><span class="sxs-lookup"><span data-stu-id="a77c5-530">It will be restored to its previous state prior to being removed on January 19, 2021.</span></span> <span data-ttu-id="a77c5-531">(Ver o [anúncio](2020-september.md#17).)</span><span class="sxs-lookup"><span data-stu-id="a77c5-531">(See the [announcement](2020-september.md#17).)</span></span>

<span data-ttu-id="a77c5-532">Note que as chaves de licença de software e links de descarregamento são valiosos e altamente procurados por ativos de propriedade intelectual.</span><span class="sxs-lookup"><span data-stu-id="a77c5-532">Note that software license keys and download links are valuable and highly sought-after intellectual property assets.</span></span> <span data-ttu-id="a77c5-533">Se vazadas, podem ser rapidamente esgotadas dos seus limites de ativação e causar uma experiência negativa de cliente e parceiro.</span><span class="sxs-lookup"><span data-stu-id="a77c5-533">If leaked, they can quickly be depleted of their activation limits and cause a negative customer and partner experience.</span></span>

### <a name="next-steps"></a><span data-ttu-id="a77c5-534">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="a77c5-534">Next steps</span></span>

<span data-ttu-id="a77c5-535">Reveja os seguintes recursos para instruções de utilização e orientações importantes sobre a distribuição das chaves do software:</span><span class="sxs-lookup"><span data-stu-id="a77c5-535">Review the following resources for usage instructions and important guidance on software key distribution:</span></span>

- [<span data-ttu-id="a77c5-536">Vender software no local através do programa CSP</span><span class="sxs-lookup"><span data-stu-id="a77c5-536">Sell on-premises software through the CSP program</span></span>](../csp-on-premise-software.md)
- <span data-ttu-id="a77c5-537">[Guia de operações](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf) do Centro Parceiro (Consulte a **secção de distribuição de chaves de software.)**</span><span class="sxs-lookup"><span data-stu-id="a77c5-537">[Partner Center New Commerce Operations Guide](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf) (See the **Guidance on Software Key Distribution** section.)</span></span>

### <a name="questions"></a><span data-ttu-id="a77c5-538">Perguntas?</span><span class="sxs-lookup"><span data-stu-id="a77c5-538">Questions?</span></span>

<span data-ttu-id="a77c5-539">Se tiver mais perguntas sobre este aviso, consulte as suas comunidades Yammer relevantes.</span><span class="sxs-lookup"><span data-stu-id="a77c5-539">If you have any further questions about this notice, check your relevant Yammer communities.</span></span>

________________
## <a name="migrate-your-deals-from-partner-sales-connect-psc-to-partner-center"></a><a name="3"></a><span data-ttu-id="a77c5-540">Migrar as suas ofertas de Partner Sales Connect (PSC) para Partner Center</span><span class="sxs-lookup"><span data-stu-id="a77c5-540">Migrate your deals from Partner Sales Connect (PSC) to Partner Center</span></span>

### <a name="categories"></a><span data-ttu-id="a77c5-541">Categorias</span><span class="sxs-lookup"><span data-stu-id="a77c5-541">Categories</span></span>

- <span data-ttu-id="a77c5-542">Data: 2021-03-04</span><span class="sxs-lookup"><span data-stu-id="a77c5-542">Date: 2021-03-04</span></span>
- <span data-ttu-id="a77c5-543">Capacidades</span><span class="sxs-lookup"><span data-stu-id="a77c5-543">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="a77c5-544">Resumo</span><span class="sxs-lookup"><span data-stu-id="a77c5-544">Summary</span></span>

<span data-ttu-id="a77c5-545">A Partner Sales Connect (PSC) passará para o acesso apenas à leitura a partir de 31 de março de 2021, pelo que pedimos que comece a migrar as suas ofertas do PSC para o Partner Center.</span><span class="sxs-lookup"><span data-stu-id="a77c5-545">Partner Sales Connect (PSC) will move to read-only access starting March 31, 2021, so we urge you to begin migrating your deals from PSC to Partner Center.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="a77c5-546">Audiência impactada</span><span class="sxs-lookup"><span data-stu-id="a77c5-546">Impacted audience</span></span>

<span data-ttu-id="a77c5-547">Parceiros com negócios no PSC</span><span class="sxs-lookup"><span data-stu-id="a77c5-547">Partners with deals in PSC</span></span>

### <a name="details"></a><span data-ttu-id="a77c5-548">Detalhes</span><span class="sxs-lookup"><span data-stu-id="a77c5-548">Details</span></span>

<span data-ttu-id="a77c5-549">Como parte do nosso compromisso comum com o crescimento, **co-vender com** a Microsoft é o caminho para que **você seja descoberto, entregue a sua experiência e expanda a sua pegada de cliente** para resultados positivos do cliente.</span><span class="sxs-lookup"><span data-stu-id="a77c5-549">As part of our shared commitment to growth, **co-sell with Microsoft** is the path for you to **be discovered, deliver your expertise, and expand your customer footprint** for positive customer outcomes.</span></span> <span data-ttu-id="a77c5-550">Com uma oferta média **3,5 vezes mais rápida** do que o normal, gerir a sua experiência de co-venda no Partner Center permite-lhe vender através dos canais de clientes diretos, parceiro e vendedor da Microsoft, e gerir todo o seu pipeline de referência num local.</span><span class="sxs-lookup"><span data-stu-id="a77c5-550">With an average deal that’s **3.5 times faster** than normal, managing your co-sell experience in Partner Center allows you to sell across the direct customer, partner, and Microsoft seller channels, and manage your entire referral pipeline in one location.</span></span>

<span data-ttu-id="a77c5-551">**O PSC** passará a **ter acesso apenas** a leitura a partir de 31 de março de **2021,** por isso pedimos-lhe que inicie a sua mudança para o Partner Center e aceda a estas melhorias de capacidade:</span><span class="sxs-lookup"><span data-stu-id="a77c5-551">**PSC** will move to **read-only access** starting **March 31, 2021**, so we urge you to start your move to Partner Center and access these capability improvements:</span></span> 

- <span data-ttu-id="a77c5-552">**Encaminhamento mais preciso** das ofertas que partilha com a Microsoft para o vendedor certo, com base no tipo de assistência que necessita.</span><span class="sxs-lookup"><span data-stu-id="a77c5-552">**More accurate routing** of the deals that you share with Microsoft to the right seller, based on the type of assistance you need.</span></span>
- <span data-ttu-id="a77c5-553">**Validação de elegibilidade do negócio inicial** para soluções elegíveis para incentivos e para cumprir os critérios do programa ISV Connect, simplificando o processo de aprovação e a prova final de execução (POE).</span><span class="sxs-lookup"><span data-stu-id="a77c5-553">**Upfront deal eligibility validation** for incentive-eligible solutions and to meet the ISV Connect program criteria, simplifying the approval process and final proof of execution (POE) attestation.</span></span>
- <span data-ttu-id="a77c5-554">**Experiência de utilizador sem emenda** para gerir todas as suas oportunidades de co-venda e vendas qualificadas lidera num só local.</span><span class="sxs-lookup"><span data-stu-id="a77c5-554">**Seamless user experience** to manage all your co-sell opportunities and sales qualified leads in one place.</span></span>

<span data-ttu-id="a77c5-555">Também adicionámos recentemente novas funcionalidades no Partner Center para ajudar no seu movimento:</span><span class="sxs-lookup"><span data-stu-id="a77c5-555">We’ve also recently added new features in Partner Center to assist in your move:</span></span>

- [<span data-ttu-id="a77c5-556">Operações a granel para co-vender oportunidades</span><span class="sxs-lookup"><span data-stu-id="a77c5-556">Bulk operations for co-sell opportunities</span></span>](../bulk-operations.md)
- <span data-ttu-id="a77c5-557">[Recurso de migração de acordo](../psc-to-pc.md) (ver a secção **de migração do PSC Deals.)**</span><span class="sxs-lookup"><span data-stu-id="a77c5-557">[Deal migration feature](../psc-to-pc.md) (See the **PSC Deals migration** section.)</span></span>

<span data-ttu-id="a77c5-558">Utilizando a experiência de co-venda no Partner Center, as suas equipas de vendas terão mais tempo para se concentrarem em nutrir leads e oportunidades, fechar ofertas e criar relações duradouras com o cliente.</span><span class="sxs-lookup"><span data-stu-id="a77c5-558">Using the co-sell experience in Partner Center, your sales teams will have more time to focus on nurturing leads and opportunities, closing deals, and creating lasting customer relationships.</span></span>

### <a name="next-steps"></a><span data-ttu-id="a77c5-559">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="a77c5-559">Next steps</span></span>

<span data-ttu-id="a77c5-560">Utilize o [guia de transição](../psc-to-pc.md) do Centro de Parceiros para o acompanhar através dos passos para migrar as suas ofertas do PSC para o Partner Center.</span><span class="sxs-lookup"><span data-stu-id="a77c5-560">Use the Partner Center [transition guide](../psc-to-pc.md) to walk you through the steps to migrate your deals from PSC to Partner Center.</span></span>

### <a name="questions"></a><span data-ttu-id="a77c5-561">Perguntas?</span><span class="sxs-lookup"><span data-stu-id="a77c5-561">Questions?</span></span>

<span data-ttu-id="a77c5-562">Para mais perguntas, contacte [o Support](https://partner.microsoft.com/support/?stage=1).</span><span class="sxs-lookup"><span data-stu-id="a77c5-562">For any further questions, contact [Support](https://partner.microsoft.com/support/?stage=1).</span></span>

________________
## <a name="new-microsoft-dynamics-365-products-and-offers-available-on-april-1-2021"></a><a name="2"></a><span data-ttu-id="a77c5-563">Novos produtos e ofertas microsoft Dynamics 365 disponíveis a 1 de abril de 2021</span><span class="sxs-lookup"><span data-stu-id="a77c5-563">New Microsoft Dynamics 365 products and offers available on April 1, 2021</span></span>

### <a name="categories"></a><span data-ttu-id="a77c5-564">Categorias</span><span class="sxs-lookup"><span data-stu-id="a77c5-564">Categories</span></span>

- <span data-ttu-id="a77c5-565">Data: 2021-03-04</span><span class="sxs-lookup"><span data-stu-id="a77c5-565">Date: 2021-03-04</span></span>
- <span data-ttu-id="a77c5-566">Capacidades</span><span class="sxs-lookup"><span data-stu-id="a77c5-566">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="a77c5-567">Resumo</span><span class="sxs-lookup"><span data-stu-id="a77c5-567">Summary</span></span>

<span data-ttu-id="a77c5-568">No dia 1 de abril de 2021, a Microsoft lançará vários novos produtos e ofertas para o programa Cloud Solution Provider (CSP).</span><span class="sxs-lookup"><span data-stu-id="a77c5-568">On April 1, 2021, Microsoft will be launching several new products and offers for the Cloud Solution Provider (CSP) program.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="a77c5-569">Audiência impactada</span><span class="sxs-lookup"><span data-stu-id="a77c5-569">Impacted audience</span></span>

<span data-ttu-id="a77c5-570">Todos os parceiros que transacionam através do programa Cloud Solution Provider (CSP)</span><span class="sxs-lookup"><span data-stu-id="a77c5-570">All partners transacting through the Cloud Solution Provider (CSP) program</span></span>

### <a name="details"></a><span data-ttu-id="a77c5-571">Detalhes</span><span class="sxs-lookup"><span data-stu-id="a77c5-571">Details</span></span>

<span data-ttu-id="a77c5-572">No dia 1 de abril de 2021, a Microsoft lançará os seguintes novos produtos e ofertas:</span><span class="sxs-lookup"><span data-stu-id="a77c5-572">On April 1, 2021, Microsoft will be launching the following new products and offers:</span></span>

- <span data-ttu-id="a77c5-573">Power BI Premium por utilizador</span><span class="sxs-lookup"><span data-stu-id="a77c5-573">Power BI Premium Per User</span></span>
- <span data-ttu-id="a77c5-574">Expansão geo e segmento usl de voz do cliente e marketing USL</span><span class="sxs-lookup"><span data-stu-id="a77c5-574">Customer Voice and Marketing USL geo and segment expansion</span></span>

<span data-ttu-id="a77c5-575">**Power BI Premium por utilizador**</span><span class="sxs-lookup"><span data-stu-id="a77c5-575">**Power BI Premium Per User**</span></span>

<span data-ttu-id="a77c5-576">A Microsoft introduzirá as primeiras ofertas do Power BI Premium por utilizador.</span><span class="sxs-lookup"><span data-stu-id="a77c5-576">Microsoft will introduce the first per-user Power BI Premium offers.</span></span> <span data-ttu-id="a77c5-577">O Power BI Premium é atualmente vendido apenas numa construção de capacidade.</span><span class="sxs-lookup"><span data-stu-id="a77c5-577">Power BI Premium is currently sold only in a capacity construct.</span></span> <span data-ttu-id="a77c5-578">Power BI Premium Per User fornece acesso a inteligência empresarial (BI) e capacidades de análise.</span><span class="sxs-lookup"><span data-stu-id="a77c5-578">Power BI Premium Per User provides access to enterprise business intelligence (BI) and analytics capabilities.</span></span> <span data-ttu-id="a77c5-579">O seu licenciamento individual flexível atende às pequenas e médias empresas.</span><span class="sxs-lookup"><span data-stu-id="a77c5-579">Its flexible individual seat licensing caters to small and medium-sized businesses.</span></span>

<span data-ttu-id="a77c5-580">Reveja os [detalhes de lançamento](/power-platform-release-plan/2020wave2/power-bi/planned-features) do Power BI para saber mais sobre esta oferta.</span><span class="sxs-lookup"><span data-stu-id="a77c5-580">Review the [Power BI release details](/power-platform-release-plan/2020wave2/power-bi/planned-features) to learn more about this offer.</span></span>


<span data-ttu-id="a77c5-581">**Oferecer detalhes**</span><span class="sxs-lookup"><span data-stu-id="a77c5-581">**Offer details**</span></span>

<span data-ttu-id="a77c5-582">Note que o nome da oferta difere ligeiramente da pré-visualização da lista de preços.</span><span class="sxs-lookup"><span data-stu-id="a77c5-582">Note that the offer name differs slightly from the price list preview.</span></span>

| <span data-ttu-id="a77c5-583">Nome da oferta</span><span class="sxs-lookup"><span data-stu-id="a77c5-583">Offer name</span></span> | <span data-ttu-id="a77c5-584">ID da oferta</span><span class="sxs-lookup"><span data-stu-id="a77c5-584">Offer ID</span></span> |
| ------ |----------- |
| <span data-ttu-id="a77c5-585">Power BI Premium por utilizador</span><span class="sxs-lookup"><span data-stu-id="a77c5-585">Power BI Premium Per User</span></span> | <span data-ttu-id="a77c5-586">9c810018-9356-4903-95ab-eeb956289290</span><span class="sxs-lookup"><span data-stu-id="a77c5-586">9c810018-9356-4903-95ab-eeb956289290</span></span> | 
| <span data-ttu-id="a77c5-587">Power BI Premium Por Utilizador para Docente</span><span class="sxs-lookup"><span data-stu-id="a77c5-587">Power BI Premium Per User for Faculty</span></span> | <span data-ttu-id="a77c5-588">3affc44f-f372-4ad5-8657-aadd9574fce0</span><span class="sxs-lookup"><span data-stu-id="a77c5-588">3affc44f-f372-4ad5-8657-aadd9574fce0</span></span> | 
| <span data-ttu-id="a77c5-589">Power BI Premium Por Utilizador para Estudantes</span><span class="sxs-lookup"><span data-stu-id="a77c5-589">Power BI Premium Per User for Students</span></span> | <span data-ttu-id="a77c5-590">657eea87-d0b0-4c89-8c8e-9b04395bd940</span><span class="sxs-lookup"><span data-stu-id="a77c5-590">657eea87-d0b0-4c89-8c8e-9b04395bd940</span></span> | 
| <span data-ttu-id="a77c5-591">Power BI Premium por Utilizador (Preço do Pessoal sem fins lucrativos)</span><span class="sxs-lookup"><span data-stu-id="a77c5-591">Power BI Premium Per User (Nonprofit Staff Pricing)</span></span> | <span data-ttu-id="a77c5-592">7a0a856c-059f-45dd-9d26-ae27992e706a</span><span class="sxs-lookup"><span data-stu-id="a77c5-592">7a0a856c-059f-45dd-9d26-ae27992e706a</span></span> | 
| <span data-ttu-id="a77c5-593">Power BI Premium por utilizador Add-On</span><span class="sxs-lookup"><span data-stu-id="a77c5-593">Power BI Premium Per User Add-On</span></span> | <span data-ttu-id="a77c5-594">244ff87e-5925-44a0-bf31-cea189719b58</span><span class="sxs-lookup"><span data-stu-id="a77c5-594">244ff87e-5925-44a0-bf31-cea189719b58</span></span> | 
| <span data-ttu-id="a77c5-595">Power BI Premium por utilizador Add-On para a Faculdade</span><span class="sxs-lookup"><span data-stu-id="a77c5-595">Power BI Premium Per User Add-On for Faculty</span></span> | <span data-ttu-id="a77c5-596">5da849bd-b8f7-4340-b4f4-3a9eaeb8987e</span><span class="sxs-lookup"><span data-stu-id="a77c5-596">5da849bd-b8f7-4340-b4f4-3a9eaeb8987e</span></span> | 
| <span data-ttu-id="a77c5-597">Power BI Premium por utilizador Add-On para estudantes</span><span class="sxs-lookup"><span data-stu-id="a77c5-597">Power BI Premium Per User Add-On for Students</span></span> | <span data-ttu-id="a77c5-598">cf62d70d-5af5-422a-bda8-97936402ac8e</span><span class="sxs-lookup"><span data-stu-id="a77c5-598">cf62d70d-5af5-422a-bda8-97936402ac8e</span></span> | 
| <span data-ttu-id="a77c5-599">Power BI Premium por utilizador Add-On (Preços de Pessoal sem fins lucrativos)</span><span class="sxs-lookup"><span data-stu-id="a77c5-599">Power BI Premium Per User Add-On (Nonprofit Staff Pricing)</span></span> | <span data-ttu-id="a77c5-600">31c03289-47ab-4ab0-8df1-03742c127ac6</span><span class="sxs-lookup"><span data-stu-id="a77c5-600">31c03289-47ab-4ab0-8df1-03742c127ac6</span></span> | 

<span data-ttu-id="a77c5-601">**Expansão geo e segmento usl de voz do cliente e marketing USL**</span><span class="sxs-lookup"><span data-stu-id="a77c5-601">**Customer Voice and Marketing USL geo and segment expansion**</span></span>

<span data-ttu-id="a77c5-602">No seguimento do lançamento de dezembro de 2020, as ofertas de Voz e Marketing USL da Dynamics 365 foram alteradas para adicionar novos países e MAIS SKUs sem fins lucrativos e educativos.</span><span class="sxs-lookup"><span data-stu-id="a77c5-602">As a follow-up to the December 2020 launch, Dynamics 365 Customer Voice and Marketing USL offers have been changed to add new countries and more nonprofit and educational SKUs.</span></span>

| <span data-ttu-id="a77c5-603">Nome da oferta</span><span class="sxs-lookup"><span data-stu-id="a77c5-603">Offer name</span></span> | <span data-ttu-id="a77c5-604">ID da oferta</span><span class="sxs-lookup"><span data-stu-id="a77c5-604">Offer ID</span></span> |
| ------ |----------- |
| <span data-ttu-id="a77c5-605">Dinâmica 365 Customer Voice USL (Preços de pessoal sem fins lucrativos)</span><span class="sxs-lookup"><span data-stu-id="a77c5-605">Dynamics 365 Customer Voice USL (Nonprofit Staff Pricing)</span></span> | <span data-ttu-id="a77c5-606">7a8642a5-481e-4906-a642-b56dbeeb62a0</span><span class="sxs-lookup"><span data-stu-id="a77c5-606">7a8642a5-481e-4906-a642-b56dbeeb62a0</span></span> |
| <span data-ttu-id="a77c5-607">Dinâmica 365 Voz do Cliente USL para Faculdade</span><span class="sxs-lookup"><span data-stu-id="a77c5-607">Dynamics 365 Customer Voice USL for Faculty</span></span> | <span data-ttu-id="a77c5-608">85162d70-9676-4cf6-a4bc-a0d6672f2657</span><span class="sxs-lookup"><span data-stu-id="a77c5-608">85162d70-9676-4cf6-a4bc-a0d6672f2657</span></span> |

<span data-ttu-id="a77c5-609">Visite as seguintes páginas para saber mais sobre estas ofertas:</span><span class="sxs-lookup"><span data-stu-id="a77c5-609">Visit the following pages to find out more about these offers:</span></span>

- [<span data-ttu-id="a77c5-610">Página inicial da Página inicial da Voz do Serviço ao Cliente Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="a77c5-610">Dynamics 365 Customer Service Voice home page</span></span>](https://dynamics.microsoft.com/customer-voice/overview/)
- [<span data-ttu-id="a77c5-611">Página inicial de Marketing Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="a77c5-611">Dynamics 365 Marketing home page</span></span>](https://dynamics.microsoft.com/customer-voice/overview/)

### <a name="next-steps"></a><span data-ttu-id="a77c5-612">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="a77c5-612">Next steps</span></span>

<span data-ttu-id="a77c5-613">Reveja os recursos sobre este tema e partilhe esta informação com as partes interessadas apropriadas na sua organização.</span><span class="sxs-lookup"><span data-stu-id="a77c5-613">Review the resources on this topic, and share this information with the appropriate stakeholders in your organization.</span></span>  

### <a name="questions"></a><span data-ttu-id="a77c5-614">Perguntas?</span><span class="sxs-lookup"><span data-stu-id="a77c5-614">Questions?</span></span>

<span data-ttu-id="a77c5-615">Para quaisquer questões sobre estas ofertas, consulte as suas comunidades Yammer relevantes.</span><span class="sxs-lookup"><span data-stu-id="a77c5-615">For any questions about these offers, check your relevant Yammer communities.</span></span> 

________________
## <a name="microsoft-universal-print-now-available-in-some-suites"></a><a name="1"></a> <span data-ttu-id="a77c5-616">Microsoft Universal Print já disponível em algumas suites</span><span class="sxs-lookup"><span data-stu-id="a77c5-616">Microsoft Universal Print now available in some suites</span></span>

### <a name="categories"></a><span data-ttu-id="a77c5-617">Categorias</span><span class="sxs-lookup"><span data-stu-id="a77c5-617">Categories</span></span>

- <span data-ttu-id="a77c5-618">Data: 2021-03-33</span><span class="sxs-lookup"><span data-stu-id="a77c5-618">Date: 2021-03-33</span></span>
- <span data-ttu-id="a77c5-619">Capacidades</span><span class="sxs-lookup"><span data-stu-id="a77c5-619">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="a77c5-620">Resumo</span><span class="sxs-lookup"><span data-stu-id="a77c5-620">Summary</span></span>

<span data-ttu-id="a77c5-621">A Microsoft Universal Print estará disponível para transacionar dentro de suites Microsoft 365 selecionadas e como um addon autónomo a partir de 1 de março de 2021.</span><span class="sxs-lookup"><span data-stu-id="a77c5-621">Microsoft Universal Print will be available to transact within select Microsoft 365 suites and as a standalone add-on from March 1, 2021.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="a77c5-622">Audiência impactada</span><span class="sxs-lookup"><span data-stu-id="a77c5-622">Impacted audience</span></span>

<span data-ttu-id="a77c5-623">Todos os parceiros que transacionam através do programa Cloud Solution Provider (CSP)</span><span class="sxs-lookup"><span data-stu-id="a77c5-623">All partners transacting through the Cloud Solution Provider (CSP) program</span></span>

### <a name="details"></a><span data-ttu-id="a77c5-624">Detalhes</span><span class="sxs-lookup"><span data-stu-id="a77c5-624">Details</span></span>

<span data-ttu-id="a77c5-625">[Universal Print](https://aka.ms/universalprint) é um serviço de impressão Microsoft 365 que remove a necessidade de servidores de impressão no local e permite que os dispositivos Windows imprimam para impressoras registadas no Azure.</span><span class="sxs-lookup"><span data-stu-id="a77c5-625">[Universal Print](https://aka.ms/universalprint) is a Microsoft 365 print service that removes the need for on-premises print servers, and enables Windows devices to print to Azure-registered printers.</span></span> <span data-ttu-id="a77c5-626">Estará disponível para transações a partir de 1 de março de 2021.</span><span class="sxs-lookup"><span data-stu-id="a77c5-626">It will be available to transact from March 1, 2021.</span></span>

<span data-ttu-id="a77c5-627">Os trabalhadores beneficiam da impressão sem condutor, da descoberta da impressora baseada em localização e de uma experiência de impressão intuitiva sem curva de aprendizagem.</span><span class="sxs-lookup"><span data-stu-id="a77c5-627">Workers benefit from driverless printing, streamlined location-based printer discovery, and an intuitive printing experience with no learning curve.</span></span> <span data-ttu-id="a77c5-628">Os dispositivos que se unem ao Azure Ative Directory (Azure AD) utilizam credenciais AZure AD existentes para imprimir de forma segura.</span><span class="sxs-lookup"><span data-stu-id="a77c5-628">Devices that are joined to Azure Active Directory (Azure AD) use existing Azure AD credentials to print securely.</span></span> <span data-ttu-id="a77c5-629">Os administradores gerem a impressão utilizando o portal Azure e podem facilmente ligar impressoras com suporte nativo para impressão universal.</span><span class="sxs-lookup"><span data-stu-id="a77c5-629">Administrators manage printing by using the Azure portal, and can easily connect printers with native support for Universal Print.</span></span> <span data-ttu-id="a77c5-630">A Impressão Universal pode ser implantada com impressoras não compatíveis utilizando o software de conector de impressão universal.</span><span class="sxs-lookup"><span data-stu-id="a77c5-630">Universal Print can be deployed with non-compatible printers by using Universal Print connector software.</span></span>

<span data-ttu-id="a77c5-631">A Universal Print será reensitada no lançamento para Windows E3, A3, E5 e A5, e Microsoft 365 BP, F3, E3, A3, E5 e A5.</span><span class="sxs-lookup"><span data-stu-id="a77c5-631">Universal Print will be backfilled at launch to Windows E3, A3, E5, and A5, and Microsoft 365 BP, F3, E3, A3, E5, and A5.</span></span>  

<span data-ttu-id="a77c5-632">**Oferecer detalhes**</span><span class="sxs-lookup"><span data-stu-id="a77c5-632">**Offer details**</span></span>

<span data-ttu-id="a77c5-633">Note que o nome da oferta difere ligeiramente da pré-visualização da lista de preços.</span><span class="sxs-lookup"><span data-stu-id="a77c5-633">Note that the offer name differs slightly from the price list preview.</span></span>

| <span data-ttu-id="a77c5-634">Nome da oferta</span><span class="sxs-lookup"><span data-stu-id="a77c5-634">Offer name</span></span> | <span data-ttu-id="a77c5-635">ID da oferta</span><span class="sxs-lookup"><span data-stu-id="a77c5-635">Offer ID</span></span> | <span data-ttu-id="a77c5-636">Material ID</span><span class="sxs-lookup"><span data-stu-id="a77c5-636">Material ID</span></span> |
| ------ |----------- |----------- |  
| <span data-ttu-id="a77c5-637">Universal Print volume add-on (500 empregos) - Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="a77c5-637">Universal Print volume add-on (500 jobs) - Microsoft 365</span></span>  | <span data-ttu-id="a77c5-638">cb131356-45ee-4ae2-8537-873b706c8e75</span><span class="sxs-lookup"><span data-stu-id="a77c5-638">cb131356-45ee-4ae2-8537-873b706c8e75</span></span>     | <span data-ttu-id="a77c5-639">9BI-00004</span><span class="sxs-lookup"><span data-stu-id="a77c5-639">9BI-00004</span></span>   |
| <span data-ttu-id="a77c5-640">Complemento de volume de impressão universal (500 empregos) para docentes - Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="a77c5-640">Universal Print volume add-on (500 jobs) for faculty - Microsoft 365</span></span>   | <span data-ttu-id="a77c5-641">477bee81-9872-43d6-91d3-c72390bfcf49</span><span class="sxs-lookup"><span data-stu-id="a77c5-641">477bee81-9872-43d6-91d3-c72390bfcf49</span></span>   | <span data-ttu-id="a77c5-642">9BK-00004</span><span class="sxs-lookup"><span data-stu-id="a77c5-642">9BK-00004</span></span>   |
| <span data-ttu-id="a77c5-643">Complemento de volume de impressão universal (500 empregos) - Windows</span><span class="sxs-lookup"><span data-stu-id="a77c5-643">Universal Print volume add-on (500 jobs) - Windows</span></span>    | <span data-ttu-id="a77c5-644">d3ddc493-5741-4e0d-a02d-07edbb72e</span><span class="sxs-lookup"><span data-stu-id="a77c5-644">d3ddc493-5741-4e0d-a02d-07edbb0bb72e</span></span>   | <span data-ttu-id="a77c5-645">9BI-00002</span><span class="sxs-lookup"><span data-stu-id="a77c5-645">9BI-00002</span></span>   |
| <span data-ttu-id="a77c5-646">Complemento de volume de impressão universal (500 empregos) para docentes - Windows</span><span class="sxs-lookup"><span data-stu-id="a77c5-646">Universal Print volume add-on (500 jobs) for faculty - Windows</span></span>   |  <span data-ttu-id="a77c5-647">d0862f05-80f5-4fd4-8432-fe72dd893cc7</span><span class="sxs-lookup"><span data-stu-id="a77c5-647">d0862f05-80f5-4fd4-8432-fe72dd893cc7</span></span>  | <span data-ttu-id="a77c5-648">9BK-00002</span><span class="sxs-lookup"><span data-stu-id="a77c5-648">9BK-00002</span></span>   |

### <a name="next-steps"></a><span data-ttu-id="a77c5-649">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="a77c5-649">Next steps</span></span>

<span data-ttu-id="a77c5-650">Familiarize-se com a tabela de preços e a [visão geral](/universal-print/fundamentals/universal-print-whatis)da Impressão Universal .</span><span class="sxs-lookup"><span data-stu-id="a77c5-650">Familiarize yourself with the price list and the [Universal Print overview](/universal-print/fundamentals/universal-print-whatis).</span></span> <span data-ttu-id="a77c5-651">Partilhe esta informação com todos os contactos apropriados na sua organização.</span><span class="sxs-lookup"><span data-stu-id="a77c5-651">Share this information with all appropriate contacts in your organization.</span></span>

### <a name="questions"></a><span data-ttu-id="a77c5-652">Perguntas?</span><span class="sxs-lookup"><span data-stu-id="a77c5-652">Questions?</span></span>

<span data-ttu-id="a77c5-653">Para quaisquer questões sobre estas ofertas, consulte as suas comunidades Yammer relevantes.</span><span class="sxs-lookup"><span data-stu-id="a77c5-653">For any questions about these offers, check your relevant Yammer communities.</span></span>
