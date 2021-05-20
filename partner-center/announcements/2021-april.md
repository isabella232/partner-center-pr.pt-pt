---
title: Anúncios de abril de 2021
description: Anúncios de abril de 2021 para o Microsoft Partner Center, incluindo novas capacidades, promoções, ofertas, mercados ou alterações às ofertas existentes.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.custom:
- announcement
- references_regions
ms.localizationpriority: high
ms.date: 04/29/2021
ms.openlocfilehash: 13b8ec9ddd82b38a265606809b8c39c07436e548
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150136"
---
# <a name="april-2021-announcements"></a><span data-ttu-id="a8563-103">Anúncios de abril de 2021</span><span class="sxs-lookup"><span data-stu-id="a8563-103">April 2021 announcements</span></span>

<span data-ttu-id="a8563-104">Esta página fornece os anúncios para o Microsoft Partner Center para abril de 2021.</span><span class="sxs-lookup"><span data-stu-id="a8563-104">This page provides the announcements for Microsoft Partner Center for April 2021.</span></span>

## <a name="readiness-updated-csp-customer-address-validation-api-going-live-in-june-testing-capability-now-available"></a><a name="10"></a><span data-ttu-id="a8563-105">Prontidão: Validação de endereço do cliente CSP atualizada API em direto em junho; capacidade de teste agora disponível</span><span class="sxs-lookup"><span data-stu-id="a8563-105">Readiness: Updated CSP customer address validation API going live in June; testing capability now available</span></span>

### <a name="categories"></a><span data-ttu-id="a8563-106">Categorias</span><span class="sxs-lookup"><span data-stu-id="a8563-106">Categories</span></span>

- <span data-ttu-id="a8563-107">Data: 2021-04-30</span><span class="sxs-lookup"><span data-stu-id="a8563-107">Date: 2021-04-30</span></span>
- <span data-ttu-id="a8563-108">Preparação</span><span class="sxs-lookup"><span data-stu-id="a8563-108">Readiness</span></span>

### <a name="summary"></a><span data-ttu-id="a8563-109">Resumo</span><span class="sxs-lookup"><span data-stu-id="a8563-109">Summary</span></span>

<span data-ttu-id="a8563-110">Para ajudar parceiros e clientes a gerir o seu negócio com base na confiança, vamos convidar parceiros para testar alterações na API de Endereço Validado para todos os países do mundo.</span><span class="sxs-lookup"><span data-stu-id="a8563-110">To help partners and customers run their business based on trust, we’ll be inviting partners to test changes to the Validate Address API for all countries worldwide.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="a8563-111">Audiência impactada</span><span class="sxs-lookup"><span data-stu-id="a8563-111">Impacted audience</span></span>

<span data-ttu-id="a8563-112">Parceiros de conta direta da CSP e fornecedores indiretos que criam novos ou atualizaram os detalhes do endereço dos clientes existentes</span><span class="sxs-lookup"><span data-stu-id="a8563-112">CSP direct bill partners and indirect providers who create new or update existing customers’ address details</span></span>

### <a name="details"></a><span data-ttu-id="a8563-113">Detalhes</span><span class="sxs-lookup"><span data-stu-id="a8563-113">Details</span></span>

<span data-ttu-id="a8563-114">A Microsoft tem confiança.</span><span class="sxs-lookup"><span data-stu-id="a8563-114">Microsoft runs on trust.</span></span> <span data-ttu-id="a8563-115">Estamos empenhados em fornecer um método compatível, seguro e seguro de validação de endereços do cliente para transação de subscrições de clientes no programa CSP.</span><span class="sxs-lookup"><span data-stu-id="a8563-115">We’re committed to providing a compliant, safe, and secure method of customer address validation for transacting customer subscriptions in the CSP program.</span></span> <span data-ttu-id="a8563-116">A partir de 31 de março de 2021, introduzimos alterações à API de Endereço Validado.</span><span class="sxs-lookup"><span data-stu-id="a8563-116">As of March 31, 2021, we have introduced changes to the Validate Address API.</span></span> <span data-ttu-id="a8563-117">Convidamos parceiros a testar a API antes do go-live no final de junho de 2021.</span><span class="sxs-lookup"><span data-stu-id="a8563-117">We invite partners to test the API prior to the  go-live at the end of June 2021.</span></span> 

<span data-ttu-id="a8563-118">Note que estas alterações afetam apenas a API do Endereço Validado.</span><span class="sxs-lookup"><span data-stu-id="a8563-118">Note that these changes affect the Validate Address API only.</span></span> <span data-ttu-id="a8563-119">Criar APIs de Perfil de Faturação de Clientes e Atualização não são afetados.</span><span class="sxs-lookup"><span data-stu-id="a8563-119">Create Customer and Update Billing Profile APIs aren’t affected.</span></span> <span data-ttu-id="a8563-120">Embora o endereço sugerido não tenha atualmente de ser usado com a API do Cliente Criar, é altamente recomendado.</span><span class="sxs-lookup"><span data-stu-id="a8563-120">Although the suggested address doesn’t currently have to be used with the Create Customer API, it’s highly recommended.</span></span>

<span data-ttu-id="a8563-121">A resposta devolverá uma das seguintes mensagens de estado:</span><span class="sxs-lookup"><span data-stu-id="a8563-121">The response will return one of the following status messages:</span></span>

| <span data-ttu-id="a8563-122">Estado</span><span class="sxs-lookup"><span data-stu-id="a8563-122">Status</span></span>     | <span data-ttu-id="a8563-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8563-123">Description</span></span> |    <span data-ttu-id="a8563-124">Número de endereços sugeridos devolvidos</span><span class="sxs-lookup"><span data-stu-id="a8563-124">Number of suggested addresses returned</span></span> |
|-------|---------------|-------------------|
|<span data-ttu-id="a8563-125">Envio verificado</span><span class="sxs-lookup"><span data-stu-id="a8563-125">Verified shippable</span></span> | <span data-ttu-id="a8563-126">O endereço é verificado e pode ser enviado para.</span><span class="sxs-lookup"><span data-stu-id="a8563-126">Address is verified and can be shipped to.</span></span> | <span data-ttu-id="a8563-127">Único</span><span class="sxs-lookup"><span data-stu-id="a8563-127">Single</span></span> |
|<span data-ttu-id="a8563-128">Verificado</span><span class="sxs-lookup"><span data-stu-id="a8563-128">Verified</span></span> | <span data-ttu-id="a8563-129">O endereço está verificado.</span><span class="sxs-lookup"><span data-stu-id="a8563-129">Address is verified.</span></span> | <span data-ttu-id="a8563-130">Único</span><span class="sxs-lookup"><span data-stu-id="a8563-130">Single</span></span> |
|<span data-ttu-id="a8563-131">Interação necessária</span><span class="sxs-lookup"><span data-stu-id="a8563-131">Interaction required</span></span> | <span data-ttu-id="a8563-132">O endereço sugerido foi alterado significativamente e precisa de confirmação do utilizador.</span><span class="sxs-lookup"><span data-stu-id="a8563-132">Suggested address has been changed significantly and needs user confirmation.</span></span> | <span data-ttu-id="a8563-133">Único</span><span class="sxs-lookup"><span data-stu-id="a8563-133">Single</span></span> |
|<span data-ttu-id="a8563-134">Parcial de rua</span><span class="sxs-lookup"><span data-stu-id="a8563-134">Street partial</span></span> | <span data-ttu-id="a8563-135">A rua dada no endereço é parcial e precisa de mais informações.</span><span class="sxs-lookup"><span data-stu-id="a8563-135">The given street in the address is partial and needs more info.</span></span> | <span data-ttu-id="a8563-136">Múltiplos — máximo de três</span><span class="sxs-lookup"><span data-stu-id="a8563-136">Multiple—maximum of three</span></span> |
|<span data-ttu-id="a8563-137">Instalações parciais</span><span class="sxs-lookup"><span data-stu-id="a8563-137">Premises partial</span></span> | <span data-ttu-id="a8563-138">As instalações dadas (número de edifício, número de suite, entre outras) são parciais e precisam de mais informações.</span><span class="sxs-lookup"><span data-stu-id="a8563-138">The given premises (building number, suite number, and others) are partial and need more info.</span></span> | <span data-ttu-id="a8563-139">Múltiplos — máximo de três</span><span class="sxs-lookup"><span data-stu-id="a8563-139">Multiple—maximum of three</span></span> |
|<span data-ttu-id="a8563-140">Vários</span><span class="sxs-lookup"><span data-stu-id="a8563-140">Multiple</span></span> | <span data-ttu-id="a8563-141">Existem vários campos que são parciais no endereço (potencialmente também incluindo a parcial da rua e as instalações parciais).</span><span class="sxs-lookup"><span data-stu-id="a8563-141">There are multiple fields that are partial in the address (potentially also including street partial and premises partial).</span></span> | <span data-ttu-id="a8563-142">Múltiplos — máximo de três</span><span class="sxs-lookup"><span data-stu-id="a8563-142">Multiple—maximum of three</span></span> |
|<span data-ttu-id="a8563-143">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="a8563-143">None</span></span> | <span data-ttu-id="a8563-144">O endereço está incorreto.</span><span class="sxs-lookup"><span data-stu-id="a8563-144">Address is incorrect.</span></span> | <span data-ttu-id="a8563-145">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="a8563-145">None</span></span> |
|<span data-ttu-id="a8563-146">Não validado</span><span class="sxs-lookup"><span data-stu-id="a8563-146">Not validated</span></span> | <span data-ttu-id="a8563-147">O endereço não pôde ser enviado através do processo de validação.</span><span class="sxs-lookup"><span data-stu-id="a8563-147">Address was not able to be sent through the validation process.</span></span> | <span data-ttu-id="a8563-148">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="a8563-148">None</span></span> |

<span data-ttu-id="a8563-149">Os códigos postais dos EUA devolverão mais quatro dígitos + hífen, por exemplo, 12345-6789.</span><span class="sxs-lookup"><span data-stu-id="a8563-149">US post codes will return an additional four digits + hyphen, for example, 12345-6789.</span></span>

### <a name="next-steps"></a><span data-ttu-id="a8563-150">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="a8563-150">Next steps</span></span>

- <span data-ttu-id="a8563-151">Reveja a documentação técnica e questione frequentemente na [coleção de parceiros dedicados](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) para obter uma orientação mais detalhada.</span><span class="sxs-lookup"><span data-stu-id="a8563-151">Review the technical documentation and frequently asked questions in the [dedicated partner collection](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) for more detailed guidance.</span></span>
- <span data-ttu-id="a8563-152">Prepare-se para incorporar as alterações utilizando a API do Partner Center e a experiência do utilizador web.</span><span class="sxs-lookup"><span data-stu-id="a8563-152">Prepare to incorporate the changes using the Partner Center API and web user experience.</span></span> 
- <span data-ttu-id="a8563-153">Partilhe o seu ID do inquilino da caixa de areia com o especialista em assuntos (Ali Khaki) a ser incluído no voo de teste, para que possa começar a preparar-se para a atualização.</span><span class="sxs-lookup"><span data-stu-id="a8563-153">Share your sandbox tenant ID with the subject matter expert (Ali Khaki) to be included in the test flight, so that you can begin preparing for the update.</span></span> 
- <span data-ttu-id="a8563-154">Se estiver a utilizar uma solução de fornecedor de painéis de controlo (CPV), consulte o seu CPV.</span><span class="sxs-lookup"><span data-stu-id="a8563-154">If you’re using a control panel vendor (CPV) solution, consult your CPV.</span></span>

### <a name="questions"></a><span data-ttu-id="a8563-155">Perguntas?</span><span class="sxs-lookup"><span data-stu-id="a8563-155">Questions?</span></span>

<span data-ttu-id="a8563-156">Se precisar de apoio para as suas operações com a Microsoft, contacte o grupo Yammer ou abra um pedido de [serviço.](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8)</span><span class="sxs-lookup"><span data-stu-id="a8563-156">If you need support for your operations with Microsoft, reach out to your partner support Yammer group or open a [service request](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span></span>

_______________
## <a name="new-location-for-partner-center-api-swagger-documentation"></a><a name="9"></a><span data-ttu-id="a8563-157">Nova localização para a documentação da API Swagger do Partner Center</span><span class="sxs-lookup"><span data-stu-id="a8563-157">New location for Partner Center API Swagger documentation</span></span>

### <a name="categories"></a><span data-ttu-id="a8563-158">Categorias</span><span class="sxs-lookup"><span data-stu-id="a8563-158">Categories</span></span>

- <span data-ttu-id="a8563-159">Data: 2021-04-26</span><span class="sxs-lookup"><span data-stu-id="a8563-159">Date: 2021-04-26</span></span>
- <span data-ttu-id="a8563-160">Capacidades</span><span class="sxs-lookup"><span data-stu-id="a8563-160">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="a8563-161">Resumo</span><span class="sxs-lookup"><span data-stu-id="a8563-161">Summary</span></span>

<span data-ttu-id="a8563-162">Os documentos da API Swagger do Centro Parceiro foram migrados do anterior site de [documentação da Swagger](https://apidocs.microsoft.com/services/partnercenter) para um [novo site de documentação swagger.](/rest/api/partner-center-rest/)</span><span class="sxs-lookup"><span data-stu-id="a8563-162">Partner Center API Swagger documents have been migrated from the [previous Swagger Documentation site](https://apidocs.microsoft.com/services/partnercenter) to a [new Swagger Documentation site](/rest/api/partner-center-rest/).</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="a8563-163">Audiência impactada</span><span class="sxs-lookup"><span data-stu-id="a8563-163">Impacted audience</span></span>

<span data-ttu-id="a8563-164">Parceiros de conta direta e fornecedores indiretos que participam no programa Cloud Solution Provider (CSP) que estão a utilizar as APIs do Partner Center</span><span class="sxs-lookup"><span data-stu-id="a8563-164">Direct bill partners and Indirect Providers participating in the Cloud Solution Provider (CSP) program who are using the Partner Center APIs</span></span>

### <a name="details"></a><span data-ttu-id="a8563-165">Detalhes</span><span class="sxs-lookup"><span data-stu-id="a8563-165">Details</span></span>

<span data-ttu-id="a8563-166">A partir de 26 de abril de 2021, a documentação da API Swagger do Partner Center, incluindo o conteúdo da API de Repouso, está localizada num [novo site.](/rest/api/partner-center-rest/)</span><span class="sxs-lookup"><span data-stu-id="a8563-166">As of April 26, 2021 the Partner Center API Swagger documentation, including Rest API content, is located on a [new site](/rest/api/partner-center-rest/).</span></span> <span data-ttu-id="a8563-167">O antigo local ficará inacessível após várias semanas.</span><span class="sxs-lookup"><span data-stu-id="a8563-167">The old site will be inaccessible after several weeks.</span></span>

### <a name="benefits"></a><span data-ttu-id="a8563-168">Benefícios</span><span class="sxs-lookup"><span data-stu-id="a8563-168">Benefits</span></span>

<span data-ttu-id="a8563-169">A documentação da API Swagger do Centro Parceiro fornecerá uma função **try it.**</span><span class="sxs-lookup"><span data-stu-id="a8563-169">The Partner Center API Swagger documentation will provide a **Try It** function.</span></span> <span data-ttu-id="a8563-170">Para utilizar esta função, terá de ter um Token Bearer, que pode gerar seguindo os passos listados na [Autenticação do Centro de Parceiros.](/partner-center/develop/partner-center-authentication#app--user-authentication)</span><span class="sxs-lookup"><span data-stu-id="a8563-170">To use this function, you’ll need to have a Bearer Token, which you can generate by following the steps listed in [Partner Center Authentication](/partner-center/develop/partner-center-authentication#app--user-authentication).</span></span>

### <a name="next-steps"></a><span data-ttu-id="a8563-171">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="a8563-171">Next steps</span></span>

<span data-ttu-id="a8563-172">Partilhe esta informação dentro da sua organização para que a equipa adequada possa rever e atualizar os seus processos.</span><span class="sxs-lookup"><span data-stu-id="a8563-172">Share this information within your organization so that the appropriate team can review and update their processes.</span></span>

### <a name="questions"></a><span data-ttu-id="a8563-173">Perguntas?</span><span class="sxs-lookup"><span data-stu-id="a8563-173">Questions?</span></span>

<span data-ttu-id="a8563-174">Para questões sobre estas ofertas, consulte as suas comunidades Yammer relevantes.</span><span class="sxs-lookup"><span data-stu-id="a8563-174">For questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="cloud-solution-provider-csp-software-return-period-policy-and-download-link-expiry-notice"></a><a name="8"></a><span data-ttu-id="a8563-175">Cloud Solution Provider (CSP) software devolução de tempo e aviso de expiração do link de descarregamento</span><span class="sxs-lookup"><span data-stu-id="a8563-175">Cloud Solution Provider (CSP) software return period policy and download link expiry notice</span></span>

### <a name="categories"></a><span data-ttu-id="a8563-176">Categorias</span><span class="sxs-lookup"><span data-stu-id="a8563-176">Categories</span></span>

- <span data-ttu-id="a8563-177">Data: 2021-04-21</span><span class="sxs-lookup"><span data-stu-id="a8563-177">Date: 2021-04-21</span></span>
- <span data-ttu-id="a8563-178">Capacidades</span><span class="sxs-lookup"><span data-stu-id="a8563-178">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="a8563-179">Resumo</span><span class="sxs-lookup"><span data-stu-id="a8563-179">Summary</span></span>

<span data-ttu-id="a8563-180">Existem alterações na política do período de devolução do software CSP e na expiração do link de descarregamento.</span><span class="sxs-lookup"><span data-stu-id="a8563-180">There are changes to the CSP software return period policy and download link expiry.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="a8563-181">Audiência impactada</span><span class="sxs-lookup"><span data-stu-id="a8563-181">Impacted audience</span></span>

<span data-ttu-id="a8563-182">Parceiros que transacionam ofertas de subscrição de software perpétuo ou software em CSP</span><span class="sxs-lookup"><span data-stu-id="a8563-182">Partners transacting perpetual software or software subscription offers in CSP</span></span>

### <a name="details"></a><span data-ttu-id="a8563-183">Detalhes</span><span class="sxs-lookup"><span data-stu-id="a8563-183">Details</span></span>

<span data-ttu-id="a8563-184">Note as seguintes notificações importantes relativas a compras perpétuas de software e subscrição de software através do Partner Center:</span><span class="sxs-lookup"><span data-stu-id="a8563-184">Note the following important notifications regarding perpetual software and software subscription purchases through Partner Center:</span></span>

#### <a name="software-return-period-policy"></a><span data-ttu-id="a8563-185">Política do período de devolução do software</span><span class="sxs-lookup"><span data-stu-id="a8563-185">Software return period policy</span></span>

<span data-ttu-id="a8563-186">A partir de 1 de junho de 2021, o período de devolução das ofertas de software em CSP, conforme indicado no Microsoft Partner Agreement (MPA), passará de 60 dias da data de encomenda para 30 dias a contar da data da encomenda.</span><span class="sxs-lookup"><span data-stu-id="a8563-186">From June 1, 2021, the return period for software offers in CSP, as stated in the Microsoft Partner Agreement (MPA), will change from 60 days from order date to 30 days from order date.</span></span>

<span data-ttu-id="a8563-187">Após a apresentação de uma encomenda de uma oferta de software, os parceiros terão 30 dias a contar da data da encomenda para submeter quaisquer revisões a tal encomenda:</span><span class="sxs-lookup"><span data-stu-id="a8563-187">After an order for a software offer is submitted, partners will have 30 days from the order date to submit any revisions to such order:</span></span>

- <span data-ttu-id="a8563-188">Qualquer licença de software perpétuo devolvida dentro do período de devolução de 30 dias receberá um crédito total do preço de compra pago.</span><span class="sxs-lookup"><span data-stu-id="a8563-188">Any perpetual software license returned within the 30-day return period will receive a full credit of the paid purchase price.</span></span>

- <span data-ttu-id="a8563-189">Qualquer produto de subscrição de software devolvido dentro do período de devolução de 30 dias receberá um crédito prostimado do preço de compra pago.</span><span class="sxs-lookup"><span data-stu-id="a8563-189">Any software subscription product returned within the 30-day return period will receive a prorated credit of the paid purchase price.</span></span>

<span data-ttu-id="a8563-190">Esta mensagem é um seguimento das nossas comunicações por email enviadas em dezembro de 2020 e abril de 2021 a todos os parceiros da CSP relativamente ao período de devolução e outras atualizações à MPA.</span><span class="sxs-lookup"><span data-stu-id="a8563-190">This message is a follow-up to our email communications sent on December 2020 and April 2021 to all CSP partners regarding the return period and other updates to the MPA.</span></span> <span data-ttu-id="a8563-191">Consulte esses avisos para obter todos os detalhes sobre as alterações que afetam a MPA.</span><span class="sxs-lookup"><span data-stu-id="a8563-191">Refer to those notices for full details regarding changes affecting the MPA.</span></span>

#### <a name="software-download-link-expiry"></a><span data-ttu-id="a8563-192">Expiração do link de descarregamento de software</span><span class="sxs-lookup"><span data-stu-id="a8563-192">Software download link expiry</span></span>

<span data-ttu-id="a8563-193">A partir de 3 de junho de 2021, os links de descarregamento de software para compras perpétuas de software e produtos de subscrição de software através do Partner Center terão uma data de validade de cinco dias a partir do download inicial.</span><span class="sxs-lookup"><span data-stu-id="a8563-193">From June 3, 2021, the software download links for perpetual software and software subscription product purchases through Partner Center will have an expiration date of five days from the initial download.</span></span> <span data-ttu-id="a8563-194">O prazo de validade será aplicável a todas as compras até 3 de junho de 2021, bem como a 3 de junho de 2021.</span><span class="sxs-lookup"><span data-stu-id="a8563-194">The expiry period will apply to all purchases before June 3, 2021, as well as on or after June 3, 2021.</span></span>

### <a name="next-steps"></a><span data-ttu-id="a8563-195">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="a8563-195">Next steps</span></span>

<span data-ttu-id="a8563-196">Reveja o período de devolução do [CSP e o link de descarregamento expirando faQ,](https://partner.microsoft.com/resources/detail/csp-software-return-period-download-expiry-faq-pdf)e informe todas as equipas apropriadas dentro da sua organização destas alterações:</span><span class="sxs-lookup"><span data-stu-id="a8563-196">Review the [CSP return period and download link expiry FAQ](https://partner.microsoft.com/resources/detail/csp-software-return-period-download-expiry-faq-pdf), and inform all appropriate teams within your organization of these changes:</span></span>

### <a name="questions"></a><span data-ttu-id="a8563-197">Perguntas?</span><span class="sxs-lookup"><span data-stu-id="a8563-197">Questions?</span></span>

<span data-ttu-id="a8563-198">Para questões sobre estas ofertas, consulte as suas comunidades Yammer relevantes.</span><span class="sxs-lookup"><span data-stu-id="a8563-198">For questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="open-licensing-program-transitioning-resellers-to-the-cloud-solution-provider-csp-program"></a><a name="7"></a><span data-ttu-id="a8563-199">Programa de Licenciamento Aberto: Revendedores de transição para o programa Cloud Solution Provider (CSP)</span><span class="sxs-lookup"><span data-stu-id="a8563-199">Open Licensing program: Transitioning resellers to the Cloud Solution Provider (CSP) program</span></span>

### <a name="categories"></a><span data-ttu-id="a8563-200">Categorias</span><span class="sxs-lookup"><span data-stu-id="a8563-200">Categories</span></span>

- <span data-ttu-id="a8563-201">Data: 2021-04-19</span><span class="sxs-lookup"><span data-stu-id="a8563-201">Date: 2021-04-19</span></span>
- <span data-ttu-id="a8563-202">Cresça o seu negócio</span><span class="sxs-lookup"><span data-stu-id="a8563-202">Grow Your Business</span></span>

### <a name="summary"></a><span data-ttu-id="a8563-203">Resumo</span><span class="sxs-lookup"><span data-stu-id="a8563-203">Summary</span></span>

<span data-ttu-id="a8563-204">Esta comunicação detalha como se preparar para as alterações que estão para breve no programa open licensing.</span><span class="sxs-lookup"><span data-stu-id="a8563-204">This communication details how to prepare for the changes that are coming soon to the Open Licensing program.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="a8563-205">Audiência impactada</span><span class="sxs-lookup"><span data-stu-id="a8563-205">Impacted audience</span></span>

<span data-ttu-id="a8563-206">CSP e parceiros de Licença Aberta</span><span class="sxs-lookup"><span data-stu-id="a8563-206">CSP and Open License partners</span></span>

### <a name="details"></a><span data-ttu-id="a8563-207">Detalhes</span><span class="sxs-lookup"><span data-stu-id="a8563-207">Details</span></span>

<span data-ttu-id="a8563-208">Em 2020, a Microsoft [anunciou](https://blogs.partner.microsoft.com/mpn/general-availability-of-perpetual-software-licenses-in-the-cloud-solution-provider-program/) que as licenças de software perpétuos estarão amplamente disponíveis para parceiros e clientes através do programa Cloud Solution Provider (CSP).</span><span class="sxs-lookup"><span data-stu-id="a8563-208">In 2020, Microsoft [announced](https://blogs.partner.microsoft.com/mpn/general-availability-of-perpetual-software-licenses-in-the-cloud-solution-provider-program/) that perpetual software licenses will be broadly available to partners and customers through the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="a8563-209">O primeiro marco foi alcançado em janeiro de 2021, quando as ofertas comerciais de software perpétuo ficaram disponíveis.</span><span class="sxs-lookup"><span data-stu-id="a8563-209">The first milestone was reached in January 2021, when commercial perpetual software offers became available.</span></span> <span data-ttu-id="a8563-210">O próximo marco-chave acontecerá em julho de 2021, quando as ofertas do [sector público](https://aka.ms/openlicensepublicsector) ficarem disponíveis.</span><span class="sxs-lookup"><span data-stu-id="a8563-210">The next key milestone will happen in July 2021, when [public sector](https://aka.ms/openlicensepublicsector) offers become available.</span></span> <span data-ttu-id="a8563-211">Também [comunicámos](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) que a partir de 1 de janeiro de 2022, nenhuma nova compra de licença de software ou renovações de Software Assurance ou serviços online pode ser feita através do programa Open License.</span><span class="sxs-lookup"><span data-stu-id="a8563-211">We also [communicated](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) that effective January 1, 2022, no new software license purchases or renewals of Software Assurance or online services can be made through the Open License program.</span></span>

<span data-ttu-id="a8563-212">A transição do software perpétuo para o programa CSP na nova experiência de comércio ajudará os parceiros a expandir as oportunidades para oferecer soluções diversas e serviços geridos.</span><span class="sxs-lookup"><span data-stu-id="a8563-212">The transition of perpetual software to the CSP program in the new commerce experience will help partners to expand the opportunities to offer diverse solutions and managed services.</span></span> <span data-ttu-id="a8563-213">Isto também vai acelerar a transição dos clientes para a nuvem.</span><span class="sxs-lookup"><span data-stu-id="a8563-213">This will also accelerate customers’ transition to the cloud.</span></span>  <span data-ttu-id="a8563-214">Para ajudar a garantir uma transição suave tanto para os nossos parceiros como para os nossos clientes, fizemos estes ajustes e materiais para acelerar esta transformação digital:</span><span class="sxs-lookup"><span data-stu-id="a8563-214">To help ensure a smooth transition for both our partners and customers, we’ve made these adjustments and materials to accelerate this digital transformation:</span></span>

#### <a name="april-2021"></a><span data-ttu-id="a8563-215">abril de 2021</span><span class="sxs-lookup"><span data-stu-id="a8563-215">April 2021</span></span>

<span data-ttu-id="a8563-216">[Disponível:](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/)Abrir materiais de transição licença-csp para revendedores</span><span class="sxs-lookup"><span data-stu-id="a8563-216">[Now available](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/): Open License-to-CSP transition materials for resellers</span></span>

#### <a name="july-2021"></a><span data-ttu-id="a8563-217">julho de 2021</span><span class="sxs-lookup"><span data-stu-id="a8563-217">July 2021</span></span>

##### <a name="csp"></a><span data-ttu-id="a8563-218">CSP</span><span class="sxs-lookup"><span data-stu-id="a8563-218">CSP</span></span>

- <span data-ttu-id="a8563-219">1 de julho: Licenças de software perpétuos disponíveis para clientes do sector público</span><span class="sxs-lookup"><span data-stu-id="a8563-219">July 1: Perpetual software licenses available to public sector customers</span></span>

- <span data-ttu-id="a8563-220">7 de julho: Visual Studio Pro e Obter licenças de software perpétuos do Acordo de Windows genuínas disponíveis para todos os segmentos</span><span class="sxs-lookup"><span data-stu-id="a8563-220">July 7: Visual Studio Pro and Get Genuine Windows Agreement  perpetual software licenses available to all segments</span></span>

##### <a name="open-value"></a><span data-ttu-id="a8563-221">Valor Aberto</span><span class="sxs-lookup"><span data-stu-id="a8563-221">Open Value</span></span>

- <span data-ttu-id="a8563-222">1 de julho: SKUs adicionais disponíveis no programa Open Value para educação e sem fins lucrativos, oferecendo ofertas semelhantes ao programa De Licença Aberta</span><span class="sxs-lookup"><span data-stu-id="a8563-222">July 1: Additional SKUs available in the Open Value program for education and nonprofit, providing similar offers to the Open License program</span></span>

##### <a name="open-license"></a><span data-ttu-id="a8563-223">Licença Aberta</span><span class="sxs-lookup"><span data-stu-id="a8563-223">Open License</span></span>

- <span data-ttu-id="a8563-224">1 de julho: A Microsoft deixará de lançar novas ofertas no programa Open License.</span><span class="sxs-lookup"><span data-stu-id="a8563-224">July 1: Microsoft will no longer launch new offers in the Open License program.</span></span>

#### <a name="january-2022"></a><span data-ttu-id="a8563-225">janeiro de 2022</span><span class="sxs-lookup"><span data-stu-id="a8563-225">January 2022</span></span>

- <span data-ttu-id="a8563-226">1 de janeiro: Não podem ser feitas novas compras ou renovações através do programa Licença Aberta</span><span class="sxs-lookup"><span data-stu-id="a8563-226">January 1: No new purchases or renewals can be made through the Open License program</span></span>

### <a name="next-steps"></a><span data-ttu-id="a8563-227">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="a8563-227">Next steps</span></span>

#### <a name="csp-indirect-providers"></a><span data-ttu-id="a8563-228">Fornecedores indiretos da CSP</span><span class="sxs-lookup"><span data-stu-id="a8563-228">CSP indirect providers</span></span>

<span data-ttu-id="a8563-229">Utilize os próximos meses para ajudar os revendedores open license orientando para o programa CSP, assistindo a eventos comunitários parceiros e usando os materiais de transição Open License-to-CSP para revendedores:</span><span class="sxs-lookup"><span data-stu-id="a8563-229">Use the coming months to help Open License resellers orient into the CSP program by attending partner community events and using the Open License-to-CSP transition materials for resellers:</span></span>

- <span data-ttu-id="a8563-230">[Abra materiais de transição licença-para-CSP para revendedores](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/)— Apresentação geral personalizável, modelo de e-mail, guia de revendedor indireto CSP e muito mais para ajudá-lo a conduzir a adoção para os seus revendedores em escala.</span><span class="sxs-lookup"><span data-stu-id="a8563-230">[Open License-to-CSP transition materials for resellers](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/)—Customizable overview presentation, email template, CSP indirect reseller onboarding guide, and more to help you drive the adoption for your resellers at scale.</span></span>

- <span data-ttu-id="a8563-231">[CSP Partner Community Events](https://globalpbocomm.eventbuilder.com/GlobalCSP) organizados pela Microsoft Business Operations.</span><span class="sxs-lookup"><span data-stu-id="a8563-231">[CSP Partner Community Events](https://globalpbocomm.eventbuilder.com/GlobalCSP) hosted by Microsoft Business Operations.</span></span>  <span data-ttu-id="a8563-232">Junte-se às várias sessões para aprender básicos de CSP (CSP Fundamentals) ou ficar atualizado, e fazer perguntas sobre Software em CSP (Q&A Sessions).</span><span class="sxs-lookup"><span data-stu-id="a8563-232">Join the various sessions to learn CSP basics (CSP Fundamentals) or stay up to date, and ask questions regarding Software in CSP (Q&A Sessions).</span></span>

- <span data-ttu-id="a8563-233">(Em breve) Sessão de formação centrada no revendedor indireto da CSP, organizada pela Microsoft Business Operations.</span><span class="sxs-lookup"><span data-stu-id="a8563-233">(Coming soon) CSP indirect reseller–focused training session hosted by Microsoft Business Operations.</span></span>

#### <a name="open-license-resellers"></a><span data-ttu-id="a8563-234">Revendedores de Licença Aberta</span><span class="sxs-lookup"><span data-stu-id="a8563-234">Open License resellers</span></span>

- <span data-ttu-id="a8563-235">Se a sua organização não estiver atualmente inscrita no programa CSP, contacte o seu distribuidor para obter informações sobre como começar.</span><span class="sxs-lookup"><span data-stu-id="a8563-235">If your organization isn’t currently enrolled in the CSP program, contact your distributor for information on how to get started.</span></span> <span data-ttu-id="a8563-236">Conecte-se com um fornecedor indireto [aqui.](https://partner.microsoft.com/membership/cloud-solution-provider/find-a-provider)</span><span class="sxs-lookup"><span data-stu-id="a8563-236">Connect with an indirect provider [here](https://partner.microsoft.com/membership/cloud-solution-provider/find-a-provider).</span></span>

- <span data-ttu-id="a8563-237">Se a sua organização já está inscrita no programa CSP, saiba mais sobre software perpétuo em CSP [aqui.](https://partner.microsoft.com/resources/collection/software-in-csp)</span><span class="sxs-lookup"><span data-stu-id="a8563-237">If your organization is already enrolled in the CSP program, learn more about perpetual software in CSP [here](https://partner.microsoft.com/resources/collection/software-in-csp).</span></span>

### <a name="questions"></a><span data-ttu-id="a8563-238">Perguntas?</span><span class="sxs-lookup"><span data-stu-id="a8563-238">Questions?</span></span>

<span data-ttu-id="a8563-239">Para mais perguntas sobre estas ofertas, consulte as suas comunidades Yammer relevantes.</span><span class="sxs-lookup"><span data-stu-id="a8563-239">For further questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="now-live-global-promo-readiness-guide"></a><a name="6"></a><span data-ttu-id="a8563-240">Agora ao vivo: Guia global de prontidão promocional</span><span class="sxs-lookup"><span data-stu-id="a8563-240">Now live: Global promo readiness guide</span></span>

### <a name="categories"></a><span data-ttu-id="a8563-241">Categorias</span><span class="sxs-lookup"><span data-stu-id="a8563-241">Categories</span></span>

- <span data-ttu-id="a8563-242">Data: 2021-04-16</span><span class="sxs-lookup"><span data-stu-id="a8563-242">Date: 2021-04-16</span></span>
- <span data-ttu-id="a8563-243">Capacidades</span><span class="sxs-lookup"><span data-stu-id="a8563-243">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="a8563-244">Resumo</span><span class="sxs-lookup"><span data-stu-id="a8563-244">Summary</span></span>

<span data-ttu-id="a8563-245">A Prontidão de Lançamento publicou um novo [guia global de prontidão promocional](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) na galeria de recursos de prontidão de operações.</span><span class="sxs-lookup"><span data-stu-id="a8563-245">Launch Readiness has published a new [global promo readiness guide](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) on the Operations Readiness resource gallery.</span></span> <span data-ttu-id="a8563-246">Este guia proporciona uma visão consolidada de todas as [promoções globais ativas.](https://partner.microsoft.com/resources/collection/global-promo-readiness-guide-collection#/)</span><span class="sxs-lookup"><span data-stu-id="a8563-246">This guide provides a consolidated view of all active [global promotions](https://partner.microsoft.com/resources/collection/global-promo-readiness-guide-collection#/).</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="a8563-247">Audiência impactada</span><span class="sxs-lookup"><span data-stu-id="a8563-247">Impacted audience</span></span>

<span data-ttu-id="a8563-248">Todos os parceiros de Licenciamento de Volume (VL), Dynamics Price List (DPL) e Cloud Solution Provider (CSP)</span><span class="sxs-lookup"><span data-stu-id="a8563-248">All Volume Licensing (VL), Dynamics Price List (DPL), and Cloud Solution Provider (CSP) partners</span></span>

### <a name="details"></a><span data-ttu-id="a8563-249">Detalhes</span><span class="sxs-lookup"><span data-stu-id="a8563-249">Details</span></span>

<span data-ttu-id="a8563-250">Os parceiros da Microsoft partilharam connosco a necessidade de fornecer uma visão consolidada de todas as promoções globais com detalhes de suporte.</span><span class="sxs-lookup"><span data-stu-id="a8563-250">Microsoft partners have shared with us the need to provide a consolidated view of all global promotions with supporting details.</span></span> <span data-ttu-id="a8563-251">Você queria este guia consolidado para ajudá-lo a usar promoções com a confiança de que toda a informação disponível será facilmente acessível em um local central e conveniente.</span><span class="sxs-lookup"><span data-stu-id="a8563-251">You wanted this consolidated guide to help you use promotions with the confidence that all the available information will be readily accessible in a central and convenient location.</span></span>

<span data-ttu-id="a8563-252">A partir de abril de 2021, a Microsoft atualizará este guia mensalmente, estando disponível numa coleção dedicada global promo promoinginess Guide na galeria de recursos de prontidão de operações.</span><span class="sxs-lookup"><span data-stu-id="a8563-252">Beginning in April 2021, Microsoft will update this guide on a monthly basis, and it will be available in a dedicated Global Promo Readiness Guide collection in the Operations Readiness resource gallery.</span></span>

<span data-ttu-id="a8563-253">As ligações a este guia também serão incluídas nas seguintes coleções:</span><span class="sxs-lookup"><span data-stu-id="a8563-253">Links to this guide will also be included in the following collections:</span></span>

- <span data-ttu-id="a8563-254">[A coleção de calendário](https://partner.microsoft.com/resources/collection/csp-announcement-calendar#/)de lançamento, que proporciona uma visão centralizada das próximas mudanças e lançamentos.</span><span class="sxs-lookup"><span data-stu-id="a8563-254">[Launch calendar collection](https://partner.microsoft.com/resources/collection/csp-announcement-calendar#/), which provides a centralized view of upcoming changes and launches.</span></span>

- <span data-ttu-id="a8563-255">[Coleções comunitárias](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/), que contêm materiais de apoio para as nossas chamadas mensais de parceiros, destacando as próximas mudanças e temas oportunos de interesse operacional.</span><span class="sxs-lookup"><span data-stu-id="a8563-255">[Community collections](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/), which contain supporting materials for our monthly partner calls, highlighting upcoming changes and timely topics of operational interest.</span></span>

- <span data-ttu-id="a8563-256">[Newsletters de parceiros](https://partner.microsoft.com/resources/collection/csp-monthly-update#/), tais como CSP Monthly Update</span><span class="sxs-lookup"><span data-stu-id="a8563-256">[Partner newsletters](https://partner.microsoft.com/resources/collection/csp-monthly-update#/), such as CSP Monthly Update</span></span>

<span data-ttu-id="a8563-257">Como lembrete mensal, também publicaremos um anúncio do Partner Center com cada nova edição do guia global de prontidão promocional.</span><span class="sxs-lookup"><span data-stu-id="a8563-257">As a monthly reminder, we will also publish a Partner Center announcement with each new issue of the global promo readiness guide.</span></span>

### <a name="next-steps"></a><span data-ttu-id="a8563-258">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="a8563-258">Next steps</span></span>

<span data-ttu-id="a8563-259">No início de cada mês, encontrará o mais recente [guia global de prontidão promocional](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) na galeria de recursos de [prontidão de operações.](https://partner.microsoft.com/resources)</span><span class="sxs-lookup"><span data-stu-id="a8563-259">At the start of each month, you will find the latest [global promo readiness guide](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) in the [Operations Readiness resource gallery](https://partner.microsoft.com/resources).</span></span>

<span data-ttu-id="a8563-260">Partilhe esta informação com os contactos adequados nas suas organizações e informe-nos de quão útil o guia é através do "Foi útil esta página?"</span><span class="sxs-lookup"><span data-stu-id="a8563-260">Share this information with the appropriate contacts in your organizations and let us know how helpful the guide is through the “Was this page helpful?”</span></span> <span data-ttu-id="a8563-261">botão no final de cada página.</span><span class="sxs-lookup"><span data-stu-id="a8563-261">button at the end of each page.</span></span>

________________
## <a name="april-cloud-solution-provider-csp-community-update-and-reminders"></a><a name="5"></a><span data-ttu-id="a8563-262">Atualização e lembretes da comunidade April Cloud Solution Provider (CSP)</span><span class="sxs-lookup"><span data-stu-id="a8563-262">April Cloud Solution Provider (CSP) community update and reminders</span></span>

### <a name="categories"></a><span data-ttu-id="a8563-263">Categorias</span><span class="sxs-lookup"><span data-stu-id="a8563-263">Categories</span></span>

- <span data-ttu-id="a8563-264">Data: 2021-04-16</span><span class="sxs-lookup"><span data-stu-id="a8563-264">Date: 2021-04-16</span></span>
- <span data-ttu-id="a8563-265">| comunitários Convites e lembretes</span><span class="sxs-lookup"><span data-stu-id="a8563-265">Community | Invites and reminders</span></span>

### <a name="summary"></a><span data-ttu-id="a8563-266">Resumo</span><span class="sxs-lookup"><span data-stu-id="a8563-266">Summary</span></span>

<span data-ttu-id="a8563-267">Os recursos comunitários da CSP estão disponíveis a pedido e atualizados mensalmente para mantê-lo informado e preparado para a mudança no programa CSP.</span><span class="sxs-lookup"><span data-stu-id="a8563-267">CSP community resources are available on demand and updated monthly to keep you informed and prepared for change in the CSP program.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="a8563-268">Audiência impactada</span><span class="sxs-lookup"><span data-stu-id="a8563-268">Impacted audience</span></span>

<span data-ttu-id="a8563-269">Parceiros de conta direta da CSP e fornecedores indiretos</span><span class="sxs-lookup"><span data-stu-id="a8563-269">CSP direct bill partners and indirect providers</span></span>

### <a name="details"></a><span data-ttu-id="a8563-270">Detalhes</span><span class="sxs-lookup"><span data-stu-id="a8563-270">Details</span></span>

<span data-ttu-id="a8563-271">Este mês, os recursos incluem os seguintes tópicos-chave:</span><span class="sxs-lookup"><span data-stu-id="a8563-271">This month, the resources include the following key topics:</span></span>

- [<span data-ttu-id="a8563-272">Atualização para evolução do programa CSP e alterações do programa Open License</span><span class="sxs-lookup"><span data-stu-id="a8563-272">Update to CSP program evolution and Open License program changes</span></span>](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/)

- [<span data-ttu-id="a8563-273">Alterações aos requisitos de embarque de clientes da CSP em determinadas regiões</span><span class="sxs-lookup"><span data-stu-id="a8563-273">Changes to CSP customer onboarding requirements in certain regions</span></span>](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/)

- [<span data-ttu-id="a8563-274">Novo formato para a nova fatura PDF do comércio no programa CSP</span><span class="sxs-lookup"><span data-stu-id="a8563-274">New format for the new commerce PDF invoice in the CSP program</span></span>](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/)

<span data-ttu-id="a8563-275">Dentro da [coleção comunitária CSP,](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/)você encontrará:</span><span class="sxs-lookup"><span data-stu-id="a8563-275">Within the [CSP community collection](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/), you’ll find:</span></span>

- <span data-ttu-id="a8563-276">A [newsletter de Atualização Mensal da CSP,](https://partner.microsoft.com/resources/detail/csp-monthly-update-april-2021-global)que agrega anúncios, atualizações, eventos e lembretes recentes num documento de fácil leitura.</span><span class="sxs-lookup"><span data-stu-id="a8563-276">The downloadable [CSP Monthly Update newsletter](https://partner.microsoft.com/resources/detail/csp-monthly-update-april-2021-global), which aggregates recent CSP announcements, updates, events, and reminders in an easy-to-read document.</span></span>

- <span data-ttu-id="a8563-277">O [Calendário de Anúncios da CSP,](https://partner.microsoft.com/resources/detail/csp-announcement-calendar-april-2021)que fornece uma visão de linha do tempo das próximas alterações que afetam o programa.</span><span class="sxs-lookup"><span data-stu-id="a8563-277">The [CSP Announcement Calendar](https://partner.microsoft.com/resources/detail/csp-announcement-calendar-april-2021), which provides a timeline view of upcoming changes affecting the program.</span></span>

- <span data-ttu-id="a8563-278">O novo [calendário de lançamento do produto,](https://partner.microsoft.com/resources/detail/product-launch-calendar-april-pdf)onde pode ver os próximos lançamentos e ofertas de produtos.</span><span class="sxs-lookup"><span data-stu-id="a8563-278">The new [product launch calendar](https://partner.microsoft.com/resources/detail/product-launch-calendar-april-pdf), where you can view upcoming product launches and offers.</span></span>

- <span data-ttu-id="a8563-279">[A CSP lança recursos](https://partner.microsoft.com/resources/collection/april-2021-csp-launch-topics-collection#/) de atualização com conteúdo fácil de consumir em mudanças operacionais chave.</span><span class="sxs-lookup"><span data-stu-id="a8563-279">[CSP launch update resources](https://partner.microsoft.com/resources/collection/april-2021-csp-launch-topics-collection#/) with easy-to-consume content on key operational changes.</span></span>

- <span data-ttu-id="a8563-280">[Refreshers e lembretes](https://partner.microsoft.com/resources/detail/csp-april-2021-refreshers-and-reminders-pdf) sobre os principais tópicos da CSP que recebem interesse e consultas.</span><span class="sxs-lookup"><span data-stu-id="a8563-280">[Refreshers and reminders](https://partner.microsoft.com/resources/detail/csp-april-2021-refreshers-and-reminders-pdf) on key CSP topics receiving interest and queries.</span></span>

#### <a name="csp-community-call-qas"></a><span data-ttu-id="a8563-281">CSP Community Call Q&As</span><span class="sxs-lookup"><span data-stu-id="a8563-281">CSP Community Call Q&As</span></span>

<span data-ttu-id="a8563-282">A Chamada Comunitária Q&Como estão disponíveis para o ajudar com questões relacionadas com as próximas alterações.</span><span class="sxs-lookup"><span data-stu-id="a8563-282">Community Call Q&As are available to help you with questions related to upcoming changes.</span></span> <span data-ttu-id="a8563-283">Registe-se agora para a CSP Community Call Q&Tal como está a decorrer em abril, maio e junho.</span><span class="sxs-lookup"><span data-stu-id="a8563-283">Register now for CSP Community Call Q&As that are taking place in April, May, and June.</span></span> <span data-ttu-id="a8563-284">Estes irão focar-se nos mais recentes lançamentos, atualizações importantes e lembretes.</span><span class="sxs-lookup"><span data-stu-id="a8563-284">These will focus on the latest launches, important refreshers, and reminders.</span></span>

<span data-ttu-id="a8563-285">[Registe-se aqui.](https://globalpbocomm.eventbuilder.com/GlobalCSP)</span><span class="sxs-lookup"><span data-stu-id="a8563-285">[Register here](https://globalpbocomm.eventbuilder.com/GlobalCSP).</span></span>

### <a name="next-steps"></a><span data-ttu-id="a8563-286">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="a8563-286">Next steps</span></span>

<span data-ttu-id="a8563-287">Reveja os recursos comunitários e registe-se para a Chamada Comunitária Q&A.</span><span class="sxs-lookup"><span data-stu-id="a8563-287">Review the community resources and register for the Community Call Q&A.</span></span>

<span data-ttu-id="a8563-288">Para garantir que obtém o máximo da Chamada Comunitária Q&A, reveja o conteúdo da comunidade a pedido e envie as suas perguntas até 48 horas antes da chamada.</span><span class="sxs-lookup"><span data-stu-id="a8563-288">To ensure that you get the most from the Community Call Q&A, review the on-demand community content and submit your questions up to 48 hours before the call.</span></span>

### <a name="questions"></a><span data-ttu-id="a8563-289">Perguntas?</span><span class="sxs-lookup"><span data-stu-id="a8563-289">Questions?</span></span>

<span data-ttu-id="a8563-290">A chamada comunitária mensal CSP Q&A é o melhor local para questões relacionadas com alterações no programa CSP.</span><span class="sxs-lookup"><span data-stu-id="a8563-290">The monthly CSP Community Call Q&A is the best place for questions related to changes in the CSP program.</span></span> <span data-ttu-id="a8563-291">Todos os meses, reveja o material e envie as suas perguntas com antecedência para que possamos passar a sessão sobre os tópicos que são mais importantes para si.</span><span class="sxs-lookup"><span data-stu-id="a8563-291">Each month, review the material and submit your questions in advance so that we can spend the session on the topics that are most important to you.</span></span>

<span data-ttu-id="a8563-292">Para mais informações, contacte [o Suporte.](https://partner.microsoft.com/dashboard/support/csp/servicerequests/create?category=csp)</span><span class="sxs-lookup"><span data-stu-id="a8563-292">For more information, contact [Support](https://partner.microsoft.com/dashboard/support/csp/servicerequests/create?category=csp).</span></span>

________________
## <a name="final-reminder-deprecation-of-get-qualification-on-may-6-2021"></a><a name="4"></a><span data-ttu-id="a8563-293">Lembrete final: Depreciação da qualificação do GET em 6 de maio de 2021</span><span class="sxs-lookup"><span data-stu-id="a8563-293">Final reminder: Deprecation of GET qualification on May 6, 2021</span></span>

### <a name="categories"></a><span data-ttu-id="a8563-294">Categorias</span><span class="sxs-lookup"><span data-stu-id="a8563-294">Categories</span></span>

- <span data-ttu-id="a8563-295">Data: 2021-05-04</span><span class="sxs-lookup"><span data-stu-id="a8563-295">Date: 2021-05-04</span></span>

- <span data-ttu-id="a8563-296">Capacidades</span><span class="sxs-lookup"><span data-stu-id="a8563-296">Capabilities</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="a8563-297">Audiência impactada</span><span class="sxs-lookup"><span data-stu-id="a8563-297">Impacted audience</span></span>

<span data-ttu-id="a8563-298">Parceiros que vendem ofertas académicas, sem fins lucrativos e comunidade governamental (GCC) através do programa Cloud Solution Provider utilizando a API do Partner Center</span><span class="sxs-lookup"><span data-stu-id="a8563-298">Partners selling Academic, Nonprofit, and Government Community Cloud (GCC) offers through the Cloud Solution Provider program using the Partner Center API</span></span>

### <a name="details"></a><span data-ttu-id="a8563-299">Detalhes</span><span class="sxs-lookup"><span data-stu-id="a8563-299">Details</span></span>

<span data-ttu-id="a8563-300">Este anúncio é um seguimento das melhorias do Partner Center [lançadas em dezembro.](./2020-december.md#1)</span><span class="sxs-lookup"><span data-stu-id="a8563-300">This announcement is a follow-up to the Partner Center [enhancements released in December](./2020-december.md#1).</span></span> <span data-ttu-id="a8563-301">Como parte desse lançamento, foram implementadas novas APIs get e post qualifications e, consequentemente, **a qualificação get existente será aposentada no dia 6 de maio de 2021**.</span><span class="sxs-lookup"><span data-stu-id="a8563-301">As part of that release, new GET and POST Qualifications APIs were deployed and, as a result, **the existing GET qualification will be retired on May 6, 2021**.</span></span> <span data-ttu-id="a8563-302">Nessa altura, terás de te ter transitado para usar as novas APIs do Post Partner Center.</span><span class="sxs-lookup"><span data-stu-id="a8563-302">By that time, you will need to have transitioned to using the new POST Partner Center APIs.</span></span> <span data-ttu-id="a8563-303">As novas APIs post permitir-lhe-ão adquirir ofertas de Educação, enquanto as novas APIs GET permitir-lhe-ão adquirir ofertas pré-qualificadas sem fins lucrativos e GCC.</span><span class="sxs-lookup"><span data-stu-id="a8563-303">The new POST APIs will enable you to purchase Education offers, while the new GET APIs will enable you to purchase pre-qualified Nonprofit and GCC offers.</span></span>

### <a name="next-steps"></a><span data-ttu-id="a8563-304">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="a8563-304">Next steps</span></span>

- <span data-ttu-id="a8563-305">**Atualize as novas APIs** para uma transição bem sucedida e oportuna.</span><span class="sxs-lookup"><span data-stu-id="a8563-305">**Update to the new APIs** for a successful and timely transition.</span></span>

- <span data-ttu-id="a8563-306">**Reveja as novas alterações e guia** do Centro de Parceiros na API nos recursos de prontidão de operações: [Melhorias do processo de validação do processo de validação do cliente do Partner Center Education](https://partner.microsoft.com/resources/collection/partner-center-edu-validation-enhancements#/).</span><span class="sxs-lookup"><span data-stu-id="a8563-306">**Review the new Partner Center API changes and Guide** in the Operations Readiness resources: [Partner Center Education customer validation process enhancements](https://partner.microsoft.com/resources/collection/partner-center-edu-validation-enhancements#/).</span></span>

- <span data-ttu-id="a8563-307">Partilhe esta informação com as equipas apropriadas dentro da sua organização e com os seus revendedores para ajudá-los a prepararem-se para estas mudanças.</span><span class="sxs-lookup"><span data-stu-id="a8563-307">Share this information with the appropriate teams within your organization and with your resellers to help them prepare for these changes.</span></span>

### <a name="questions"></a><span data-ttu-id="a8563-308">Perguntas?</span><span class="sxs-lookup"><span data-stu-id="a8563-308">Questions?</span></span>

<span data-ttu-id="a8563-309">Para quaisquer questões relacionadas com esta notificação, contacte [o Suporte do Centro de Parceiros](https://partner.microsoft.com/dashboard/support/referrals/servicerequests?category=referrals).</span><span class="sxs-lookup"><span data-stu-id="a8563-309">For any questions related to this notification, contact [Partner Center support](https://partner.microsoft.com/dashboard/support/referrals/servicerequests?category=referrals).</span></span>

### <a name="change-log"></a><span data-ttu-id="a8563-310">Change log</span><span class="sxs-lookup"><span data-stu-id="a8563-310">Change log</span></span>

- <span data-ttu-id="a8563-311">4 de maio de 2021: Lembrete final da próxima depreciação da qualificação do GET</span><span class="sxs-lookup"><span data-stu-id="a8563-311">May 4, 2021: Final reminder of upcoming deprecation of GET qualification</span></span>

- <span data-ttu-id="a8563-312">9 de abril de 2021: Lembrete da próxima depreciação da qualificação do GET</span><span class="sxs-lookup"><span data-stu-id="a8563-312">April 9, 2021: Reminder of upcoming deprecation of GET qualification</span></span> 

- <span data-ttu-id="a8563-313">Fevereiro: Prazos atualizados para depreciação das qualificações GET & PUT</span><span class="sxs-lookup"><span data-stu-id="a8563-313">February: Updated timelines for deprecation of GET & PUT qualifications</span></span>

- <span data-ttu-id="a8563-314">Janeiro: Lembrete das próximas depreciações das qualificações GET & PUT</span><span class="sxs-lookup"><span data-stu-id="a8563-314">January: Reminder of upcoming deprecations of GET & PUT qualifications</span></span>

________________
## <a name="new-format-for-the-new-commerce-pdf-invoice-in-csp"></a><a name="3"></a><span data-ttu-id="a8563-315">Novo formato para o novo comércio fatura PDF em CSP</span><span class="sxs-lookup"><span data-stu-id="a8563-315">New format for the new commerce PDF invoice in CSP</span></span>

### <a name="categories"></a><span data-ttu-id="a8563-316">Categorias</span><span class="sxs-lookup"><span data-stu-id="a8563-316">Categories</span></span>

- <span data-ttu-id="a8563-317">Data: 2021-04-05</span><span class="sxs-lookup"><span data-stu-id="a8563-317">Date: 2021-04-05</span></span>
- <span data-ttu-id="a8563-318">Capacidades</span><span class="sxs-lookup"><span data-stu-id="a8563-318">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="a8563-319">Resumo</span><span class="sxs-lookup"><span data-stu-id="a8563-319">Summary</span></span>

<span data-ttu-id="a8563-320">A Microsoft está a introduzir um novo formato para a nova fatura PDF do comércio no programa Cloud Solution Provider (CSP) para apresentar detalhes de faturação por detalhes do produto em vez da descrição do SKU.</span><span class="sxs-lookup"><span data-stu-id="a8563-320">Microsoft is introducing a new format for the new commerce PDF invoice in the Cloud Solution Provider (CSP) program to display billing details by product detail instead of SKU description.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="a8563-321">Audiência impactada</span><span class="sxs-lookup"><span data-stu-id="a8563-321">Impacted audience</span></span>

<span data-ttu-id="a8563-322">Parceiros transacionando através do programa CSP</span><span class="sxs-lookup"><span data-stu-id="a8563-322">Partners transacting through the CSP program</span></span>

### <a name="details"></a><span data-ttu-id="a8563-323">Detalhes</span><span class="sxs-lookup"><span data-stu-id="a8563-323">Details</span></span>

<span data-ttu-id="a8563-324">A partir de maio de 2021, a Microsoft está a introduzir um novo formato para a nova fatura PDF do comércio no programa CSP para apresentar detalhes de faturação por detalhes do produto em vez da descrição do SKU.</span><span class="sxs-lookup"><span data-stu-id="a8563-324">Starting May 2021, Microsoft is introducing a new format for the new commerce PDF invoice in the CSP program to display billing details by product detail instead of SKU description.</span></span> <span data-ttu-id="a8563-325">Com esta nova atualização, vamos agregar os itens de linha por tipo de produto enquanto exibimos todos os produtos numa linha individual.</span><span class="sxs-lookup"><span data-stu-id="a8563-325">With this new update, we will be aggregating the line items by product type while displaying every product on an individual line.</span></span>

<span data-ttu-id="a8563-326">Os parceiros vão notar esta alteração que entra em vigor na sua fatura de maio para o período de faturação entre 1 de abril de 2021 e 30 de abril de 2021.</span><span class="sxs-lookup"><span data-stu-id="a8563-326">Partners will notice this change coming into effect in their May invoice for the billing period between April 1, 2021 and April 30, 2021.</span></span> <span data-ttu-id="a8563-327">As ofertas afetadas são a Microsoft Azure Reserved Instance, as subscrições Azure (plano Azure) e o Marketplace.</span><span class="sxs-lookup"><span data-stu-id="a8563-327">The affected offers are Microsoft Azure Reserved Instance, Azure subscriptions (Azure plan), and Marketplace.</span></span>

<span data-ttu-id="a8563-328">Quaisquer pedidos de crédito-rebill feitos após a atualização do formato da fatura serão gerados no novo formato.</span><span class="sxs-lookup"><span data-stu-id="a8563-328">Any credit-rebill requests made after the invoice format has been updated will be generated in the new format.</span></span>

#### <a name="partner-benefits"></a><span data-ttu-id="a8563-329">Benefícios do parceiro</span><span class="sxs-lookup"><span data-stu-id="a8563-329">Partner benefits</span></span>

<span data-ttu-id="a8563-330">Esta atualização irá oferecer as seguintes melhorias à experiência de faturação para os parceiros:</span><span class="sxs-lookup"><span data-stu-id="a8563-330">This update will offer the following improvements to the invoicing experience for partners:</span></span>

- <span data-ttu-id="a8563-331">Tamanho da fatura reduzida ao mesmo tempo que retém dados críticos</span><span class="sxs-lookup"><span data-stu-id="a8563-331">Reduced invoice size while retaining critical data</span></span>

- <span data-ttu-id="a8563-332">Alinhamento do formato aos padrões da indústria para faturas compactas e fáceis de utilizar</span><span class="sxs-lookup"><span data-stu-id="a8563-332">Alignment of the format to the industry standards for compact and user-friendly invoices</span></span> 

<span data-ttu-id="a8563-333">Os seguintes elementos não serão afetados:</span><span class="sxs-lookup"><span data-stu-id="a8563-333">The following elements will not be affected:</span></span>

- <span data-ttu-id="a8563-334">Página de resumo de faturação na fatura PDF</span><span class="sxs-lookup"><span data-stu-id="a8563-334">Billing summary page on the invoice PDF</span></span>

- <span data-ttu-id="a8563-335">APIs de faturação existentes</span><span class="sxs-lookup"><span data-stu-id="a8563-335">Existing invoicing APIs</span></span>

- <span data-ttu-id="a8563-336">Ficheiros de reconciliação (os ficheiros Recon podem ser utilizados para recuperar dados granulares.)</span><span class="sxs-lookup"><span data-stu-id="a8563-336">Reconciliation files (Recon files can be used for retrieving granular data.)</span></span> 

- <span data-ttu-id="a8563-337">Faturas de encargos baseadas em licenças e de utilização</span><span class="sxs-lookup"><span data-stu-id="a8563-337">Usage and license-based charges invoices</span></span>

### <a name="next-steps"></a><span data-ttu-id="a8563-338">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="a8563-338">Next steps</span></span>

<span data-ttu-id="a8563-339">Reveja as informações sobre este tópico na [galeria de recursos de prontidão de operações](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/) no site do parceiro da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="a8563-339">Review the information about this topic in the [Operations Readiness resource gallery](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/) on the Microsoft partner website.</span></span> <span data-ttu-id="a8563-340">Para mais informações sobre faturação e tópicos fiscais, incluindo recursos de faturação, faturas, faturação de CSP e impostos, visite [a secção de Faturação](../billing.md) no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="a8563-340">For more information about billing and tax topics including billing resources, invoices, CSP billing, and taxes, visit the [Billing section](../billing.md) in Partner Center.</span></span>

________________
## <a name="changes-to-the-cloud-solution-provider-csp-customer-onboarding-requirements"></a><a name="2"></a><span data-ttu-id="a8563-341">Alterações aos requisitos de embarque do fornecedor de solução cloud (CSP)</span><span class="sxs-lookup"><span data-stu-id="a8563-341">Changes to the Cloud Solution Provider (CSP) customer onboarding requirements</span></span>

### <a name="categories"></a><span data-ttu-id="a8563-342">Categorias</span><span class="sxs-lookup"><span data-stu-id="a8563-342">Categories</span></span>

- <span data-ttu-id="a8563-343">Data: 2021-04-02</span><span class="sxs-lookup"><span data-stu-id="a8563-343">Date: 2021-04-02</span></span>
- <span data-ttu-id="a8563-344">Ofertas/Mercados</span><span class="sxs-lookup"><span data-stu-id="a8563-344">Offers/Markets</span></span>

### <a name="summary"></a><span data-ttu-id="a8563-345">Resumo</span><span class="sxs-lookup"><span data-stu-id="a8563-345">Summary</span></span>

<span data-ttu-id="a8563-346">Como parte do nosso compromisso de ajudar parceiros e clientes a gerir o seu negócio com base na confiança, vamos solicitar informações adicionais ao cliente, a partir de 25 de março de 2021.</span><span class="sxs-lookup"><span data-stu-id="a8563-346">As part of our commitment to help partners and customers run their business based on trust, we will request additional customer information, effective March 25, 2021.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="a8563-347">Audiência impactada</span><span class="sxs-lookup"><span data-stu-id="a8563-347">Impacted audience</span></span>

<span data-ttu-id="a8563-348">Parceiros de conta direta da CSP e fornecedores indiretos que tenham clientes novos ou existentes nos países listados na secção seguinte</span><span class="sxs-lookup"><span data-stu-id="a8563-348">CSP direct bill partners and indirect providers who have new or existing customers in the countries listed in the next section</span></span>

### <a name="details"></a><span data-ttu-id="a8563-349">Detalhes</span><span class="sxs-lookup"><span data-stu-id="a8563-349">Details</span></span>

<span data-ttu-id="a8563-350">A Microsoft tem confiança.</span><span class="sxs-lookup"><span data-stu-id="a8563-350">Microsoft runs on trust.</span></span> <span data-ttu-id="a8563-351">Estamos empenhados em fornecer um método de validação de clientes conforme, seguro e seguro para a transação de subscrições de clientes no programa CSP.</span><span class="sxs-lookup"><span data-stu-id="a8563-351">We’re committed to providing a compliant, safe, and secure method of customer validation for transacting customer subscriptions in the CSP program.</span></span> <span data-ttu-id="a8563-352">No dia 25 de março de 2021, apresentaremos melhorias no Partner Center API e na interface de utilizador (UI) que afetarão os parceiros que cumprem ambos os seguintes critérios:</span><span class="sxs-lookup"><span data-stu-id="a8563-352">On March 25, 2021, we will be introducing Partner Center API and user interface (UI) enhancements that will affect partners who meet both of the following criteria:</span></span>

- <span data-ttu-id="a8563-353">O parceiro tem uma relação de faturação direta com a Microsoft (o que significa que o parceiro é ou um parceiro de conta direta ou um fornecedor indireto).</span><span class="sxs-lookup"><span data-stu-id="a8563-353">The partner has a direct billing relationship with Microsoft (which means that the partner is either a direct bill partner or an indirect provider).</span></span>

- <span data-ttu-id="a8563-354">O parceiro negoceia com clientes novos ou existentes nos seguintes países:</span><span class="sxs-lookup"><span data-stu-id="a8563-354">The partner does business with new or existing customers in the following countries:</span></span>

    - <span data-ttu-id="a8563-355">Tailândia</span><span class="sxs-lookup"><span data-stu-id="a8563-355">Thailand</span></span>
    - <span data-ttu-id="a8563-356">Vietname</span><span class="sxs-lookup"><span data-stu-id="a8563-356">Vietnam</span></span>
    - <span data-ttu-id="a8563-357">Turquia</span><span class="sxs-lookup"><span data-stu-id="a8563-357">Turkey</span></span>
    - <span data-ttu-id="a8563-358">Polónia</span><span class="sxs-lookup"><span data-stu-id="a8563-358">Poland</span></span>
    - <span data-ttu-id="a8563-359">África do Sul</span><span class="sxs-lookup"><span data-stu-id="a8563-359">South Africa</span></span>
    - <span data-ttu-id="a8563-360">Índia</span><span class="sxs-lookup"><span data-stu-id="a8563-360">India</span></span>
    - <span data-ttu-id="a8563-361">Brasil</span><span class="sxs-lookup"><span data-stu-id="a8563-361">Brazil</span></span>
    - <span data-ttu-id="a8563-362">Iraque</span><span class="sxs-lookup"><span data-stu-id="a8563-362">Iraq</span></span>
    - <span data-ttu-id="a8563-363">Mianmar</span><span class="sxs-lookup"><span data-stu-id="a8563-363">Myanmar</span></span>
    - <span data-ttu-id="a8563-364">Sudão do Sul</span><span class="sxs-lookup"><span data-stu-id="a8563-364">South Sudan</span></span>
    - <span data-ttu-id="a8563-365">Arábia Saudita</span><span class="sxs-lookup"><span data-stu-id="a8563-365">Saudi Arabia</span></span>
    - <span data-ttu-id="a8563-366">Emirados Árabes Unidos</span><span class="sxs-lookup"><span data-stu-id="a8563-366">United Arab Emirates</span></span>
    - <span data-ttu-id="a8563-367">Venezuela</span><span class="sxs-lookup"><span data-stu-id="a8563-367">Venezuela</span></span>

<span data-ttu-id="a8563-368">Os parceiros que satisfaçam os critérios terão de submeter o ID de registo da empresa de um cliente (também conhecido como organização do cliente INN) e o número de telefone quando atualizarem ou criarem uma subscrição para esse cliente.</span><span class="sxs-lookup"><span data-stu-id="a8563-368">Partners who meet the criteria will have to submit a customer's company registration ID (also known as the customer's organization INN) and phone number when they next update or create a subscription for that customer.</span></span> <span data-ttu-id="a8563-369">Estes parceiros também podem introduzir um nome do meio opcional para o cliente.</span><span class="sxs-lookup"><span data-stu-id="a8563-369">These partners can also enter an optional middle name for the customer.</span></span>

<span data-ttu-id="a8563-370">Note que quando adicionar o ID de registo da sua empresa deve usar o seu ID de imposto de negócio e não o ID pessoal do cliente.</span><span class="sxs-lookup"><span data-stu-id="a8563-370">Note that when you add your company registration ID you should use your business tax ID and not the customer personal ID.</span></span>

<span data-ttu-id="a8563-371">Os parceiros que fazem negócios com clientes novos ou já existentes nos seguintes países já foram a bordo com um lançamento anterior em novembro de 2020.</span><span class="sxs-lookup"><span data-stu-id="a8563-371">Partners who do business with new or existing customers in the following countries have already been onboarded with a previous release in November 2020.</span></span>

- <span data-ttu-id="a8563-372">Arménia</span><span class="sxs-lookup"><span data-stu-id="a8563-372">Armenia</span></span>
- <span data-ttu-id="a8563-373">Azerbaijão</span><span class="sxs-lookup"><span data-stu-id="a8563-373">Azerbaijan</span></span>
- <span data-ttu-id="a8563-374">Bielorrússia</span><span class="sxs-lookup"><span data-stu-id="a8563-374">Belarus</span></span>
- <span data-ttu-id="a8563-375">Hungria</span><span class="sxs-lookup"><span data-stu-id="a8563-375">Hungary</span></span>
- <span data-ttu-id="a8563-376">Cazaquistão</span><span class="sxs-lookup"><span data-stu-id="a8563-376">Kazakhstan</span></span>
- <span data-ttu-id="a8563-377">Quirguistão</span><span class="sxs-lookup"><span data-stu-id="a8563-377">Kyrgyzstan</span></span>
- <span data-ttu-id="a8563-378">Moldávia</span><span class="sxs-lookup"><span data-stu-id="a8563-378">Moldova</span></span>
- <span data-ttu-id="a8563-379">Rússia</span><span class="sxs-lookup"><span data-stu-id="a8563-379">Russia</span></span>
- <span data-ttu-id="a8563-380">Tajiquistão</span><span class="sxs-lookup"><span data-stu-id="a8563-380">Tajikistan</span></span>
- <span data-ttu-id="a8563-381">Ucrânia</span><span class="sxs-lookup"><span data-stu-id="a8563-381">Ukraine</span></span>
- <span data-ttu-id="a8563-382">Usbequistão</span><span class="sxs-lookup"><span data-stu-id="a8563-382">Uzbekistan</span></span>

<span data-ttu-id="a8563-383">Os parceiros com clientes no resto do mundo terão a capacidade, no final de março de 2021, de introduzir o ID de registo da empresa, número de telefone e nome do meio para os clientes como detalhes opcionais.</span><span class="sxs-lookup"><span data-stu-id="a8563-383">Partners with customers in the rest of the world will have the ability at the end of March 2021 to enter the company registration ID, phone number, and middle name for customers as optional details.</span></span>

### <a name="next-steps"></a><span data-ttu-id="a8563-384">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="a8563-384">Next steps</span></span>

- <span data-ttu-id="a8563-385">Reveja a documentação técnica e questione frequentemente na coleção de [parceiros](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) dedicados para obter uma orientação mais detalhada.</span><span class="sxs-lookup"><span data-stu-id="a8563-385">Review the technical documentation and frequently asked questions in the dedicated [partner collection](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) for more detailed guidance.</span></span>
- <span data-ttu-id="a8563-386">Prepare-se para incorporar as alterações utilizando a API do Partner Center e a experiência do utilizador web.</span><span class="sxs-lookup"><span data-stu-id="a8563-386">Prepare to incorporate the changes using Partner Center API and web user experience.</span></span> <span data-ttu-id="a8563-387">A API/SDKs estará disponível para testes.</span><span class="sxs-lookup"><span data-stu-id="a8563-387">API/SDKs will be available for testing.</span></span>
- <span data-ttu-id="a8563-388">Certifique-se de submeter os dados adicionais ao embarcar em novos clientes ou modificar os dados do cliente existentes.</span><span class="sxs-lookup"><span data-stu-id="a8563-388">Make sure to submit the additional data when onboarding new customers or modifying existing customer details.</span></span>
- <span data-ttu-id="a8563-389">Se estiver a utilizar uma solução de fornecedor de painéis de controlo (CPV), consulte o seu CPV.</span><span class="sxs-lookup"><span data-stu-id="a8563-389">If you’re using a control panel vendor (CPV) solution, consult your CPV.</span></span>

### <a name="questions"></a><span data-ttu-id="a8563-390">Perguntas?</span><span class="sxs-lookup"><span data-stu-id="a8563-390">Questions?</span></span>

<span data-ttu-id="a8563-391">Contacte o seu consultor fiscal ou o fisco local se tiver alguma questão relacionada com o ID de registo da empresa (também chamado INN ou TIN).</span><span class="sxs-lookup"><span data-stu-id="a8563-391">Contact your tax advisor or local tax office if you have any questions related to the company registration ID (also called INN or TIN).</span></span> <span data-ttu-id="a8563-392">A Microsoft não pode fornecer orientações sobre questões fiscais.</span><span class="sxs-lookup"><span data-stu-id="a8563-392">Microsoft cannot provide guidance on tax matters.</span></span>

<span data-ttu-id="a8563-393">Se precisar de apoio com as suas operações com a Microsoft, abra um [pedido de serviço](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span><span class="sxs-lookup"><span data-stu-id="a8563-393">If you need support with your operations with Microsoft, open a [service request](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span></span>

## <a name="view-this-months-product-launches-and-offers"></a><a name="1"></a><span data-ttu-id="a8563-394">Veja os lançamentos e ofertas deste mês</span><span class="sxs-lookup"><span data-stu-id="a8563-394">View this month’s product launches and offers</span></span>

### <a name="categories"></a><span data-ttu-id="a8563-395">Categorias</span><span class="sxs-lookup"><span data-stu-id="a8563-395">Categories</span></span>

- <span data-ttu-id="a8563-396">Data: 2021-04-01</span><span class="sxs-lookup"><span data-stu-id="a8563-396">Date: 2021-04-01</span></span>
- <span data-ttu-id="a8563-397">Capacidades</span><span class="sxs-lookup"><span data-stu-id="a8563-397">Capabilities</span></span>
 
### <a name="summary"></a><span data-ttu-id="a8563-398">Resumo</span><span class="sxs-lookup"><span data-stu-id="a8563-398">Summary</span></span>

<span data-ttu-id="a8563-399">O calendário de lançamento do produto de abril de 2021 já foi publicado.</span><span class="sxs-lookup"><span data-stu-id="a8563-399">The April 2021 product launch calendar is now published.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="a8563-400">Audiência impactada</span><span class="sxs-lookup"><span data-stu-id="a8563-400">Impacted audience</span></span>

<span data-ttu-id="a8563-401">Todos os parceiros que transacionam através do programa Cloud Solution Provider (CSP)</span><span class="sxs-lookup"><span data-stu-id="a8563-401">All partners transacting through the Cloud Solution Provider (CSP) program</span></span>

### <a name="details"></a><span data-ttu-id="a8563-402">Detalhes</span><span class="sxs-lookup"><span data-stu-id="a8563-402">Details</span></span>

<span data-ttu-id="a8563-403">O calendário de [lançamento do produto](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) de abril de 2021 já está disponível na galeria de recursos de prontidão operações.</span><span class="sxs-lookup"><span data-stu-id="a8563-403">The April 2021 [product launch calendar](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) is now available in the Operations readiness resource gallery.</span></span> <span data-ttu-id="a8563-404">Veja aqui os próximos lançamentos e ofertas de produtos.</span><span class="sxs-lookup"><span data-stu-id="a8563-404">View the upcoming product launches and offers here.</span></span>

### <a name="next-steps"></a><span data-ttu-id="a8563-405">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="a8563-405">Next steps</span></span>

<span data-ttu-id="a8563-406">Reveja o [calendário de lançamento](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/)do produto e partilhe a informação com as partes interessadas apropriadas na sua organização.</span><span class="sxs-lookup"><span data-stu-id="a8563-406">Review the [product launch calendar](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/), and share the information with the appropriate stakeholders in your organization.</span></span>  

### <a name="questions"></a><span data-ttu-id="a8563-407">Perguntas?</span><span class="sxs-lookup"><span data-stu-id="a8563-407">Questions?</span></span>

<span data-ttu-id="a8563-408">Para mais perguntas sobre estas ofertas, consulte as suas comunidades Yammer relevantes.</span><span class="sxs-lookup"><span data-stu-id="a8563-408">For any further questions about these offers, check your relevant Yammer communities.</span></span>