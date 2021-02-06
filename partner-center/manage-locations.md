---
title: Gerir localizações na sua conta de parceiro
ms.topic: how-to
ms.date: 02/05/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Saiba como adicionar uma nova localização e como a localização MPN ID é usada em programas de incentivo, negócios de CSP, subscrições e outras transações.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c5ac31b772c6757468c5ea9d463643731571b31f
ms.sourcegitcommit: d37a3f353426e52dfbbac577b7576f9c3f6d2ddf
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/06/2021
ms.locfileid: "99624277"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a><span data-ttu-id="49da3-103">Gerencie as localizações da sua conta MPN e adicione uma nova localização</span><span class="sxs-lookup"><span data-stu-id="49da3-103">Manage your MPN account locations and add a new location</span></span>


<span data-ttu-id="49da3-104">**Funções adequadas**</span><span class="sxs-lookup"><span data-stu-id="49da3-104">**Appropriate roles**</span></span>

- <span data-ttu-id="49da3-105">Administrador global</span><span class="sxs-lookup"><span data-stu-id="49da3-105">Global admin</span></span>
- <span data-ttu-id="49da3-106">Administrador de conta</span><span class="sxs-lookup"><span data-stu-id="49da3-106">Account admin</span></span>

<span data-ttu-id="49da3-107">A localização MPN ID identifica cada localização específica da sua empresa.</span><span class="sxs-lookup"><span data-stu-id="49da3-107">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="49da3-108">Utiliza a localização MPN ID para se inscrever em programas de incentivo, para transacionar negócios do Cloud Solution Provider (CSP) e outras transações comerciais.</span><span class="sxs-lookup"><span data-stu-id="49da3-108">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="49da3-109">O ID MPN global é utilizado para atividades não transacionais, tais como pedidos de apoio.</span><span class="sxs-lookup"><span data-stu-id="49da3-109">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-is-a-typical-scenario"></a><span data-ttu-id="49da3-110">Segue-se um cenário típico:</span><span class="sxs-lookup"><span data-stu-id="49da3-110">The following is a typical scenario:</span></span>

<span data-ttu-id="49da3-111">A Contoso tem a sua conta global Partner (PGA) no Reino Unido.</span><span class="sxs-lookup"><span data-stu-id="49da3-111">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="49da3-112">Este é o seu negócio legal registrado, e o seu ID MPN global é usado para gerir todos os negócios não transacionais.</span><span class="sxs-lookup"><span data-stu-id="49da3-112">This is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="49da3-113">A Contoso também tem contas de localização partner (PLA) equivalentes a subsidiárias ou divisões em outro local no Reino Unido, França e EUA.</span><span class="sxs-lookup"><span data-stu-id="49da3-113">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="49da3-114">Na estrutura da Conta MPN, estas PLAs são representadas como IDs MPN de localização única.</span><span class="sxs-lookup"><span data-stu-id="49da3-114">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="49da3-115">As PLAs são utilizadas para negócios transacionais, como CSP ou programas de incentivos.</span><span class="sxs-lookup"><span data-stu-id="49da3-115">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="49da3-116">Os pagamentos estão ligados a locais específicos.</span><span class="sxs-lookup"><span data-stu-id="49da3-116">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="49da3-117">Há uma relação 1-1 entre um inquilino da CSP e uma identificação de localização MPN.</span><span class="sxs-lookup"><span data-stu-id="49da3-117">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="Estrutura das localizações da MPN":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a><span data-ttu-id="49da3-119">Pré-requisitos para adicionar uma nova conta para uma empresa de CSP</span><span class="sxs-lookup"><span data-stu-id="49da3-119">Prerequisites in order to add a new account for a CSP business</span></span>

<span data-ttu-id="49da3-120">Para adicionar uma nova conta de negócios da CSP, comece por garantir que cumpriu os pré-requisitos.</span><span class="sxs-lookup"><span data-stu-id="49da3-120">To add a new CSP business account, start by ensuring that you have fulfilled the prerequisites.</span></span>

1. <span data-ttu-id="49da3-121">Você deve ter uma identificação MPN de localização no país onde você quer fazer negócios com CSP.</span><span class="sxs-lookup"><span data-stu-id="49da3-121">You must have a location MPN ID in the country where you want to do CSP business.</span></span> <span data-ttu-id="49da3-122">Para criar uma nova localização MPN, leia "Adicionar uma localização MPN" abaixo.</span><span class="sxs-lookup"><span data-stu-id="49da3-122">To create a new MPN location, read “Add an MPN location” below.</span></span>
  
1. <span data-ttu-id="49da3-123">Para criar uma nova inscrição de Revendedor Indireto CSP, leia [Trabalhar com fornecedores indiretos](indirect-reseller-tasks-in-partner-center.md#get-started)</span><span class="sxs-lookup"><span data-stu-id="49da3-123">To create a new CSP Indirect Reseller enrollment, read [Work with Indirect providers](indirect-reseller-tasks-in-partner-center.md#get-started)</span></span> 

>[!NOTE] 
 ><span data-ttu-id="49da3-124">Lembre-se de assinar com as **novas** credenciais para a **nova** conta CSP.</span><span class="sxs-lookup"><span data-stu-id="49da3-124">Remember to sign in with the **new** credentials for the **new** CSP account.</span></span> <span data-ttu-id="49da3-125">Não use as suas credenciais existentes como Partner Center irá reconhecê-lo como tendo já uma conta.</span><span class="sxs-lookup"><span data-stu-id="49da3-125">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

2. <span data-ttu-id="49da3-126">Aceite o Acordo de Parceiro da Microsoft e ative a conta.</span><span class="sxs-lookup"><span data-stu-id="49da3-126">Accept the Microsoft Partner Agreement and activate the account.</span></span>

1. <span data-ttu-id="49da3-127">Se quiser inscrever-se como parceiro direct Bill, leia [requisitos para parceiros direct Bill](direct-partner-new-requirements.md)</span><span class="sxs-lookup"><span data-stu-id="49da3-127">If you want to enroll as a Direct Bill partner, read [Requirements for Direct Bill partners](direct-partner-new-requirements.md)</span></span>

## <a name="view-your-mpn-locations"></a><span data-ttu-id="49da3-128">Ver as suas localizações de MPN</span><span class="sxs-lookup"><span data-stu-id="49da3-128">View your MPN locations</span></span>

1. <span data-ttu-id="49da3-129">Inscreva-se no painel partner [Center](https://partner.microsoft.com/dashboard/home) com as suas credenciais de conta MPN.</span><span class="sxs-lookup"><span data-stu-id="49da3-129">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/home) with your MPN account credentials.</span></span> <span data-ttu-id="49da3-130">(As suas credenciais MPN podem ser diferentes das suas credenciais de CSP)</span><span class="sxs-lookup"><span data-stu-id="49da3-130">(Your MPN credentials may be different from your CSP credentials)</span></span> 
 
1. <span data-ttu-id="49da3-131">A partir do ícone **Definições,** selecione **definições de conta**, **perfil de organização,** **Legal**.</span><span class="sxs-lookup"><span data-stu-id="49da3-131">From the **Settings** icon, select **Account settings**, **Organization profile**, **Legal**.</span></span> 

1. <span data-ttu-id="49da3-132">No **separador Partner** verifique se não existe uma mensagem de erro de banner a pedir-lhe para corrigir locais migrados a partir de PMC.</span><span class="sxs-lookup"><span data-stu-id="49da3-132">On the **Partner** tab verify that there isn't a banner error message asking you to fix migrated locations from PMC.</span></span> <span data-ttu-id="49da3-133">Se houver, siga as instruções e fixe os locais.</span><span class="sxs-lookup"><span data-stu-id="49da3-133">If there is, follow instructions and fix those locations.</span></span> 

3. <span data-ttu-id="49da3-134">Se não houver uma mensagem de erro, então a partir de  **Definições**, selecione  **Definições** de Conta , **Perfil da Organização,** **Identificadores**.</span><span class="sxs-lookup"><span data-stu-id="49da3-134">If there isn't an error message, then from  **Settings**, select  **Account Settings**, **Organization profile**, **Identifiers**.</span></span>

4. <span data-ttu-id="49da3-135">Encontre o ID MPN com o Tipo "Localização" que corresponda ao país desta conta CSP e use-o para pesquisar abaixo e completar a associação.</span><span class="sxs-lookup"><span data-stu-id="49da3-135">Find the MPN ID with Type "Location" that matches the country of this CSP account and use it to search below and complete association.</span></span>

5. <span data-ttu-id="49da3-136">Se não conseguir encontrar o ID MPN de localização que corresponda à conta CSP que pretende utilizar, pode adicionar uma nova localização que irá criar um novo ID MPN.</span><span class="sxs-lookup"><span data-stu-id="49da3-136">If you can’t find the location MPN ID that matches the CSP account you want to use, you can add a new location which will create a new MPN ID.</span></span> <span data-ttu-id="49da3-137">Consulte **a localização mpn** abaixo.</span><span class="sxs-lookup"><span data-stu-id="49da3-137">See **Add an MPN location** below.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="49da3-138">Adicione uma localização MPN</span><span class="sxs-lookup"><span data-stu-id="49da3-138">Add an MPN location</span></span>

1. <span data-ttu-id="49da3-139">Inscreva-se usando a conta MPN no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="49da3-139">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="49da3-140">(As suas credenciais MPN podem ser diferentes das suas credenciais CSP) .</span><span class="sxs-lookup"><span data-stu-id="49da3-140">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="49da3-141">A conta MPN deve ter privilégios de Administração Global ou Administração de Contas.</span><span class="sxs-lookup"><span data-stu-id="49da3-141">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="49da3-142">A partir do **ícone Definições,** selecione as **definições de Conta** e, em seguida, selecione o perfil da **Organização**.</span><span class="sxs-lookup"><span data-stu-id="49da3-142">From the **Settings icon**, select the **Account settings** and then select **Organization profile**.</span></span>

2. <span data-ttu-id="49da3-143">Selecione **Legal** e, em seguida, no separador **Parceiro,** selecione **localizações de Negócios** e clique em **Adicionar uma localização.**</span><span class="sxs-lookup"><span data-stu-id="49da3-143">Select **Legal** and then, on the **Partner** tab, select **Business locations,** and click on **Add a location.**</span></span>

3. <span data-ttu-id="49da3-144">Forneça os dados necessários, incluindo o nome comercial, endereço e contato para a localização que pretende adicionar à sua empresa.</span><span class="sxs-lookup"><span data-stu-id="49da3-144">Provide the required details including business name, address, and contact for the location that you want to add to your company.</span></span>
 
1. <span data-ttu-id="49da3-145">Clique **em Adicionar localização**.</span><span class="sxs-lookup"><span data-stu-id="49da3-145">Click **Add location**.</span></span> <span data-ttu-id="49da3-146">Isto criará um novo ID MPN para o novo local que pode utilizar para transações e incentivos da CSP.</span><span class="sxs-lookup"><span data-stu-id="49da3-146">This will create a new MPN ID for the new location which you can use for CSP transactions and incentives.</span></span>

:::image type="content" source="images/legal-biz.png" alt-text="Adicione um novo negócio legal":::

> [!NOTE]
> <span data-ttu-id="49da3-148">Uma vez que uma localização é adicionada no Centro de Parceiros, não pode ser removida.</span><span class="sxs-lookup"><span data-stu-id="49da3-148">Once a location is added in Partner Center, it cannot be removed.</span></span> <span data-ttu-id="49da3-149">Verá **MPN** no menu esquerdo do Partner Center se tiver usado o ID MPN correto para iniciar sins.</span><span class="sxs-lookup"><span data-stu-id="49da3-149">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="change-country-of-partner-global-account"></a><span data-ttu-id="49da3-150">Mudar país de conta global partner</span><span class="sxs-lookup"><span data-stu-id="49da3-150">Change country of Partner global account</span></span> 

1. <span data-ttu-id="49da3-151">Inscreva-se usando a conta MPN no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="49da3-151">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="49da3-152">(As suas credenciais MPN podem ser diferentes das suas credenciais CSP) .</span><span class="sxs-lookup"><span data-stu-id="49da3-152">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="49da3-153">A conta MPN deve ter privilégios de Administração Global ou Administração de Contas.</span><span class="sxs-lookup"><span data-stu-id="49da3-153">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

2. <span data-ttu-id="49da3-154">No separador **Partner,** vá às localizações do **Negócios** e verifique a lista de locais para garantir que o local que deseja como entidade legal está listado.</span><span class="sxs-lookup"><span data-stu-id="49da3-154">On the **Partner** tab, go to **Business locations** and check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> 
 
1. <span data-ttu-id="49da3-155">Para adicionar uma localização, clique em **Adicionar uma localização** e, no voo para fora, forneça os detalhes necessários, incluindo o nome do negócio, endereço e contacto primário para a localização que pretende adicionar à sua empresa.</span><span class="sxs-lookup"><span data-stu-id="49da3-155">To add a location, click **Add a location**, and, in the fly out, provide the required details including business name, address, and primary contact for the location that you want to add to your company.</span></span> 
 
1. <span data-ttu-id="49da3-156">Selecione **Mude o seu país** junto ao **país/região** drop-down e siga os passos.</span><span class="sxs-lookup"><span data-stu-id="49da3-156">Select **Change your country** next to the **Country/region** drop-down and follow the steps.</span></span> 

:::image type="content" source="images/lbp.png" alt-text="Os dados do perfil de negócio legal voam para fora":::

5. <span data-ttu-id="49da3-158">Clique em **Guardar**.</span><span class="sxs-lookup"><span data-stu-id="49da3-158">Click **Save**.</span></span>

6. <span data-ttu-id="49da3-159">O país da conta global da MPN será alterado para o novo país legal.</span><span class="sxs-lookup"><span data-stu-id="49da3-159">MPN global account country will be changed to the new legal country.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="49da3-160">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="49da3-160">Next steps</span></span>

- <span data-ttu-id="49da3-161">Conheça o [processo de verificação.](verification-responses.md)</span><span class="sxs-lookup"><span data-stu-id="49da3-161">Learn about the [verification process](verification-responses.md).</span></span>
