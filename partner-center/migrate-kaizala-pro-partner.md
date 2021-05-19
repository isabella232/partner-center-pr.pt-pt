---
title: Migrar subscrições do Kaizala Pro para o Microsoft 365
description: Saiba como migrar as subscrições do Kaizala Pro para as versões Microsoft 365 ou Office 365. Leia este artigo para mais detalhes sobre a transição dos seus clientes.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.author: sukumart
author: sukumart
ms.date: 06/01/2020
localization_priority: Normal
ms.openlocfilehash: 583e9c40bb8d161c30440f12331dc8dcbf3db417
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110146430"
---
# <a name="migrate-kaizala-pro-standalone-subscriptions-to-microsoft-365-or-office-365-versions"></a><span data-ttu-id="17be1-104">Migrar subscrições kaizala Pro Standalone para versões Microsoft 365 ou Office 365</span><span class="sxs-lookup"><span data-stu-id="17be1-104">Migrate Kaizala Pro Standalone subscriptions to Microsoft 365 or Office 365 versions</span></span>

<span data-ttu-id="17be1-105">**Funções adequadas**: Agente de vendas</span><span class="sxs-lookup"><span data-stu-id="17be1-105">**Appropriate roles**: Sales agent</span></span>

<span data-ttu-id="17be1-106">A partir de 1 de julho de 2020, a Microsoft está a terminar as vendas do serviço autónomo Kaizala Pro.</span><span class="sxs-lookup"><span data-stu-id="17be1-106">Effective July 1, 2020, Microsoft is ending sales of the Kaizala Pro standalone service.</span></span> <span data-ttu-id="17be1-107">Os clientes deixarão de poder adquirir novas subscrições kaizala Pro após esta data, e as subscrições existentes do Kaizala Pro não serão renovadas automaticamente quando expirarem.</span><span class="sxs-lookup"><span data-stu-id="17be1-107">Customers will no longer be able to purchase new Kaizala Pro subscriptions after this date, and existing Kaizala Pro subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="17be1-108">Para garantir a continuidade dos clientes, deve transitar os clientes com assinaturas autónomas kaizala Pro para uma opção SKU suportada, listada abaixo.</span><span class="sxs-lookup"><span data-stu-id="17be1-108">To ensure continuity for customers, you should transition customers with expiring Kaizala Pro standalone subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="17be1-109">Recomendamos que os clientes mudem os clientes para novas subscrições antes da data de fim anual da subscrição para evitar eventuais interrupções de serviço para os clientes.</span><span class="sxs-lookup"><span data-stu-id="17be1-109">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="17be1-110">Se utilizar a API (CREST ou Partner Center), pode descobrir subscrições caducadas avaliando a data final da subscrição juntamente com a propriedade de renovação automática definida como falsa: `auto renew = False` .</span><span class="sxs-lookup"><span data-stu-id="17be1-110">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew property set to false: `auto renew = False`.</span></span>

<span data-ttu-id="17be1-111">As assinaturas E4 serão marcadas para `auto renew=False` 1 de julho de 2020.</span><span class="sxs-lookup"><span data-stu-id="17be1-111">The E4 subscriptions will be set to `auto renew=False` on July 1, 2020.</span></span> <span data-ttu-id="17be1-112">Pode mover os clientes para um novo plano a qualquer momento.</span><span class="sxs-lookup"><span data-stu-id="17be1-112">You can move customers to a new plan at any time.</span></span>

## <a name="kaizala-pro-standalone-replacement-plans"></a><span data-ttu-id="17be1-113">Planos de substituição Kaizala Pro Autónomo</span><span class="sxs-lookup"><span data-stu-id="17be1-113">Kaizala Pro Standalone replacement plans</span></span>

<span data-ttu-id="17be1-114">Com os novos planos, os seus clientes podem tirar partido das funcionalidades e funcionalidades mais recentes da Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="17be1-114">With the new plans, your customers can take advantage of newer features and functionality in Microsoft 365.</span></span> <span data-ttu-id="17be1-115">Os detalhes dos preços encontram-se na lista de preços e a matriz da lista de ofertas no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="17be1-115">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span>

- <span data-ttu-id="17be1-116">[**Microsoft 365 para Negócios,**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2)incluindo:</span><span class="sxs-lookup"><span data-stu-id="17be1-116">[**Microsoft 365 for Business**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2), including:</span></span>  
   - <span data-ttu-id="17be1-117">Microsoft 365 Business Basic</span><span class="sxs-lookup"><span data-stu-id="17be1-117">Microsoft 365 Business Basic</span></span>
   - <span data-ttu-id="17be1-118">Microsoft 365 Business Standard</span><span class="sxs-lookup"><span data-stu-id="17be1-118">Microsoft 365 Business Standard</span></span>
   - <span data-ttu-id="17be1-119">Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="17be1-119">Microsoft 365 Business Premium</span></span>
    
- <span data-ttu-id="17be1-120">[**Microsoft 365 para Linha da Frente,**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab)incluindo:</span><span class="sxs-lookup"><span data-stu-id="17be1-120">[**Microsoft 365 for Frontline**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab), including:</span></span>
   - <span data-ttu-id="17be1-121">Microsoft 365 F3 (anteriormente Microsoft 365 F1) e Office 365 F3</span><span class="sxs-lookup"><span data-stu-id="17be1-121">Microsoft 365 F3 (formerly Microsoft 365 F1) and Office 365 F3</span></span>
    
- <span data-ttu-id="17be1-122">[**Microsoft 365 para Enterprise,**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans)incluindo:</span><span class="sxs-lookup"><span data-stu-id="17be1-122">[**Microsoft 365 for Enterprise**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans), including:</span></span> 
   - <span data-ttu-id="17be1-123">Escritório 365 E1</span><span class="sxs-lookup"><span data-stu-id="17be1-123">Office 365 E1</span></span>
   - <span data-ttu-id="17be1-124">Microsoft 365 E3 e Office 365 E3</span><span class="sxs-lookup"><span data-stu-id="17be1-124">Microsoft 365 E3 and Office 365 E3</span></span>
   - <span data-ttu-id="17be1-125">Microsoft 365 E5 e Office 365 E5</span><span class="sxs-lookup"><span data-stu-id="17be1-125">Microsoft 365 E5 and Office 365 E5</span></span>

- <span data-ttu-id="17be1-126">[**Microsoft 365 para educação,**](https://www.microsoft.com/education/buy-license/microsoft365)incluindo:</span><span class="sxs-lookup"><span data-stu-id="17be1-126">[**Microsoft 365 for Education**](https://www.microsoft.com/education/buy-license/microsoft365), including:</span></span> 
    - <span data-ttu-id="17be1-127">Microsoft 365 A1 e Office 365 A1</span><span class="sxs-lookup"><span data-stu-id="17be1-127">Microsoft 365 A1 and Office 365 A1</span></span>
    - <span data-ttu-id="17be1-128">Microsoft 365 A3 e Office 365 A3</span><span class="sxs-lookup"><span data-stu-id="17be1-128">Microsoft 365 A3 and Office 365 A3</span></span>
    - <span data-ttu-id="17be1-129">Microsoft 365 A5 e Office 365 A5</span><span class="sxs-lookup"><span data-stu-id="17be1-129">Microsoft 365 A5 and Office 365 A5</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="17be1-130">Transição de clientes para novos planos de produtos</span><span class="sxs-lookup"><span data-stu-id="17be1-130">Transition customers to new product plans</span></span>

<span data-ttu-id="17be1-131">A Microsoft oferece continuamente novos produtos e serviços aos nossos parceiros.</span><span class="sxs-lookup"><span data-stu-id="17be1-131">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="17be1-132">Nestes casos, poderá ter de atualizar os clientes para novos serviços ou migrar as suas subscrições de SKUs que acabarão por ser encerradas.</span><span class="sxs-lookup"><span data-stu-id="17be1-132">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="17be1-133">Os clientes migradores de SKUs reformados para os mais recentes requerem os seguintes passos:</span><span class="sxs-lookup"><span data-stu-id="17be1-133">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

<span data-ttu-id="17be1-134">A.</span><span class="sxs-lookup"><span data-stu-id="17be1-134">A.</span></span> <span data-ttu-id="17be1-135">Comprar a nova subscrição</span><span class="sxs-lookup"><span data-stu-id="17be1-135">Purchase the new subscription</span></span>

<span data-ttu-id="17be1-136">B.</span><span class="sxs-lookup"><span data-stu-id="17be1-136">B.</span></span> <span data-ttu-id="17be1-137">Reatribuir licenças de utilizador atuais</span><span class="sxs-lookup"><span data-stu-id="17be1-137">Reassign current user licenses</span></span>

<span data-ttu-id="17be1-138">C.</span><span class="sxs-lookup"><span data-stu-id="17be1-138">C.</span></span> <span data-ttu-id="17be1-139">Cancelar subscrição antiga</span><span class="sxs-lookup"><span data-stu-id="17be1-139">Cancel old subscription</span></span>


## <a name="migrate-your-customers-to-new-plans"></a><span data-ttu-id="17be1-140">Migrar os seus clientes para novos planos</span><span class="sxs-lookup"><span data-stu-id="17be1-140">Migrate your customers to new plans</span></span>

### <a name="a-purchase-the-new-subscription"></a><span data-ttu-id="17be1-141">A.</span><span class="sxs-lookup"><span data-stu-id="17be1-141">A.</span></span> <span data-ttu-id="17be1-142">Comprar a nova subscrição</span><span class="sxs-lookup"><span data-stu-id="17be1-142">Purchase the new subscription</span></span>

1. <span data-ttu-id="17be1-143">Para adquirir a nova subscrição, a partir do menu **Partner Center,** selecione **Clientes,** selecione o cliente que pretende mover e, em seguida, selecione **Adicionar subscrições**.</span><span class="sxs-lookup"><span data-stu-id="17be1-143">To purchase the new subscription, from the **Partner Center** menu, select **Customers**, select the customer you want to move, and then select **Add subscriptions**.</span></span>

2. <span data-ttu-id="17be1-144">Selecione a subscrição que pretende adquirir no catálogo (neste caso, uma das opções acima), introduza o número de licenças e, em seguida, **selecione Enviar por isso**.</span><span class="sxs-lookup"><span data-stu-id="17be1-144">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span>

<span data-ttu-id="17be1-145">O seu cliente deve agora ter subscrições antigas e novas, a antiga subscrição Kaizala Pro Standalone e a nova subscrição 'target', por exemplo, Opção 1 - Office 365 Enterprise F1.</span><span class="sxs-lookup"><span data-stu-id="17be1-145">Your customer should now have both old and new subscriptions, the old Kaizala Pro Standalone subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise F1.</span></span>

### <a name="b-reassign-current-user-licenses"></a><span data-ttu-id="17be1-146">B.</span><span class="sxs-lookup"><span data-stu-id="17be1-146">B.</span></span> <span data-ttu-id="17be1-147">Reatribuir licenças de utilizador atuais</span><span class="sxs-lookup"><span data-stu-id="17be1-147">Reassign current user licenses</span></span>

1. <span data-ttu-id="17be1-148">Para reatribuir as licenças dos utilizadores do cliente, a partir do menu **Partner Center,** selecione **Clientes,** selecione o cliente que está a mover e, em seguida, selecione **Utilizadores e licenças**.</span><span class="sxs-lookup"><span data-stu-id="17be1-148">To reassign the customer's users' licenses, from the **Partner Center** menu, select **Customers**, select the customer you are moving, and then select **Users and licenses**.</span></span> <span data-ttu-id="17be1-149">A página de Utilizadores e Licenças do cliente abre.</span><span class="sxs-lookup"><span data-stu-id="17be1-149">The customer's Users and Licenses page opens.</span></span>

2. <span data-ttu-id="17be1-150">Para reatribuir a licença de utilizador, selecione o utilizador para reatribuir e, em seguida, **selecione Gerir licenças**.</span><span class="sxs-lookup"><span data-stu-id="17be1-150">To reassign user license, select the user to reassign and then select **Manage licenses**.</span></span>

3. <span data-ttu-id="17be1-151">Na página **'Gerir licenças',** limpe a caixa de verificação da licença Kaizala Pro Standalone e selecione um novo plano de serviço para a subscrição para a qual o cliente está a mover-se.</span><span class="sxs-lookup"><span data-stu-id="17be1-151">On the **Manage licenses** page, clear the Kaizala Pro Standalone license check box, and select a new service plan for the subscription the customer is moving to.</span></span>

4.  <span data-ttu-id="17be1-152">Selecione **Submeter**.</span><span class="sxs-lookup"><span data-stu-id="17be1-152">Select **Submit**.</span></span> <span data-ttu-id="17be1-153">Uma página de confirmação lista as novas atribuições de licença.</span><span class="sxs-lookup"><span data-stu-id="17be1-153">A confirmation page lists the new license assignments.</span></span> <span data-ttu-id="17be1-154">Continue este mesmo processo para outros utilizadores que necessitem de atribuição de licenças.</span><span class="sxs-lookup"><span data-stu-id="17be1-154">Continue this same process for other users who need license assignments.</span></span>

### <a name="c-cancel-old-subscription"></a><span data-ttu-id="17be1-155">C.</span><span class="sxs-lookup"><span data-stu-id="17be1-155">C.</span></span> <span data-ttu-id="17be1-156">Cancelar subscrição antiga</span><span class="sxs-lookup"><span data-stu-id="17be1-156">Cancel old subscription</span></span>

<span data-ttu-id="17be1-157">Depois de transferir a licença do utilizador para o novo serviço, pode cancelar com segurança a subscrição aposentada a nível do cliente.</span><span class="sxs-lookup"><span data-stu-id="17be1-157">After moving the user license to the new service, you can safely cancel the retired subscription at the customer level.</span></span>

1.  <span data-ttu-id="17be1-158">A partir do menu **Partner Center,** selecione **Clientes.**</span><span class="sxs-lookup"><span data-stu-id="17be1-158">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="17be1-159">Selecione o cliente cuja subscrição está a cancelar.</span><span class="sxs-lookup"><span data-stu-id="17be1-159">Select the customer whose subscription you are canceling.</span></span>

2.  <span data-ttu-id="17be1-160">Na página de detalhes da subscrição, desa estale a subscrição **de Suspended**.</span><span class="sxs-lookup"><span data-stu-id="17be1-160">In the subscription detail page, set the subscription to **Suspended**.</span></span>

3.  <span data-ttu-id="17be1-161">Selecione **Submeter**.</span><span class="sxs-lookup"><span data-stu-id="17be1-161">Select **Submit**.</span></span>

<span data-ttu-id="17be1-162">A subscrição antiga está suspensa e a nova subscrição está ativa.</span><span class="sxs-lookup"><span data-stu-id="17be1-162">The old subscription is suspended, and the new subscription is active.</span></span> <span data-ttu-id="17be1-163">A subscrição suspensa será desavisionada automaticamente após 120 dias.</span><span class="sxs-lookup"><span data-stu-id="17be1-163">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="17be1-164">O cliente não incorre em custos adicionais para a subscrição antiga.</span><span class="sxs-lookup"><span data-stu-id="17be1-164">The customer incurs no additional costs for the old subscription.</span></span>
