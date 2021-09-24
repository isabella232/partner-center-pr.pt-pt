---
title: Parceiro ganhou crédito por serviços geridos
ms.topic: article
ms.date: 08/12/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Saiba como o parceiro da Microsoft ganhou crédito (PEC) por serviços geridos é calculado e pago e como garantir que é elegível.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 56884a5a6cbfbade881154275129c63dcd3456d8
ms.sourcegitcommit: fb9ca808f6362e81d65a6ba5770dc8820834a0ed
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/24/2021
ms.locfileid: "128422439"
---
# <a name="how-the-partner-earned-credit-is-calculated-and-paid"></a>Como o crédito de parceiro ganho é calculado e pago

**Funções adequadas**: Administração global | Administração de administração de utilizadores | Agente administrativo | Administrador de faturação | Agente comercial

O parceiro ganhou crédito (PEC) por serviços geridos reconhece e recompensa parceiros que detêm controlo operacional de TI e gestão de algum ou todo o ambiente Azure de um cliente. 

Por padrão, como parceiro da CSP, é-lhe concedido o direito de acesso necessário à subscrição do seu cliente, permitindo-lhe realizar gestão operacional e controlo dos recursos na subscrição. Na secção seguinte, são descritas outras formas pelas quais os clientes podem ter acesso a parceiros de transação.

O valor da fatura mensal é o líquido do sócio que ganhou crédito. Pode ver detalhes do PEC no seu ficheiro mensal de reconhecimento. Para obter formas adicionais de acesso ao parceiro de transação, consulte os seguintes artigos:

- [Manage subscriptions and resources under the Azure plan](azure-plan-manage.md) (Gerir subscrições e recursos ao abrigo do plano do Azure)
- [Reinstate admin privileges for Azure CSP subscriptions](revoke-reinstate-csp.md) (Restabelecer os privilégios de administrador para as subscrições do Azure CSP)

## <a name="eligibility"></a>Elegibilidade

Para receber o Crédito Adquirido do Parceiro (PEC), aplicam-se os seguintes requisitos:

- Você deve ter um acordo mpn ativo e papel válido [de controlo](azure-roles-perms-pec.md) de acesso baseado em [funções (RBAC).](/azure/role-based-access-control/overview)
- Você deve ter Admin em nome de privilégios [(AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) na subscrição Azure do cliente, grupo de recursos Azure, ou recurso Azure, ou um [papel DE RBAC](azure-roles-perms-pec.md)válido .
- No caso dos fornecedores indiretos e dos seus revendedores indiretos, um fornecedor indireto é elegível para a PEC se o fornecedor indireto ou o revendedor indireto tiverem privilégios AOBO ou uma função de RBAC elegível. Para obter mais informações, consulte [os privilégios de administração da Reinstate para as assinaturas Azure CSP](revoke-reinstate-csp.md).
- O mpn iD sócio deve pertencer ao mesmo v-org que o comprador MPN ID ou o Sócio da Record (POR) MPN ID. Para obter mais informações, veja [Ligar o seu ID de parceiro para controlar o impacto nos recursos delegados](/azure/lighthouse/how-to/partner-earned-credit).
- O PEC é obtido a nível de recursos Azure, grupo de recursos ou subscrição. Se um parceiro tiver acesso válido a nível de subscrição ou grupo de recursos, cada recurso que se ausse para a entidade superior ganhará PEC.
- A PEC não é aplicável aos seguintes serviços:
    - Reservas do plano Azure
    - Produtos de terceiros identificados como terceiros na coluna Tags do preço de consumo do plano Azure
    - Produtos na tabela de preços do Mercado
    - [Máquinas virtuais Azure Spot](https://partner.microsoft.com/resources/collection/azure-spot-in-csp#/)

Além dos requisitos acima referidos, o PEC só é aplicável aos serviços enumerados no plano Azure de preços de consumo. Pode ver e exportar isso a partir da página de preços do [plano Azure.](https://partner.microsoft.com/commerce/sales)

Para obter mais informações sobre o PEC, consulte a página [de gestão de Custos Azure.](/azure/cost-management-billing/costs/get-started-partners)

Para obter mais informações sobre a elegibilidade, consulte [as funções e permissões necessárias para ganhar crédito a sócio.](azure-roles-perms-pec.md)

## <a name="calculation"></a>Cálculo

O PEC é calculado diariamente. É pago por cada dia que tiver acesso elegível em cada subscrição. Embora os detalhes do PEC não apareçam na sua fatura mensal, os ganhos da PEC são contabilizados na linha de encargos líquidos ajustados dentro da fatura. Pode encontrar mais detalhes do PEC no [ficheiro de utilização diária](daily-rated-usage-recon-files.md) e no ficheiro mensal de reconhecimento de fatura.

:::image type="content" source="images/advanced-specializations/recon-file.png" alt-text="Screenshot de um ficheiro de reconciliação do Partner Center identificando colunas." border="false":::

A tabela abaixo descreve os elementos PEC encontrados no ficheiro mensal de reconhecimento de fatura. Todos os valores estão em USD, como mostrado na coluna AI, PricingCurrency.

| Coluna  | Descrição  |
| --------  | -------  |
| Coluna C  | CustomerName  |
| Coluna P | UnitPrice |
| Anúncio de coluna | EffectiveUnitPrice. Este é o preço após a aplicação do PEC e os requisitos foram cumpridos. Quando o PEC é aplicado, verá que o EffectiveUnitPrice na coluna AD é uma percentagem inferior à UnitPrice na coluna P.   |
| Coluna V  | PreçoDjustmentDescription. Isto ficará em branco se não forem cumpridos quaisquer requisitos para o PEC ou se tiver o PEC % que será aplicado à UnitPrice. No entanto, poderá ser elegível para créditos adicionais. Em caso afirmativo, estarão listados nesta coluna. Exemplo: Desconto de nível 1 1 1.   |

Para monitorizar o acesso ao PEC:

- **O ficheiro de utilização nominal diária** mostra onde o PEC é aplicado (ou não) diariamente

- [**O monitor Azure alerta**](azure-plan-manage.md) monitorizar alterações ao acesso privilegiado persistente.

O ficheiro de utilização nominal diária:

:::image type="content" source="images/advanced-specializations/partner-daily.png" alt-text="Screenshot de um ficheiro de utilização avaliado diariamente no Partner Center, realçando o preço unitário eficaz." border="false":::

## <a name="partner-earned-credit-api"></a>Parceiro ganhou crédito API

Uma API PEC está disponível como parte do instrumento de ferramentas Azure API. Para obter informações sobre powerShell e CLI APIs, consulte [link a conta Azure a um ID do parceiro](/azure/cost-management-billing/manage/link-partner-id).

## <a name="azure-cost-management-and-pec"></a>Azure Cost Management e PEC

A Azure Cost Management (ACM) utilizando a Análise de Custos permite-lhe, como parceiro, visualizar os custos que receberam o benefício da PEC. Para uma apresentação detalhada sobre a ACM, consulte a [chamada de Destaque para maio de 2021.](https://commercial_licensing.eventbuilder.com/2021MayCSPSpotlight)

## <a name="use-acm-to-view-your-partner-earned-credit"></a>Use a ACM para ver o seu parceiro ganhou crédito

1. No [portal Azure,](https://portal.azure.com/)inscreva-se no seu inquilino parceiro e selecione **Gestão de Custos + Faturação.**
2. Selecione **gestão de custos**.
3. Selecione **Análise de Custos**.
A vista De Análise de Custos apresentará os custos da sua conta de faturação, para todos os serviços comprados e consumidos aos preços que paga à Microsoft.

:::image type="content" source="images/advanced-specializations/partner-cost.png" alt-text="Screenshot de uma página de análise de custos de gestão de custos." border="false":::

4. Na lista de drop-down do gráfico de pílferos, selecione PartnerEarnedCreditApplied. 

    Se este valor for **Verdadeiro,** o custo associado tem o benefício do parceiro a ganhar crédito.

    Se este valor for **Falso,** o custo associado não cumpriu a elegibilidade exigida para o crédito, ou o serviço adquirido não é elegível para o parceiro auferido.

>[!NOTE]
>Normalmente, o uso para serviços demora 8-24 horas a aparecer na Gestão de Custos, e os créditos PEC aparecerão dentro de 48 horas a partir do momento de acesso na Azure Cost Management.

Também pode agrupar e filtrar a propriedade **PartnerEarnedCreditApplied** utilizando as funcionalidades do filtro **Group by** e **Add.** Estes permitem perfurar custos que têm PEC e os custos que não têm PEC aplicados.

## <a name="how-is-pec-paid"></a>Como é pago o PEC?
Os ganhos do PEC são contabilizados na linha de encargos líquidos ajustada dentro da fatura. O **total** da fatura abaixo mostrada ilustra-o. Para obter detalhes de ajuste, consulte o ficheiro de reconciliação mensal da fatura e o ficheiro de utilização diária do Azure.

:::image type="content" source="images/advanced-specializations/invoice.png" alt-text="Screenshot de uma fatura do Partner Center indicando que os detalhes de ajuste aparecem nos ficheiros de utilização diário do reconhecimento e do Azure." border="false":::

## <a name="next-steps"></a>Passos seguintes

- [Tabela de preços para a nova experiência de comércio para a Azure na CSP](azure-plan-price-list.md)
- [Manage subscriptions and resources under the Azure plan](azure-plan-manage.md) (Gerir subscrições e recursos ao abrigo do plano do Azure)
- [Nova experiência comercial no CSP – faturação do Azure](azure-plan-billing.md)
- [Reinstate admin privileges for Azure CSP subscriptions](revoke-reinstate-csp.md) (Restabelecer os privilégios de administrador para as subscrições do Azure CSP)
- [Parceiro ganhou crédito - visão geral](partner-earned-credit.md)
- [Funções, permissões para sócio ganhou crédito](azure-roles-perms-pec.md)
- [Compreensão do parceiro Crédito Adquirido (guia)](https://partner.microsoft.com/resources/detail/understanding-partner-earned-credit-pdf) (inscrição obrigatória)