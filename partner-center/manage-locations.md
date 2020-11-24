---
title: Gerir localizações na sua conta de parceiro
ms.topic: how-to
ms.date: 11/23/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Saiba como adicionar uma nova localização e como a localização MPN ID é usada em programas de incentivo, negócios de CSP, subscrições e outras transações.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 03c4fb5a4adeb49602fe3736971e140ac6da6f4f
ms.sourcegitcommit: 245b4792e8221468f781f6effd1c9b23be05499a
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/24/2020
ms.locfileid: "95514807"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a><span data-ttu-id="7aab3-103">Gerencie as localizações da sua conta MPN e adicione uma nova localização</span><span class="sxs-lookup"><span data-stu-id="7aab3-103">Manage your MPN account locations and add a new location</span></span>

<span data-ttu-id="7aab3-104">**Aplica-se a**</span><span class="sxs-lookup"><span data-stu-id="7aab3-104">**Applies to**</span></span>

- <span data-ttu-id="7aab3-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="7aab3-105">Partner Center</span></span>

<span data-ttu-id="7aab3-106">**Funções adequadas**</span><span class="sxs-lookup"><span data-stu-id="7aab3-106">**Appropriate roles**</span></span>

- <span data-ttu-id="7aab3-107">Administrador global</span><span class="sxs-lookup"><span data-stu-id="7aab3-107">Global admin</span></span>
- <span data-ttu-id="7aab3-108">Administrador de conta</span><span class="sxs-lookup"><span data-stu-id="7aab3-108">Account admin</span></span>

<span data-ttu-id="7aab3-109">A localização MPN ID identifica cada localização específica da sua empresa.</span><span class="sxs-lookup"><span data-stu-id="7aab3-109">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="7aab3-110">Utiliza a localização MPN ID para se inscrever em programas de incentivo, para transacionar negócios do Cloud Solution Provider (CSP) e outras transações comerciais.</span><span class="sxs-lookup"><span data-stu-id="7aab3-110">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="7aab3-111">O ID MPN global é utilizado para atividades não transacionais, tais como pedidos de apoio.</span><span class="sxs-lookup"><span data-stu-id="7aab3-111">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-is-a-typical-scenario"></a><span data-ttu-id="7aab3-112">Segue-se um cenário típico:</span><span class="sxs-lookup"><span data-stu-id="7aab3-112">The following is a typical scenario:</span></span>

<span data-ttu-id="7aab3-113">A Contoso tem a sua conta global Partner (PGA) no Reino Unido.</span><span class="sxs-lookup"><span data-stu-id="7aab3-113">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="7aab3-114">Este é o seu negócio legal registrado, e o seu ID MPN global é usado para gerir todos os negócios não transacionais.</span><span class="sxs-lookup"><span data-stu-id="7aab3-114">This is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="7aab3-115">A Contoso também tem contas de localização partner (PLA) equivalentes a subsidiárias ou divisões em outro local no Reino Unido, França e EUA.</span><span class="sxs-lookup"><span data-stu-id="7aab3-115">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="7aab3-116">Na estrutura da Conta MPN, estas PLAs são representadas como IDs MPN de localização única.</span><span class="sxs-lookup"><span data-stu-id="7aab3-116">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="7aab3-117">As PLAs são utilizadas para negócios transacionais, como CSP ou programas de incentivos.</span><span class="sxs-lookup"><span data-stu-id="7aab3-117">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="7aab3-118">Os pagamentos estão ligados a locais específicos.</span><span class="sxs-lookup"><span data-stu-id="7aab3-118">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="7aab3-119">Há uma relação 1-1 entre um inquilino da CSP e uma identificação de localização MPN.</span><span class="sxs-lookup"><span data-stu-id="7aab3-119">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="Estrutura das localizações da MPN":::

## <a name="prerequisites-in-order-to-add-a-new-location-for-a-csp-business"></a><span data-ttu-id="7aab3-121">Pré-requisitos para adicionar um novo local para uma empresa de CSP</span><span class="sxs-lookup"><span data-stu-id="7aab3-121">Prerequisites in order to add a new location for a CSP business</span></span>

<span data-ttu-id="7aab3-122">Para adicionar uma nova localização comercial da CSP, existem vários pré-requisitos:</span><span class="sxs-lookup"><span data-stu-id="7aab3-122">To add a new CSP business location, there are several prerequisites:</span></span>

1. <span data-ttu-id="7aab3-123">Você deve ter uma identificação mpn de localização no país onde você quer fazer negócios.</span><span class="sxs-lookup"><span data-stu-id="7aab3-123">You must have a location MPN ID in the country where you want to do business.</span></span>

1. <span data-ttu-id="7aab3-124">Precisa de um novo inquilino da AZure AD na [região de negócios](regional-authorization-overview.md) que ainda não esteja inscrito na CSP.</span><span class="sxs-lookup"><span data-stu-id="7aab3-124">You need a new Azure AD tenant in the [region of business](regional-authorization-overview.md) which is not already enrolled into CSP.</span></span> <span data-ttu-id="7aab3-125">Crie isto quando se inscrever na CSP.</span><span class="sxs-lookup"><span data-stu-id="7aab3-125">Create this when you enroll in CSP.</span></span>
 
3. <span data-ttu-id="7aab3-126">Use o novo inquilino da AAD para se inscrever no programa CSP na região.</span><span class="sxs-lookup"><span data-stu-id="7aab3-126">Use the new AAD tenant to enroll into CSP program in the region.</span></span>
<span data-ttu-id="7aab3-127">Fornecendo detalhes legais da empresa, incluindo o nome da empresa legal, endereço, detalhes de contato primário.</span><span class="sxs-lookup"><span data-stu-id="7aab3-127">Providing legal company details including the legal company name, address, primary contact details.</span></span> <span data-ttu-id="7aab3-128">Esta conta será submetida a verificação, por isso certifique-se de adicionar informações válidas.</span><span class="sxs-lookup"><span data-stu-id="7aab3-128">This account will undergo verification, so make sure to add valid information.</span></span>

>[!NOTE] 
 ><span data-ttu-id="7aab3-129">Lembre-se de assinar com as **novas** credenciais para o **novo** inquilino da AD AZure.</span><span class="sxs-lookup"><span data-stu-id="7aab3-129">Remember to sign in with the **new** credentials for the **new** Azure AD tenant.</span></span> <span data-ttu-id="7aab3-130">Não use as suas credenciais existentes como Partner Center irá reconhecê-lo como tendo já uma conta.</span><span class="sxs-lookup"><span data-stu-id="7aab3-130">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

4. <span data-ttu-id="7aab3-131">Aceite o Acordo de Parceiro da Microsoft e ative a conta.</span><span class="sxs-lookup"><span data-stu-id="7aab3-131">Accept the Microsoft Partner Agreement and activate the account.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="7aab3-132">Adicione uma localização MPN</span><span class="sxs-lookup"><span data-stu-id="7aab3-132">Add an MPN location</span></span>

1. <span data-ttu-id="7aab3-133">Inscreva-se utilizando a conta MPN no Partner Center .</span><span class="sxs-lookup"><span data-stu-id="7aab3-133">Sign in using the MPN account in Partner Center .</span></span> <span data-ttu-id="7aab3-134">A conta MPN deve ter privilégios de Administração Global ou Administração de Contas.</span><span class="sxs-lookup"><span data-stu-id="7aab3-134">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="7aab3-135">A partir do **ícone Definição,** selecione as **definições da Organização**.</span><span class="sxs-lookup"><span data-stu-id="7aab3-135">From the **Setting icon**, select the **Organization settings**.</span></span>

2. <span data-ttu-id="7aab3-136">Selecione **Legal** e, em seguida, selecione **Localizações.**</span><span class="sxs-lookup"><span data-stu-id="7aab3-136">Select **Legal** and then select **Locations.**</span></span>

3. <span data-ttu-id="7aab3-137">**Selecione Adicione uma localização** e insira os detalhes do endereço da localização que pretende adicionar à sua empresa, bem como um contacto primário para a localização.</span><span class="sxs-lookup"><span data-stu-id="7aab3-137">Select **Add a location**, and insert the address details of the location that you want to add to your company as well as a primary contact for the location.</span></span>

> [!NOTE]
> <span data-ttu-id="7aab3-138">Uma vez que uma localização é adicionada no Centro de Parceiros, não pode ser removida.</span><span class="sxs-lookup"><span data-stu-id="7aab3-138">Once a location is added in Partner Center, it cannot be removed.</span></span> <span data-ttu-id="7aab3-139">Verá **MPN** no menu esquerdo do Partner Center se tiver usado o ID MPN correto para iniciar sins.</span><span class="sxs-lookup"><span data-stu-id="7aab3-139">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="change-global-partner-account-location"></a><span data-ttu-id="7aab3-140">Alterar localização da conta de parceiro global</span><span class="sxs-lookup"><span data-stu-id="7aab3-140">Change Global partner account location</span></span>

1. <span data-ttu-id="7aab3-141">Nas **[localizações empresariais,](https://partner.microsoft.com/dashboard/account/v3/organization/legalinfo#mpn)** consulte a lista de locais para garantir que a localização desejada como entidade jurídica está listada.</span><span class="sxs-lookup"><span data-stu-id="7aab3-141">On **[Business locations](https://partner.microsoft.com/dashboard/account/v3/organization/legalinfo#mpn)**, check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> <span data-ttu-id="7aab3-142">Se não for, adicione.</span><span class="sxs-lookup"><span data-stu-id="7aab3-142">If it isn't, add it.</span></span>

   :::image type="content" source="images/accountsettings/location1.png" alt-text="Screenshot da página de Localizações de Conta do Centro de Parceiros com lista de todas as localizações atuais.":::

2. <span data-ttu-id="7aab3-144">Selecione **Legal** e, em seguida, selecione **Update legal business profile**</span><span class="sxs-lookup"><span data-stu-id="7aab3-144">Select **Legal** and then select **Update legal business profile**</span></span>
  
3. <span data-ttu-id="7aab3-145">Selecione a região e entidade legal e **envie-a.**</span><span class="sxs-lookup"><span data-stu-id="7aab3-145">Select the region and legal entity and **Submit** it.</span></span>

  
## <a name="next-steps"></a><span data-ttu-id="7aab3-146">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="7aab3-146">Next steps</span></span>

- <span data-ttu-id="7aab3-147">Conheça o [processo de verificação.](verification-responses.md)</span><span class="sxs-lookup"><span data-stu-id="7aab3-147">Learn about the [verification process](verification-responses.md).</span></span>
