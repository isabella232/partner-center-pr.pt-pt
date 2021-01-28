---
title: Faturação do plano Azure - fatura & arquivos de reconhecimento
ms.topic: article
ms.date: 01/20/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como aceder e compreender a estrutura de ficheiros de fatura e reconciliação relacionada com a faturação do plano Azure.
author: khpavan
ms.author: sakhanda
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 819f90ca9a8467de4a8001a1b10f8409d3fb1b81
ms.sourcegitcommit: fc1f9cb5a542bdc92d62d2a7e1ab2f4e69903e49
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/28/2021
ms.locfileid: "98924992"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a><span data-ttu-id="f1335-103">Nova experiência comercial no CSP – faturação do Azure</span><span class="sxs-lookup"><span data-stu-id="f1335-103">New commerce experience in CSP - Azure billing</span></span> 

<span data-ttu-id="f1335-104">**Funções adequadas**</span><span class="sxs-lookup"><span data-stu-id="f1335-104">**Appropriate roles**</span></span>

- <span data-ttu-id="f1335-105">Agente administrativo</span><span class="sxs-lookup"><span data-stu-id="f1335-105">Admin agent</span></span>
- <span data-ttu-id="f1335-106">Administrador de faturação</span><span class="sxs-lookup"><span data-stu-id="f1335-106">Billing admin</span></span>
- <span data-ttu-id="f1335-107">Administrador global</span><span class="sxs-lookup"><span data-stu-id="f1335-107">Global admin</span></span>

<span data-ttu-id="f1335-108">Este artigo explica como aceder e compreender a estrutura de ficheiros de fatura e reconciliação relacionada com a faturação do plano Azure.</span><span class="sxs-lookup"><span data-stu-id="f1335-108">This article explains how to access and understand the invoice and reconciliation file structure related to billing for the Azure plan.</span></span> <span data-ttu-id="f1335-109">A faturação ao abrigo do plano Azure é uma experiência de faturação simplificada usando uma data de faturação única alinhada e período de faturação de um mês de calendário.</span><span class="sxs-lookup"><span data-stu-id="f1335-109">Billing under the Azure plan is a simplified billing experience using an aligned single billing date and calendar month-based billing period.</span></span>

## <a name="summary-of-billing-essentials"></a><span data-ttu-id="f1335-110">Resumo do essencial da faturação</span><span class="sxs-lookup"><span data-stu-id="f1335-110">Summary of billing essentials</span></span>

- <span data-ttu-id="f1335-111">**Data da fatura**: A fatura e o ficheiro de reconciliação estarão disponíveis no painel de instrumentos/API do Centro Parceiro até ao dia 8 (meia-noite UTC).</span><span class="sxs-lookup"><span data-stu-id="f1335-111">**Invoice date**: Invoice and reconciliation file will be available in the Partner Center dashboard/API by the 8th (midnight UTC).</span></span>

- <span data-ttu-id="f1335-112">**Período de faturação**: O período de faturação está alinhado com o mês civil, por exemplo, 10/1-10/31, 11/1-11/30.</span><span class="sxs-lookup"><span data-stu-id="f1335-112">**Invoice billing period**: The invoice billing period is aligned to the calendar month, for example,  10/1-10/31, 11/1-11/30.</span></span>

- <span data-ttu-id="f1335-113">**Períodos de serviço de cobrança**: As taxas irão alinhar-se com o mês civil.</span><span class="sxs-lookup"><span data-stu-id="f1335-113">**Charge service periods**: Charges will align to the calendar month.</span></span> <span data-ttu-id="f1335-114">Por exemplo, se o parceiro faturado adicionar serviços Azure através de um plano Azure em 10/15 e o cliente iniciar o consumo de serviços Azure em 10/15, então o parceiro faturado receberá fatura/reconhecimento em 11/8 para consumo de clientes para o período de serviço 10/15 - 10/31.</span><span class="sxs-lookup"><span data-stu-id="f1335-114">For example, if billed partner adds Azure services through an Azure plan on 10/15 and the customer begins consumption of Azure services on 10/15, then billed partner will receive invoice/recon on 11/8 for customer consumption for the service period 10/15 - 10/31.</span></span> <span data-ttu-id="f1335-115">A fatura do próximo mês que será gerada em 12/8 contém todos os encargos para o período de serviço 11/1- 11/31.</span><span class="sxs-lookup"><span data-stu-id="f1335-115">The next month's invoice that is going to be generated on 12/8 contains all the charges for the service period 11/1- 11/31.</span></span>

- <span data-ttu-id="f1335-116">**Prazo de pagamento da fatura:** Líquido 60 dias.</span><span class="sxs-lookup"><span data-stu-id="f1335-116">**Invoice payment term**: Net 60 days.</span></span>

- <span data-ttu-id="f1335-117">**Moeda de fatura**: A partir de 28 de janeiro de 2021, os parceiros da região UE/EFTA e reino unido que tenham novos clientes e clientes CSP existentes que adquiram novas ofertas de comércio pela primeira vez, cujos inquilinos foram criados antes de 11 de maio de 2020, serão cobrados para essas compras em moeda de localização parceira.</span><span class="sxs-lookup"><span data-stu-id="f1335-117">**Invoice currency**: Starting January 28th 2021, partners in the EU/EFTA and UK region who have new customers and existing CSP customers purchasing new commerce offers for the first time whose tenants were created prior to 11 May 2020, will be billed for those purchases in partner location currency.</span></span> <span data-ttu-id="f1335-118">Os parceiros situados fora da região UE/EFTA e reino unido continuarão a ser faturados em moeda de localização de parceiros.</span><span class="sxs-lookup"><span data-stu-id="f1335-118">Partners located outside of the EU/EFTA and UK region will continue to be billed in partner location currency.</span></span>

- <span data-ttu-id="f1335-119">**Incentivos ao parceiro**: Pago 45 dias a partir do final do mês de fatura.</span><span class="sxs-lookup"><span data-stu-id="f1335-119">**Partner incentives**: Paid 45 days from the end of the invoice month.</span></span>

## <a name="access-your-invoices-and-reconciliation-files"></a><span data-ttu-id="f1335-120">Aceda às suas faturas e ficheiros de reconciliação</span><span class="sxs-lookup"><span data-stu-id="f1335-120">Access your invoices and reconciliation files</span></span>

<span data-ttu-id="f1335-121">O administrador global ou administrador de faturação da sua empresa receberá um e-mail quando uma fatura estiver pronta para ver.</span><span class="sxs-lookup"><span data-stu-id="f1335-121">The global admin or billing admin for your company will receive an email when an invoice is ready to view.</span></span>

<span data-ttu-id="f1335-122">Para aceder à fatura e ao ficheiro de reconciliação:</span><span class="sxs-lookup"><span data-stu-id="f1335-122">To access the invoice and reconciliation file:</span></span>

1. <span data-ttu-id="f1335-123">Inicie sessão no [dashboard](https://partner.microsoft.com/dashboard/) do Centro de Parceiros.</span><span class="sxs-lookup"><span data-stu-id="f1335-123">Sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="f1335-124">No menu Partner Center, selecione **Billing**.</span><span class="sxs-lookup"><span data-stu-id="f1335-124">From the Partner Center menu, select **Billing**.</span></span>

3. <span data-ttu-id="f1335-125">Selecione o separador para o **Recorrente** e **uma vez** e a moeda em que está interessado.</span><span class="sxs-lookup"><span data-stu-id="f1335-125">Select the tab for the **Recurring** and **One-time** and the currency you are interested in.</span></span>

   :::image type="content" source="images/azure/billing3.png" alt-text="faturação":::

4. <span data-ttu-id="f1335-127">Selecione o ficheiro **Fatura** ou **Reconciliação.**</span><span class="sxs-lookup"><span data-stu-id="f1335-127">Select **Invoice** or **Reconciliation file**.</span></span>  

   <span data-ttu-id="f1335-128">Para ver faturas históricas e ficheiros de reconhecimento expande a linha de história de Billing abaixo.</span><span class="sxs-lookup"><span data-stu-id="f1335-128">To view historical invoices and recon files expand the Billing history row below.</span></span>

## <a name="understanding-usage-data"></a><span data-ttu-id="f1335-129">Compreender os dados de utilização</span><span class="sxs-lookup"><span data-stu-id="f1335-129">Understanding usage data</span></span> 

1. <span data-ttu-id="f1335-130">O plano Azure é a raiz ou o recipiente de nível superior para utilização.</span><span class="sxs-lookup"><span data-stu-id="f1335-130">Azure plan is the root or top-level container for usage.</span></span> <span data-ttu-id="f1335-131">Todo o uso está ligado a um único plano Azure.</span><span class="sxs-lookup"><span data-stu-id="f1335-131">All usage is tied back to a single Azure plan.</span></span>

2. <span data-ttu-id="f1335-132">Dentro de um plano, haverá uma ou mais subscrições da Azure.</span><span class="sxs-lookup"><span data-stu-id="f1335-132">Within a plan, there will be one or more Azure subscriptions.</span></span> <span data-ttu-id="f1335-133">Estes são recipientes utilizados para a gestão e implantação de recursos.</span><span class="sxs-lookup"><span data-stu-id="f1335-133">These are containers used for resource management and deployment.</span></span> 

3. <span data-ttu-id="f1335-134">Dentro de uma subscrição, os grupos de recursos adicionam recursos de grupo.</span><span class="sxs-lookup"><span data-stu-id="f1335-134">Within a subscription, resource groups add to group resources.</span></span> <span data-ttu-id="f1335-135">Todos os recursos são implantados num grupo de recursos.</span><span class="sxs-lookup"><span data-stu-id="f1335-135">Every resource is deployed to one resource group.</span></span> 

4. <span data-ttu-id="f1335-136">Exemplos de recursos incluem máquinas virtuais e contas de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="f1335-136">Examples of resources include virtual machines and storage accounts.</span></span> 

5. <span data-ttu-id="f1335-137">Contadores de recursos: Os contadores são medições de consumo de um recurso, e um recurso pode emitir uso para vários metros.</span><span class="sxs-lookup"><span data-stu-id="f1335-137">Resource emit meters: Meters are measurements of consumption of a resource, and one resource may emit usage for multiple meters.</span></span> <span data-ttu-id="f1335-138">Os contadores são identificados por um ProductId, SKUId e AvailabilityId.</span><span class="sxs-lookup"><span data-stu-id="f1335-138">Meters are identified by a ProductId, SKUId, and AvailabilityId.</span></span> 

### <a name="hierarchy-of-subscription-resource-groups-and-metering"></a><span data-ttu-id="f1335-139">Hierarquia dos grupos de recursos de subscrição e da medição</span><span class="sxs-lookup"><span data-stu-id="f1335-139">Hierarchy of subscription resource groups and metering</span></span>

<span data-ttu-id="f1335-140">**Conta Azure (inquilino)**</span><span class="sxs-lookup"><span data-stu-id="f1335-140">**Azure account (tenant)**</span></span>

- <span data-ttu-id="f1335-141">Assinatura A</span><span class="sxs-lookup"><span data-stu-id="f1335-141">Subscription A</span></span>
    - <span data-ttu-id="f1335-142">Grupo de Recursos 1</span><span class="sxs-lookup"><span data-stu-id="f1335-142">ResourceGroup 1</span></span>
        - <span data-ttu-id="f1335-143">Máquina virtual (recurso)</span><span class="sxs-lookup"><span data-stu-id="f1335-143">Virtual machine (resource)</span></span>
            - <span data-ttu-id="f1335-144">Contador de cálculo</span><span class="sxs-lookup"><span data-stu-id="f1335-144">Compute meter</span></span>
        - <span data-ttu-id="f1335-145">Rede virtual (recurso)</span><span class="sxs-lookup"><span data-stu-id="f1335-145">Virtual network (resource)</span></span>
            - <span data-ttu-id="f1335-146">Sem medidor de faturação</span><span class="sxs-lookup"><span data-stu-id="f1335-146">No billing meter</span></span>

    - <span data-ttu-id="f1335-147">Grupo de Recursos 2</span><span class="sxs-lookup"><span data-stu-id="f1335-147">ResourceGroup 2</span></span>
        - <span data-ttu-id="f1335-148">Máquina virtual (recurso)</span><span class="sxs-lookup"><span data-stu-id="f1335-148">Virtual machine (resource)</span></span>
            - <span data-ttu-id="f1335-149">Medidor de computador</span><span class="sxs-lookup"><span data-stu-id="f1335-149">Computer meter</span></span>
        - <span data-ttu-id="f1335-150">Disco gerido por SSD premium (recurso)</span><span class="sxs-lookup"><span data-stu-id="f1335-150">Premium SSD-managed disk (resource)</span></span>
            - <span data-ttu-id="f1335-151">Contador de capacidade de armazenamento</span><span class="sxs-lookup"><span data-stu-id="f1335-151">Storage capacity meter</span></span>
            - <span data-ttu-id="f1335-152">Contador de operações de armazenamento</span><span class="sxs-lookup"><span data-stu-id="f1335-152">Storage operations meter</span></span>

- <span data-ttu-id="f1335-153">Assinatura B -ResourceGroup 1 - Azure SQL (recurso) - Medidor DTU - VPN Gateway (recurso) - Medidor de gateway VPN</span><span class="sxs-lookup"><span data-stu-id="f1335-153">Subscription B   -ResourceGroup 1       - Azure SQL (resource)           - DTU meter       - VPN Gateway (resource)           - VPN gateway meter</span></span>

    - <span data-ttu-id="f1335-154">Grupo de Recursos 2</span><span class="sxs-lookup"><span data-stu-id="f1335-154">ResourceGroup 2</span></span>
        - <span data-ttu-id="f1335-155">Interface de rede virtual (recurso)</span><span class="sxs-lookup"><span data-stu-id="f1335-155">Virtual Network Interface (resource)</span></span>
            - <span data-ttu-id="f1335-156">Sem medidor de faturação</span><span class="sxs-lookup"><span data-stu-id="f1335-156">No billing meter</span></span>

## <a name="read-the-invoice"></a><span data-ttu-id="f1335-157">Leia a fatura</span><span class="sxs-lookup"><span data-stu-id="f1335-157">Read the invoice</span></span>

1. <span data-ttu-id="f1335-158">A fatura estará disponível o mais tardar no oitavo de cada mês.</span><span class="sxs-lookup"><span data-stu-id="f1335-158">Invoice will be available no later than the eighth of each month.</span></span>

2. <span data-ttu-id="f1335-159">Os sócios têm 60 dias para pagar.</span><span class="sxs-lookup"><span data-stu-id="f1335-159">Partners have 60 days to remit payment.</span></span>

3. <span data-ttu-id="f1335-160">O período de faturação abrangerá um determinado mês civil, por exemplo, 10/1-10/31.</span><span class="sxs-lookup"><span data-stu-id="f1335-160">The billing period will cover a given calendar month, for example, 10/1-10/31.</span></span>

4. <span data-ttu-id="f1335-161">Os encargos são líquidos de ajustamentos (o montante é líquido de "Partner earned credit for services managed").</span><span class="sxs-lookup"><span data-stu-id="f1335-161">Charges are net of adjustments (amount is net of “Partner earned credit for services managed").</span></span>

5. <span data-ttu-id="f1335-162">Reveja o ficheiro de reconhecimento de fatura e o ficheiro de utilização nominal diário para obter detalhes adicionais de faturação.</span><span class="sxs-lookup"><span data-stu-id="f1335-162">Review the invoice recon file and daily rated usage file for additional billing details.</span></span>

   :::image type="content" source="images/azure/invoice1.png" alt-text="fatura":::

## <a name="read-the-invoice-reconciliation-file"></a><span data-ttu-id="f1335-164">Leia o ficheiro de reconciliação da fatura</span><span class="sxs-lookup"><span data-stu-id="f1335-164">Read the invoice reconciliation file</span></span>

1. <span data-ttu-id="f1335-165">Cada plano Azure e combinação de contadores podem ter até duas linhas de faturação no ficheiro de reconhecimento.</span><span class="sxs-lookup"><span data-stu-id="f1335-165">Each Azure plan and meter combination may have up to two billing lines on the recon file.</span></span>

2. <span data-ttu-id="f1335-166">Se o contador se qualificar para qualquer tipo de desconto ou crédito (como descontos hierárquicos ou o Parceiro ganhou crédito pelos serviços geridos) durante todo o mês civil, então o ficheiro de reconhecimento conterá apenas uma linha de faturação.</span><span class="sxs-lookup"><span data-stu-id="f1335-166">If the meter qualified for any type of discount or credit (such as tiered discounts or the Partner earned credit for services managed) throughout the entire calendar month, then the recon file will only contain one billing line.</span></span> <span data-ttu-id="f1335-167">A coluna **PriceAdjusmentDescription** referenciará o desconto ou o crédito auferido.</span><span class="sxs-lookup"><span data-stu-id="f1335-167">The column **PriceAdjusmentDescription** will reference the discount or earned credit.</span></span>

3. <span data-ttu-id="f1335-168">Se não houver recursos para um determinado contador que se qualiou para desconto ou parceiro ganhou crédito, então o ficheiro de reconhecimento conterá apenas uma linha de faturação e o preço unitário efetivo será o preço de venda ao público (que é o preço unitário).</span><span class="sxs-lookup"><span data-stu-id="f1335-168">If there are no resources for a particular meter that qualified for discount or partner earned credit, then the recon file will only contain one billing line and the effective unit price will be the retail price (which is the unit price).</span></span>

4. <span data-ttu-id="f1335-169">Se o contador, ou quaisquer recursos que emitem esse contador, se qualificasse para **Partner a ganhar crédito pelos serviços geridos** durante uma parte do mês, o ficheiro de reconhecimento conterá duas linhas de faturação.</span><span class="sxs-lookup"><span data-stu-id="f1335-169">If the meter, or any resources emitting that meter, qualified for **Partner earned credit for services managed** for a part of the month, the recon file will contain two billing lines.</span></span> <span data-ttu-id="f1335-170">Uma linha representará os dias em que o contador se qualificou e a segunda linha representará os dias em que o contador não se qualificou.</span><span class="sxs-lookup"><span data-stu-id="f1335-170">One line will represent the days the meter qualified and the second line will represent the days the meter did not qualify.</span></span>

## <a name="read-the-daily-usage-file"></a><span data-ttu-id="f1335-171">Leia o ficheiro de utilização diária</span><span class="sxs-lookup"><span data-stu-id="f1335-171">Read the daily usage file</span></span>

- <span data-ttu-id="f1335-172">Os contadores de subscrição ao abrigo de um plano Azure são avaliados, e são acumulados, diariamente.</span><span class="sxs-lookup"><span data-stu-id="f1335-172">Subscription meters under an Azure plan are rated, and are cumulated, on a daily basis.</span></span>

- <span data-ttu-id="f1335-173">**O parceiro que ganhou crédito pelos serviços geridos** é determinado e aplicado diariamente.</span><span class="sxs-lookup"><span data-stu-id="f1335-173">**Partner earned credit for services managed** is determined and applied on a daily basis.</span></span>

- <span data-ttu-id="f1335-174">Cada contador de assinaturas terá uma linha para cada dia do mês onde houve consumo.</span><span class="sxs-lookup"><span data-stu-id="f1335-174">Every subscription meter will have a row for every day of the month where there was consumption.</span></span>

- <span data-ttu-id="f1335-175">No exemplo abaixo:</span><span class="sxs-lookup"><span data-stu-id="f1335-175">In the example below:</span></span>

  - <span data-ttu-id="f1335-176">O medidor qualificado para **Parceiro ganhou crédito por serviços geridos** de 7/1 - 7/3 (note que o preço unitário efetivo é o preço de venda a retalho menos parceiro ganho crédito.</span><span class="sxs-lookup"><span data-stu-id="f1335-176">Meter qualified for **Partner earned credit for services managed** from 7/1 - 7/3 (note the effective unit price is retail price less partner earned credit.</span></span>

  - <span data-ttu-id="f1335-177">A Meter não se qualificou para **o Partner a ganhar crédito pelos serviços geridos** de 7/4 - 7/7 (note que o preço unitário efetivo é o preço de venda ao público).</span><span class="sxs-lookup"><span data-stu-id="f1335-177">Meter didn't qualify for **Partner earned credit for services managed** from 7/4 - 7/7 (note the effective unit price is retail price).</span></span>

  - <span data-ttu-id="f1335-178">O medidor qualificado para **Partner ganhou crédito por serviços geridos** de 7/8 - 7/31 (note que o preço unitário efetivo é o preço de venda a retalho menos parceiro ganho crédito).</span><span class="sxs-lookup"><span data-stu-id="f1335-178">Meter qualified for **Partner earned credit for services managed** from 7/8 - 7/31 (note the effective unit price is retail price less partner earned credit).</span></span>

   :::image type="content" source="images/azure/pecfinal.png" alt-text="recon2":::

## <a name="invoice-in-customer-currency"></a><span data-ttu-id="f1335-180">Fatura em moeda de cliente</span><span class="sxs-lookup"><span data-stu-id="f1335-180">Invoice in customer currency</span></span>

<span data-ttu-id="f1335-181">Os serviços Azure através de um plano Azure serão avaliados em USD e faturados na moeda atribuída pelo país cliente.</span><span class="sxs-lookup"><span data-stu-id="f1335-181">Azure services through an Azure plan will be priced in USD and billed in the customer country assigned currency.</span></span> <span data-ttu-id="f1335-182">Se a moeda de faturação não for USD, então a taxa cambial (FX) utilizada será mostrada na última página da fatura.</span><span class="sxs-lookup"><span data-stu-id="f1335-182">If the billing currency is non-USD, then the Foreign exchange (FX) rate used will be shown on the last page of the invoice.</span></span> <span data-ttu-id="f1335-183">As tarifas FX são determinadas mensalmente e aplicadas à seguinte fatura.</span><span class="sxs-lookup"><span data-stu-id="f1335-183">FX rates are determined monthly and applied to the following invoice.</span></span> <span data-ttu-id="f1335-184">Para obter uma lista completa de moedas de país, por favor, veja o [novo comércio oferece disponibilidade do país e matriz de moeda de cliente.](https://go.microsoft.com/fwlink/?linkid=2112354)</span><span class="sxs-lookup"><span data-stu-id="f1335-184">For a full list of country currencies, please view the [new commerce offers country availability and customer currency matrix](https://go.microsoft.com/fwlink/?linkid=2112354).</span></span>

<span data-ttu-id="f1335-185">A Microsoft segue a Bolsa de Valores de Londres para conversão.</span><span class="sxs-lookup"><span data-stu-id="f1335-185">Microsoft follows the London Stock Exchange for conversion.</span></span> <span data-ttu-id="f1335-186">Usamos a taxa de câmbio, que é igual à taxa de câmbio capturada no último segundo do último dia útil do mês na Bolsa de Valores de Londres.</span><span class="sxs-lookup"><span data-stu-id="f1335-186">We use the exchange rate, which is equal to the exchange rate captured on the last second of the last business day of the month on the London Stock Exchange.</span></span> <span data-ttu-id="f1335-187">As tarifas de FX serão atualizadas e disponíveis na véspera do primeiro dia do mês para o qual se candidatam.</span><span class="sxs-lookup"><span data-stu-id="f1335-187">The FX rates will be refreshed and available on the day before the first of the month for which they apply.</span></span>

## <a name="azure-reservations"></a><span data-ttu-id="f1335-188">Reservas do Azure</span><span class="sxs-lookup"><span data-stu-id="f1335-188">Azure reservations</span></span>


<span data-ttu-id="f1335-189">Se comprar [reservas do Azure](azure-reservations.md) através de um plano Azure, pode escolher faturação única ou mensal.</span><span class="sxs-lookup"><span data-stu-id="f1335-189">If purchasing [Azure reservations](azure-reservations.md) through an Azure plan, you can choose either one-time or monthly billing.</span></span>


## <a name="azure-spending"></a><span data-ttu-id="f1335-190">Despesas do Azure</span><span class="sxs-lookup"><span data-stu-id="f1335-190">Azure spending</span></span>

<span data-ttu-id="f1335-191">A experiência de gastos azure existente é atualizada para apoiar a nova faturação do plano Azure no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="f1335-191">The existing Azure spending experience is updated to support the new Azure plan billing in Partner Center.</span></span> <span data-ttu-id="f1335-192">Isto permite que os parceiros:</span><span class="sxs-lookup"><span data-stu-id="f1335-192">This enables partners to:</span></span>

- <span data-ttu-id="f1335-193">Ver, gerir e receber alertas de orçamento definidos ao nível do cliente</span><span class="sxs-lookup"><span data-stu-id="f1335-193">View, manage, and receive alerts for budget set at a customer level</span></span> 

- <span data-ttu-id="f1335-194">Ver os gastos totais estimados num plano Azure (discriminado pelo nível de recursos e contadores)</span><span class="sxs-lookup"><span data-stu-id="f1335-194">View total estimated spending on an Azure plan (broken down by resource and meter level)</span></span>

<span data-ttu-id="f1335-195">Uma vez que o modelo de faturação dos serviços Azure através de um plano Azure é o consumo pós-pagamento, para evitar uma fatura maior do que o previsto, os parceiros podem aplicar um orçamento mensal e acompanhar a percentagem de utilização.</span><span class="sxs-lookup"><span data-stu-id="f1335-195">Because the billing model for Azure services through an Azure plan is post-pay consumption, to avoid a bigger bill than anticipated, partners can apply a monthly budget and track the percentage of usage.</span></span> <span data-ttu-id="f1335-196">Um orçamento pode ser aplicado a um cliente ou a vários clientes de uma só vez.</span><span class="sxs-lookup"><span data-stu-id="f1335-196">A budget can be applied to one customer or multiple customers at one time.</span></span> 

:::image type="content" source="images/azure/azurespend.png" alt-text="Despesas do Azure":::

## <a name="next-steps"></a><span data-ttu-id="f1335-198">Próximos passos</span><span class="sxs-lookup"><span data-stu-id="f1335-198">Next steps</span></span>

- <span data-ttu-id="f1335-199">Veja como o parceiro obteve crédito (PEC) é calculado.</span><span class="sxs-lookup"><span data-stu-id="f1335-199">See how the partner earned credit (PEC) is calculated.</span></span> <span data-ttu-id="f1335-200">Inscreva-se no [painel do](https://partner.microsoft.com/dashboard/) Partner Center e localize a lista de preços disponíveis.</span><span class="sxs-lookup"><span data-stu-id="f1335-200">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/) and locate the price list available.</span></span>

- <span data-ttu-id="f1335-201">Conheça [a compra do plano Azure](purchase-azure-plan.md)</span><span class="sxs-lookup"><span data-stu-id="f1335-201">Learn about [purchasing the Azure plan](purchase-azure-plan.md)</span></span>

- <span data-ttu-id="f1335-202">Veja a [tabela de preços para a nova experiência de comércio na CSP](azure-plan-price-list.md)</span><span class="sxs-lookup"><span data-stu-id="f1335-202">See the [price list for the new commerce experience in CSP](azure-plan-price-list.md)</span></span>
