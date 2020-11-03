---
title: Gerir localizações na sua conta de parceiro
ms.topic: article
ms.date: 10/12/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Saiba como adicionar uma nova localização e como a localização MPN ID é usada em programas de incentivo, negócios de CSP, subscrições e outras transações.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c6b0fc84636befedbc51aa0672ce19110eb4d9aa
ms.sourcegitcommit: 1719ff11409cd6953602b7798f8cfe821b8ea15e
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/15/2020
ms.locfileid: "92530428"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a><span data-ttu-id="fa32a-103">Gerencie as localizações da sua conta MPN e adicione uma nova localização</span><span class="sxs-lookup"><span data-stu-id="fa32a-103">Manage your MPN account locations and add a new location</span></span>

<span data-ttu-id="fa32a-104">**Aplica-se a**</span><span class="sxs-lookup"><span data-stu-id="fa32a-104">**Applies to**</span></span>

- <span data-ttu-id="fa32a-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="fa32a-105">Partner Center</span></span>

<span data-ttu-id="fa32a-106">**Funções adequadas**</span><span class="sxs-lookup"><span data-stu-id="fa32a-106">**Appropriate roles**</span></span>

- <span data-ttu-id="fa32a-107">Administrador global</span><span class="sxs-lookup"><span data-stu-id="fa32a-107">Global admin</span></span>
- <span data-ttu-id="fa32a-108">Administrador de conta</span><span class="sxs-lookup"><span data-stu-id="fa32a-108">Account admin</span></span>

<span data-ttu-id="fa32a-109">A localização MPN ID identifica cada localização específica da sua empresa.</span><span class="sxs-lookup"><span data-stu-id="fa32a-109">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="fa32a-110">Utiliza a localização MPN ID para se inscrever em programas de incentivo, para transacionar negócios do Cloud Solution Provider (CSP) e outras transações comerciais.</span><span class="sxs-lookup"><span data-stu-id="fa32a-110">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="fa32a-111">O ID MPN global é utilizado para atividades não transacionais, tais como pedidos de apoio.</span><span class="sxs-lookup"><span data-stu-id="fa32a-111">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-is-a-typical-scenario"></a><span data-ttu-id="fa32a-112">Segue-se um cenário típico:</span><span class="sxs-lookup"><span data-stu-id="fa32a-112">The following is a typical scenario:</span></span>

<span data-ttu-id="fa32a-113">A Contoso tem a sua conta global Partner (PGA) no Reino Unido.</span><span class="sxs-lookup"><span data-stu-id="fa32a-113">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="fa32a-114">Este é o seu negócio legal registrado, e o seu ID MPN global é usado para gerir todos os negócios não transacionais.</span><span class="sxs-lookup"><span data-stu-id="fa32a-114">This is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="fa32a-115">A Contoso também tem contas de localização partner (PLA) equivalentes a subsidiárias ou divisões em outro local no Reino Unido, França e EUA.</span><span class="sxs-lookup"><span data-stu-id="fa32a-115">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="fa32a-116">Na estrutura da Conta MPN, estas PLAs são representadas como IDs MPN de localização única.</span><span class="sxs-lookup"><span data-stu-id="fa32a-116">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="fa32a-117">As PLAs são utilizadas para negócios transacionais, como CSP ou programas de incentivos.</span><span class="sxs-lookup"><span data-stu-id="fa32a-117">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="fa32a-118">Os pagamentos estão ligados a locais específicos.</span><span class="sxs-lookup"><span data-stu-id="fa32a-118">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="fa32a-119">Há uma relação 1-1 entre um inquilino da CSP e uma identificação de localização MPN.</span><span class="sxs-lookup"><span data-stu-id="fa32a-119">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="Estrutura das localizações da MPN":::

## <a name="prerequisites-in-order-to-add-a-new-location-for-a-csp-business"></a><span data-ttu-id="fa32a-121">Pré-requisitos para adicionar um novo local para uma empresa de CSP</span><span class="sxs-lookup"><span data-stu-id="fa32a-121">Prerequisites in order to add a new location for a CSP business</span></span>

<span data-ttu-id="fa32a-122">Para adicionar uma nova localização comercial da CSP, existem vários pré-requisitos:</span><span class="sxs-lookup"><span data-stu-id="fa32a-122">To add a new CSP business location, there are several prerequisites:</span></span>

1. <span data-ttu-id="fa32a-123">Você deve ter uma identificação mpn de localização no país onde você quer fazer negócios.</span><span class="sxs-lookup"><span data-stu-id="fa32a-123">You must have a location MPN ID in the country where you want to do business.</span></span>

1. <span data-ttu-id="fa32a-124">Precisa de um novo inquilino da AZure AD na [região de negócios](regional-authorization-overview.md) que ainda não esteja inscrito na CSP.</span><span class="sxs-lookup"><span data-stu-id="fa32a-124">You need a new Azure AD tenant in the [region of business](regional-authorization-overview.md) which is not already enrolled into CSP.</span></span> <span data-ttu-id="fa32a-125">Crie isto quando se inscrever na CSP.</span><span class="sxs-lookup"><span data-stu-id="fa32a-125">Create this when you enroll in CSP.</span></span>
 
3. <span data-ttu-id="fa32a-126">Use o novo inquilino da AAD para se inscrever no programa CSP na região.</span><span class="sxs-lookup"><span data-stu-id="fa32a-126">Use the new AAD tenant to enroll into CSP program in the region.</span></span>
<span data-ttu-id="fa32a-127">Fornecendo detalhes legais da empresa, incluindo o nome da empresa legal, endereço, detalhes de contato primário.</span><span class="sxs-lookup"><span data-stu-id="fa32a-127">Providing legal company details including the legal company name, address, primary contact details.</span></span> <span data-ttu-id="fa32a-128">Esta conta será submetida a verificação, por isso certifique-se de adicionar informações válidas.</span><span class="sxs-lookup"><span data-stu-id="fa32a-128">This account will undergo verification, so make sure to add valid information.</span></span>

>[!NOTE] 
 ><span data-ttu-id="fa32a-129">Lembre-se de assinar com as **novas** credenciais para o **novo** inquilino da AD AZure.</span><span class="sxs-lookup"><span data-stu-id="fa32a-129">Remember to sign in with the **new** credentials for the **new** Azure AD tenant.</span></span> <span data-ttu-id="fa32a-130">Não use as suas credenciais existentes como Partner Center irá reconhecê-lo como tendo já uma conta.</span><span class="sxs-lookup"><span data-stu-id="fa32a-130">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

4. <span data-ttu-id="fa32a-131">Aceite o Acordo de Parceiro da Microsoft e ative a conta.</span><span class="sxs-lookup"><span data-stu-id="fa32a-131">Accept the Microsoft Partner Agreement and activate the account.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="fa32a-132">Adicione uma localização MPN</span><span class="sxs-lookup"><span data-stu-id="fa32a-132">Add an MPN location</span></span>

1. <span data-ttu-id="fa32a-133">Inscreva-se utilizando a conta MPN no Partner Center .</span><span class="sxs-lookup"><span data-stu-id="fa32a-133">Sign in using the MPN account in Partner Center .</span></span> <span data-ttu-id="fa32a-134">A conta MPN deve ter privilégios de Administração Global ou Administração de Contas.</span><span class="sxs-lookup"><span data-stu-id="fa32a-134">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="fa32a-135">A partir do **ícone Definição,** selecione as **definições do Parceiro** .</span><span class="sxs-lookup"><span data-stu-id="fa32a-135">From the **Setting icon** , select the **Partner settings** .</span></span>

2. <span data-ttu-id="fa32a-136">Selecione **Locais.**</span><span class="sxs-lookup"><span data-stu-id="fa32a-136">Select **Locations.**</span></span>

3. <span data-ttu-id="fa32a-137">**Selecione Adicione uma localização** e insira os detalhes do endereço da localização que pretende adicionar à sua empresa, bem como um contacto primário para a localização.</span><span class="sxs-lookup"><span data-stu-id="fa32a-137">Select **Add a location** , and insert the address details of the location that you want to add to your company as well as a primary contact for the location.</span></span>

> [!NOTE]
> <span data-ttu-id="fa32a-138">Uma vez que uma localização é adicionada no Centro de Parceiros, não pode ser removida.</span><span class="sxs-lookup"><span data-stu-id="fa32a-138">Once a location is added in Partner Center, it cannot be removed.</span></span> <span data-ttu-id="fa32a-139">Verá **MPN** no menu esquerdo do Partner Center se tiver usado o ID MPN correto para iniciar sins.</span><span class="sxs-lookup"><span data-stu-id="fa32a-139">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="change-global-partner-account-location"></a><span data-ttu-id="fa32a-140">Alterar localização da conta de parceiro global</span><span class="sxs-lookup"><span data-stu-id="fa32a-140">Change Global partner account location</span></span>

1. <span data-ttu-id="fa32a-141">Na página **['Localizações',](https://partner.microsoft.com/pcv/accountsettings/locationsprofile)** consulte a lista de locais para garantir que o local que pretende como entidade legal está listado.</span><span class="sxs-lookup"><span data-stu-id="fa32a-141">On the **[Locations](https://partner.microsoft.com/pcv/accountsettings/locationsprofile)** page, check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> <span data-ttu-id="fa32a-142">Se não for, adicione.</span><span class="sxs-lookup"><span data-stu-id="fa32a-142">If it isn't, add it.</span></span>

   :::image type="content" source="images/updatepartnerprofile2.png" alt-text="Screenshot da página de Localizações de Conta do Centro de Parceiros com lista de todas as localizações atuais.":::

2. <span data-ttu-id="fa32a-144">Selecione **o perfil de Parceiro** e, em seguida, selecione Update legal business **profile**</span><span class="sxs-lookup"><span data-stu-id="fa32a-144">Select **Partner profile** and then select **Update legal business profile**</span></span>

   :::image type="content" source="images/updatepartnerprofile1.png" alt-text="Screenshot mostrando informações de perfil do Parceiro de Conta do Centro de Parceiros com opção de Atualização selecionável.":::

3. <span data-ttu-id="fa32a-146">Selecione a região e entidade legal e **envie-a.**</span><span class="sxs-lookup"><span data-stu-id="fa32a-146">Select the region and legal entity and **Submit** it.</span></span>

   :::image type="content" source="images/updatepartnerprofile3.png" alt-text="Screenshot para atualizar o perfil de negócio legal do parceiro mostra listas de drop-down para atualizar o país ou região e a entidade legal.":::

## <a name="next-steps"></a><span data-ttu-id="fa32a-148">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="fa32a-148">Next steps</span></span>

- <span data-ttu-id="fa32a-149">Conheça o [processo de verificação.](verification-responses.md)</span><span class="sxs-lookup"><span data-stu-id="fa32a-149">Learn about the [verification process](verification-responses.md).</span></span>
