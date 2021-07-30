---
title: Gerir não pagamento, fraude ou uso indevido
description: Conheça os vários riscos envolvidos em transações online e as melhores práticas para gerir e mitigar esses riscos no Partner Center.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-payouts
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 07/14/2020
ms.openlocfilehash: f74a1c091a4c5cd838f8856152c1498f3ecd9d2b
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/29/2021
ms.locfileid: "114836749"
---
# <a name="managing-non-payment-fraud-or-misuse-in-partner-center"></a>Managing non-payment, fraud, or misuse in Partner Center (Gestão de não pagamento, fraude ou utilização indevida no Centro de Parceiros)

**Aplica-se a**: Partner Center | Centro de Parceiros para Microsoft Cloud for US Government

**Funções adequadas**: Administração global | Administração de administração de utilizadores | Agente administrativo | Administrador de faturação

É financeiramente responsável por compras fraudulentas por parte dos seus clientes e/ou do não pagamento dos serviços adquiridos. Por isso, *recomendamos vivamente que coloque em prática controlos de prevenção e deteção de riscos de deteção.*

Para evitar e/ou abordar atividades fraudulentas ou uso indevido, é importante compreender os riscos potenciais e desenvolver políticas e práticas que possam reduzir a sua exposição.

## <a name="enforcement-of-microsoft-acceptable-use-policy"></a>Aplicação da Política de Utilização Aceitável da Microsoft

Se a Microsoft detetar atividade de parceiro ou cliente que confirmamos ou suspeitamos violar a Política de Utilização Aceitável, tomaremos medidas de execução. O cliente pode ser imediatamente suspenso. Será notificado das ações de execução ou atualizado sobre os seus pedidos pela Microsoft.

## <a name="abuse-of-service-risks"></a>Abuso de riscos de serviço

**Abuso de** riscos de serviço significa clientes que usam serviços na nuvem em violação da Política de Utilização Aceitável da Microsoft.

### <a name="examples-of-abuse-of-service"></a>Exemplos de abuso de serviço

Exemplos destas violações da política de utilização aceitável da Microsoft podem incluir:

- Spamming
- Hacking
- Ataques de negação de serviço distribuídos (DDoS)
- Mineração de Bitcoin
- Distribuição de malware
- Revenda de assinaturas piratas

## <a name="theft-of-service-risks"></a>Roubo de riscos de serviço

**O roubo de** riscos de serviço significa clientes que não têm intenção de pagar por serviços consumidos. Este roubo pode envolver a utilização de instrumentos de pagamento roubados, a disponibilização de informações falsas de faturação e/ou incumprimento de saldos pendentes.

### <a name="examples-of-service-theft"></a>Exemplos de roubo de serviço

Exemplos destes riscos de transação online podem incluir:

- Transações que não ocorrem presencialmente ("cartão de crédito não presente" transações)
- Identidades mal representadas
- Serviços prestados e utilizados antes do pagamento inicial
- Mercados emergentes e/ou regiões de alto risco para fraudes em linha
- Automatizar a criação e compra de contas por maus atores

## <a name="managing-online-risk"></a>Gerir o risco online

Pode utilizar as seguintes recomendações para o ajudar a desenvolver políticas e práticas para reduzir a sua exposição a riscos de transação online no ciclo de vida das suas relações com o cliente.

### <a name="onboarding-new-customers"></a>Embarque de novos clientes

As sugestões para reduzir os riscos on-line ao embarcar novos clientes incluem:

- Estabelecer relações pessoais com os clientes quando possível (por exemplo, contactar os clientes por telefone).
- Verifique as credenciais e antecedentes dos clientes através de melhores métodos (tais como a utilização de agências de crédito ou agências de relatórios comerciais comerciais).
- Utilize a autenticação de vários fatores (como a verificação de SMS) durante a inscrição para minimizar a exposição à criação e compra de contas robóticas.
- Gerir e rastrear identidades utilizando serviços (como serviços de identidade digital).
- Avaliar a solidez financeira do cliente através de rigorosos sistemas de deteção de fraudes com cartões de crédito.
- Estabeleça uma política clara de cobranças. Detalhe o seu processo de cobranças e quando o acesso a subscrições será impactado pelo não pagamento. (Pode desativar o acesso ou [suspender as subscrições de um cliente](create-a-new-subscription.md#suspend-a-subscription) por não pagamento.)

### <a name="managing-customer-accounts"></a>Managing customer accounts (Gerir contas de clientes)

As sugestões para gerir as contas dos clientes após a compra incluem:

- Implementar um processo para receber, rever, agir e responder às notificações da Microsoft.
- Trabalhe com os clientes para compreender as suas necessidades de negócio de uso em nuvem, ao mesmo tempo que estabelece limiares de monitorização apropriados. (Por exemplo, pode [definir um orçamento mensal de gastos da Azure](set-an-azure-spending-budget-for-your-customers.md) no Partner Center. Este entendimento permite-lhe monitorizar o uso do cliente durante o mês e ser notificado quando os clientes estão próximos do seu orçamento.)
- Monitorize [regularmente os registos de atividade do cliente](activity-logs.md) para ajudar a detetar a fraude precocemente.
- Tome medidas rápidas quando forem detetadas atividades suspeitas.
- Evite dar aos clientes acesso administrativo total a subscrições sem primeiro implementar controlos de mitigação de riscos.

### <a name="managing-customer-billing"></a>Gestão da faturação do cliente

As sugestões para gerir a faturação do cliente após a compra incluem:

- Solicite pré-pagamentos antes das transações iniciais e faturação.
- Não aceite instrumentos de pagamento de alto risco (como cartões pré-pagos ou cartões de valor armazenado).
- Monitorize os pagamentos dos clientes e as contas de envelhecimento a receber. Aplicar agressivamente processos de dunning padronizados para pagamentos em atraso ou não pagamento.

Para estratégias mais detalhadas para mitigar o risco online, consulte o guia de gestão de [risco de transação online.](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4Bhtt)
