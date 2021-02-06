---
title: Parceiro ganhou crédito por serviços geridos
ms.topic: article
ms.date: 12/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como o parceiro da Microsoft ganhou crédito (PEC) por serviços geridos é calculado e pago e como garantir que é elegível.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 010f74164b0428a5cd6ffcde5000b52ac6a6993f
ms.sourcegitcommit: d37a3f353426e52dfbbac577b7576f9c3f6d2ddf
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/06/2021
ms.locfileid: "99624005"
---
# <a name="how-the-partner-earned-credit-is-calculated-and-paid"></a>Como o crédito de parceiro ganho é calculado e pago

**Funções adequadas**

- Administrador global
- Administrador de utilizadores
- Agente administrativo
- Administrador de faturação
- Agente comercial

O parceiro ganhou crédito pelos serviços geridos (PEC) reconhece e recompensa parceiros que detêm o controlo operacional de TI 24x7 e a gestão de partes de, ou todo, ambiente Azure dos seus clientes. Por padrão, na CSP, aos parceiros são concedidos os direitos de acesso necessários à subscrição do cliente, permitindo-lhes realizar 24 X 7 gestão operacional e controlo dos recursos na subscrição. As formas adicionais de acesso ao cliente para o parceiro de transação são descritas na secção seguinte. O valor da fatura mensal é líquido do crédito ganho pelo parceiro. Os parceiros podem ver os detalhes do PEC no seu ficheiro mensal de reconhecimento. Para formas adicionais de acesso a um cliente, leia [Gerir subscrições e recursos ao abrigo do plano Azure.](azure-plan-manage.md)

Leia Também [os privilégios de administração da Reinstate para as assinaturas Azure CSP](revoke-reinstate-csp.md)

## <a name="eligibility"></a>Elegibilidade

Para receber o parceiro auferido crédito (PEC), aplicam-se os seguintes requisitos: 

- Você deve ter um acordo mPN ativo e papel válido de controlo de acesso baseado em funções (RBAC) para receber crédito ganho pelos ativos Azure que você gere.

- Deve ter controlo operacional 24x7 e gestão dos recursos Azure do cliente em CSP. Isto significa que deve ter privilégios administrativos na subscrição Azure do cliente, grupo de recursos Azure, recurso Azure. No caso dos fornecedores indiretos e dos seus revendedores indiretos, o fornecedor indireto será elegível para o PEC se o fornecedor indireto ou o revendedor indireto tiverem esse controlo operacional. Para saber mais sobre isto, consulte [os privilégios de administração da Reinstate para as assinaturas Azure CSP](./revoke-reinstate-csp.md).

- Além dos requisitos acima referidos, o PEC só é aplicável aos serviços listados no preço de consumo do plano Azure, que pode exportar a partir da página de preços do [plano Azure.](https://partner.microsoft.com/commerce/sales)

- A PEC **não** se aplica aos seguintes serviços:
    - Reservas do Plano Azure
    - Produtos de terceiros identificados como terceiros na coluna Tags do preço de consumo do plano Azure
    - Produtos na tabela de preços do Mercado
    - [Máquinas virtuais Azure Spot](https://partner.microsoft.com/resources/collection/azure-spot-in-csp#/)

- O PEC é ganho até ao nível de recursos Azure. Se tiver acesso válido a nível de subscrição ou grupo de recursos, cada recurso que se ause até à entidade superior ganhará PEC.

- Os detalhes sobre o PEC também estão disponíveis na página [de gestão do Custo Azure.](/azure/cost-management-billing/costs/get-started-partners)

### <a name="calculation"></a>Cálculo

O PEC é calculado diariamente e pode ser visto no ficheiro de utilização diária e no ficheiro mensal de reconhecimento de fatura. Um parceiro (fornecedor indireto ou revendedor indireto) deve ter acesso durante todo o dia (24x7) para garantir que obtém PEC. O PEC é calculado diariamente com base nos ativos geridos da Azure. Os parceiros que mantêm o acesso privilegiado persistente ao longo do mês (período de acesso) e para todos os recursos elegíveis (âmbito de acesso) ganharão o PEC completo. A redução do âmbito e do alcance resultará numa taxa de PEC mais baixa para o mês. O ficheiro de utilização avaliado diariamente mostra diariamente um ativo Azure, quer o PEC seja aplicado ou não. Os parceiros também podem inscrever-se em alertas para monitorizar as alterações ao acesso privilegiado persistente.

## <a name="azure-cost-management"></a>Azure Cost Management

A Azure Cost Management (ACM) utilizando a Análise de Custos permite-lhe, como parceiro, visualizar os custos que receberam o benefício da PEC.  

1. No [portal Azure,](https://portal.azure.com)inscreva-se no seu inquilino parceiro e selecione **Cost Management + Billing**.

2. Selecione **gestão de custos**

3. Selecione **análise de custos**

   A visão de Análise de Custos apresentará os custos da sua conta de faturação, para todos os serviços comprados e consumidos aos preços que paga à Microsoft.

4. Selecione **PartnerEarnedCreditApplied** na queda em um gráfico de pivô para ver os custos que têm PEC aplicado. Quando a propriedade **PartnerEarnedCreditApplied** é Verdadeira, o custo associado tem o benefício do parceiro que ganhou crédito. 

   Quando a propriedade PartnerEarnedCreditApplied é falsa, o custo associado não cumpriu a elegibilidade exigida para o crédito ou o serviço adquirido não é elegível para o parceiro obtido crédito.

   >[!NOTE] 
   >Normalmente, o uso dos serviços demora 8-24 horas a aparecer na **Gestão de Custos** e os créditos PEC aparecerão dentro de 48 horas a partir do momento de acesso na Azure Cost Management.

5. Também pode agrupar e filtrar a propriedade **PartnerEarnedCreditApplied** utilizando as funcionalidades de filtro **do Grupo por e Adicionar** para perfurar custos que têm PEC e os custos que não têm PEC aplicados.

## <a name="next-steps"></a>Passos seguintes

- [Parceiro ganhou crédito - visão geral](partner-earned-credit.md)

- Exemplos detalhados de cálculos de crédito obtidos pelo parceiro estão localizados na tabela de preços que pode chegar através do painel de instrumentos do Partner Center (inscrição obrigatória).

- [Move to Azure plan - começa](azure-plan-get-started.md)

- [Manage subscriptions and resources under the Azure plan](azure-plan-manage.md) (Gerir subscrições e recursos ao abrigo do plano do Azure)

- [Revogar ou reinserir privilégios de administração para subscrições da Azure CSP](revoke-reinstate-csp.md)
