---
title: Gerir localizações na sua conta de parceiro
ms.topic: how-to
ms.date: 01/25/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Saiba como adicionar uma nova localização e como a localização MPN ID é usada em programas de incentivo, negócios de CSP, subscrições e outras transações.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 38ea8a451f51d80998643e2a023420ea3efaa6ba
ms.sourcegitcommit: e99882e9b6c9b1a0f7427fb133693b1d977be76b
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/26/2021
ms.locfileid: "98773425"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a><span data-ttu-id="bb4c8-103">Gerencie as localizações da sua conta MPN e adicione uma nova localização</span><span class="sxs-lookup"><span data-stu-id="bb4c8-103">Manage your MPN account locations and add a new location</span></span>


<span data-ttu-id="bb4c8-104">**Funções adequadas**</span><span class="sxs-lookup"><span data-stu-id="bb4c8-104">**Appropriate roles**</span></span>

- <span data-ttu-id="bb4c8-105">Administrador global</span><span class="sxs-lookup"><span data-stu-id="bb4c8-105">Global admin</span></span>
- <span data-ttu-id="bb4c8-106">Administrador de conta</span><span class="sxs-lookup"><span data-stu-id="bb4c8-106">Account admin</span></span>

<span data-ttu-id="bb4c8-107">A localização MPN ID identifica cada localização específica da sua empresa.</span><span class="sxs-lookup"><span data-stu-id="bb4c8-107">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="bb4c8-108">Utiliza a localização MPN ID para se inscrever em programas de incentivo, para transacionar negócios do Cloud Solution Provider (CSP) e outras transações comerciais.</span><span class="sxs-lookup"><span data-stu-id="bb4c8-108">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="bb4c8-109">O ID MPN global é utilizado para atividades não transacionais, tais como pedidos de apoio.</span><span class="sxs-lookup"><span data-stu-id="bb4c8-109">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-is-a-typical-scenario"></a><span data-ttu-id="bb4c8-110">Segue-se um cenário típico:</span><span class="sxs-lookup"><span data-stu-id="bb4c8-110">The following is a typical scenario:</span></span>

<span data-ttu-id="bb4c8-111">A Contoso tem a sua conta global Partner (PGA) no Reino Unido.</span><span class="sxs-lookup"><span data-stu-id="bb4c8-111">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="bb4c8-112">Este é o seu negócio legal registrado, e o seu ID MPN global é usado para gerir todos os negócios não transacionais.</span><span class="sxs-lookup"><span data-stu-id="bb4c8-112">This is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="bb4c8-113">A Contoso também tem contas de localização partner (PLA) equivalentes a subsidiárias ou divisões em outro local no Reino Unido, França e EUA.</span><span class="sxs-lookup"><span data-stu-id="bb4c8-113">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="bb4c8-114">Na estrutura da Conta MPN, estas PLAs são representadas como IDs MPN de localização única.</span><span class="sxs-lookup"><span data-stu-id="bb4c8-114">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="bb4c8-115">As PLAs são utilizadas para negócios transacionais, como CSP ou programas de incentivos.</span><span class="sxs-lookup"><span data-stu-id="bb4c8-115">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="bb4c8-116">Os pagamentos estão ligados a locais específicos.</span><span class="sxs-lookup"><span data-stu-id="bb4c8-116">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="bb4c8-117">Há uma relação 1-1 entre um inquilino da CSP e uma identificação de localização MPN.</span><span class="sxs-lookup"><span data-stu-id="bb4c8-117">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="Estrutura das localizações da MPN":::

## <a name="prerequisites-in-order-to-add-a-new-account-location-for-a-csp-business"></a><span data-ttu-id="bb4c8-119">Pré-requisitos para adicionar uma nova localização de conta para uma empresa de CSP</span><span class="sxs-lookup"><span data-stu-id="bb4c8-119">Prerequisites in order to add a new account location for a CSP business</span></span>

<span data-ttu-id="bb4c8-120">Para adicionar uma nova localização comercial da CSP, existem vários pré-requisitos:</span><span class="sxs-lookup"><span data-stu-id="bb4c8-120">To add a new CSP business location, there are several prerequisites:</span></span>

1. <span data-ttu-id="bb4c8-121">Você deve ter uma identificação mpn de localização no país onde você quer fazer negócios.</span><span class="sxs-lookup"><span data-stu-id="bb4c8-121">You must have a location MPN ID in the country where you want to do business.</span></span>

1. <span data-ttu-id="bb4c8-122">Precisa de um novo inquilino da AZure AD na [região de negócios](regional-authorization-overview.md) que ainda não esteja inscrito na CSP.</span><span class="sxs-lookup"><span data-stu-id="bb4c8-122">You need a new Azure AD tenant in the [region of business](regional-authorization-overview.md) which is not already enrolled into CSP.</span></span> <span data-ttu-id="bb4c8-123">Crie isto quando se inscrever na CSP.</span><span class="sxs-lookup"><span data-stu-id="bb4c8-123">Create this when you enroll in CSP.</span></span>
 
3. <span data-ttu-id="bb4c8-124">Use o novo inquilino da AAD para se inscrever no programa CSP na região.</span><span class="sxs-lookup"><span data-stu-id="bb4c8-124">Use the new AAD tenant to enroll into CSP program in the region.</span></span>
<span data-ttu-id="bb4c8-125">Fornecendo detalhes legais da empresa, incluindo o nome da empresa legal, endereço, detalhes de contato primário.</span><span class="sxs-lookup"><span data-stu-id="bb4c8-125">Providing legal company details including the legal company name, address, primary contact details.</span></span> <span data-ttu-id="bb4c8-126">Esta conta será submetida a verificação, por isso certifique-se de adicionar informações válidas.</span><span class="sxs-lookup"><span data-stu-id="bb4c8-126">This account will undergo verification, so make sure to add valid information.</span></span>

>[!NOTE] 
 ><span data-ttu-id="bb4c8-127">Lembre-se de assinar com as **novas** credenciais para o **novo** inquilino da AD AZure.</span><span class="sxs-lookup"><span data-stu-id="bb4c8-127">Remember to sign in with the **new** credentials for the **new** Azure AD tenant.</span></span> <span data-ttu-id="bb4c8-128">Não use as suas credenciais existentes como Partner Center irá reconhecê-lo como tendo já uma conta.</span><span class="sxs-lookup"><span data-stu-id="bb4c8-128">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

4. <span data-ttu-id="bb4c8-129">Aceite o Acordo de Parceiro da Microsoft e ative a conta.</span><span class="sxs-lookup"><span data-stu-id="bb4c8-129">Accept the Microsoft Partner Agreement and activate the account.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="bb4c8-130">Adicione uma localização MPN</span><span class="sxs-lookup"><span data-stu-id="bb4c8-130">Add an MPN location</span></span>

1. <span data-ttu-id="bb4c8-131">Inscreva-se utilizando a conta MPN no Partner Center .</span><span class="sxs-lookup"><span data-stu-id="bb4c8-131">Sign in using the MPN account in Partner Center .</span></span> <span data-ttu-id="bb4c8-132">A conta MPN deve ter privilégios de Administração Global ou Administração de Contas.</span><span class="sxs-lookup"><span data-stu-id="bb4c8-132">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="bb4c8-133">A partir do **ícone Definição,** selecione as **definições da Organização**.</span><span class="sxs-lookup"><span data-stu-id="bb4c8-133">From the **Setting icon**, select the **Organization settings**.</span></span>

2. <span data-ttu-id="bb4c8-134">Selecione **Legal** e, em seguida, selecione **Localizações.**</span><span class="sxs-lookup"><span data-stu-id="bb4c8-134">Select **Legal** and then select **Locations.**</span></span>

3. <span data-ttu-id="bb4c8-135">**Selecione Adicione uma localização** e insira os detalhes do endereço da localização que pretende adicionar à sua empresa, bem como um contacto primário para a localização.</span><span class="sxs-lookup"><span data-stu-id="bb4c8-135">Select **Add a location**, and insert the address details of the location that you want to add to your company as well as a primary contact for the location.</span></span>

> [!NOTE]
> <span data-ttu-id="bb4c8-136">Uma vez que uma localização é adicionada no Centro de Parceiros, não pode ser removida.</span><span class="sxs-lookup"><span data-stu-id="bb4c8-136">Once a location is added in Partner Center, it cannot be removed.</span></span> <span data-ttu-id="bb4c8-137">Verá **MPN** no menu esquerdo do Partner Center se tiver usado o ID MPN correto para iniciar sins.</span><span class="sxs-lookup"><span data-stu-id="bb4c8-137">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="change-global-partner-account-location"></a><span data-ttu-id="bb4c8-138">Alterar localização da conta de parceiro global</span><span class="sxs-lookup"><span data-stu-id="bb4c8-138">Change Global partner account location</span></span>

1. <span data-ttu-id="bb4c8-139">Nas **[localizações empresariais,](https://partner.microsoft.com/dashboard/account/v3/organization/legalinfo#mpn)** consulte a lista de locais para garantir que a localização desejada como entidade jurídica está listada.</span><span class="sxs-lookup"><span data-stu-id="bb4c8-139">On **[Business locations](https://partner.microsoft.com/dashboard/account/v3/organization/legalinfo#mpn)**, check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> <span data-ttu-id="bb4c8-140">Se não for, adicione.</span><span class="sxs-lookup"><span data-stu-id="bb4c8-140">If it isn't, add it.</span></span>

   :::image type="content" source="images/accountsettings/location1.png" alt-text="Screenshot da página de Localizações de Conta do Centro de Parceiros com lista de todas as localizações atuais.":::

2. <span data-ttu-id="bb4c8-142">Selecione **Legal** e, em seguida, selecione **Update legal business profile**</span><span class="sxs-lookup"><span data-stu-id="bb4c8-142">Select **Legal** and then select **Update legal business profile**</span></span>
  
3. <span data-ttu-id="bb4c8-143">Selecione a região e entidade legal e **envie-a.**</span><span class="sxs-lookup"><span data-stu-id="bb4c8-143">Select the region and legal entity and **Submit** it.</span></span>

  
## <a name="next-steps"></a><span data-ttu-id="bb4c8-144">Próximos passos</span><span class="sxs-lookup"><span data-stu-id="bb4c8-144">Next steps</span></span>

- <span data-ttu-id="bb4c8-145">Conheça o [processo de verificação.](verification-responses.md)</span><span class="sxs-lookup"><span data-stu-id="bb4c8-145">Learn about the [verification process](verification-responses.md).</span></span>
