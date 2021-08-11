---
title: Adicionar inquilinos à conta do Centro de Parceiros
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-account
description: Saiba como adicionar, consolidar ou gerir vários inquilinos AZure AD na sua conta partner Center, e saiba por que quer fazê-lo.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 7c3231d824afe1f9c449e9809971c97125908815449fda5605e64655d88c1b03
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/06/2021
ms.locfileid: "115685928"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a>Adicione e gere vários inquilinos na sua conta Partner Center


**Funções adequadas**: Administração global | Administrador de conta

Este artigo discute como consolidar vários inquilinos Azure Ative Directory (Azure AD) para a sua empresa e, em seguida, adicioná-los e geri-los na sua conta partner Center. Há muitas razões para o fazer. Por exemplo:

- Digamos que a sua empresa, Contoso, adquiriu outra empresa, a Fabrikam. Quer que as duas empresas permaneçam separadas, mas quer que os novos colaboradores possam usar o Partner Center. Neste caso, associa o inquilino Azure AD da nova empresa à sua conta global partner (PGA). Esta associação permite que os utilizadores de ambas as empresas trabalhem no Partner Center.

- Se gere o seu negócio com mais de um inquilino (por exemplo, *contoso.com*, *contoso.uk*, e *contoso.in),* pode utilizar a multitenência para agrupar na mesma conta de PC.

- Se as diretrizes de fusões e aquisições exigirem que você trabalhe com inquilinos de ambas as empresas, você usaria tanto o *constoso.com* como *fabrikam.com* inquilinos.

- Os utilizadores de qualquer um dos inquilinos devem ser capazes de:
    * Access Partner Center para formação, downloads digitais ou associação Microsoft Certified Professional (MCP).
    * Ser designado funções partner center tais como Microsoft Partner Network (MPN) administração ou administração de incentivos.

## <a name="add-an-azure-ad-tenant-to-your-account"></a>Adicione um inquilino AZure AD à sua conta

1. Inscreva-se como administrador global para o [Microsoft Partner Center](https://partner.microsoft.com/dashboard).

1. No canto superior direito, selecione **Definições,** selecione **as definições de Conta** e, em seguida, selecione **Inquilinos**.
 
   :::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="Screenshot do botão Associado no painel de perfil Ad Azure."::: 

1. Selecione **Associado** e, em seguida, indique o inquilino que deseja associar.

1. No momento, inscreva-se como administrador global para o inquilino que pretende associar e, em seguida, **selecione Confirmar**. 

   :::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="Screenshot do botão Confirmar no painel de associação Confirm novo Azure AD."::: 

   Depois de ter confirmado a associação, é exibida uma mensagem **all set.** Para ver o recém-adicionado inquilino, **selecione Devolver à gestão de inquilinos.** 
 
>[!NOTE]
>Não pode associar um inquilino a uma conta se já estiver associado a outra conta do Partner Center.


## <a name="remove-a-tenant-from-your-account"></a>Retire um inquilino da sua conta
 
1. Inscreva-se como administrador global para o [Microsoft Partner Center](https://partner.microsoft.com/dashboard).

1. No canto superior direito, selecione o ícone **Definições** e, em seguida, selecione **as definições de Conta**.

1. No painel esquerdo, selecione **Inquilinos.** No **âmbito do Manage Azure AD,** selecione o **separador Partner.**
 
1. **Selecione Remova** ao lado do inquilino cuja associação pretende remover.

   :::image type="content" source="images/disassociate.png" alt-text="Screenshot das atuais associações de inquilinos e seus links Remove.":::

   Como mostrado na imagem anterior, os links **Remove** estão habilitados para todos os inquilinos associados, exceto para o inquilino principal e o inquilino que você está atualmente assinado. 

   > [!NOTE]   
   > Quando você retira um inquilino, os utilizadores desse inquilino já não têm acesso à conta do Centro de Parceiros, e a remoção pode ter um impacto nas suas competências. 

## <a name="next-steps"></a>Passos seguintes

- [Criar contas de utilizador](create-user-accounts-and-set-permissions.md)






