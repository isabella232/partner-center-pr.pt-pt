---
title: Gerir reservas da Azure para clientes
description: Saiba como gerir as reservas da Azure para um cliente, incluindo como cancelar uma reserva, trocar uma reserva ou solicitar um reembolso.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
author: amitravat
ms.author: amrava
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 08/06/2020
ms.openlocfilehash: 627c6f8d09a904e7d988c4229ec10eeac38dc2e9
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/29/2021
ms.locfileid: "114841475"
---
# <a name="manage-cancel-exchange-or-refund-microsoft-azure-reservations-for-customers"></a>Gerir, cancelar, trocar ou reembolsar reservas Microsoft Azure para clientes

**Funções adequadas**: Agente administrador | Administração global | Agente helpdesk | Agente comercial | Administração de gestão de utilizadores

Este artigo explica como gerir as reservas do Azure para um cliente, incluindo como cancelar uma reserva, trocar uma reserva ou solicitar um reembolso.

> [!NOTE]
> Este artigo aplica-se apenas aos parceiros do programa Fornecedor de Soluções em Nuvem (CSP). Os clientes que utilizem outros tipos de subscrições (como, por exemplo, pay-as-you-go, individual, Microsoft Customer Agreement ou Contrato Enterprise subscrições) devem, em vez disso, ler [esta documentação de reservas Azure](/azure/cost-management-billing/reservations).

Para gerir as reservas Azure dos seus clientes após a compra, seleciona o cliente e a reserva que pretende gerir no Partner Center e, em seguida, efetua alterações na reserva no portal Azure.

1. Para começar, selecione **Clientes** do menu Partner Center e, em seguida, selecione o cliente cujas reservas pretende gerir. 

2. No menu de página de pormenor do cliente, selecione **reservas Azure** e, em seguida, selecione a reserva específica que pretende gerir.  

3. Em **Ações**, **selecione Gerir** para o registo de reservas do cliente no portal Azure. Na página de detalhes da reserva, siga os passos abaixo para completar as tarefas.  

    | **Selecionar**   | **Para**    |
    |:-----------------------------|:-----------------|
    | **Descrição geral**   | Ver detalhes da reserva de um cliente, incluindo data de validade, âmbito e dados de utilização. **NOTA** Selecione **Reembolso** para criar um pedido de apoio para um reembolso com classificação profissional. Selecione **Exchange** para criar um pedido de apoio para trocar a parte não utilizada do seu termo de reserva.  
    | **Controlo de Acesso (IAM)**   | Gerir o acesso à informação de reserva do cliente.|
    | **Configuração**   | Altere o âmbito da reserva e/ou a subscrição do Azure a que a reserva está associada.    |
    | **Propriedades**   | Veja as propriedades da reserva e copie para a área de transferência o ID de reserva e o ID do pedido de reserva. **NOTA** O suporte poderá pedir-lhe o ID da reserva e o ID da encomenda de reservas quando solicitar apoio em nome de um cliente.    |
    | **Novo pedido de apoio**    | Solicite ajuda ao Microsoft Support.   |
 
## <a name="cancel-or-exchange-a-reservation"></a>Cancelar ou trocar uma reserva

Se em algum momento o negócio de um cliente precisar de ser alterado, eles podem querer cancelar uma reserva e obter um reembolso ou trocar o valor de reembolso proratado de uma reserva para ser usado para o preço de uma nova reserva.

Em ambos os cenários, a Microsoft reembolsa o valor para que possa gerir as transações financeiras resultantes com os seus clientes. A Microsoft não contacta diretamente os clientes sobre faturação, cancelamentos ou reembolsos.

### <a name="how-cancellations-work"></a>Como funcionam os cancelamentos

Os clientes podem solicitar o cancelamento de uma reserva a qualquer momento (valor de reembolso limitado a $50.000 por ano). O cancelamento de uma reserva permite ao cliente devolver o valor dos meses restantes de uma reserva Azure para uma taxa de rescisão antecipada. O saldo remanescente, menos a taxa de rescisão antecipada, é reembolsado na sua conta para que possa reembolsar a conta do cliente. 

Veja abaixo os detalhes e taxas de cancelamento.


|**Data de cancelamento**<br> (dias)   |**Utilização**    |**Crédito**  |**Rescisão antecipada**<br> taxa    |**Limite máximo de reembolso** | 
|:----------------------------------|:------------|:-----------|:--------------------------------|:--------------|
|5 ou menos                         | Não          | 100%       | Não                              | $50.000 USD   |
|5 ou menos                         | Sim         | Pro-rated  | Não                              | $50.000 USD   |
|Mais de 5                        | Não          | Pro-rated  | 12%                             | $50.000 USD   |
|Mais de 5                        | Sim         | Pro-rated  | 12%                             | $50.000 USD   |

### <a name="how-exchanges-work"></a>Como funcionam as trocas 

Se um cliente quiser comprar uma reserva diferente da que originalmente lhe compraram, pode solicitar uma troca. Trocar uma reserva pode ser uma alternativa atraente para cancelar uma reserva porque permite ao cliente usar o valor de reembolso protuado para o preço da nova reserva. 

O valor do reembolso procitado é creditado na sua conta para que possa oferecer ao cliente uma troca.

## <a name="request-a-refund-or-exchange-on-behalf-of-a-customer"></a>Solicitar um reembolso ou troca em nome de um cliente

Para apresentar um pedido de apoio para reembolso ou troca em nome dos seus clientes, irá selecionar o cliente e a reserva no Partner Center e, em seguida, criar o pedido de suporte no portal Azure. 

>[!NOTE]
>Os agentes do Microsoft Support podem pedir-lhe para fornecer o ID de reserva e o ID da encomenda de reserva. Pode encontrar esta informação na página **Propriedades** da reserva no portal Azure.

1. Para começar, selecione **Clientes** do menu Partner Center e, em seguida, selecione o cliente que quer um reembolso. 

2. Na página de detalhes do cliente, selecione **reservas Azure** e, em seguida, selecione a reserva específica que o cliente quer que seja reembolsada.  

3. Em **Ações**, **selecione Refund** para ir ao registo de reservas do cliente no portal Azure e inicie um pedido de apoio.  

4. Na página de **novo pedido de apoio,** siga os passos abaixo para solicitar o reembolso. Selecione **Seguinte** após cada passo. 

   |**Passo**                    |**Seleções**    |
   |:---------------------------|:-----------------|
   |**1 Básicos**                |Tipo de edição: Faturação.  |
   |**2 Problema**               |Tipo de problema: Gestão de reservas. Categoria: Trocas e reembolsos. |
   |**3 Informações de contacto**   |Selecione as suas preferências e introduza as informações necessárias. 

5. **Selecione Criar** quando feito.

## <a name="azure-reservations-resources"></a>Recursos de reservas Azure

|**Para obter informações sobre**   |**Leia isto**    |
|:-----------------------------|:-----------------|
|Reservas Azure em visão geral da CSP  | [Venda Microsoft Azure Instâncias Reservadas](azure-reservations.md) |
|Comprar reservas da Azure para os seus clientes no Partner Center   | [Comprar reservas Azure](azure-reservations-buying.md) |
|Determine o tamanho VM correto e verifique a utilização do VM do cliente   | [Tamanho VM para o máximo uso da reserva Azure](azure-usage.md)   |
|Compras Reservas Azure usando a API do Centro Parceiro | [Comprar Azure Reservado VM Instances](/partner-center/develop/purchase-azure-reservations) na documentação do desenvolvedor do Partner Center   |
|Dando permissão aos clientes para comprarem as suas próprias reservas Azure a partir de uma subscrição que adquiriu para eles. | [Dê permissão aos clientes para comprarem as suas próprias reservas Azure](give-customers-permission.md)   |