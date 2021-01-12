---
title: Adicione inquilinos adicionais à sua conta partner Center
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como adicionar, consolidar ou gerir vários inquilinos AZure AD na sua conta partner Center. Saiba também sobre algumas das razões pelas quais poderá querer fazê-lo.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 22f85bda0a651559da1717ae1e5365da40d62aff
ms.sourcegitcommit: 8cb98de420f6ab5bb4cb3efc9007262c4d7d3327
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/12/2021
ms.locfileid: "98105561"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="e8a16-104">Adicione e gere vários inquilinos na sua conta Partner Center</span><span class="sxs-lookup"><span data-stu-id="e8a16-104">Add and manage multiple tenants in your Partner Center account</span></span>


<span data-ttu-id="e8a16-105">**Funções adequadas**</span><span class="sxs-lookup"><span data-stu-id="e8a16-105">**Appropriate roles**</span></span>

- <span data-ttu-id="e8a16-106">Administrador global</span><span class="sxs-lookup"><span data-stu-id="e8a16-106">Global admin</span></span>

<span data-ttu-id="e8a16-107">Esta funcionalidade permite-lhe gerir vários inquilinos para a sua empresa e consolidá-los na sua conta do Centro de Parceiros.</span><span class="sxs-lookup"><span data-stu-id="e8a16-107">This feature allows you to manage multiple tenants for your company and to consolidate them into your Partner Center account.</span></span> <span data-ttu-id="e8a16-108">Existem muitas razões pelas quais você pode precisar de gerir vários inquilinos AZure AD na sua conta partner Center.</span><span class="sxs-lookup"><span data-stu-id="e8a16-108">There are many reasons why you may need to manage multiple Azure AD tenants in your Partner Center account.</span></span> <span data-ttu-id="e8a16-109">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="e8a16-109">For example:</span></span>

- <span data-ttu-id="e8a16-110">A sua empresa pode comprar outra empresa, e quer que os colaboradores da nova empresa possam utilizar o Partner Center.</span><span class="sxs-lookup"><span data-stu-id="e8a16-110">Your company may purchase another company, and you want the employees in the new company to be able to use Partner Center.</span></span> <span data-ttu-id="e8a16-111">No entanto, quer que as duas empresas permaneçam separadas.</span><span class="sxs-lookup"><span data-stu-id="e8a16-111">However, you want the two companies to remain separate.</span></span> <span data-ttu-id="e8a16-112">Neste caso, associaria o inquilino da AZure AD da nova empresa à sua conta global partner (PGA).</span><span class="sxs-lookup"><span data-stu-id="e8a16-112">In this case, you'd associate the new company's Azure AD tenant with your Partner global account (PGA).</span></span> <span data-ttu-id="e8a16-113">Esta associação permitiria que os utilizadores de ambas as empresas trabalhassem no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="e8a16-113">This association would enable users in both companies to work in Partner Center.</span></span>

- <span data-ttu-id="e8a16-114">Se tiver mais de um inquilino para gerir o seu negócio (por exemplo, contoso.com, contoso.uk, contoso.in) pode usar vários arrendamentos para os amarrar na mesma conta de PC.</span><span class="sxs-lookup"><span data-stu-id="e8a16-114">If you have more than one tenant to run your business (e.g. contoso.com, contoso.uk, contoso.in) you can use multi-tenancy to tie them under the same PC account.</span></span>

- <span data-ttu-id="e8a16-115">Fusões e aquisições obrigam a trabalhar com mais do que um inquilino (por exemplo, se a Contoso adquirir a Fabrikam, terá de ser capaz de utilizar tanto Constoso.com como Fabrikam.com respetivos inquilinos).</span><span class="sxs-lookup"><span data-stu-id="e8a16-115">Mergers and acquisitions requires you to work with more than one tenant (e.g. If Contoso acquires Fabrikam, you would need to be able to use both Constoso.com and Fabrikam.com respective tenants).</span></span>

- <span data-ttu-id="e8a16-116">Os utilizadores de qualquer um dos inquilinos teriam de ser capazes de:</span><span class="sxs-lookup"><span data-stu-id="e8a16-116">Users from any of the tenants would need to be able to:</span></span>
    1.  <span data-ttu-id="e8a16-117">Centro de Parceiros de Acesso para formação, downloads digitais, associação MCP</span><span class="sxs-lookup"><span data-stu-id="e8a16-117">Access Partner Center for training, digital downloads, MCP association</span></span>
    2.  <span data-ttu-id="e8a16-118">Ser designado Partner Center funções como MPN Admin, Incentives Admin etc.</span><span class="sxs-lookup"><span data-stu-id="e8a16-118">Be assigned Partner Center roles like MPN Admin, Incentives Admin etc.</span></span>


## <a name="add-another-azure-ad-tenant-to-your-account"></a><span data-ttu-id="e8a16-119">Adicione outro inquilino AZure AD à sua conta</span><span class="sxs-lookup"><span data-stu-id="e8a16-119">Add another Azure AD tenant to your account</span></span>

1. <span data-ttu-id="e8a16-120">Como administrador global, inscreva-se no painel partner [center](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="e8a16-120">As the global admin, sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>
1. <span data-ttu-id="e8a16-121">A partir do ícone **Definições,** selecione **as definições de Conta** e, em seguida, selecione **Inquilinos**.</span><span class="sxs-lookup"><span data-stu-id="e8a16-121">From the **Settings** icon, select **Account settings** and then select **Tenants**.</span></span>
 
:::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="inquilinos associados"::: 

3. <span data-ttu-id="e8a16-123">Selecione **Associar outro inquilino de AD** e indicar o inquilino que você deseja associar.</span><span class="sxs-lookup"><span data-stu-id="e8a16-123">Select **Associate another AD tenant** and indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="e8a16-124">Como administrador global, inscreva-se no inquilino que quer associar e confirmar a associação.</span><span class="sxs-lookup"><span data-stu-id="e8a16-124">As global admin, sign into the tenant you want to associate and confirm the association.</span></span> 

:::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="confirmar inquilinos associados"::: 

5. <span data-ttu-id="e8a16-126">Depois de confirmar, verá um aviso **de todos os conjuntos.**</span><span class="sxs-lookup"><span data-stu-id="e8a16-126">After you confirm, you will see an **All set** notice.</span></span>  <span data-ttu-id="e8a16-127">**Selecione Return to tenant management** e você verá o recém-adicionado inquilino listado.</span><span class="sxs-lookup"><span data-stu-id="e8a16-127">Select **Return to tenant management** and you'll see the newly added tenant listed.</span></span> 
 

>[!NOTE]
><span data-ttu-id="e8a16-128">Não pode associar um inquilino a uma conta se já estiver associado a outra conta do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="e8a16-128">You can't associate a tenant to an account if it is already associated to another Partner Center account.</span></span>


## <a name="remove-a-tenant-from-your-account"></a><span data-ttu-id="e8a16-129">Retire um inquilino da sua conta</span><span class="sxs-lookup"><span data-stu-id="e8a16-129">Remove a tenant from your account</span></span>
 
1. <span data-ttu-id="e8a16-130">Como administrador global, inscreva-se no painel partner [center](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="e8a16-130">As the global admin, sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="e8a16-131">A partir do ícone **Definições,** selecione **definições** de conta -> Inquilinos e clique no **separador Parceiro.**</span><span class="sxs-lookup"><span data-stu-id="e8a16-131">From the **Settings** icon, select **Account settings** -> Tenants and click on the **Partner** tab.</span></span>
 
3. <span data-ttu-id="e8a16-132">Clique em **Remover** para o inquilino que deseja dissociar.</span><span class="sxs-lookup"><span data-stu-id="e8a16-132">Click **Remove** for the tenant you want to dissociate.</span></span>

4. <span data-ttu-id="e8a16-133">Dissociar um inquilino significa que os utilizadores desse inquilino deixarão de ter acesso à conta do Centro de Parceiros, o que poderá ter impacto nas suas competências.</span><span class="sxs-lookup"><span data-stu-id="e8a16-133">Dissociating a tenant means that the users on that tenant will no longer have access to the Partner Center account, and this could have an impact on your competencies.</span></span> 

<span data-ttu-id="e8a16-134">O botão **Remover** está ativado para todos os inquilinos associados, exceto o inquilino principal e o inquilino em que você está atualmente assinado.</span><span class="sxs-lookup"><span data-stu-id="e8a16-134">The **Remove** button is enabled for all associated tenants, except the primary tenant and the tenant which you are currently signed into.</span></span>

:::image type="content" source="images/disassociate.png" alt-text="inquilinos com o botão remover":::
 

## <a name="next-steps"></a><span data-ttu-id="e8a16-136">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="e8a16-136">Next steps</span></span>

- [<span data-ttu-id="e8a16-137">Adicionar utilizadores</span><span class="sxs-lookup"><span data-stu-id="e8a16-137">Add users</span></span>](create-user-accounts-and-set-permissions.md)






