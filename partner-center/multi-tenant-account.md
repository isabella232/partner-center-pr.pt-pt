---
title: Adicione inquilinos à sua conta partner Center
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como adicionar, consolidar ou gerir vários inquilinos AZure AD na sua conta partner Center, e saiba por que quer fazê-lo.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 2f3094489f65b7164b4a55804047f9a4ab5f11cb
ms.sourcegitcommit: 79d2f00c352db61252e523f45abf93fe2a2742a5
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/04/2021
ms.locfileid: "102124810"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="78a1c-103">Adicione e gere vários inquilinos na sua conta Partner Center</span><span class="sxs-lookup"><span data-stu-id="78a1c-103">Add and manage multiple tenants in your Partner Center account</span></span>


<span data-ttu-id="78a1c-104">**Funções adequadas**</span><span class="sxs-lookup"><span data-stu-id="78a1c-104">**Appropriate roles**</span></span>

- <span data-ttu-id="78a1c-105">Administrador global</span><span class="sxs-lookup"><span data-stu-id="78a1c-105">Global admin</span></span>
- <span data-ttu-id="78a1c-106">Administrador de conta</span><span class="sxs-lookup"><span data-stu-id="78a1c-106">Account admin</span></span>

<span data-ttu-id="78a1c-107">Este artigo discute como consolidar vários inquilinos do Azure Ative Directory (Azure AD) para a sua empresa e, em seguida, adicioná-los e geri-los na sua conta partner Center.</span><span class="sxs-lookup"><span data-stu-id="78a1c-107">This article discusses how to consolidate multiple Azure Active Directory (Azure AD) tenants for your company and then add and manage them in your Partner Center account.</span></span> <span data-ttu-id="78a1c-108">Há muitas razões para o fazer.</span><span class="sxs-lookup"><span data-stu-id="78a1c-108">There are many reasons to do so.</span></span> <span data-ttu-id="78a1c-109">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="78a1c-109">For example:</span></span>

- <span data-ttu-id="78a1c-110">Digamos que a sua empresa, Contoso, adquiriu outra empresa, a Fabrikam.</span><span class="sxs-lookup"><span data-stu-id="78a1c-110">Let's say your company, Contoso, has acquired another company, Fabrikam.</span></span> <span data-ttu-id="78a1c-111">Quer que as duas empresas permaneçam separadas, mas quer que os novos colaboradores possam usar o Partner Center.</span><span class="sxs-lookup"><span data-stu-id="78a1c-111">You want the two companies to remain separate, but you want the new employees to be able to use Partner Center.</span></span> <span data-ttu-id="78a1c-112">Neste caso, associa o inquilino Azure AD da nova empresa à sua conta global partner (PGA).</span><span class="sxs-lookup"><span data-stu-id="78a1c-112">In this case, you associate the new company's Azure AD tenant with your Partner global account (PGA).</span></span> <span data-ttu-id="78a1c-113">Esta associação permite que os utilizadores de ambas as empresas trabalhem no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="78a1c-113">This association enables users in both companies to work in Partner Center.</span></span>

- <span data-ttu-id="78a1c-114">Se gere o seu negócio com mais de um inquilino (por exemplo, *contoso.com*, *contoso.uk*, e *contoso.in),* pode utilizar a multitenência para agrupar na mesma conta de PC.</span><span class="sxs-lookup"><span data-stu-id="78a1c-114">If you run your business with more than one tenant (for example, *contoso.com*, *contoso.uk*, and *contoso.in*), you can use multitenancy to group them in the same PC account.</span></span>

- <span data-ttu-id="78a1c-115">Se as diretrizes de fusões e aquisições exigirem que você trabalhe com inquilinos de ambas as empresas, você usaria tanto o *constoso.com* como *fabrikam.com* inquilinos.</span><span class="sxs-lookup"><span data-stu-id="78a1c-115">If mergers and acquisitions guidelines require you to work with tenants of both companies, you would use both the *constoso.com* and *fabrikam.com* tenants.</span></span>

- <span data-ttu-id="78a1c-116">Os utilizadores de qualquer um dos inquilinos devem ser capazes de:</span><span class="sxs-lookup"><span data-stu-id="78a1c-116">Users of any of the tenants need to be able to:</span></span>
    * <span data-ttu-id="78a1c-117">Access Partner Center para formação, downloads digitais ou associação Microsoft Certified Professional (MCP).</span><span class="sxs-lookup"><span data-stu-id="78a1c-117">Access Partner Center for training, digital downloads, or Microsoft Certified Professional (MCP) association.</span></span>
    * <span data-ttu-id="78a1c-118">Ser designado funções partner center tais como Microsoft Partner Network (MPN) administração ou administração de incentivos.</span><span class="sxs-lookup"><span data-stu-id="78a1c-118">Be assigned Partner Center roles such as Microsoft Partner Network (MPN) admin or incentives admin.</span></span>

## <a name="add-an-azure-ad-tenant-to-your-account"></a><span data-ttu-id="78a1c-119">Adicione um inquilino AZure AD à sua conta</span><span class="sxs-lookup"><span data-stu-id="78a1c-119">Add an Azure AD tenant to your account</span></span>

1. <span data-ttu-id="78a1c-120">Inscreva-se como administrador global para o [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="78a1c-120">Sign in as global admin to [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="78a1c-121">No canto superior direito, selecione **Definições**, selecione **definições de Conta** e, em seguida, selecione **Inquilinos**.</span><span class="sxs-lookup"><span data-stu-id="78a1c-121">At the upper right, select **Settings**, select **Account settings**, and then select **Tenants**.</span></span>
 
   :::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="Screenshot do botão Associado no painel de perfil Ad Azure."::: 

1. <span data-ttu-id="78a1c-123">Selecione **Associado** e, em seguida, indique o inquilino que deseja associar.</span><span class="sxs-lookup"><span data-stu-id="78a1c-123">Select **Associate**, and then indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="78a1c-124">No momento, inscreva-se como administrador global para o inquilino que pretende associar e, em seguida, **selecione Confirmar**.</span><span class="sxs-lookup"><span data-stu-id="78a1c-124">At the prompt, sign in as global admin to the tenant you want to associate, and then select **Confirm**.</span></span> 

   :::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="Screenshot do botão Confirmar no painel de associação Confirm novo Azure AD."::: 

   <span data-ttu-id="78a1c-126">Depois de ter confirmado a associação, é exibida uma mensagem **all set.**</span><span class="sxs-lookup"><span data-stu-id="78a1c-126">After you've confirmed the association, an **All set** message is displayed.</span></span> <span data-ttu-id="78a1c-127">Para ver o recém-adicionado inquilino, **selecione Devolver à gestão de inquilinos.**</span><span class="sxs-lookup"><span data-stu-id="78a1c-127">To view the newly added tenant, select **Return to tenant management**.</span></span> 
 
>[!NOTE]
><span data-ttu-id="78a1c-128">Não pode associar um inquilino a uma conta se já estiver associado a outra conta do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="78a1c-128">You can't associate a tenant with an account if it's already associated with another Partner Center account.</span></span>


## <a name="remove-a-tenant-from-your-account"></a><span data-ttu-id="78a1c-129">Retire um inquilino da sua conta</span><span class="sxs-lookup"><span data-stu-id="78a1c-129">Remove a tenant from your account</span></span>
 
1. <span data-ttu-id="78a1c-130">Inscreva-se como administrador global para o [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="78a1c-130">Sign in as global admin to [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="78a1c-131">No canto superior direito, selecione o ícone **Definições** e, em seguida, selecione **as definições de Conta**.</span><span class="sxs-lookup"><span data-stu-id="78a1c-131">At the upper right, select the **Settings** icon, and then select **Account settings**.</span></span>

1. <span data-ttu-id="78a1c-132">No painel esquerdo, selecione **Inquilinos.**</span><span class="sxs-lookup"><span data-stu-id="78a1c-132">On the left pane, select **Tenants**.</span></span> <span data-ttu-id="78a1c-133">No **âmbito do Manage Azure AD,** selecione o **separador Partner.**</span><span class="sxs-lookup"><span data-stu-id="78a1c-133">Under **Manage Azure AD tenants**, select the **Partner** tab.</span></span>
 
1. <span data-ttu-id="78a1c-134">**Selecione Remova** ao lado do inquilino cuja associação pretende remover.</span><span class="sxs-lookup"><span data-stu-id="78a1c-134">Select **Remove** next to the tenant whose association you want to remove.</span></span>

   :::image type="content" source="images/disassociate.png" alt-text="Screenshot das atuais associações de inquilinos e seus links Remove.":::

   <span data-ttu-id="78a1c-136">Como mostrado na imagem anterior, os links **Remove** estão habilitados para todos os inquilinos associados, exceto para o inquilino principal e o inquilino que você está atualmente assinado.</span><span class="sxs-lookup"><span data-stu-id="78a1c-136">As shown in the preceding screenshot, the **Remove** links are enabled for all associated tenants, except for the primary tenant and the tenant that you're currently signed in to.</span></span> 

   > [!NOTE]   
   > <span data-ttu-id="78a1c-137">Quando você retira um inquilino, os utilizadores desse inquilino já não têm acesso à conta do Centro de Parceiros, e a remoção pode ter um impacto nas suas competências.</span><span class="sxs-lookup"><span data-stu-id="78a1c-137">When you remove a tenant, the users on that tenant no longer have access to the Partner Center account, and the removal might have an impact on your competencies.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="78a1c-138">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="78a1c-138">Next steps</span></span>

- [<span data-ttu-id="78a1c-139">Criar contas de utilizador</span><span class="sxs-lookup"><span data-stu-id="78a1c-139">Create user accounts</span></span>](create-user-accounts-and-set-permissions.md)






