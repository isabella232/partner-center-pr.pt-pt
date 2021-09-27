---
title: Capacidades de faturação direta restringidas
ms.topic: article
ms.date: 09/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
description: Saiba mais sobre os requisitos do parceiro de conta direta Fornecedor de Soluções em Nuvem (CSP) e o que fazer para evitar que as capacidades sejam restringidas. Descubra se as suas capacidades foram restritas.
author: billLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: ebd364c1268217579316338e884d96491ddd70fb
ms.sourcegitcommit: d731813da1d31519dc2dc583d17899e5cf4ec1b2
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/27/2021
ms.locfileid: "129070738"
---
# <a name="restricted-direct-bill-capabilities-and-the-requirements-needed-for-csp-direct-bill-partners"></a>Capacidades de conta direta restritas e os requisitos necessários para os parceiros de conta direta da CSP

**Funções apropriadas**: Administração global

## <a name="overview"></a>Descrição Geral

Os parceiros de conta direta devem cumprir os novos [requisitos](direct-partner-new-requirements.md) para permanecer no programa de parceiros de conta direta Fornecedor de Soluções em Nuvem (CSP). Caso contrário, o seu acesso às capacidades de faturação direta acabará por ser restringido e poderá continuar a executar tarefas específicas, como fazer novas compras para os seus clientes.

> [!Note]
> Os parceiros de conta direto que não satisfaçam os novos requisitos para o programa de parceiros de conta direta CSP serão informados pela Microsoft quando as suas capacidades de conta diretas serão restringidas. Isto aplica-se a todos os parceiros de conta direta, quer tenham optado pela [transição de parceiro de conta direta para revendedores indiretos](transition-direct-to-indirect.md) ou não.  

## <a name="how-to-tell-if-your-direct-bill-capabilities-has-been-restricted"></a>Como dizer se as suas capacidades de conta direta foram restritas

Para confirmar se o acesso do inquilino do parceiro de conta direta às capacidades de conta direta foi restringido, siga estes passos.

1. Inicie sessão no [dashboard do Centro de Parceiros](https://partner.microsoft.com/dashboard).

2. Selecione o ícone de engrenagem Definições e, em seguida, **as definições de Conta** e, em seguida, selecione Perfil **Legal**.

3. Informações **do Programa,** procure **Fornecedor de Soluções em Nuvem da Microsoft estado**.

4. Se o estado do programa tiver um valor **restrito,** significa que o acesso do seu parceiro de conta direta às capacidades de conta direta foi restringido.

## <a name="affected-direct-bill-capabilities"></a>Capacidades de conta direta afetadas

Se as suas capacidades de conta direta tiverem sido restritas, já não pode fazer novas compras para os seus clientes no Partner Center. Esta restrição inclui:

- Subscrições do Azure

- Assinaturas baseadas em licenças

- Adicione novos addons às subscrições existentes baseadas em licenças.

- Faça compras únicas de software e produtos de reserva (por exemplo, subscrições de software, software perpétuo e instâncias da Azure Reserved Virtual Machine).

Também não pode utilizar a [oferta de serviços partilhados do parceiro Azure](shared-services.md) ao abrigo do programa CSP para comprar novas subscrições Azure para seu próprio uso.

As assinaturas de faturas diretas existentes não são afetadas. Permanecem válidos e são auto-autorenados. Continuará a ser cobrado diretamente pela Microsoft até que sejam cancelados. Ainda pode gerir as subscrições existentes das seguintes formas:

- Suspender as assinaturas existentes

- Ajustar a contagem de licenças das assinaturas existentes baseadas em licenças

- Ajuste a contagem de licenças de complementos existentes para uma subscrição. 

    >[!Note]
    >Não é possível adicionar novos addons às subscrições existentes, uma vez que é tratada como nova compra.

- Implemente novos recursos Azure e gere os recursos Azure existentes sob as subscrições Azure existentes. Isto inclui recursos, que estão disponíveis através do Azure Marketplace e Visual Studio subscrições.

Além de novas compras, não é possível aceder às seguintes capacidades de conta direta no Partner Center:

- Não pode criar novos inquilinos de clientes. A opção **de cliente Create** na página **cliente** no Partner Center não estará disponível.

- Não é possível gerar convite para o cliente solicitar a relação de revendedor direto. O Pedido uma opção **de relacionamento revendedor** na página **clientes** no Partner Center não estará disponível.

    >[!NOTE]
    >Como parte da transição de parceiro de conta direta para revendedor indireto, se já inscreveu o seu inquilino parceiro de conta direta como revendedor indireto, pode gerar convite para o cliente solicitar uma relação de revendedor indireto.

- Não pode criar um novo inquilino de caixa de areia. Cada inquilino parceiro de conta direta pode criar um inquilino de caixa de areia para integração direta da API de conta direta. Se ainda não criou um, não está autorizado a fazê-lo depois de a capacidade do seu parceiro de conta direta ter sido restringida.  

## <a name="next-steps"></a>Passos seguintes

- [Informações adicionais sobre se tornar um revendedor indireto](https://assetsprod.microsoft.com/csp-directbill-to-indirect-transition.pdf)

- [CSP parceiro direto novos requisitos](direct-partner-new-requirements.md)
