---
title: Encontre iD do inquilino, nome de domínio, identificação de objeto de utilizador
ms.topic: how-to
ms.date: 11/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como encontrar IDs no portal Azure - iD de inquilino Azure, nome de domínio ou ID de objeto de utilizador específico. Algumas tarefas precisam desta informação.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: cb0325aae30fe57a4be2be3e37bca1ee6aa1eab8
ms.sourcegitcommit: 7beb7327472dc1b0c07c101d121196fb2830bbf8
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/01/2020
ms.locfileid: "96439242"
---
# <a name="locate-important-ids-for-a-user"></a>Localizar iDs importantes para um utilizador

Este artigo descreve como utilizar o [portal Azure](https://portal.azure.com/) para localizar as seguintes informações para um utilizador:

- O ID do inquilino do Microsoft Azure Ative (Azure AD) da organização ou empresa do utilizador

- O nome de domínio primário da organização ou empresa associada ao inquilino AZURE AD

- O ID do objeto do utilizador

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a>Encontre o ID do inquilino da Microsoft Azure e o nome de domínio primário

Siga estes passos para localizar o ID do inquilino Azure ou o nome de domínio primário dentro do portal Azure. (Se você quiser encontrar um ID de inquilino programáticamente, consulte [Find Inetorso ID com PowerShell ou CLI](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant.md#find-tenant-id-with-powershell).)

> [!NOTE]
> A identificação do inquilino pode ser chamada de nomes diferentes em diferentes aplicações ou recursos. Por exemplo, o ID do inquilino pode ser referido como o ID do diretório, o inquilino do Azure Ative Directory (Azure AD), o Microsoft ID, ou para determinados relatórios, até mesmo o guia do *inquilino.*

1. Inicie sessão no [portal do Azure](https://portal.azure.com/).

2. Selecione **Azure Ative Directory** no menu.

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="Mostra o portal Azure selecionando a opção Azure Ative Directory a partir do menu.":::

3. Aparece uma página **geral** do Diretório Ativo Azure. Para encontrar o ID do inquilino Azure ou o nome de domínio primário, procure o campo **de identificação** do inquilino e o campo **de domínio primário.** Estes campos aparecem na secção de informação do Inquilino.

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="Mostra página geral com dois campos destacados, ID do inquilino e nome de domínio primário.":::

4. Você pode encontrar a identificação do inquilino no portal Azure de algumas outras maneiras. Selecione **Azure Ative Directory** no menu. Em seguida, localize a secção **'Gerir'** no menu e selecione **Propriedades**.

   A página Propriedades também exibe o ID do inquilino associado do utilizador.

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="Mostra a página propriedades com o campo de ID do inquilino em destaque.":::

## <a name="find-the-user-object-id"></a>Encontre o ID do objeto de utilizador

Encontrar o nome de domínio e a identificação do inquilino pode nem sempre ser suficiente. Também pode ter de localizar o ID do objeto específico atribuído a um utilizador. Siga estes passos para encontrar o ID do objeto de um utilizador no portal Azure:

1. Inicie sessão no [portal do Azure](https://portal.azure.com/).

2. Selecione **Azure Ative Directory** no menu.

3. Localizar a secção **'Gerir'** no menu e, em seguida, selecionar **Utilizadores**.

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="Mostra menu Azure Ative Directory com opção de utilizadores em destaque.":::

4. Na página Utilizadores, digite o nome do utilizador na caixa de pesquisa.

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="Mostra a página do Utilizador com caixa de pesquisa para procurar um utilizador específico.":::

5. Selecione o nome do utilizador onde aparece na lista.  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="Mostra a página do utilizador a apresentar uma linha para o utilizador pesquisado.":::

6. Localize a secção identidade na página 'Perfil' do utilizador. O campo de identificação do objeto aparece aqui com o ID do objeto único do utilizador.

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="Mostra a página do Perfil do Utilizador com a secção identidade e um campo destacado para o ID do objeto.":::

## <a name="next-steps"></a>Passos seguintes

- [Encontre o seu ID de inquilino programáticamente com PowerShell ou CLI](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant)
- [Saiba mais sobre os perfis de utilizador no Azure Ative Directory](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [Saiba como os parceiros podem ver ou exportar detalhes do cliente no Partner Center](see-your-customer-list.md)

