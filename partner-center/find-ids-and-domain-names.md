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
ms.openlocfilehash: 643b1eeb96a47ee4c438f733efe3be22234d02ff
ms.sourcegitcommit: e462f562e7f26b7d6870c22638a2a841499109d6
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/11/2021
ms.locfileid: "109740289"
---
# <a name="locate-important-ids-for-a-user"></a><span data-ttu-id="4ead3-104">Localizar iDs importantes para um utilizador</span><span class="sxs-lookup"><span data-stu-id="4ead3-104">Locate important IDs for a user</span></span>

<span data-ttu-id="4ead3-105">**Funções adequadas**</span><span class="sxs-lookup"><span data-stu-id="4ead3-105">**Appropriate roles**</span></span>

- <span data-ttu-id="4ead3-106">Administrador global</span><span class="sxs-lookup"><span data-stu-id="4ead3-106">Global admin</span></span>

<span data-ttu-id="4ead3-107">Este artigo descreve como utilizar o [portal Azure](https://portal.azure.com/) para localizar as seguintes informações para um utilizador:</span><span class="sxs-lookup"><span data-stu-id="4ead3-107">This article describes how to use the [Azure portal](https://portal.azure.com/) to locate the following information for a user:</span></span>

- <span data-ttu-id="4ead3-108">O ID do inquilino do Microsoft Azure Ative (Azure AD) da organização ou empresa do utilizador</span><span class="sxs-lookup"><span data-stu-id="4ead3-108">The Microsoft Azure Active Directory (Azure AD) tenant ID of the user's organization or company</span></span>

- <span data-ttu-id="4ead3-109">O nome de domínio primário da organização ou empresa associada ao inquilino AZURE AD</span><span class="sxs-lookup"><span data-stu-id="4ead3-109">The primary domain name of the organization or company associated with the Azure AD tenant</span></span>

- <span data-ttu-id="4ead3-110">O ID do objeto do utilizador</span><span class="sxs-lookup"><span data-stu-id="4ead3-110">The user object ID</span></span>

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a><span data-ttu-id="4ead3-111">Encontre o ID do inquilino da Microsoft Azure e o nome de domínio primário</span><span class="sxs-lookup"><span data-stu-id="4ead3-111">Find the Microsoft Azure AD tenant ID and primary domain name</span></span>

<span data-ttu-id="4ead3-112">Siga estes passos para localizar o ID do inquilino Azure ou o nome de domínio primário dentro do portal Azure.</span><span class="sxs-lookup"><span data-stu-id="4ead3-112">Follow these steps to locate the Azure AD tenant ID or primary domain name within the Azure portal.</span></span> <span data-ttu-id="4ead3-113">(Se você quiser encontrar um ID de inquilino programáticamente, consulte [Find Inetorso ID com PowerShell ou CLI](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant#find-tenant-id-with-powershell).)</span><span class="sxs-lookup"><span data-stu-id="4ead3-113">(If you'd like to find a tenant ID programmatically, see [Find tenant ID with PowerShell or CLI](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant#find-tenant-id-with-powershell).)</span></span>

> [!NOTE]
> <span data-ttu-id="4ead3-114">A identificação do inquilino pode ser chamada de nomes diferentes em diferentes aplicações ou recursos.</span><span class="sxs-lookup"><span data-stu-id="4ead3-114">The tenant ID may be called different names in different applications or resources.</span></span> <span data-ttu-id="4ead3-115">Por exemplo, o ID do inquilino pode ser referido como o ID do diretório, o inquilino do Azure Ative Directory (Azure AD), o Microsoft ID, ou para determinados relatórios, até mesmo o guia do *inquilino.*</span><span class="sxs-lookup"><span data-stu-id="4ead3-115">For example, the tenant ID may be referred to as the directory ID, the Azure Active Directory (Azure AD) tenant, Microsoft ID, or for certain reports, even the *tenantguid*.</span></span>

1. <span data-ttu-id="4ead3-116">Inicie sessão no [portal do Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="4ead3-116">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="4ead3-117">Selecione **Azure Ative Directory** no menu.</span><span class="sxs-lookup"><span data-stu-id="4ead3-117">Select **Azure Active Directory** from the menu.</span></span>

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="Mostra o portal Azure selecionando a opção Azure Ative Directory a partir do menu.":::

3. <span data-ttu-id="4ead3-119">Aparece uma página **geral** do Diretório Ativo Azure.</span><span class="sxs-lookup"><span data-stu-id="4ead3-119">An Azure Active Directory **Overview** page appears.</span></span> <span data-ttu-id="4ead3-120">Para encontrar o ID do inquilino Azure ou o nome de domínio primário, procure o campo **de identificação** do inquilino e o campo **de domínio primário.**</span><span class="sxs-lookup"><span data-stu-id="4ead3-120">To find the Azure AD tenant ID or primary domain name, look for the **Tenant ID** field and the **Primary domain** field.</span></span> <span data-ttu-id="4ead3-121">Estes campos aparecem na secção de informação do Inquilino.</span><span class="sxs-lookup"><span data-stu-id="4ead3-121">These fields appear in the Tenant information section.</span></span>

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="Mostra página geral com dois campos destacados, ID do inquilino e nome de domínio primário.":::

4. <span data-ttu-id="4ead3-123">Você pode encontrar a identificação do inquilino no portal Azure de algumas outras maneiras.</span><span class="sxs-lookup"><span data-stu-id="4ead3-123">You can find the tenant ID in the Azure portal in a few other ways.</span></span> <span data-ttu-id="4ead3-124">Selecione **Azure Ative Directory** no menu.</span><span class="sxs-lookup"><span data-stu-id="4ead3-124">Select **Azure Active Directory** from the menu.</span></span> <span data-ttu-id="4ead3-125">Em seguida, localize a secção **'Gerir'** no menu e selecione **Propriedades**.</span><span class="sxs-lookup"><span data-stu-id="4ead3-125">Then, locate the **Manage** section on the menu and select **Properties**.</span></span>

   <span data-ttu-id="4ead3-126">A página Propriedades também exibe o ID do inquilino associado do utilizador.</span><span class="sxs-lookup"><span data-stu-id="4ead3-126">The Properties page also displays the user's associated Tenant ID.</span></span>

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="Mostra a página propriedades com o campo de ID do inquilino em destaque.":::

## <a name="find-the-user-object-id"></a><span data-ttu-id="4ead3-128">Encontre o ID do objeto de utilizador</span><span class="sxs-lookup"><span data-stu-id="4ead3-128">Find the user object ID</span></span>

<span data-ttu-id="4ead3-129">Encontrar o nome de domínio e a identificação do inquilino pode nem sempre ser suficiente.</span><span class="sxs-lookup"><span data-stu-id="4ead3-129">Just finding the domain name and tenant ID may not always be enough.</span></span> <span data-ttu-id="4ead3-130">Também pode ter de localizar o ID do objeto específico atribuído a um utilizador.</span><span class="sxs-lookup"><span data-stu-id="4ead3-130">You may also need to locate the specific object ID assigned to a user.</span></span> <span data-ttu-id="4ead3-131">Siga estes passos para encontrar o ID do objeto de um utilizador no portal Azure:</span><span class="sxs-lookup"><span data-stu-id="4ead3-131">Follow these steps to find a user's object ID in the Azure portal:</span></span>

1. <span data-ttu-id="4ead3-132">Inicie sessão no [portal do Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="4ead3-132">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="4ead3-133">Selecione **Azure Ative Directory** no menu.</span><span class="sxs-lookup"><span data-stu-id="4ead3-133">Select **Azure Active Directory** from the menu.</span></span>

3. <span data-ttu-id="4ead3-134">Localizar a secção **'Gerir'** no menu e, em seguida, selecionar **Utilizadores**.</span><span class="sxs-lookup"><span data-stu-id="4ead3-134">Locate the **Manage** section on the menu, then select **Users**.</span></span>

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="Mostra menu Azure Ative Directory com opção de utilizadores em destaque.":::

4. <span data-ttu-id="4ead3-136">Na página Utilizadores, digite o nome do utilizador na caixa de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="4ead3-136">From the Users page, type the user's name in the search box.</span></span>

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="Mostra a página do Utilizador com caixa de pesquisa para procurar um utilizador específico.":::

5. <span data-ttu-id="4ead3-138">Selecione o nome do utilizador onde aparece na lista.</span><span class="sxs-lookup"><span data-stu-id="4ead3-138">Select the user's name where it appears on the list.</span></span>  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="Mostra a página do utilizador a apresentar uma linha para o utilizador pesquisado.":::

6. <span data-ttu-id="4ead3-140">Localize a secção identidade na página 'Perfil' do utilizador.</span><span class="sxs-lookup"><span data-stu-id="4ead3-140">Locate the Identity section on the user's Profile page.</span></span> <span data-ttu-id="4ead3-141">O campo de identificação do objeto aparece aqui com o ID do objeto único do utilizador.</span><span class="sxs-lookup"><span data-stu-id="4ead3-141">The Object ID field appears here with the user's unique object ID.</span></span>

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="Mostra a página do Perfil do Utilizador com a secção identidade e um campo destacado para o ID do objeto.":::

## <a name="next-steps"></a><span data-ttu-id="4ead3-143">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="4ead3-143">Next steps</span></span>

- [<span data-ttu-id="4ead3-144">Encontre o seu ID de inquilino programáticamente com PowerShell ou CLI</span><span class="sxs-lookup"><span data-stu-id="4ead3-144">Find your tenant ID programmatically with PowerShell or CLI</span></span>](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant)
- [<span data-ttu-id="4ead3-145">Saiba mais sobre os perfis de utilizador no Azure Ative Directory</span><span class="sxs-lookup"><span data-stu-id="4ead3-145">Learn more about user profiles in Azure Active Directory</span></span>](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [<span data-ttu-id="4ead3-146">Saiba como os parceiros podem ver ou exportar detalhes do cliente no Partner Center</span><span class="sxs-lookup"><span data-stu-id="4ead3-146">Find out how partners can see or export customer details in Partner Center</span></span>](see-your-customer-list.md)

