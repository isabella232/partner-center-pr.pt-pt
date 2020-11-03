---
title: Adicione inquilinos adicionais à sua conta partner Center
ms.topic: article
ms.date: 07/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como adicionar, consolidar ou gerir vários inquilinos AZure AD na sua conta partner Center. Saiba também sobre algumas das razões pelas quais poderá querer fazê-lo.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: b9379ce6b27a8ef6e5d6894a0630745794e04e04
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/19/2020
ms.locfileid: "92530512"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a>Adicione e gere vários inquilinos na sua conta Partner Center

**Aplica-se a**

- Partner Center

**Funções adequadas**

- Administrador global

Esta funcionalidade permite-lhe gerir vários inquilinos para a sua empresa e consolidá-los na sua conta do Centro de Parceiros. Existem muitas razões pelas quais você pode precisar de gerir vários inquilinos AZure AD na sua conta partner Center. Por exemplo:

- A sua empresa pode comprar outra empresa, e quer que os colaboradores da nova empresa possam utilizar o Partner Center. No entanto, quer que as duas empresas permaneçam separadas. Neste caso, associaria o inquilino da AZure AD da nova empresa à sua conta global partner (PGA). Esta associação permitiria que os utilizadores de ambas as empresas trabalhassem no Partner Center.

- Se tiver mais de um inquilino para gerir o seu negócio (por exemplo, contoso.com, contoso.uk, contoso.in) pode usar vários arrendamentos para os amarrar na mesma conta de PC.

- Fusões e aquisições obrigam a trabalhar com mais do que um inquilino (por exemplo, se a Contoso adquirir a Fabrikam, terá de ser capaz de utilizar tanto Constoso.com como Fabrikam.com respetivos inquilinos).

- Os utilizadores de qualquer um dos inquilinos teriam de ser capazes de:
    1.  Centro de Parceiros de Acesso para formação, downloads digitais, associação MCP
    2.  Ser designado Partner Center funções como MPN Admin, Incentives Admin etc.


## <a name="add-another-azure-ad-tenant-to-your-account"></a>Adicione outro inquilino AZure AD à sua conta

1. Como administrador global, inscreva-se no painel partner [center](https://partner.microsoft.com/dashboard).
1. A partir do ícone **Definições,** selecione **as definições de Conta** e, em seguida, selecione **Inquilinos** .
 
:::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="inquilinos associados"::: 

3. Selecione **Associar outro inquilino de AD** e indicar o inquilino que você deseja associar.

1. Como administrador global, inscreva-se no inquilino que quer associar e confirmar a associação. 

:::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="inquilinos associados"::: 

5. Depois de confirmar, verá um aviso **de todos os conjuntos.**  **Selecione Return to tenant management** e você verá o recém-adicionado inquilino listado. 
 

>[!NOTE]
>Não pode associar um inquilino a uma conta se já estiver associado a outra conta do Partner Center.

 
## <a name="next-steps"></a>Passos seguintes

- [Adicionar utilizadores](create-user-accounts-and-set-permissions.md)
