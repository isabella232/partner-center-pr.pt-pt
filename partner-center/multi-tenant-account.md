---
title: Adicionar inquilinos à conta do Centro de Parceiros
ms.topic: article
ms.date: 09/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-account
description: Aprenda a adicionar, consolidar ou gerir vários inquilinos AZure AD na sua conta partner Center, e saiba por que quer fazê-lo.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c1e116a6d7aa17cd01a0dfb0342c6f76ad78c448
ms.sourcegitcommit: d731813da1d31519dc2dc583d17899e5cf4ec1b2
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/27/2021
ms.locfileid: "129073667"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a>Adicione e gere vários inquilinos na sua conta Partner Center


**Funções adequadas**: Administração global | Administrador de conta

Este artigo discute como consolidar vários inquilinos Azure Ative Directory (Azure AD) para a sua empresa e, em seguida, adicioná-los e geri-los na sua conta partner Center. Há muitas razões para o fazer. Por exemplo:

- Digamos que a sua empresa, Contoso, adquiriu outra empresa, a Fabrikam. Quer que as duas empresas permaneçam separadas, mas quer que os novos colaboradores possam usar o Partner Center. Neste caso, associa o inquilino Azure AD da nova empresa à sua conta global partner (PGA). Esta associação permite que os utilizadores de ambas as empresas trabalhem no Partner Center.

- Se gere o seu negócio com mais de um inquilino (por exemplo, *contoso.com*, *contoso.uk*, e *contoso.in),* pode utilizar a multitenência para agrupar na mesma conta de PC.

- Se as diretrizes de fusões e aquisições o exigirem que trabalhe com inquilinos de ambas as empresas, usará tanto o *constoso.com* como *fabrikam.com* inquilinos.

- Os utilizadores de qualquer um dos inquilinos devem ser capazes de:
    * Access Partner Center para formação, downloads digitais ou associação Microsoft Certified Professional (MCP).
    * Ser designado funções partner center tais como Microsoft Partner Network (MPN) administração ou administração de incentivos.

## <a name="add-an-azure-ad-tenant-to-your-account"></a>Adicione um inquilino AD AZure à sua conta

1. Inscreva-se no [painel de instrumentos](https://partner.microsoft.com/dashboard) do Partner Center como administrador global.

2. Selecione o ícone de engrenagem Definições e, em seguida, **as definições de Conta** e, em seguida, selecione **Inquilinos**.
 
   :::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="Screenshot do botão Associado no painel de perfil Azure AD.":::

3. Selecione **Associado** e, em seguida, indique o inquilino que deseja associar.

4. No momento, inscreva-se como administrador global para o inquilino que pretende associar e, em seguida, **selecione Confirmar**.

   :::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="Screenshot do botão Confirmar no painel de associação Confirm novo Azure AD.":::

   Depois de ter confirmado a associação, é exibida uma mensagem **all set.** Para ver o recém-adicionado inquilino, **selecione Return to tenant management.**

> [!NOTE]
> Não pode associar um inquilino a uma conta se já estiver associado a outra conta do Partner Center.

## <a name="remove-a-tenant-from-your-account"></a>Remova um inquilino da sua conta

1. Inscreva-se como administrador global para o [Microsoft Partner Center](https://partner.microsoft.com/dashboard).

2. Selecione o ícone de engrenagem Definições e, em seguida, **as definições de Conta** e, em seguida, selecione **Inquilinos**.

3. Selecione o separador **Parceiro**.

4. **Selecione Remote** ao lado do inquilino cuja associação pretende remover.

   :::image type="content" source="images/disassociate.png" alt-text="Screenshot das atuais associações de inquilinos e seus links Remove.":::

   Como mostrado na imagem anterior, os links **Remove** estão habilitados para todos os inquilinos associados, exceto para o inquilino principal e o inquilino que você está atualmente assinado.

   > [!NOTE]
   > Quando você retira um inquilino, os utilizadores desse inquilino já não têm acesso à conta do Centro de Parceiros, e a remoção pode ter um impacto nas suas competências.

## <a name="next-steps"></a>Passos seguintes

- [Criar contas de utilizador](create-user-accounts-and-set-permissions.md)
