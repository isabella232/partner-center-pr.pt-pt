---
title: Dimensionamento da VM do Azure para a máxima utilização de reserva
description: Aprenda a dimensionar uma máquina virtual (VM) às necessidades de computação dos seus clientes quando comprar reservas do Microsoft Azure para eles.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.date: 08/06/2020
ms.openlocfilehash: 2d8bc76e0da51abf433e49028445b398c6a1db31
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276999"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a><span data-ttu-id="e502c-103">Dimensionamento da VM do Microsoft Azure para a máxima utilização de reserva</span><span class="sxs-lookup"><span data-stu-id="e502c-103">Microsoft Azure VM sizing for maximum reservation usage</span></span>

<span data-ttu-id="e502c-104">**Funções adequadas**: Agente administrador | Agente comercial</span><span class="sxs-lookup"><span data-stu-id="e502c-104">**Appropriate roles**: Admin agent | Sales agent</span></span>

<span data-ttu-id="e502c-105">Este artigo explica como dimensionar uma máquina virtual (VM) às necessidades de computação dos seus clientes quando compra reservas do Microsoft Azure para eles.</span><span class="sxs-lookup"><span data-stu-id="e502c-105">This article explains how to size a virtual machine (VM) to your customers' computing needs when you buy Microsoft Azure reservations for them.</span></span>
 
> [!NOTE]
> <span data-ttu-id="e502c-106">Este artigo aplica-se apenas aos parceiros do programa Cloud Solution Provider (CSP).</span><span class="sxs-lookup"><span data-stu-id="e502c-106">This article applies only to partners in the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="e502c-107">Os clientes que utilizem outros tipos de subscrições (tais como, pay-as-you-go, individual, Microsoft Customer Agreement ou Enterprise Agreement) devem, em vez disso, ler [esta documentação de reservas Azure](/azure/cost-management-billing/reservations).</span><span class="sxs-lookup"><span data-stu-id="e502c-107">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a><span data-ttu-id="e502c-108">Determine o tamanho VM para a reserva Azure de um cliente</span><span class="sxs-lookup"><span data-stu-id="e502c-108">Determine the VM size for a customer's Azure reservation</span></span>

<span data-ttu-id="e502c-109">Ao comprar reservas do Microsoft Azure em nome dos seus clientes, terá de escolher uma máquina virtual (VM) do tamanho de atender às necessidades de computação do cliente.</span><span class="sxs-lookup"><span data-stu-id="e502c-109">When buying Microsoft Azure reservations on behalf of your customers, you'll need to choose a virtual machine (VM) sized to meet the customer's computing needs.</span></span> <span data-ttu-id="e502c-110">Pode encontrar esta informação utilizando um destes métodos:</span><span class="sxs-lookup"><span data-stu-id="e502c-110">You can find this information using one of these methods:</span></span>

- <span data-ttu-id="e502c-111">API de utilização de Azure</span><span class="sxs-lookup"><span data-stu-id="e502c-111">Azure utilization API</span></span>
- <span data-ttu-id="e502c-112">O portal do Azure</span><span class="sxs-lookup"><span data-stu-id="e502c-112">The Azure portal</span></span>
- <span data-ttu-id="e502c-113">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="e502c-113">Azure PowerShell</span></span>
- <span data-ttu-id="e502c-114">A API gestora de recursos da Azure (ARM)</span><span class="sxs-lookup"><span data-stu-id="e502c-114">The Azure Resource Manager (ARM) API</span></span>

<span data-ttu-id="e502c-115">As instruções para a utilização de cada um destes métodos estão abaixo.</span><span class="sxs-lookup"><span data-stu-id="e502c-115">Instructions for using each of these methods are below.</span></span> <span data-ttu-id="e502c-116">Depois de comprar uma reserva, o desconto de reserva é aplicado automaticamente a máquinas virtuais que correspondam aos atributos e quantidade da reserva.</span><span class="sxs-lookup"><span data-stu-id="e502c-116">After you buy a reservation, the reservation discount is applied automatically to virtual machines matching the attributes and quantity of the reservation.</span></span> <span data-ttu-id="e502c-117">Não precisa atribuir a reserva a um VM.</span><span class="sxs-lookup"><span data-stu-id="e502c-117">You don't need to assign the reservation to a VM.</span></span>

>[!NOTE]
><span data-ttu-id="e502c-118">Os descontos de reserva não se aplicam a VMs clássicos ou promocionais.</span><span class="sxs-lookup"><span data-stu-id="e502c-118">Reservation discounts don't apply to classic or promotional VMs.</span></span>

>[!IMPORTANT]
><span data-ttu-id="e502c-119">Para identificar corretamente o tipo e o tamanho de VM para comprar em nome do seu cliente, deve utilizar um dos métodos descritos abaixo, uma vez que o tipo de série VM não está corretamente apresentado nos ficheiros de reconciliação do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="e502c-119">To correctly identify the type and size of VM to buy on behalf of your customer, you must use one of the methods described below as the VM series type is not correctly displayed in Partner Center reconciliation files.</span></span>

### <a name="get-vm-sizing-information-using-the-azure-utilization-api"></a><span data-ttu-id="e502c-120">Obtenha informações de tamanho VM utilizando a API de utilização do Azure</span><span class="sxs-lookup"><span data-stu-id="e502c-120">Get VM sizing information using the Azure utilization API</span></span>

1. <span data-ttu-id="e502c-121">Utilize o valor para atributo ServiceType de informação adicional deInfo na resposta API para identificar o tamanho VM para comprar.</span><span class="sxs-lookup"><span data-stu-id="e502c-121">Use the value for ServiceType attribute from additionalInfo in the API response to identify the VM size to buy.</span></span>

2. <span data-ttu-id="e502c-122">Para obter mais informações, [consulte os registos de utilização de um cliente para a Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) na [API](/partner-center/develop/)do Partner Center .</span><span class="sxs-lookup"><span data-stu-id="e502c-122">For more information, see [Get a customer's utilization records for Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](/partner-center/develop/).</span></span>

### <a name="get-vm-sizing-information-using-the-microsoft-azure-portal"></a><span data-ttu-id="e502c-123">Obtenha informações de tamanho VM utilizando o portal Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="e502c-123">Get VM sizing information using the Microsoft Azure portal</span></span>

1. <span data-ttu-id="e502c-124">No Partner Center, vá à página **dos seus Clientes.**</span><span class="sxs-lookup"><span data-stu-id="e502c-124">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="e502c-125">Encontre o cliente que quer comprar reservas Azure VM e, em seguida, selecione a seta para baixo para expandir a informação do cliente.</span><span class="sxs-lookup"><span data-stu-id="e502c-125">Find the customer who wants to buy Azure VM reservations and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="e502c-126">Selecione **o Microsoft Azure Management Portal** para abrir o registo do cliente no portal Azure.</span><span class="sxs-lookup"><span data-stu-id="e502c-126">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>

3. <span data-ttu-id="e502c-127">Selecione **máquinas Virtuais** a partir do menu do portal e, em seguida, selecione o VM para o qual deseja comprar uma reserva.</span><span class="sxs-lookup"><span data-stu-id="e502c-127">Select **Virtual machines** from the portal menu and then select the VM for which you want to buy a reservation.</span></span>

4. <span data-ttu-id="e502c-128">Na página de detalhes do VM, encontre as informações sobre o tamanho e a região, conforme ilustrado abaixo, e use esta informação para comprar a reserva no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="e502c-128">On the VM's detail page, find the size and region information, as illustrated below, and use this information to purchase the reservation in Partner Center.</span></span>  

   :::image type="content" source="images/usage1.png" alt-text="Informações sobre tamanho e região na página de detalhes.":::

### <a name="get-vm-sizing-information-using-microsoft-azure-powershell"></a><span data-ttu-id="e502c-130">Obtenha informações de tamanho VM usando Microsoft Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="e502c-130">Get VM sizing information using Microsoft Azure PowerShell</span></span>

<span data-ttu-id="e502c-131">Utilize as informações na imagem abaixo para obter a localização e o tamanho do VM para o qual pretende comprar uma reserva.</span><span class="sxs-lookup"><span data-stu-id="e502c-131">Use the information in the image below to get the location and size of the VM for which you want to buy a reservation.</span></span> 

:::image type="content" source="images/usage2.png" alt-text="Localização e tamanho VM.":::

### <a name="get-vm-sizing-information-using-the-azure-resource-manager-arm-api"></a><span data-ttu-id="e502c-133">Obtenha informações de tamanho VM utilizando a API AZure Resource Manager (ARM)</span><span class="sxs-lookup"><span data-stu-id="e502c-133">Get VM sizing information using the Azure Resource Manager (ARM) API</span></span>

1. <span data-ttu-id="e502c-134">Utilizando o ARMClient ou as APIs ARM, ligue para o cliente ARM para o VM para o qual pretende comprar uma reserva.</span><span class="sxs-lookup"><span data-stu-id="e502c-134">Using the ARMClient or the ARM APIs, call the ARM client for the VM for which you want to buy a reservation.</span></span>

2. <span data-ttu-id="e502c-135">/subscrições/ <Subscription ID> /resourceGroups/ <Resource group name> /providers/Microsoft.Compute/virtualMachines/ <VM Instance Name> ?api-version=2017-12-01</span><span class="sxs-lookup"><span data-stu-id="e502c-135">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span></span>

3. <span data-ttu-id="e502c-136">A chamada devolve os valores para **vmSize** e **localização,** conforme ilustrado abaixo.</span><span class="sxs-lookup"><span data-stu-id="e502c-136">The call returns the values for **vmSize** and **location**, as illustrated below.</span></span>

    :::image type="content" source="images/usage3.png" alt-text="valor vmSize.":::
    :::image type="content" source="images/usage4.png" alt-text="valor de localização.":::

## <a name="verify-azure-vm-usage-and-reservation-discount"></a><span data-ttu-id="e502c-139">Verifique o uso do Azure VM e o desconto de reserva</span><span class="sxs-lookup"><span data-stu-id="e502c-139">Verify Azure VM usage and reservation discount</span></span>

<span data-ttu-id="e502c-140">Depois de adquirir uma Instância VM Reservada Azure em nome de um cliente, o desconto para pagar antecipadamente o espaço VM é aplicado automaticamente às máquinas virtuais que correspondem aos atributos e quantidade da reserva do cliente.</span><span class="sxs-lookup"><span data-stu-id="e502c-140">After you purchase an Azure Reserved VM Instance on behalf of a customer, the discount for paying for VM space in advance is automatically applied to the virtual machines that match the attributes and quantity of the customer's reservation.</span></span>

<span data-ttu-id="e502c-141">Pode verificar o uso da reserva do cliente e ver a que máquinas virtuais são aplicadas os descontos de reserva utilizando um dos seguintes métodos:</span><span class="sxs-lookup"><span data-stu-id="e502c-141">You can verify the customer's reservation usage and see which virtual machines the reservation discounts are applied to by using one of the following methods:</span></span>

- <span data-ttu-id="e502c-142">O portal do Azure</span><span class="sxs-lookup"><span data-stu-id="e502c-142">The Azure portal</span></span>
- <span data-ttu-id="e502c-143">API de utilização de Azure</span><span class="sxs-lookup"><span data-stu-id="e502c-143">Azure utilization API</span></span>

<span data-ttu-id="e502c-144">As instruções para a utilização de cada um destes métodos estão abaixo.</span><span class="sxs-lookup"><span data-stu-id="e502c-144">Instructions for using each of these methods are below.</span></span>

>[!NOTE]
><span data-ttu-id="e502c-145">Apenas a API de utilização Azure mostra a que máquina virtual o desconto está a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="e502c-145">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a><span data-ttu-id="e502c-146">Verifique a utilização da reserva do cliente no portal Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="e502c-146">Verify the customer's reservation usage in the Microsoft Azure portal</span></span>

1. <span data-ttu-id="e502c-147">No Partner Center, vá à página **dos seus Clientes.**</span><span class="sxs-lookup"><span data-stu-id="e502c-147">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="e502c-148">Encontre o cliente cujo desconto e utilização de reserva pretende verificar e, em seguida, selecione a seta para baixo para expandir as informações do cliente.</span><span class="sxs-lookup"><span data-stu-id="e502c-148">Find the customer whose reservation discount and usage you want to verify and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="e502c-149">Selecione **o Microsoft Azure Management Portal** para abrir o registo do cliente no portal Azure.</span><span class="sxs-lookup"><span data-stu-id="e502c-149">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>
3. <span data-ttu-id="e502c-150">Selecione **Reservas** no menu do portal e, em seguida, selecione a reserva para a quais pretende verificar a utilização.</span><span class="sxs-lookup"><span data-stu-id="e502c-150">Select **Reservations** from the portal menu and then select the reservation you want to check usage for.</span></span>
4. <span data-ttu-id="e502c-151">Na página **'Visão Geral'** verifique o gráfico de utilização da reserva, que mostra quanto da reserva foi aplicada a máquinas virtuais.</span><span class="sxs-lookup"><span data-stu-id="e502c-151">On the **Overview** page check the reservation's utilization graph, which shows how much of the reservation was applied to virtual machines.</span></span>

    >[!NOTE]
    ><span data-ttu-id="e502c-152">Os dados de utilização podem ser adiados até 8 horas.</span><span class="sxs-lookup"><span data-stu-id="e502c-152">Utilization data may be delayed by up to 8 hours.</span></span>

    <span data-ttu-id="e502c-153">a.</span><span class="sxs-lookup"><span data-stu-id="e502c-153">a.</span></span> <span data-ttu-id="e502c-154">Se a utilização da reserva for de 100%, o seu cliente está a receber todas as poupanças possíveis que a compra da reserva pode fornecer.</span><span class="sxs-lookup"><span data-stu-id="e502c-154">If the reservation's utilization is 100%, your customer is getting all the possible savings that the reservation purchase can provide.</span></span>
    <span data-ttu-id="e502c-155">b.</span><span class="sxs-lookup"><span data-stu-id="e502c-155">b.</span></span> <span data-ttu-id="e502c-156">Se o uso da reserva for de 0%, o desconto não está a ser aplicado a nenhuma máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="e502c-156">If the reservation's usage is 0%, the discount is not being applied to any virtual machine.</span></span>
    <span data-ttu-id="e502c-157">c.</span><span class="sxs-lookup"><span data-stu-id="e502c-157">c.</span></span> <span data-ttu-id="e502c-158">Se o uso da reserva for entre 1% e 99%, existem benefícios não uusados.</span><span class="sxs-lookup"><span data-stu-id="e502c-158">If the reservation's usage is between 1% and 99%, there are unused benefits.</span></span>

5. <span data-ttu-id="e502c-159">Para evitar esta situação, determine o tamanho correto VM para suportar as necessidades de computação do cliente antes de efetuar a compra.</span><span class="sxs-lookup"><span data-stu-id="e502c-159">To avoid this situation, determine the correct size VM to support the customer's computing needs before making the purchase.</span></span>

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a><span data-ttu-id="e502c-160">Verifique o uso da reserva do cliente com a API de utilização de utilização Azure</span><span class="sxs-lookup"><span data-stu-id="e502c-160">Verify the customer's reservation usage with the Azure utilization API</span></span>

>[!NOTE]
><span data-ttu-id="e502c-161">Apenas a API de utilização Azure mostra a que máquina virtual o desconto está a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="e502c-161">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

<span data-ttu-id="e502c-162">Pode obter dados de utilização da reserva com a API de utilização Azure para verificar se o cliente está a receber o desconto de reserva e para ver a que VMs (máquinas virtuais) o desconto é aplicado.</span><span class="sxs-lookup"><span data-stu-id="e502c-162">You can get reservation usage data with the Azure utilization API to verify that the customer is getting the reservation discount and to see which VMs (virtual machines) the discount is applied to.</span></span> <span data-ttu-id="e502c-163">Compare o exemplo A ao exemplo B para ver como verificar o uso da reserva de um cliente.</span><span class="sxs-lookup"><span data-stu-id="e502c-163">Compare Example A to Example B to see how to verify a customer's reservation usage.</span></span>

:::image type="content" source="images/usage5.png" alt-text="Exemplos de utilização da reserva.":::

- <span data-ttu-id="e502c-165">O reservationId identifica a reserva Azure que foi usada para aplicar o desconto ao VM.</span><span class="sxs-lookup"><span data-stu-id="e502c-165">The reservationId identifies the Azure reservation that was used to apply the discount to the VM.</span></span>
- <span data-ttu-id="e502c-166">consumptionMeter é o MeterId para o VM que tem o desconto de reserva aplicado a ele.</span><span class="sxs-lookup"><span data-stu-id="e502c-166">consumptionMeter is the MeterId for the VM that has the reservation discount applied to it.</span></span>
- <span data-ttu-id="e502c-167">O ReservationMeter mostra um custo de $0 desde que o desconto de reserva foi aplicado.</span><span class="sxs-lookup"><span data-stu-id="e502c-167">The ReservationMeter shows $0 cost since the reservation discount was applied.</span></span>

<span data-ttu-id="e502c-168">Para obter mais informações, [consulte os registos de utilização de um cliente para a Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) na [API](/partner-center/develop/)do Partner Center .</span><span class="sxs-lookup"><span data-stu-id="e502c-168">For more information, see [Get a customer's utilization records for Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](/partner-center/develop/).</span></span>

>[!IMPORTANT]
><span data-ttu-id="e502c-169">Os custos do software, como o Microsoft Windows Server, não estão atualmente incluídos no preço de uma reserva VM e aparecerão como itens de linha separados no registo de encomendas e na sua fatura.</span><span class="sxs-lookup"><span data-stu-id="e502c-169">Software costs, such as Microsoft Windows Server, are not currently included in the price of a VM reservation and will appear as separate line items in the order record and on your invoice.</span></span> <span data-ttu-id="e502c-170">No entanto, se um cliente tiver o Azure Hybrid Use Benefit, os custos do software não serão aplicados.</span><span class="sxs-lookup"><span data-stu-id="e502c-170">However, if a customer has the Azure Hybrid Use Benefit, the software costs will not be applied.</span></span> <span data-ttu-id="e502c-171">Para obter mais informações, consulte [os custos do software windows não incluídos nas Instâncias Reservadas.](/azure/billing/billing-reserved-instance-windows-software-costs)</span><span class="sxs-lookup"><span data-stu-id="e502c-171">For more information, see [Windows software costs not included with Reserved Instances](/azure/billing/billing-reserved-instance-windows-software-costs).</span></span>  

## <a name="next-steps"></a><span data-ttu-id="e502c-172">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="e502c-172">Next steps</span></span>

|<span data-ttu-id="e502c-173">**Para obter informações sobre**</span><span class="sxs-lookup"><span data-stu-id="e502c-173">**For information about**</span></span>   |<span data-ttu-id="e502c-174">**Leia isto**</span><span class="sxs-lookup"><span data-stu-id="e502c-174">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
|<span data-ttu-id="e502c-175">Reservas Azure em visão geral da CSP</span><span class="sxs-lookup"><span data-stu-id="e502c-175">Azure reservations in CSP overview</span></span>  | [<span data-ttu-id="e502c-176">Vender Instâncias VM Reservadas microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="e502c-176">Sell Microsoft Azure Reserved VM Instances</span></span>](azure-reservations.md)
|<span data-ttu-id="e502c-177">Comprar reservas da Azure para os seus clientes no Partner Center</span><span class="sxs-lookup"><span data-stu-id="e502c-177">Purchasing Azure reservations for your customers in Partner Center</span></span>   | [<span data-ttu-id="e502c-178">Comprar reservas Azure</span><span class="sxs-lookup"><span data-stu-id="e502c-178">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="e502c-179">Gerir reservas da Azure no Partner Center</span><span class="sxs-lookup"><span data-stu-id="e502c-179">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="e502c-180">Gerir reservas da Azure no Partner Center</span><span class="sxs-lookup"><span data-stu-id="e502c-180">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="e502c-181">Compras Reservas do Azure no portal Azure</span><span class="sxs-lookup"><span data-stu-id="e502c-181">Purchasing Azure reservations in the Azure portal</span></span> | <span data-ttu-id="e502c-182">[Pré-pagamento para máquinas virtuais com Azure Reservado VM Instances](/azure/virtual-machines/windows/prepay-reserved-vm-instances) na Ajuda Azure</span><span class="sxs-lookup"><span data-stu-id="e502c-182">[Prepay for virtual machines with Azure Reserved VM Instances](/azure/virtual-machines/windows/prepay-reserved-vm-instances) in the Azure Help</span></span> |
|<span data-ttu-id="e502c-183">Gerir reservas do Azure no portal Azure</span><span class="sxs-lookup"><span data-stu-id="e502c-183">Managing Azure reservations in the Azure portal</span></span>   | <span data-ttu-id="e502c-184">[Gerir instâncias VM reservadas](/azure/billing/billing-manage-reserved-vm-instance) na Ajuda Azure</span><span class="sxs-lookup"><span data-stu-id="e502c-184">[Manage reserved VM instances](/azure/billing/billing-manage-reserved-vm-instance) in the Azure Help</span></span>  |
|<span data-ttu-id="e502c-185">Compras Reservas Azure usando a API do Centro Parceiro</span><span class="sxs-lookup"><span data-stu-id="e502c-185">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="e502c-186">[Comprar Azure Reservado VM Instances](/partner-center/develop/purchase-azure-reservations) na documentação do desenvolvedor do Partner Center</span><span class="sxs-lookup"><span data-stu-id="e502c-186">[Purchase Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="e502c-187">Dando permissão aos clientes para comprarem as suas próprias reservas Azure a partir de uma subscrição que adquiriu para eles.</span><span class="sxs-lookup"><span data-stu-id="e502c-187">Giving customers permission to buy their own Azure reservations from a subscription you purchased for them.</span></span> | [<span data-ttu-id="e502c-188">Dê permissão aos clientes para comprarem as suas próprias reservas Azure</span><span class="sxs-lookup"><span data-stu-id="e502c-188">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |