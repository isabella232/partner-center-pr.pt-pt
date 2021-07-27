---
title: Parceiro de resolução de problemas ganhou crédito
ms.topic: article
ms.date: 07/22/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como resolver problemas de fatura e outros problemas relacionados com o crédito obtido pelo parceiro (PEC).
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 9d7376b6224047176b5e6608ee190191a8f44824
ms.sourcegitcommit: d133c8b923b90ac5518cb989c0ce4dd69713abf4
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/22/2021
ms.locfileid: "114434223"
---
# <a name="troubleshooting-partner-earned-credit"></a>Parceiro de resolução de problemas ganhou crédito

**Funções adequadas**: Administração global | Administração de administração de utilizadores | Agente administrativo | Administrador de faturação | Agente comercial

## <a name="troubleshooting-guide"></a>Guia de resolução de problemas

Se tiver problemas com o PEC, como acesso ou falta de informação, consulte os itens abaixo na encomenda listada.

1. Certifique-se de que está a olhar para a fatura G (Moderna) e para o ficheiro de reconhecimento. O plano Azure e o PEC não são apresentados na fatura D (Legado) ou no ficheiro de reconhecimento.

2. Identifique o tipo de parceiro. (Os revendedores indiretos não são elegíveis.)

3. Confirme que o seu acordo mpn está ativo.

4. Para fornecedores indiretos, certifique-se de que o revendedor MPN ID introduzido no Partner Center (ou via API) corresponde ao ID mpn do revendedor introduzido no portal Azure.

5. Confirme que a sua oferta é elegível. (As ofertas da Old Azure, Azure Reserved Instances e produtos de terceiros não são elegíveis.)

6. Confirme que tem uma função válida de Gestão em Nome de (AOBO) ou Role-Based access Control (RBAC) para o grupo de subscrição/recursos/recurso.

7. Determine se o cliente removeu a sua função DE RBAC. Em caso afirmativo, consulte os privilégios de administração da Reinstate para as assinaturas Azure CSP de um cliente

8. Confirme que tem acesso administrativo durante todo o dia.

9. Confirme que está a rever as colunas corretas no seu ficheiro de utilização diária.

## <a name="next-steps"></a>Passos seguintes

- [Tabela de preços para a nova experiência de comércio para a Azure na CSP](azure-plan-price-list.md)
- [Manage subscriptions and resources under the Azure plan](azure-plan-manage.md) (Gerir subscrições e recursos ao abrigo do plano do Azure)
- [Nova experiência comercial no CSP – faturação do Azure](azure-plan-billing.md)
- [Reinstate admin privileges for Azure CSP subscriptions](revoke-reinstate-csp.md) (Restabelecer os privilégios de administrador para as subscrições do Azure CSP)
- [Parceiro ganhou crédito - visão geral](partner-earned-credit.md)
- [Funções, permissões para parceiro ganhou crédito](azure-roles-perms-pec.md)
- [Compreensão do parceiro Crédito Adquirido (guia)](https://partner.microsoft.com/resources/detail/understanding-partner-earned-credit-pdf) (inscrição obrigatória)
