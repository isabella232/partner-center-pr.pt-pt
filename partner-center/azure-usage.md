---
title: Dimensionamento da VM do Azure para a máxima utilização de reserva
description: Aprenda a dimensionar uma máquina virtual (VM) às necessidades de computação dos seus clientes quando comprar Microsoft Azure reservas para eles.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.date: 08/06/2020
ms.openlocfilehash: 650618de7460f4667c60ac58cbe6716530db7f16
ms.sourcegitcommit: b55f63a029d88c73cd5190bbac2df1b5990e6e44
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/08/2021
ms.locfileid: "113510198"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a><span data-ttu-id="f54fa-103">Dimensionamento da VM do Microsoft Azure para a máxima utilização de reserva</span><span class="sxs-lookup"><span data-stu-id="f54fa-103">Microsoft Azure VM sizing for maximum reservation usage</span></span>

<span data-ttu-id="f54fa-104">**Funções adequadas**: Agente administrador | Agente comercial</span><span class="sxs-lookup"><span data-stu-id="f54fa-104">**Appropriate roles**: Admin agent | Sales agent</span></span>

<span data-ttu-id="f54fa-105">Este artigo explica como dimensionar uma máquina virtual (VM) às necessidades de computação dos seus clientes quando compra reservas Microsoft Azure para eles.</span><span class="sxs-lookup"><span data-stu-id="f54fa-105">This article explains how to size a virtual machine (VM) to your customers' computing needs when you buy Microsoft Azure reservations for them.</span></span>
 
> [!NOTE]
> <span data-ttu-id="f54fa-106">Este artigo aplica-se apenas aos parceiros do programa Fornecedor de Soluções em Nuvem (CSP).</span><span class="sxs-lookup"><span data-stu-id="f54fa-106">This article applies only to partners in the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="f54fa-107">Os clientes que utilizem outros tipos de subscrições (como, por exemplo, pay-as-you-go, individual, Microsoft Customer Agreement ou Contrato Enterprise subscrições) devem, em vez disso, ler [esta documentação de reservas Azure](/azure/cost-management-billing/reservations).</span><span class="sxs-lookup"><span data-stu-id="f54fa-107">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a><span data-ttu-id="f54fa-108">Determine o tamanho VM para a reserva Azure de um cliente</span><span class="sxs-lookup"><span data-stu-id="f54fa-108">Determine the VM size for a customer's Azure reservation</span></span>

<span data-ttu-id="f54fa-109">Ao comprar reservas Microsoft Azure em nome dos seus clientes, terá de escolher uma máquina virtual (VM) de tamanho para atender às necessidades de computação do cliente.</span><span class="sxs-lookup"><span data-stu-id="f54fa-109">When buying Microsoft Azure reservations on behalf of your customers, you'll need to choose a virtual machine (VM) sized to meet the customer's computing needs.</span></span> <span data-ttu-id="f54fa-110">Pode encontrar esta informação utilizando um destes métodos:</span><span class="sxs-lookup"><span data-stu-id="f54fa-110">You can find this information using one of these methods:</span></span>

- <span data-ttu-id="f54fa-111">API de utilização de Azure</span><span class="sxs-lookup"><span data-stu-id="f54fa-111">Azure utilization API</span></span>
- <span data-ttu-id="f54fa-112">O portal do Azure</span><span class="sxs-lookup"><span data-stu-id="f54fa-112">The Azure portal</span></span>
- <span data-ttu-id="f54fa-113">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="f54fa-113">Azure PowerShell</span></span>
- <span data-ttu-id="f54fa-114">A API gestora de recursos da Azure (ARM)</span><span class="sxs-lookup"><span data-stu-id="f54fa-114">The Azure Resource Manager (ARM) API</span></span>

<span data-ttu-id="f54fa-115">As instruções para a utilização de cada um destes métodos estão abaixo.</span><span class="sxs-lookup"><span data-stu-id="f54fa-115">Instructions for using each of these methods are below.</span></span> <span data-ttu-id="f54fa-116">Depois de comprar uma reserva, o desconto de reserva é aplicado automaticamente a máquinas virtuais que correspondam aos atributos e quantidade da reserva.</span><span class="sxs-lookup"><span data-stu-id="f54fa-116">After you buy a reservation, the reservation discount is applied automatically to virtual machines matching the attributes and quantity of the reservation.</span></span> <span data-ttu-id="f54fa-117">Não precisa atribuir a reserva a um VM.</span><span class="sxs-lookup"><span data-stu-id="f54fa-117">You don't need to assign the reservation to a VM.</span></span>

>[!NOTE]
><span data-ttu-id="f54fa-118">Os descontos de reserva não se aplicam a VMs clássicos ou promocionais.</span><span class="sxs-lookup"><span data-stu-id="f54fa-118">Reservation discounts don't apply to classic or promotional VMs.</span></span>

>[!IMPORTANT]
><span data-ttu-id="f54fa-119">Para identificar corretamente o tipo e o tamanho de VM para comprar em nome do seu cliente, deve utilizar um dos métodos descritos abaixo, uma vez que o tipo de série VM não está corretamente apresentado nos ficheiros de reconciliação do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="f54fa-119">To correctly identify the type and size of VM to buy on behalf of your customer, you must use one of the methods described below as the VM series type is not correctly displayed in Partner Center reconciliation files.</span></span>

### <a name="get-vm-sizing-information-using-the-azure-utilization-api"></a><span data-ttu-id="f54fa-120">Obtenha informações de tamanho VM utilizando a API de utilização do Azure</span><span class="sxs-lookup"><span data-stu-id="f54fa-120">Get VM sizing information using the Azure utilization API</span></span>

1. <span data-ttu-id="f54fa-121">Utilize o valor para atributo ServiceType de informação adicional deInfo na resposta API para identificar o tamanho VM para comprar.</span><span class="sxs-lookup"><span data-stu-id="f54fa-121">Use the value for ServiceType attribute from additionalInfo in the API response to identify the VM size to buy.</span></span>

2. <span data-ttu-id="f54fa-122">Para obter mais informações, [consulte os registos de utilização de um cliente para a Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) na [API](/partner-center/develop/)do Partner Center .</span><span class="sxs-lookup"><span data-stu-id="f54fa-122">For more information, see [Get a customer's utilization records for Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](/partner-center/develop/).</span></span>

### <a name="get-vm-sizing-information-using-the-microsoft-azure-portal"></a><span data-ttu-id="f54fa-123">Obtenha informações de tamanho VM usando o portal Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="f54fa-123">Get VM sizing information using the Microsoft Azure portal</span></span>

1. <span data-ttu-id="f54fa-124">No Partner Center, vá à página **dos seus Clientes.**</span><span class="sxs-lookup"><span data-stu-id="f54fa-124">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="f54fa-125">Encontre o cliente que quer comprar reservas Azure VM e, em seguida, selecione a seta para baixo para expandir a informação do cliente.</span><span class="sxs-lookup"><span data-stu-id="f54fa-125">Find the customer who wants to buy Azure VM reservations and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="f54fa-126">Selecione **Microsoft Azure Portal de Gestão** para abrir o registo do cliente no portal Azure.</span><span class="sxs-lookup"><span data-stu-id="f54fa-126">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>

3. <span data-ttu-id="f54fa-127">Selecione **máquinas Virtuais** a partir do menu do portal e, em seguida, selecione o VM para o qual deseja comprar uma reserva.</span><span class="sxs-lookup"><span data-stu-id="f54fa-127">Select **Virtual machines** from the portal menu and then select the VM for which you want to buy a reservation.</span></span>

4. <span data-ttu-id="f54fa-128">Na página de detalhes do VM, encontre as informações sobre o tamanho e a região, conforme ilustrado abaixo, e use esta informação para comprar a reserva no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="f54fa-128">On the VM's detail page, find the size and region information, as illustrated below, and use this information to purchase the reservation in Partner Center.</span></span>  

   :::image type="content" source="images/usage1.png" alt-text="Informações sobre tamanho e região na página de detalhes.":::

### <a name="get-vm-sizing-information-using-microsoft-azure-powershell"></a><span data-ttu-id="f54fa-130">Obtenha informações de tamanho VM usando Microsoft Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="f54fa-130">Get VM sizing information using Microsoft Azure PowerShell</span></span>

<span data-ttu-id="f54fa-131">Utilize as informações na imagem abaixo para obter a localização e o tamanho do VM para o qual pretende comprar uma reserva.</span><span class="sxs-lookup"><span data-stu-id="f54fa-131">Use the information in the image below to get the location and size of the VM for which you want to buy a reservation.</span></span> 

:::image type="content" source="images/usage2.png" alt-text="Localização e tamanho VM.":::

### <a name="get-vm-sizing-information-using-the-azure-resource-manager-arm-api"></a><span data-ttu-id="f54fa-133">Obtenha informações de tamanho VM utilizando a API AZure Resource Manager (ARM)</span><span class="sxs-lookup"><span data-stu-id="f54fa-133">Get VM sizing information using the Azure Resource Manager (ARM) API</span></span>

1. <span data-ttu-id="f54fa-134">Utilizando o ARMClient ou as APIs ARM, ligue para o cliente ARM para o VM para o qual pretende comprar uma reserva.</span><span class="sxs-lookup"><span data-stu-id="f54fa-134">Using the ARMClient or the ARM APIs, call the ARM client for the VM for which you want to buy a reservation.</span></span>

2. `/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01`

3. <span data-ttu-id="f54fa-135">A chamada devolve os valores para **vmSize** e **localização,** conforme ilustrado abaixo.</span><span class="sxs-lookup"><span data-stu-id="f54fa-135">The call returns the values for **vmSize** and **location**, as illustrated below.</span></span>

    :::image type="content" source="images/usage3.png" alt-text="valor vmSize.":::
    :::image type="content" source="images/usage4.png" alt-text="valor de localização.":::

## <a name="verify-azure-vm-usage-and-reservation-discount"></a><span data-ttu-id="f54fa-138">Verifique o uso do Azure VM e o desconto de reserva</span><span class="sxs-lookup"><span data-stu-id="f54fa-138">Verify Azure VM usage and reservation discount</span></span>

<span data-ttu-id="f54fa-139">Depois de adquirir uma Instância VM Reservada Azure em nome de um cliente, o desconto para pagar antecipadamente o espaço VM é aplicado automaticamente às máquinas virtuais que correspondem aos atributos e quantidade da reserva do cliente.</span><span class="sxs-lookup"><span data-stu-id="f54fa-139">After you purchase an Azure Reserved VM Instance on behalf of a customer, the discount for paying for VM space in advance is automatically applied to the virtual machines that match the attributes and quantity of the customer's reservation.</span></span>

<span data-ttu-id="f54fa-140">Pode verificar o uso da reserva do cliente e ver a que máquinas virtuais são aplicadas os descontos de reserva utilizando um dos seguintes métodos:</span><span class="sxs-lookup"><span data-stu-id="f54fa-140">You can verify the customer's reservation usage and see which virtual machines the reservation discounts are applied to by using one of the following methods:</span></span>

- <span data-ttu-id="f54fa-141">O portal do Azure</span><span class="sxs-lookup"><span data-stu-id="f54fa-141">The Azure portal</span></span>
- <span data-ttu-id="f54fa-142">API de utilização de Azure</span><span class="sxs-lookup"><span data-stu-id="f54fa-142">Azure utilization API</span></span>

<span data-ttu-id="f54fa-143">As instruções para a utilização de cada um destes métodos estão abaixo.</span><span class="sxs-lookup"><span data-stu-id="f54fa-143">Instructions for using each of these methods are below.</span></span>

>[!NOTE]
><span data-ttu-id="f54fa-144">Apenas a API de utilização Azure mostra a que máquina virtual o desconto está a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="f54fa-144">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a><span data-ttu-id="f54fa-145">Verifique o uso da reserva do cliente no portal Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="f54fa-145">Verify the customer's reservation usage in the Microsoft Azure portal</span></span>

1. <span data-ttu-id="f54fa-146">No Partner Center, vá à página **dos seus Clientes.**</span><span class="sxs-lookup"><span data-stu-id="f54fa-146">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="f54fa-147">Encontre o cliente cujo desconto e utilização de reserva pretende verificar e, em seguida, selecione a seta para baixo para expandir as informações do cliente.</span><span class="sxs-lookup"><span data-stu-id="f54fa-147">Find the customer whose reservation discount and usage you want to verify and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="f54fa-148">Selecione **Microsoft Azure Portal de Gestão** para abrir o registo do cliente no portal Azure.</span><span class="sxs-lookup"><span data-stu-id="f54fa-148">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>
3. <span data-ttu-id="f54fa-149">Selecione **Reservas** no menu do portal e, em seguida, selecione a reserva para a quais pretende verificar a utilização.</span><span class="sxs-lookup"><span data-stu-id="f54fa-149">Select **Reservations** from the portal menu and then select the reservation you want to check usage for.</span></span>
4. <span data-ttu-id="f54fa-150">Na página **'Visão Geral'** verifique o gráfico de utilização da reserva, que mostra quanto da reserva foi aplicada a máquinas virtuais.</span><span class="sxs-lookup"><span data-stu-id="f54fa-150">On the **Overview** page check the reservation's utilization graph, which shows how much of the reservation was applied to virtual machines.</span></span>

    >[!NOTE]
    ><span data-ttu-id="f54fa-151">Os dados de utilização podem ser adiados até 8 horas.</span><span class="sxs-lookup"><span data-stu-id="f54fa-151">Utilization data may be delayed by up to 8 hours.</span></span>

    <span data-ttu-id="f54fa-152">a.</span><span class="sxs-lookup"><span data-stu-id="f54fa-152">a.</span></span> <span data-ttu-id="f54fa-153">Se a utilização da reserva for de 100%, o seu cliente está a receber todas as poupanças possíveis que a compra da reserva pode fornecer.</span><span class="sxs-lookup"><span data-stu-id="f54fa-153">If the reservation's utilization is 100%, your customer is getting all the possible savings that the reservation purchase can provide.</span></span>
    <span data-ttu-id="f54fa-154">b.</span><span class="sxs-lookup"><span data-stu-id="f54fa-154">b.</span></span> <span data-ttu-id="f54fa-155">Se o uso da reserva for de 0%, o desconto não está a ser aplicado a nenhuma máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="f54fa-155">If the reservation's usage is 0%, the discount is not being applied to any virtual machine.</span></span>
    <span data-ttu-id="f54fa-156">c.</span><span class="sxs-lookup"><span data-stu-id="f54fa-156">c.</span></span> <span data-ttu-id="f54fa-157">Se o uso da reserva for entre 1% e 99%, existem benefícios não uusados.</span><span class="sxs-lookup"><span data-stu-id="f54fa-157">If the reservation's usage is between 1% and 99%, there are unused benefits.</span></span>

5. <span data-ttu-id="f54fa-158">Para evitar esta situação, determine o tamanho correto VM para suportar as necessidades de computação do cliente antes de efetuar a compra.</span><span class="sxs-lookup"><span data-stu-id="f54fa-158">To avoid this situation, determine the correct size VM to support the customer's computing needs before making the purchase.</span></span>

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a><span data-ttu-id="f54fa-159">Verifique o uso da reserva do cliente com a API de utilização de utilização Azure</span><span class="sxs-lookup"><span data-stu-id="f54fa-159">Verify the customer's reservation usage with the Azure utilization API</span></span>

>[!NOTE]
><span data-ttu-id="f54fa-160">Apenas a API de utilização Azure mostra a que máquina virtual o desconto está a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="f54fa-160">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

<span data-ttu-id="f54fa-161">Pode obter dados de utilização da reserva com a API de utilização Azure para verificar se o cliente está a receber o desconto de reserva e para ver a que VMs (máquinas virtuais) o desconto é aplicado.</span><span class="sxs-lookup"><span data-stu-id="f54fa-161">You can get reservation usage data with the Azure utilization API to verify that the customer is getting the reservation discount and to see which VMs (virtual machines) the discount is applied to.</span></span> <span data-ttu-id="f54fa-162">Compare o exemplo A ao exemplo B para ver como verificar o uso da reserva de um cliente.</span><span class="sxs-lookup"><span data-stu-id="f54fa-162">Compare Example A to Example B to see how to verify a customer's reservation usage.</span></span>

:::image type="content" source="images/usage5.png" alt-text="Exemplos de utilização da reserva.":::

- <span data-ttu-id="f54fa-164">O reservationId identifica a reserva Azure que foi usada para aplicar o desconto ao VM.</span><span class="sxs-lookup"><span data-stu-id="f54fa-164">The reservationId identifies the Azure reservation that was used to apply the discount to the VM.</span></span>
- <span data-ttu-id="f54fa-165">consumptionMeter é o MeterId para o VM que tem o desconto de reserva aplicado a ele.</span><span class="sxs-lookup"><span data-stu-id="f54fa-165">consumptionMeter is the MeterId for the VM that has the reservation discount applied to it.</span></span>
- <span data-ttu-id="f54fa-166">O ReservationMeter mostra um custo de $0 desde que o desconto de reserva foi aplicado.</span><span class="sxs-lookup"><span data-stu-id="f54fa-166">The ReservationMeter shows $0 cost since the reservation discount was applied.</span></span>

<span data-ttu-id="f54fa-167">Para obter mais informações, [consulte os registos de utilização de um cliente para a Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) na [API](/partner-center/develop/)do Partner Center .</span><span class="sxs-lookup"><span data-stu-id="f54fa-167">For more information, see [Get a customer's utilization records for Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](/partner-center/develop/).</span></span>

>[!IMPORTANT]
><span data-ttu-id="f54fa-168">Os custos do software, como o Microsoft Windows Server, não estão atualmente incluídos no preço de uma reserva VM e aparecerão como itens de linha separados no registo de encomendas e na sua fatura.</span><span class="sxs-lookup"><span data-stu-id="f54fa-168">Software costs, such as Microsoft Windows Server, are not currently included in the price of a VM reservation and will appear as separate line items in the order record and on your invoice.</span></span> <span data-ttu-id="f54fa-169">No entanto, se um cliente tiver o Azure Hybrid Use Benefit, os custos do software não serão aplicados.</span><span class="sxs-lookup"><span data-stu-id="f54fa-169">However, if a customer has the Azure Hybrid Use Benefit, the software costs will not be applied.</span></span> <span data-ttu-id="f54fa-170">Para obter mais informações, consulte [Windows custos de software não incluídos nas Instâncias Reservadas.](/azure/billing/billing-reserved-instance-windows-software-costs)</span><span class="sxs-lookup"><span data-stu-id="f54fa-170">For more information, see [Windows software costs not included with Reserved Instances](/azure/billing/billing-reserved-instance-windows-software-costs).</span></span>  

## <a name="next-steps"></a><span data-ttu-id="f54fa-171">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="f54fa-171">Next steps</span></span>

|<span data-ttu-id="f54fa-172">**Para obter informações sobre**</span><span class="sxs-lookup"><span data-stu-id="f54fa-172">**For information about**</span></span>   |<span data-ttu-id="f54fa-173">**Leia isto**</span><span class="sxs-lookup"><span data-stu-id="f54fa-173">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
|<span data-ttu-id="f54fa-174">Reservas Azure em visão geral da CSP</span><span class="sxs-lookup"><span data-stu-id="f54fa-174">Azure reservations in CSP overview</span></span>  | [<span data-ttu-id="f54fa-175">Venda Microsoft Azure Instâncias VM Reservadas</span><span class="sxs-lookup"><span data-stu-id="f54fa-175">Sell Microsoft Azure Reserved VM Instances</span></span>](azure-reservations.md)
|<span data-ttu-id="f54fa-176">Comprar reservas da Azure para os seus clientes no Partner Center</span><span class="sxs-lookup"><span data-stu-id="f54fa-176">Purchasing Azure reservations for your customers in Partner Center</span></span>   | [<span data-ttu-id="f54fa-177">Comprar reservas Azure</span><span class="sxs-lookup"><span data-stu-id="f54fa-177">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="f54fa-178">Gerir reservas da Azure no Partner Center</span><span class="sxs-lookup"><span data-stu-id="f54fa-178">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="f54fa-179">Gerir reservas da Azure no Partner Center</span><span class="sxs-lookup"><span data-stu-id="f54fa-179">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="f54fa-180">Compras Reservas do Azure no portal Azure</span><span class="sxs-lookup"><span data-stu-id="f54fa-180">Purchasing Azure reservations in the Azure portal</span></span> | <span data-ttu-id="f54fa-181">[Pré-pagamento para máquinas virtuais com Azure Reservado VM Instances](/azure/virtual-machines/windows/prepay-reserved-vm-instances) na Ajuda Azure</span><span class="sxs-lookup"><span data-stu-id="f54fa-181">[Prepay for virtual machines with Azure Reserved VM Instances](/azure/virtual-machines/windows/prepay-reserved-vm-instances) in the Azure Help</span></span> |
|<span data-ttu-id="f54fa-182">Gerir reservas do Azure no portal Azure</span><span class="sxs-lookup"><span data-stu-id="f54fa-182">Managing Azure reservations in the Azure portal</span></span>   | <span data-ttu-id="f54fa-183">[Gerir instâncias VM reservadas](/azure/billing/billing-manage-reserved-vm-instance) na Ajuda Azure</span><span class="sxs-lookup"><span data-stu-id="f54fa-183">[Manage reserved VM instances](/azure/billing/billing-manage-reserved-vm-instance) in the Azure Help</span></span>  |
|<span data-ttu-id="f54fa-184">Compras Reservas Azure usando a API do Centro Parceiro</span><span class="sxs-lookup"><span data-stu-id="f54fa-184">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="f54fa-185">[Comprar Azure Reservado VM Instances](/partner-center/develop/purchase-azure-reservations) na documentação do desenvolvedor do Partner Center</span><span class="sxs-lookup"><span data-stu-id="f54fa-185">[Purchase Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="f54fa-186">Dando permissão aos clientes para comprarem as suas próprias reservas Azure a partir de uma subscrição que adquiriu para eles.</span><span class="sxs-lookup"><span data-stu-id="f54fa-186">Giving customers permission to buy their own Azure reservations from a subscription you purchased for them.</span></span> | [<span data-ttu-id="f54fa-187">Dê permissão aos clientes para comprarem as suas próprias reservas Azure</span><span class="sxs-lookup"><span data-stu-id="f54fa-187">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |