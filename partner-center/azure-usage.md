---
title: Dimensionamento da VM do Azure para a máxima utilização de reserva
description: Aprenda a dimensionar uma máquina virtual (VM) às necessidades de computação dos seus clientes quando comprar Microsoft Azure reservas para eles.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.date: 08/06/2020
ms.openlocfilehash: f6392bf0e2d5feb37db38b2c185c07b4cb2cc1e01f7ab29fa1991d8e9357d276
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/06/2021
ms.locfileid: "115680642"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a>Dimensionamento da VM do Microsoft Azure para a máxima utilização de reserva

**Funções adequadas**: Agente administrador | Agente comercial

Este artigo explica como dimensionar uma máquina virtual (VM) às necessidades de computação dos seus clientes quando compra reservas Microsoft Azure para eles.
 
> [!NOTE]
> Este artigo aplica-se apenas aos parceiros do programa Fornecedor de Soluções em Nuvem (CSP). Os clientes que utilizem outros tipos de subscrições (como, por exemplo, pay-as-you-go, individual, Microsoft Customer Agreement ou Contrato Enterprise subscrições) devem, em vez disso, ler [esta documentação de reservas Azure](/azure/cost-management-billing/reservations).

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a>Determine o tamanho VM para a reserva Azure de um cliente

Ao comprar reservas Microsoft Azure em nome dos seus clientes, terá de escolher uma máquina virtual (VM) de tamanho para atender às necessidades de computação do cliente. Pode encontrar esta informação utilizando um destes métodos:

- API de utilização de Azure
- O portal do Azure
- Azure PowerShell
- A API gestora de recursos da Azure (ARM)

As instruções para a utilização de cada um destes métodos estão abaixo. Depois de comprar uma reserva, o desconto de reserva é aplicado automaticamente a máquinas virtuais que correspondam aos atributos e quantidade da reserva. Não precisa atribuir a reserva a um VM.

>[!NOTE]
>Os descontos de reserva não se aplicam a VMs clássicos ou promocionais.

>[!IMPORTANT]
>Para identificar corretamente o tipo e o tamanho de VM para comprar em nome do seu cliente, deve utilizar um dos métodos descritos abaixo, uma vez que o tipo de série VM não está corretamente apresentado nos ficheiros de reconciliação do Partner Center.

### <a name="get-vm-sizing-information-using-the-azure-utilization-api"></a>Obtenha informações de tamanho VM utilizando a API de utilização do Azure

1. Utilize o valor para atributo ServiceType de informação adicional deInfo na resposta API para identificar o tamanho VM para comprar.

2. Para obter mais informações, [consulte os registos de utilização de um cliente para a Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) na [API](/partner-center/develop/)do Partner Center .

### <a name="get-vm-sizing-information-using-the-microsoft-azure-portal"></a>Obtenha informações de tamanho VM usando o portal Microsoft Azure

1. No Partner Center, vá à página **dos seus Clientes.**

2. Encontre o cliente que quer comprar reservas Azure VM e, em seguida, selecione a seta para baixo para expandir a informação do cliente. Selecione **Microsoft Azure Portal de Gestão** para abrir o registo do cliente no portal Azure.

3. Selecione **máquinas Virtuais** a partir do menu do portal e, em seguida, selecione o VM para o qual deseja comprar uma reserva.

4. Na página de detalhes do VM, encontre as informações sobre o tamanho e a região, conforme ilustrado abaixo, e use esta informação para comprar a reserva no Partner Center.  

   :::image type="content" source="images/usage1.png" alt-text="Informações sobre tamanho e região na página de detalhes.":::

### <a name="get-vm-sizing-information-using-microsoft-azure-powershell"></a>Obtenha informações de tamanho VM usando Microsoft Azure PowerShell

Utilize as informações na imagem abaixo para obter a localização e o tamanho do VM para o qual pretende comprar uma reserva. 

:::image type="content" source="images/usage2.png" alt-text="Localização e tamanho VM.":::

### <a name="get-vm-sizing-information-using-the-azure-resource-manager-arm-api"></a>Obtenha informações de tamanho VM utilizando a API AZure Resource Manager (ARM)

1. Utilizando o ARMClient ou as APIs ARM, ligue para o cliente ARM para o VM para o qual pretende comprar uma reserva.

2. `/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01`

3. A chamada devolve os valores para **vmSize** e **localização,** conforme ilustrado abaixo.

    :::image type="content" source="images/usage3.png" alt-text="valor vmSize.":::
    :::image type="content" source="images/usage4.png" alt-text="valor de localização.":::

## <a name="verify-azure-vm-usage-and-reservation-discount"></a>Verifique o uso do Azure VM e o desconto de reserva

Depois de adquirir uma Instância VM Reservada Azure em nome de um cliente, o desconto para pagar antecipadamente o espaço VM é aplicado automaticamente às máquinas virtuais que correspondem aos atributos e quantidade da reserva do cliente.

Pode verificar o uso da reserva do cliente e ver a que máquinas virtuais são aplicadas os descontos de reserva utilizando um dos seguintes métodos:

- O portal do Azure
- API de utilização de Azure

As instruções para a utilização de cada um destes métodos estão abaixo.

>[!NOTE]
>Apenas a API de utilização Azure mostra a que máquina virtual o desconto está a ser aplicado.  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a>Verifique o uso da reserva do cliente no portal Microsoft Azure

1. No Partner Center, vá à página **dos seus Clientes.**

2. Encontre o cliente cujo desconto e utilização de reserva pretende verificar e, em seguida, selecione a seta para baixo para expandir as informações do cliente. Selecione **Microsoft Azure Portal de Gestão** para abrir o registo do cliente no portal Azure.
3. Selecione **Reservas** no menu do portal e, em seguida, selecione a reserva para a quais pretende verificar a utilização.
4. Na página **'Visão Geral'** verifique o gráfico de utilização da reserva, que mostra quanto da reserva foi aplicada a máquinas virtuais.

    >[!NOTE]
    >Os dados de utilização podem ser adiados até 8 horas.

    a. Se a utilização da reserva for de 100%, o seu cliente está a receber todas as poupanças possíveis que a compra da reserva pode fornecer.
    b. Se o uso da reserva for de 0%, o desconto não está a ser aplicado a nenhuma máquina virtual.
    c. Se o uso da reserva for entre 1% e 99%, existem benefícios não uusados.

5. Para evitar esta situação, determine o tamanho correto VM para suportar as necessidades de computação do cliente antes de efetuar a compra.

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a>Verifique o uso da reserva do cliente com a API de utilização de utilização Azure

>[!NOTE]
>Apenas a API de utilização Azure mostra a que máquina virtual o desconto está a ser aplicado.  

Pode obter dados de utilização da reserva com a API de utilização Azure para verificar se o cliente está a receber o desconto de reserva e para ver a que VMs (máquinas virtuais) o desconto é aplicado. Compare o exemplo A ao exemplo B para ver como verificar o uso da reserva de um cliente.

:::image type="content" source="images/usage5.png" alt-text="Exemplos de utilização da reserva.":::

- O reservationId identifica a reserva Azure que foi usada para aplicar o desconto ao VM.
- consumptionMeter é o MeterId para o VM que tem o desconto de reserva aplicado a ele.
- O ReservationMeter mostra um custo de $0 desde que o desconto de reserva foi aplicado.

Para obter mais informações, [consulte os registos de utilização de um cliente para a Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) na [API](/partner-center/develop/)do Partner Center .

>[!IMPORTANT]
>Os custos do software, como o Microsoft Windows Server, não estão atualmente incluídos no preço de uma reserva VM e aparecerão como itens de linha separados no registo de encomendas e na sua fatura. No entanto, se um cliente tiver o Azure Hybrid Use Benefit, os custos do software não serão aplicados. Para obter mais informações, consulte [Windows custos de software não incluídos nas Instâncias Reservadas.](/azure/billing/billing-reserved-instance-windows-software-costs)  

## <a name="next-steps"></a>Passos seguintes

|**Para obter informações sobre**   |**Leia isto**    |
|:-----------------------------|:-----------------|
|Reservas Azure em visão geral da CSP  | [Venda Microsoft Azure Instâncias VM Reservadas](azure-reservations.md)
|Comprar reservas da Azure para os seus clientes no Partner Center   | [Comprar reservas Azure](azure-reservations-buying.md)
|Gerir reservas da Azure no Partner Center | [Gerir reservas da Azure no Partner Center](azure-reservations-manage.md)
|Compras Reservas do Azure no portal Azure | [Pré-pagamento para máquinas virtuais com Azure Reservado VM Instances](/azure/virtual-machines/windows/prepay-reserved-vm-instances) na Ajuda Azure |
|Gerir reservas do Azure no portal Azure   | [Gerir instâncias VM reservadas](/azure/billing/billing-manage-reserved-vm-instance) na Ajuda Azure  |
|Compras Reservas Azure usando a API do Centro Parceiro | [Comprar Azure Reservado VM Instances](/partner-center/develop/purchase-azure-reservations) na documentação do desenvolvedor do Partner Center   |
|Dando permissão aos clientes para comprarem as suas próprias reservas Azure a partir de uma subscrição que adquiriu para eles. | [Dê permissão aos clientes para comprarem as suas próprias reservas Azure](give-customers-permission.md)   |