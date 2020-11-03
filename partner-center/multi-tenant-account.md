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
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="4fe20-104">Adicione e gere vários inquilinos na sua conta Partner Center</span><span class="sxs-lookup"><span data-stu-id="4fe20-104">Add and manage multiple tenants in your Partner Center account</span></span>

<span data-ttu-id="4fe20-105">**Aplica-se a**</span><span class="sxs-lookup"><span data-stu-id="4fe20-105">**Applies to**</span></span>

- <span data-ttu-id="4fe20-106">Partner Center</span><span class="sxs-lookup"><span data-stu-id="4fe20-106">Partner Center</span></span>

<span data-ttu-id="4fe20-107">**Funções adequadas**</span><span class="sxs-lookup"><span data-stu-id="4fe20-107">**Appropriate roles**</span></span>

- <span data-ttu-id="4fe20-108">Administrador global</span><span class="sxs-lookup"><span data-stu-id="4fe20-108">Global admin</span></span>

<span data-ttu-id="4fe20-109">Esta funcionalidade permite-lhe gerir vários inquilinos para a sua empresa e consolidá-los na sua conta do Centro de Parceiros.</span><span class="sxs-lookup"><span data-stu-id="4fe20-109">This feature allows you to manage multiple tenants for your company and to consolidate them into your Partner Center account.</span></span> <span data-ttu-id="4fe20-110">Existem muitas razões pelas quais você pode precisar de gerir vários inquilinos AZure AD na sua conta partner Center.</span><span class="sxs-lookup"><span data-stu-id="4fe20-110">There are many reasons why you may need to manage multiple Azure AD tenants in your Partner Center account.</span></span> <span data-ttu-id="4fe20-111">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="4fe20-111">For example:</span></span>

- <span data-ttu-id="4fe20-112">A sua empresa pode comprar outra empresa, e quer que os colaboradores da nova empresa possam utilizar o Partner Center.</span><span class="sxs-lookup"><span data-stu-id="4fe20-112">Your company may purchase another company, and you want the employees in the new company to be able to use Partner Center.</span></span> <span data-ttu-id="4fe20-113">No entanto, quer que as duas empresas permaneçam separadas.</span><span class="sxs-lookup"><span data-stu-id="4fe20-113">However, you want the two companies to remain separate.</span></span> <span data-ttu-id="4fe20-114">Neste caso, associaria o inquilino da AZure AD da nova empresa à sua conta global partner (PGA).</span><span class="sxs-lookup"><span data-stu-id="4fe20-114">In this case, you'd associate the new company's Azure AD tenant with your Partner global account (PGA).</span></span> <span data-ttu-id="4fe20-115">Esta associação permitiria que os utilizadores de ambas as empresas trabalhassem no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="4fe20-115">This association would enable users in both companies to work in Partner Center.</span></span>

- <span data-ttu-id="4fe20-116">Se tiver mais de um inquilino para gerir o seu negócio (por exemplo, contoso.com, contoso.uk, contoso.in) pode usar vários arrendamentos para os amarrar na mesma conta de PC.</span><span class="sxs-lookup"><span data-stu-id="4fe20-116">If you have more than one tenant to run your business (e.g. contoso.com, contoso.uk, contoso.in) you can use multi-tenancy to tie them under the same PC account.</span></span>

- <span data-ttu-id="4fe20-117">Fusões e aquisições obrigam a trabalhar com mais do que um inquilino (por exemplo, se a Contoso adquirir a Fabrikam, terá de ser capaz de utilizar tanto Constoso.com como Fabrikam.com respetivos inquilinos).</span><span class="sxs-lookup"><span data-stu-id="4fe20-117">Mergers and acquisitions requires you to work with more than one tenant (e.g. If Contoso acquires Fabrikam, you would need to be able to use both Constoso.com and Fabrikam.com respective tenants).</span></span>

- <span data-ttu-id="4fe20-118">Os utilizadores de qualquer um dos inquilinos teriam de ser capazes de:</span><span class="sxs-lookup"><span data-stu-id="4fe20-118">Users from any of the tenants would need to be able to:</span></span>
    1.  <span data-ttu-id="4fe20-119">Centro de Parceiros de Acesso para formação, downloads digitais, associação MCP</span><span class="sxs-lookup"><span data-stu-id="4fe20-119">Access Partner Center for training, digital downloads, MCP association</span></span>
    2.  <span data-ttu-id="4fe20-120">Ser designado Partner Center funções como MPN Admin, Incentives Admin etc.</span><span class="sxs-lookup"><span data-stu-id="4fe20-120">Be assigned Partner Center roles like MPN Admin, Incentives Admin etc.</span></span>


## <a name="add-another-azure-ad-tenant-to-your-account"></a><span data-ttu-id="4fe20-121">Adicione outro inquilino AZure AD à sua conta</span><span class="sxs-lookup"><span data-stu-id="4fe20-121">Add another Azure AD tenant to your account</span></span>

1. <span data-ttu-id="4fe20-122">Como administrador global, inscreva-se no painel partner [center](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="4fe20-122">As the global admin, sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>
1. <span data-ttu-id="4fe20-123">A partir do ícone **Definições,** selecione **as definições de Conta** e, em seguida, selecione **Inquilinos** .</span><span class="sxs-lookup"><span data-stu-id="4fe20-123">From the **Settings** icon, select **Account settings** and then select **Tenants** .</span></span>
 
:::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="inquilinos associados"::: 

3. <span data-ttu-id="4fe20-125">Selecione **Associar outro inquilino de AD** e indicar o inquilino que você deseja associar.</span><span class="sxs-lookup"><span data-stu-id="4fe20-125">Select **Associate another AD tenant** and indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="4fe20-126">Como administrador global, inscreva-se no inquilino que quer associar e confirmar a associação.</span><span class="sxs-lookup"><span data-stu-id="4fe20-126">As global admin, sign into the tenant you want to associate and confirm the association.</span></span> 

:::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="confirmar inquilinos associados"::: 

5. <span data-ttu-id="4fe20-128">Depois de confirmar, verá um aviso **de todos os conjuntos.**</span><span class="sxs-lookup"><span data-stu-id="4fe20-128">After you confirm, you will see an **All set** notice.</span></span>  <span data-ttu-id="4fe20-129">**Selecione Return to tenant management** e você verá o recém-adicionado inquilino listado.</span><span class="sxs-lookup"><span data-stu-id="4fe20-129">Select **Return to tenant management** and you will see the newly added tenant listed.</span></span> 
 

>[!NOTE]
><span data-ttu-id="4fe20-130">Não pode associar um inquilino a uma conta se já estiver associado a outra conta do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="4fe20-130">You can't associate a tenant to an account if it is already associated to another Partner Center account.</span></span>

 
## <a name="next-steps"></a><span data-ttu-id="4fe20-131">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="4fe20-131">Next steps</span></span>

- [<span data-ttu-id="4fe20-132">Adicionar utilizadores</span><span class="sxs-lookup"><span data-stu-id="4fe20-132">Add users</span></span>](create-user-accounts-and-set-permissions.md)
