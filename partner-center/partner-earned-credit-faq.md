---
title: Parceiro ganhou crédito FAQ
ms.topic: article
ms.date: 08/13/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Encontrar respostas a perguntas frequentes sobre o parceiro ganhou crédito (PEC).
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 7e09a4f82704a7336ea7a30241219f9e19d2ef5c
ms.sourcegitcommit: 76a7dac540d129ae15cd4c251a4ff43d768370da
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/06/2021
ms.locfileid: "129593281"
---
# <a name="frequently-asked-questions-for-partner-earned-credit"></a>Perguntas frequentes para parceiro ganhou crédito

Funções adequadas: Administração global | Administração de administração de utilizadores | Agente administrativo | Administrador de faturação | Agente comercial

Segue-se uma lista de perguntas frequentes sobre o parceiro que ganhou crédito.

## <a name="how-much-is-pec"></a>Quanto custa o PEC?

O valor que os parceiros ganham para o PEC variará (ver [Cálculo).](partner-earned-credit-explanation.md#calculation) A tarifa pode ser encontrada na página da lista de preços dentro do Partner Center.

## <a name="what-azure-services-are-eligible-for-pec"></a>Que serviços da Azure são elegíveis para o PEC?

A PEC é elegível para todos os serviços relacionados com a nova oferta Azure em CSP (plano Azure), com exceção dos seguintes: 
- Novas reservas de oferta Azure (plano Azure)
- Produtos de terceiros identificados como Terceiros na coluna Tags da lista de preços de consumo do plano Azure
- Produtos na tabela de preços do Mercado
- [Máquinas virtuais Azure Spot](https://partner.microsoft.com/resources/collection/azure-spot-in-csp#/)

## <a name="where-can-i-see-pec"></a>Onde posso ver o PEC?

Ver [Cálculo](partner-earned-credit-explanation.md#calculation).

## <a name="where-can-i-find-pec-details"></a>Onde posso encontrar detalhes do PEC?

Os detalhes do PEC podem ser consultados pela API, [pelo arquivo de reconhecimento diário](partner-earned-credit-explanation.md#calculation) e pela [ACM (Azure Cost Mgmt)](partner-earned-credit-explanation.md#azure-cost-management-and-pec) pelos parceiros diretamente.

## <a name="how-can-i-reconcile-my-pec-information-across-the-two-recon-files"></a>Como posso conciliar a minha informação do PEC nos dois ficheiros de reconhecimento?

Existem dois ficheiros de reconciliação encontrados no Partner Center em Billing que podem ser usados.

- Atividade recente de reconciliação de utilização avaliada diariamente (.csv)
- Atividade reconciliação recente (.csv)

Para conciliar, o parceiro pode comparar os campos ProductID, SKUID, AvailabilityID destes dois ficheiros para cada SubscriçãoID.

:::image type="content" source="images/advanced-specializations/partner-billing.png" alt-text="Screenshot do separador Partner Center Billing realçando compras recorrentes e únicas." border="false":::

## <a name="for-an-indirect-reseller-working-with-an-indirect-provider-does-an-indirect-provider-need-to-add-the-indirect-resellers-account-as-an-rbac-identity-and-access-management-iam-role-to-the-end-customers-subscription-in-order-to-utilize-acm"></a>Para um Revendedor Indireto que trabalhe com um Fornecedor Indireto, um Fornecedor Indireto precisa de adicionar a conta do Revendedor Indireto como papel rbac identity and Access Management (IAM) à subscrição do cliente final para utilizar a ACM?

Sim, o Fornecedor Indireto CSP deve permitir o acesso do [RBAC](/azure/role-based-access-control/overview) ao Revendedor Indireto na assinatura Azure.

## <a name="what-happens-if-a-customer-removes-a-partners-rbac-admin-access"></a>O que acontece se um cliente remover o acesso de administração RBAC de um parceiro?

Um parceiro sem acesso adequado ao RBAC em CSP ainda mantém a relação de faturação e a prestação de contas do cliente com a Microsoft. Embora isso não afete um parceiro que venda a anterior oferta da Azure na CSP, para a nova oferta da Azure na CSP, o parceiro faturado não será elegível para a PEC na sua fatura Azure. Os parceiros podem obter acesso administrativo parcial em CSP através de uma conta de utilizador através do acesso do Diretório/Hóspede através do RBAC ou através do Farol de Azure. Para obter mais informações, consulte [os privilégios de administração da Reinstate para as assinaturas Azure CSP de um cliente.](reinstate-csp.md)

:::image type="content" source="images/advanced-specializations/permissions.png" alt-text="Screenshot da página de controlo Access onde pode restabelecer permissões de administração." border="false":::

## <a name="how-do-i-know-if-im-earning-pec"></a>Como sei se estou a ganhar PEC?

Existem várias formas de um parceiro confirmar que tem o acesso adequado aos recursos Azure de um cliente.

- Reveja o ficheiro de utilização diária: Se um parceiro estiver a receber o Crédito Adquirido de Parceiro para Serviços Geridos, então eles têm acesso administrativo. Isto pode ser determinado através da revisão do preço unitário e do preço unitário efetivo dentro do ficheiro de utilização diária e confirmando se está a ser aplicado um desconto.
- Crie um Alerta de Monitor Azure: Pode [criar alertas de registo de atividade utilizando](/azure/azure-monitor/platform/alerts-activity-log) o Azure Monitor para receber notificações quando o seu acesso ao RBAC for removido das subscrições do CSP. Consulte o guia de crédito adquirido do Parceiro de Entendimento e documentação técnica.

## <a name="why-dont-i-see-pec-on-the-invoice"></a>Por que não vejo o PEC na fatura?

O PEC não é explicitamente chamado na fatura e não existe um item de linha separada para visualizar o PEC, no entanto, os ganhos do PEC são contabilizados no valor dos encargos líquidos ajustados na fatura. Veja o cálculo e como é que as secções pagas pela PEC são pagas para saber mais sobre onde pode ver detalhes do PEC.

## <a name="next-steps"></a>Passos seguintes

- [Tabela de preços para a nova experiência de comércio para a Azure na CSP](azure-plan-price-list.md)
- [Manage subscriptions and resources under the Azure plan](azure-plan-manage.md) (Gerir subscrições e recursos ao abrigo do plano do Azure)
- [Nova experiência comercial no CSP – faturação do Azure](azure-plan-billing.md)
- [Reinstate admin privileges for Azure CSP subscriptions](reinstate-csp.md) (Restabelecer os privilégios de administrador para as subscrições do Azure CSP)
- [Parceiro ganhou crédito - visão geral](partner-earned-credit.md)
- [Funções, permissões para sócio ganhou crédito](azure-roles-perms-pec.md)
- [Compreensão do parceiro Crédito Adquirido (guia)](https://partner.microsoft.com/resources/detail/understanding-partner-earned-credit-pdf) (inscrição obrigatória)
