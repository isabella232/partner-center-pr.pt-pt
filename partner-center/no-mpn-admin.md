---
title: O que fazer se o único administrador do seu programa MPN tiver deixado a empresa?
ms.topic: how-to
ms.date: 09/08/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba o que fazer para encontrar um novo administrador mpn ou obter ajuda da administração Global da sua empresa. Além disso, aprenda a adicionar um novo administrador partner center global.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 21042169a33d9a413f17f951c4daad0c5fc86a17
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/17/2021
ms.locfileid: "112277679"
---
# <a name="what-to-do-if-the-only-admin-for-your-mpn-program-has-left-the-company"></a>O que fazer se o único administrador do seu programa MPN tiver deixado a empresa?

**Funções adequadas**: administrador de parceiros da MPN | Administração de contas | Administração global

O seguinte artigo acompanha-o através de três cenários típicos sobre o que fazer se o seu administrador MPN tiver deixado a empresa.

## <a name="scenario-1-mpn-partner-adminaccount-admin-has-left-the-company-but-there-are-still-global-admins-in-the-account"></a>Cenário 1: MPN Partner Admin/Account Admin deixou a empresa mas ainda existem Administradores Globais na conta

Neste caso, outra pessoa na empresa pode ser atribuída ao cargo de administradora mpn Partner. A atribuir o papel de administrador específico do MPN Partner/Administração de Contas:

1. Inscreva-se na sua conta Partner Center com a sua conta de trabalho (por exemplo, tom@contoso.com ).
1. Do filtro da página **de Gestão** de Utilizadores no administrador global para ver quem são os Administradores Globais para a sua empresa. 
1. Contacte um dos administradores globais e peça-lhes que lhe atribuam o papel específico da MPN de que necessita. 

## <a name="scenario-2-mpn-partner-adminaccount-admin-has-left-the-company-and-there-are-no-global-admins-in-the-account"></a>Cenário 2: MPN Partner Admin/Account Admin deixou a empresa, e não há administradores globais na conta 

Se for à página **de Gestão** de Utilizadores e filtrar a administração Global, mas descobrir que não existe nenhum Administrador Global na sua empresa que possa ajudá-lo a ganhar o papel específico da MPN, siga estes passos:

1. Vá a [portal.azure.com,](https://ms.portal.azure.com/)faça sômis com a sua conta de trabalho (por exemplo, tom@contoso.com ). 
1. Selecione a opção **Ajuda + Suporte** na barra de navegação do menu esquerdo.
1. Na página seguinte, selecione **Novo Pedido de Suporte** e Tipo de **Emissão Técnica** no menu suspenso, insira quaisquer detalhes adicionais e clique em **Seguinte: Soluções.**

:::image type="content" source="images/accountsettings/adminfinder.png" alt-text="Localize a administração no portal Azure.":::

4. Depois de rever as Soluções recomendadas na página seguinte, selecione **Seguinte: Detalhes** e complete os campos necessários.
1. Reveja e crie o pedido de apoio.


## <a name="scenario-3-mpn-partner-adminaccount-adminglobal-admin-has-left-the-company-and-there-are-no-other-users-who-can-access-the-companys-azure-ad-this-is-a-complete-loss-of-access"></a>Cenário 3: Mpn Partner admin/Account admin/Global admin deixou a empresa e não há outros utilizadores que possam aceder ao Azure AD da empresa. Isto é uma completa perda de acesso.

Siga as medidas [de tomada de posse do administrador](/azure/active-directory/users-groups-roles/domains-admin-takeover#internal-admin-takeover) para assumir um diretório não gerido como administrador do Azure Ative Directory.

## <a name="not-sure-if-your-company-already-has-a-work-account"></a>Não tem certeza se a sua empresa já tem uma conta de trabalho?

Se não tem certeza se a sua empresa tem uma conta de trabalho, siga estes passos para verificar.

1. Inscreva-se no [portal de administração Azure](https://ms.portal.azure.com).
2. Selecione **O Diretório Ativo Azure** a partir do menu esquerdo e, em seguida, selecione **nomes de Domínio**.
Se já tiver uma conta de trabalho, o seu nome de domínio será listado.

>[!Note]
>Se tem uma subscrição ativa do Microsoft Azure ou do Office 365, já tem uma conta de trabalho e o seu sinal em credenciais deve ser o mesmo que os utilizados para aceder a esses serviços.