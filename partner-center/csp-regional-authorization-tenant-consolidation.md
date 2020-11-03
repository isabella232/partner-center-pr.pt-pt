---
title: Consolidação de inquilinos de autorização regional da CSP
ms.topic: how-to
ms.date: 07/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Utilize estas instruções para consolidar inquilinos para diferentes países/regiões. Isto inclui passos para migrar contas de clientes e subscrições de clientes.
author: billLinzbach
ms.author: billLi
ms.localizationpriority: medium
robots: noindex,nofollow
ms.custom: SEOMAY.20
ms.openlocfilehash: 0ae107c005eaf6b8ff8a6d99a91075ebc560cf81
ms.sourcegitcommit: 940dad4527f51781f6f966e196b3aa08389613a2
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/13/2020
ms.locfileid: "92530251"
---
# <a name="instructions-for-csp-regional-authorization-tenant-consolidation"></a><span data-ttu-id="ba7d1-104">Instruções para consolidação de inquilinos de autorização regional da CSP</span><span class="sxs-lookup"><span data-stu-id="ba7d1-104">Instructions for CSP regional authorization tenant consolidation</span></span>

<span data-ttu-id="ba7d1-105">**Aplica-se a**</span><span class="sxs-lookup"><span data-stu-id="ba7d1-105">**Applies to**</span></span>

-  <span data-ttu-id="ba7d1-106">Partner Center</span><span class="sxs-lookup"><span data-stu-id="ba7d1-106">Partner Center</span></span>
-  <span data-ttu-id="ba7d1-107">Centro de Parceiros para Microsoft Cloud para governo dos EUA</span><span class="sxs-lookup"><span data-stu-id="ba7d1-107">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="ba7d1-108">**Funções adequadas**</span><span class="sxs-lookup"><span data-stu-id="ba7d1-108">**Appropriate roles**</span></span>

- <span data-ttu-id="ba7d1-109">Administrador global</span><span class="sxs-lookup"><span data-stu-id="ba7d1-109">Global admin</span></span>
- <span data-ttu-id="ba7d1-110">Agente administrativo</span><span class="sxs-lookup"><span data-stu-id="ba7d1-110">Admin agent</span></span>

<span data-ttu-id="ba7d1-111">\[Algumas informações dizem respeito a um produto pré-lançado que pode ser substancialmente modificado antes de ser lançado comercialmente.</span><span class="sxs-lookup"><span data-stu-id="ba7d1-111">\[Some information relates to pre-released product which may be substantially modified before it's commercially released.</span></span> <span data-ttu-id="ba7d1-112">A Microsoft não faz garantias, de forma expressa ou implícita, em relação à informação aqui apresentada.\]</span><span class="sxs-lookup"><span data-stu-id="ba7d1-112">Microsoft makes no warranties, express or implied, with respect to the information provided here.\]</span></span>

<span data-ttu-id="ba7d1-113">Pode consolidar inquilinos para o seu negócio.</span><span class="sxs-lookup"><span data-stu-id="ba7d1-113">You can consolidate tenants for your business.</span></span> <span data-ttu-id="ba7d1-114">Utilize estas instruções para consolidar inquilinos para diferentes países/regiões.</span><span class="sxs-lookup"><span data-stu-id="ba7d1-114">Use these instructions to consolidate tenants for different country/regions.</span></span>

>[!NOTE]  
><span data-ttu-id="ba7d1-115">Deve estar ciente de todas as assinaturas e contagens de licença para cada um dos seus clientes na conta de que está em transição.</span><span class="sxs-lookup"><span data-stu-id="ba7d1-115">You must be aware of all of the provisioned subscriptions and license counts for each of your customers in the account you are transitioning from.</span></span> <span data-ttu-id="ba7d1-116">Irá re-a provisionar essas mesmas assinaturas exatas com as mesmas contagens de licença ao abrigo da nova conta central da CSP como parte do processo de migração.</span><span class="sxs-lookup"><span data-stu-id="ba7d1-116">You will be re-provisioning those same exact subscriptions with the same license counts under the new central CSP account as part of the migration process.</span></span> <span data-ttu-id="ba7d1-117">Utilize a funcionalidade de lista de exportação para ajudar a criar uma lista de clientes para passar para o inquilino centralizado.</span><span class="sxs-lookup"><span data-stu-id="ba7d1-117">Use the export list feature to help create a list of customers to move over to the centralized tenant.</span></span>  <span data-ttu-id="ba7d1-118">Uma vez que a consolidação esteja completa, não pode voltar ao estado inquilino anterior.</span><span class="sxs-lookup"><span data-stu-id="ba7d1-118">Once consolidation is complete, you can't revert to the previous tenant state.</span></span> <span data-ttu-id="ba7d1-119">A ação do cliente também pode ser necessária.</span><span class="sxs-lookup"><span data-stu-id="ba7d1-119">Customer action may also be required.</span></span>

## <a name="prepare-for-migration"></a><span data-ttu-id="ba7d1-120">Prepare para a migração</span><span class="sxs-lookup"><span data-stu-id="ba7d1-120">Prepare for migration</span></span>

- <span data-ttu-id="ba7d1-121">Inscreva-se no **Partner Center**  utilizando a conta de Transição (a que irá **transitar** para a nova conta), e reveja todos os clientes e todos os serviços prestados a esses clientes.</span><span class="sxs-lookup"><span data-stu-id="ba7d1-121">Sign in to **Partner Center**  using the **Transitioning** account (the one you will transition to the new account), and review of all customers and all of the services provisioned for those customers.</span></span>

- <span data-ttu-id="ba7d1-122">Assine fora desta conta.</span><span class="sxs-lookup"><span data-stu-id="ba7d1-122">Sign out of this account.</span></span>

## <a name="migrate-customer-accounts"></a><span data-ttu-id="ba7d1-123">Migrar contas de clientes</span><span class="sxs-lookup"><span data-stu-id="ba7d1-123">Migrate customer accounts</span></span>

1. <span data-ttu-id="ba7d1-124">Inscreva-se no **Partner Center**  com a conta **de transição** (nova) (aquela em que está a transitar clientes).</span><span class="sxs-lookup"><span data-stu-id="ba7d1-124">Sign in to **Partner Center**  with the **Transitioning** (new) account (the one you are transitioning customers into).</span></span>

2. <span data-ttu-id="ba7d1-125">Selecione **Clientes** .</span><span class="sxs-lookup"><span data-stu-id="ba7d1-125">Select **Customers** .</span></span>

3. <span data-ttu-id="ba7d1-126">Clique **em Solicitar uma relação de revendedor** .</span><span class="sxs-lookup"><span data-stu-id="ba7d1-126">Click **Request a reseller relationship** .</span></span> <span data-ttu-id="ba7d1-127">É-lhe apresentada uma mensagem de correio eletrónico padrão para enviar aos seus clientes.</span><span class="sxs-lookup"><span data-stu-id="ba7d1-127">You are presented with a default email message to send to your customers.</span></span> <span data-ttu-id="ba7d1-128">Esta mensagem contém um URL com o iD org exclusivo da sua nova conta Partner Center.</span><span class="sxs-lookup"><span data-stu-id="ba7d1-128">This message contains a URL with the org ID unique to your new Partner Center account.</span></span>

4. <span data-ttu-id="ba7d1-129">**Ação do Cliente:** Certifique-se de que cada um dos clientes ativos que pretende migrar visita este URL.</span><span class="sxs-lookup"><span data-stu-id="ba7d1-129">**Customer Action:** Ensure that each of the active customers you want to migrate visits this URL.</span></span> <span data-ttu-id="ba7d1-130">Ao abrir o URL, o cliente é solicitado a iniciar sedução no portal do Office 365.</span><span class="sxs-lookup"><span data-stu-id="ba7d1-130">When opening the URL, the customer is prompted to sign in to the Office 365 portal.</span></span> <span data-ttu-id="ba7d1-131">O cliente assina na utilização do mesmo ID Org que utiliza para aceder aos portais de administração Azure e Office 365.</span><span class="sxs-lookup"><span data-stu-id="ba7d1-131">The customer signs in using the same Org ID that they use to access the Azure and Office 365 admin portals.</span></span>

5. <span data-ttu-id="ba7d1-132">Após a sua assinatura, o Administrador Global para a conta do **cliente** é solicitado a apresentar um acordo que dê privilégios de administração delegados à nova conta CSP.</span><span class="sxs-lookup"><span data-stu-id="ba7d1-132">After signing in, the Global Admin for the **customer account** is prompted to submit an agreement that gives delegated admin privileges to the new CSP account.</span></span> <span data-ttu-id="ba7d1-133">Se concordarem, o cliente seleciona a caixa de verificação e concorda em autorizar a relação.</span><span class="sxs-lookup"><span data-stu-id="ba7d1-133">If they agree, the customer selects the checkbox and agrees to authorize the relationship.</span></span>

<span data-ttu-id="ba7d1-134">Os clientes aparecerão na lista de clientes do parceiro depois de terem apresentado o contrato, um a um.</span><span class="sxs-lookup"><span data-stu-id="ba7d1-134">The customers will appear in the partner's customer list after they have submitted the agreement, one by one.</span></span>

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a><span data-ttu-id="ba7d1-135">Subscrições baseadas em uso do Gabinete Migratório 365 e não-Azure</span><span class="sxs-lookup"><span data-stu-id="ba7d1-135">Migrating Office 365 and non-Azure usage-based subscriptions</span></span>

1. <span data-ttu-id="ba7d1-136">Uma vez que o seu cliente tenha assinado o contrato, pode recriar as suas subscrições sob o seu Inquilino Centralizado.</span><span class="sxs-lookup"><span data-stu-id="ba7d1-136">Once your customer has signed the agreement, you can recreate their subscriptions under your Centralized Partner Tenant.</span></span>

2. <span data-ttu-id="ba7d1-137">A partir do **Partner Center** selecione **Clientes.**</span><span class="sxs-lookup"><span data-stu-id="ba7d1-137">From **Partner Center** select **Customers** .</span></span>

3. <span data-ttu-id="ba7d1-138">Abra o nome da empresa para o cliente que pretende migrar.</span><span class="sxs-lookup"><span data-stu-id="ba7d1-138">Open the company name for the customer you want to migrate.</span></span>

4. <span data-ttu-id="ba7d1-139">Selecione **Adicionar subscrição** .</span><span class="sxs-lookup"><span data-stu-id="ba7d1-139">Select **Add subscription** .</span></span>

5. <span data-ttu-id="ba7d1-140">Adicione as assinaturas corretas e as contagens de licença do catálogo.</span><span class="sxs-lookup"><span data-stu-id="ba7d1-140">Add the correct subscriptions and license counts from the catalog.</span></span> <span data-ttu-id="ba7d1-141">Verifique com as informações fornecidas nas contas **de parceiros.**</span><span class="sxs-lookup"><span data-stu-id="ba7d1-141">Verify with the information provided in the **Transitioning From** partner accounts.</span></span>

   :::image type="content" source="images/regionalcustomer2.png" alt-text="lista de clientes":::

6. <span data-ttu-id="ba7d1-143">Clique **em Enviar.**</span><span class="sxs-lookup"><span data-stu-id="ba7d1-143">Click **Submit.**</span></span>

   <span data-ttu-id="ba7d1-144">Os serviços são agora prestados ao cliente a partir da conta **de transição para** parceiro.</span><span class="sxs-lookup"><span data-stu-id="ba7d1-144">The services are now provided to the customer from the **Transitioning To** partner account.</span></span>

7. <span data-ttu-id="ba7d1-145">Repita estes passos para migrar subscrições para todos os clientes adicionais.</span><span class="sxs-lookup"><span data-stu-id="ba7d1-145">Repeat these steps to migrate subscriptions for all additional customers.</span></span>

<span data-ttu-id="ba7d1-146">Antes de avançar para a secção seguinte, certifique-se de que todas as subscrições de clientes existentes no âmbito das contas **de** parceiros são realoadas na conta **de transição para** parceiro.</span><span class="sxs-lookup"><span data-stu-id="ba7d1-146">Before proceeding to the next section, ensure all customer subscriptions existing under the **Transitioning From** partner accounts are re-provisioned under the **Transitioning To** partner account.</span></span>

> [!NOTE]
> <span data-ttu-id="ba7d1-147">Os parceiros devem suspender as subscrições na conta **de "Transição de** Inquilinos Parceiros" no Centro de Parceiros no mesmo dia em que essas assinaturas são transitadas e criadas ao abrigo da conta **de "Transição para** Inquilino Parceiro" no Centro de Parceiros para garantir que a faturação dupla não ocorre.</span><span class="sxs-lookup"><span data-stu-id="ba7d1-147">Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="ba7d1-148">Os pedidos de apoio serão negados para créditos devido a qualquer sobreposição na faturação que ocorra de não desativar corretamente as subscrições **de Transição** de Assinaturas.</span><span class="sxs-lookup"><span data-stu-id="ba7d1-148">Support requests will be denied for credits due to any overlap in billing that occurs from not correctly disabling the **Transitioning From** subscriptions.</span></span>

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a><span data-ttu-id="ba7d1-149">Desativação das 365 assinaturas do Office no âmbito da conta de transição de parceiros</span><span class="sxs-lookup"><span data-stu-id="ba7d1-149">Disabling the Office 365 subscriptions under the Transitioning From partner account</span></span>

<span data-ttu-id="ba7d1-150">A desativação da subscrição do CSP ao abrigo das contas de parceiros em **transição** impede qualquer faturação futura.</span><span class="sxs-lookup"><span data-stu-id="ba7d1-150">Disabling the CSP subscription under the **Transitioning From** partner accounts stops any future billing.</span></span> <span data-ttu-id="ba7d1-151">Não é preciso desativar manualmente as subscrições do Azure, porque as subscrições do Azure são automaticamente desativadas durante o processo de migração.</span><span class="sxs-lookup"><span data-stu-id="ba7d1-151">You don't have to manually disable Azure subscriptions, because Azure subscriptions are automatically disabled during the migration process.</span></span>

1. <span data-ttu-id="ba7d1-152">Inscreva-se no **Centro de Parceiros** com a conta **de transição da** CSP e navegue para a lista de clientes.</span><span class="sxs-lookup"><span data-stu-id="ba7d1-152">Sign in to the **Partner Center** with the **Transitioning From** CSP account and navigate to the customer list.</span></span>

2. <span data-ttu-id="ba7d1-153">Abra o cliente com subscrições para desativar e, em seguida, selecione a primeira oferta para desativar.</span><span class="sxs-lookup"><span data-stu-id="ba7d1-153">Open the customer with subscriptions to disable, and then select the first offer to disable.</span></span>

3. <span data-ttu-id="ba7d1-154">Desfie a subscrição para **suspender** e, em seguida, clique **em submeter** .</span><span class="sxs-lookup"><span data-stu-id="ba7d1-154">Set the subscription to **suspended** , and then click **submit** .</span></span>

   >[!Note]
   ><span data-ttu-id="ba7d1-155">A suspensão da subscrição garante que não ocorra uma faturação dupla.</span><span class="sxs-lookup"><span data-stu-id="ba7d1-155">Suspending the subscription ensures double billing does not occur.</span></span>

   <span data-ttu-id="ba7d1-156">A subscrição mostra **suspensa** na lista de assinaturas.</span><span class="sxs-lookup"><span data-stu-id="ba7d1-156">The subscription shows **suspended** on the subscriptions list.</span></span>

4. <span data-ttu-id="ba7d1-157">Repita estes passos para todas as subscrições sob o cliente.</span><span class="sxs-lookup"><span data-stu-id="ba7d1-157">Repeat these steps for all subscriptions under the customer.</span></span> <span data-ttu-id="ba7d1-158">Verifique todos os **espetáculos suspensos.**</span><span class="sxs-lookup"><span data-stu-id="ba7d1-158">Verify all show **suspended.**</span></span>

5. <span data-ttu-id="ba7d1-159">Selecione o próximo cliente da lista e repita o processo de desativação de todas as subscrições.</span><span class="sxs-lookup"><span data-stu-id="ba7d1-159">Select the next customer on the list and repeat the process of disabling all subscriptions.</span></span>

## <a name="migrating-azure-usage-based-subscriptions"></a><span data-ttu-id="ba7d1-160">Subscrições baseadas em uso do Azure migratório</span><span class="sxs-lookup"><span data-stu-id="ba7d1-160">Migrating Azure usage-based subscriptions</span></span>

<span data-ttu-id="ba7d1-161">Ao contrário das assinaturas CSP do Office 365, a Azure, as assinaturas CSP baseadas na utilização não precisam de ser migradas manualmente.</span><span class="sxs-lookup"><span data-stu-id="ba7d1-161">Unlike the Office 365 CSP subscriptions, Azure, usage-based CSP subscriptions do not need to be migrated manually.</span></span> <span data-ttu-id="ba7d1-162">O Microsoft Azure Support migrará as subscrições do Azure, bem como todos os serviços ou recursos implantados desde as contas **de revendedores de CSP** para a conta de revendedor **de transição para** CSP.</span><span class="sxs-lookup"><span data-stu-id="ba7d1-162">Microsoft Azure Support will migrate the Azure subscriptions as well as all deployed services or resources from the **Transitioning From** CSP reseller accounts to the **Transitioning To** CSP reseller account.</span></span> <span data-ttu-id="ba7d1-163">Não haverá interrupção do serviço ao cliente durante esta transição.</span><span class="sxs-lookup"><span data-stu-id="ba7d1-163">There will be no disruption of service to the customer during this transition.</span></span>

1. <span data-ttu-id="ba7d1-164">Certifique-se de que as contas de clientes que terão as assinaturas Azure migradas aceitaram o acordo para ser associado à nova conta **de Transição para** CSP.</span><span class="sxs-lookup"><span data-stu-id="ba7d1-164">Ensure that the customer accounts that will have Azure subscriptions migrated have accepted the agreement to be associated with the new **Transitioning To** CSP account.</span></span>

2. <span data-ttu-id="ba7d1-165">Irá notificar a Microsoft de quais as contas de clientes prontas a migrar e fornecer os nomes da empresa desses clientes.</span><span class="sxs-lookup"><span data-stu-id="ba7d1-165">You will notify Microsoft of which customer accounts are ready to migrate, and provide those customer's company names.</span></span>

3. <span data-ttu-id="ba7d1-166">A Microsoft migra as subscrições baseadas em uso do Azure e notifica-o quando a migração estiver completa.</span><span class="sxs-lookup"><span data-stu-id="ba7d1-166">Microsoft migrates the Azure usage-based subscriptions and notifies you when the migration is complete.</span></span>

4. <span data-ttu-id="ba7d1-167">Tem de confirmar que a subscrição do Azure no âmbito da conta de **revendedor de transição de** CSP está agora marcada **suspensa** no Partner Center sob a secção de subscrições de clientes.</span><span class="sxs-lookup"><span data-stu-id="ba7d1-167">You need to confirm that the Azure subscription under the **Transitioning From** CSP reseller account now is marked **suspended** in Partner Center under the customer subscriptions section.</span></span>

5. <span data-ttu-id="ba7d1-168">Confirme que a subscrição do Azure ao abrigo da conta de **revendedor de transição para** CSP mostra agora um estado ativo no Partner Center sob a secção de subscrições do cliente. **active**</span><span class="sxs-lookup"><span data-stu-id="ba7d1-168">Confirm that the Azure subscription under the **Transitioning To** CSP reseller account now shows a status of **active** in Partner Center under the customer subscriptions section.</span></span>

   >[!Note]
   > <span data-ttu-id="ba7d1-169">A desativação das subscrições ao abrigo do cliente não altera o aparecimento do cliente na lista de Clientes.</span><span class="sxs-lookup"><span data-stu-id="ba7d1-169">Disabling the subscriptions under the customer does not change the appearance of the customer in the Customers list.</span></span> <span data-ttu-id="ba7d1-170">Atualmente não existe opção de retirar clientes da lista.</span><span class="sxs-lookup"><span data-stu-id="ba7d1-170">There is currently no option to remove customers from the list.</span></span> <span data-ttu-id="ba7d1-171">Os parceiros devem evitar adicionar subscrições a estes clientes da sua conta **de Transição de A partir** do futuro.</span><span class="sxs-lookup"><span data-stu-id="ba7d1-171">Partners should avoid adding subscriptions back to these customers from their **Transitioning From** account in the future.</span></span>

6. <span data-ttu-id="ba7d1-172">Repita estes passos para todas as subscrições sob todos os seus clientes para parar os encargos futuros na conta **(s) de Transição.**</span><span class="sxs-lookup"><span data-stu-id="ba7d1-172">Repeat these steps for all subscriptions under all of your customers to stop future charges on the **Transitioning From** account(s).</span></span> <span data-ttu-id="ba7d1-173">O parceiro receberá uma fatura final com crédito pelo número de dias não reutilizados entre o dia de cancelamento e o último dia do período de faturação.</span><span class="sxs-lookup"><span data-stu-id="ba7d1-173">The partner will receive one final invoice with a credit for the number of unused days between the day of cancellation and the last day of the billing period.</span></span> <span data-ttu-id="ba7d1-174">Nenhuma fatura futura gerará após o período final de faturação.</span><span class="sxs-lookup"><span data-stu-id="ba7d1-174">No future invoices will generate after that final billing period.</span></span>

### <a name="additional-information"></a><span data-ttu-id="ba7d1-175">Informações adicionais</span><span class="sxs-lookup"><span data-stu-id="ba7d1-175">Additional information</span></span>

- <span data-ttu-id="ba7d1-176">A desativação da subscrição da conta **de transição da** CSP não afeta o serviço do cliente final desde que o serviço tenha sido prestado a partir da conta **de transição para** CSP antes de desativar a subscrição.</span><span class="sxs-lookup"><span data-stu-id="ba7d1-176">Disabling the subscription from the **Transitioning From** CSP account does not impact end customer's service as long as the service was provisioned from the **Transitioning To** CSP account prior to disabling the subscription.</span></span>

- <span data-ttu-id="ba7d1-177">As subscrições não podem ser utilizadas pelo cliente e não geram encargos quando suspensas ou canceladas.</span><span class="sxs-lookup"><span data-stu-id="ba7d1-177">Subscriptions cannot be used by the customer and do not generate charges when suspended or canceled.</span></span>

- <span data-ttu-id="ba7d1-178">De momento não existe forma de remover completamente um cliente da lista de **Clientes.**</span><span class="sxs-lookup"><span data-stu-id="ba7d1-178">There is currently no way to remove a customer completely from the **Customers** list.</span></span>
- 
    >[!Note]
    > <span data-ttu-id="ba7d1-179">Os parceiros devem suspender as subscrições na conta **de** inquilinos parceiros no Centro de Parceiros no mesmo dia em que essas subscrições são transitadas e criadas ao abrigo da conta **Transição Para** garantir que a faturação dupla não ocorre.</span><span class="sxs-lookup"><span data-stu-id="ba7d1-179">Partners must suspend subscriptions on the **Transitioning From** partner tenant account in Partner Center the same day those subscriptions are transitioned to and set up under the **Transitioning To** account to ensure double billing does not occur.</span></span> <span data-ttu-id="ba7d1-180">A Microsoft não apoiará pedidos de créditos devido a qualquer sobreposição na faturação que ocorra de não definir corretamente as subscrições **de Transição** de subscrições para suspensas.</span><span class="sxs-lookup"><span data-stu-id="ba7d1-180">Microsoft will not support requests for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to suspended.</span></span>

### <a name="simplify-migration-using-export"></a><span data-ttu-id="ba7d1-181">Simplificar a migração usando exportação</span><span class="sxs-lookup"><span data-stu-id="ba7d1-181">Simplify migration using Export</span></span>

<span data-ttu-id="ba7d1-182">Utilizando a **Função Exportação,** pode capturar as subscrições que necessita de utilizar na sua nova estrutura consolidada:</span><span class="sxs-lookup"><span data-stu-id="ba7d1-182">Using the **Export Function** , you can capture the subscriptions you need to use in your new consolidated structure:</span></span>

1. <span data-ttu-id="ba7d1-183">Clique em **Clientes** no Partner Center para ver a lista de clientes.</span><span class="sxs-lookup"><span data-stu-id="ba7d1-183">Click **Customers** on Partner Center to see the list of customers.</span></span> 

2. <span data-ttu-id="ba7d1-184">Abra o nome do cliente desejado.</span><span class="sxs-lookup"><span data-stu-id="ba7d1-184">Open the desired customer name.</span></span>

3. <span data-ttu-id="ba7d1-185">Na página **de Subscrições,** clique em **Exportar Subscrições** para exportar detalhes de subscrições para um ficheiro Excel.</span><span class="sxs-lookup"><span data-stu-id="ba7d1-185">On the **Subscriptions** page, click **Export Subscriptions** to export details of subscriptions to an Excel file.</span></span>

4. <span data-ttu-id="ba7d1-186">Utilize esta lista para recriar as subscrições no seu novo inquilino consolidado.</span><span class="sxs-lookup"><span data-stu-id="ba7d1-186">Use this list to recreate the subscriptions in your new consolidated tenant.</span></span>

### <a name="api-registration"></a><span data-ttu-id="ba7d1-187">Registo da API</span><span class="sxs-lookup"><span data-stu-id="ba7d1-187">API registration</span></span>

<span data-ttu-id="ba7d1-188">Para obter mais informações sobre o registo da API, consulte [configurar o acesso a API no Partner Center.](/partner-center/develop/set-up-api-access-in-partner-center)</span><span class="sxs-lookup"><span data-stu-id="ba7d1-188">For more information about API registration, see [Set up API access in Partner Center](/partner-center/develop/set-up-api-access-in-partner-center).</span></span>

## <a name="next-steps"></a><span data-ttu-id="ba7d1-189">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="ba7d1-189">Next steps</span></span>

- [<span data-ttu-id="ba7d1-190">Cloud Solution Provider programa mercados regionais e moedas onde pode vender ofertas de CSP</span><span class="sxs-lookup"><span data-stu-id="ba7d1-190">Cloud Solution Provider program regional markets and currencies where you can sell CSP offers</span></span>](regional-authorization-overview.md)
