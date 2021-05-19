---
title: Problemas de associação dos clientes aos Incentivos
description: Saiba como resolver problemas que surgem quando trabalhar com associações de clientes Claimed Partner of Record (CPOR).
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.date: 09/11/2020
ms.openlocfilehash: 8f1c087911e6dd7e58182c99e2b97b7a6b2246d8
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110152176"
---
# <a name="issues-with-claimed-partner-of-record-cpor-customer-associations"></a>Problemas com associações de clientes do Parceiro Reclamado da Record (CPOR)

**Funções apropriadas**: Administrador de Faturação | Administração global | Administradores de incentivos

O conteúdo abaixo irá ajudá-lo a resolver problemas que podem surgir quando trabalha com associações de clientes.

## <a name="domain-tenant-mismatch"></a>Desfasamento entre o inacompusado do inquilino de domínio

No fluxo de reclamação do Parceiro Reclamado da Record (CPOR), será solicitado que forneça o ID e subdomínio do cliente. Se receber um erro indicando que não correspondem, contacte o seu cliente para garantir que tem os detalhes corretos.

## <a name="subscription-errors-in-the-cpor-association-claim-flow"></a>Erros de subscrição no fluxo de reclamação da associação CPOR

No fluxo de reclamação da associação CPOR, poderá ser-lhe solicitada a subscrição de um produto que está a tentar reivindicar através de Aplicações Empresariais (Dynamics 365). Pedimos a assinatura porque estamos a verificar dinamicamente se o produto e a subscrição pertencem ao inquilino que está a ser reclamado. Também estamos verificando se a subscrição está em estado de ativa/em graça.

Se receber o erro, pode ser por várias razões:

- O produto selecionado não existe no inquilino do cliente
- A subscrição fornecida não é para a Dynamics
- A subscrição indicada é do CSP
- O cliente ainda não ativou/a forteou os produtos para essa subscrição
- A subscrição já foi pedida
- O identificador fornecido não é um ID de assinatura

Se tiver alguma dúvida sobre a exatidão da sua subscrição, trabalhe com o seu cliente para garantir que a subscrição está correta e que está a utilizar o ID do inquilino correto.

Se esta rota não tiver resolvido o seu problema, contacte [o suporte](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives).

## <a name="when-subscriptions-will-be-available-to-claim"></a>Quando as subscrições estarão disponíveis para reclamar

Ao reclamar uma subscrição, receberá um erro se a subscrição ainda não tiver sido a provisionada. Existem vários passos que o cliente precisa de tomar para que a subscrição fique disponível para a plataforma CPOR para buscá-la e disponibilizá-la para reclamar. Se estiver a receber um erro ao tentar reclamar uma subscrição, contacte o seu cliente para garantir que foi a provisionada e que a subscrição que está a reivindicar está correta. Se já tomou esta rota, contacte [o suporte.](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives)

## <a name="which-activity-do-i-choose"></a>Que atividade escolho?

A plataforma de reclamação CPOR permite reclamações de associação CPOR relacionadas com aplicações empresariais e áreas de solução Microsoft 365. As atividades que são aplicáveis a cada área de solução estão abaixo. Selecione a atividade correta com base nas descrições para evitar ter que recuperar no futuro. Reivindicar com uma atividade incorreta pode resultar em ganhos de elegibilidade e incentivos perdidos.


| Área de solução | Atividade | Aplicável para |
| ------ | ----------- | ----------- |
| Aplicações empresariais      | Pré-venda   | Selecione se influenciou a sua compra de um produto elegível e deseja solicitar incentivos de pré-venda. Esta opção só é aplicável se o cliente tiver adquirido estes produtos através de contrato de licenciamento de volume ou web-direct. |
|    |  Utilização  | Selecione se você conduzir a sua adoção e uso de uma carga de trabalho elegível, e quer solicitar incentivos de uso. Esta opção só é aplicável se o cliente tiver adquirido estes produtos através de contrato de licenciamento de volume ou web-direct. |
|    | Associação de receitas   | Selecione se influenciou a sua seleção de um produto elegível como Influenciador de Negócios. Esta opção é apenas para associação de receitas, não para pagamentos de incentivos. Esta opção só é aplicável se o cliente tiver adquirido estes produtos através de contrato de licenciamento de volume ou web-direct.   |
| Microsoft 365   | Utilização   | Selecione se você conduzir a sua adoção e uso de uma carga de trabalho elegível, e quer solicitar incentivos de uso. |

## <a name="which-mpn-do-i-choose"></a>Que MPN escolho?

No fluxo de reclamação da associação CPOR, será solicitado que escolha uma empresa MPN que deve estar associada ao trabalho que reclama no cliente final. A sua empresa pode ter muitos MPNs, alguns dos quais podem estar matriculados em programas de incentivo, e outros associados a um tipo de parceiro como o FRP FastTrack. A associação CPOR alega que o fluxo irá identificar quais mpNs estão inscritos num programa de incentivos, mas não lhe dirá se é um parceiro específico mpn. É importante selecionar o MPN correto, para evitar ter que recuperar no futuro. Alegar com uma MPN incorreta pode resultar em ganhos de elegibilidade e incentivos perdidos.

Se não souber qual a MPN a utilizar, contacte o seu administrador global.

Se o MPN que pretende utilizar não estiver inscrito, pode geri-lo no [separador Visão Geral](https://partner.microsoft.com/dashboard/incentives/enrollment/summary) dos Incentivos (inscrição obrigatória).

## <a name="choosing-a-product-vs-entering-a-subscription"></a>Escolher um produto vs inserindo uma subscrição

Quando um produto Dynamics é reclamado e aprovado, o parceiro pode ver o ID de subscrição na própria reivindicação da associação CPOR. Quando esta subscrição é reclamada, está em estado ativo ou em estado de graça, mas pode haver um momento em que a subscrição termina, e as novas subscrições terão de ser reclamadas numa reivindicação separada da associação CPOR.

## <a name="competing-claims"></a>Créditos concorrentes

Se estiver a criar uma reivindicação de associação CPOR para um cliente e seus produtos(s) que já está associado a outro parceiro, a sua reclamação passará por arbitragem:

1. Depois de criar uma nova associação de clientes, a Microsoft verificará os detalhes da associação e a prova de execução indicada para garantir a precisão.

2. Se você e outro parceiro reclamarem o mesmo cliente e produto/carga de trabalho, a Microsoft irá rever a documentação de execução de cada parceiro para determinar que parceiro aprovar.

3. Informações adicionais podem ser solicitadas a ambos os parceiros, o que pode causar atrasos no processamento do seu pedido de associação.

4. A sua reivindicação de associação CPOR ainda será revista dentro de cinco dias úteis, embora o seu estatuto possa permanecer como _Under Review_ por um período de tempo mais longo. Este cenário pode acontecer quando a Microsoft trabalha com o parceiro que possui atualmente o produto/carga de trabalho. Será notificado na secção de comentários da sua reclamação, se for esse o caso. 

>[!IMPORTANT]
>Se precisarmos de informações adicionais para verificar a sua prova de execução (PoE) da sua associação CPOR, entraremos em contacto consigo através da secção de comentários da associação CPOR.

## <a name="next-steps"></a>Passos seguintes

- [Introdução aos incentivos](incentives-get-started-intro.md)
