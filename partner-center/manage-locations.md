---
title: Gerir localizações na sua conta de parceiro
ms.topic: how-to
ms.date: 04/05/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Saiba como adicionar uma nova localização e como a localização MPN ID é usada em programas de incentivo, negócios de CSP, subscrições e outras transações.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 7ca8c866479fbe153c1e0192edd33e8258b9d6e7
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441337"
---
# <a name="manage-your-mpn-account-locations-and-add-delete-a-location"></a><span data-ttu-id="e2f78-103">Gerencie as localizações da sua conta MPN e adicione (excluir) uma localização</span><span class="sxs-lookup"><span data-stu-id="e2f78-103">Manage your MPN account locations and add (delete) a location</span></span>


<span data-ttu-id="e2f78-104">**Funções adequadas**</span><span class="sxs-lookup"><span data-stu-id="e2f78-104">**Appropriate roles**</span></span>

- <span data-ttu-id="e2f78-105">Administrador global</span><span class="sxs-lookup"><span data-stu-id="e2f78-105">Global admin</span></span>
- <span data-ttu-id="e2f78-106">Administrador de conta</span><span class="sxs-lookup"><span data-stu-id="e2f78-106">Account admin</span></span>

<span data-ttu-id="e2f78-107">A localização MPN ID identifica cada localização específica da sua empresa.</span><span class="sxs-lookup"><span data-stu-id="e2f78-107">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="e2f78-108">Utiliza a localização MPN ID para se inscrever em programas de incentivo, para transacionar negócios do Cloud Solution Provider (CSP) e outras transações comerciais.</span><span class="sxs-lookup"><span data-stu-id="e2f78-108">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="e2f78-109">O ID MPN global é utilizado para atividades não transacionais, tais como pedidos de apoio.</span><span class="sxs-lookup"><span data-stu-id="e2f78-109">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-scenario-is-typical"></a><span data-ttu-id="e2f78-110">O seguinte cenário é típico:</span><span class="sxs-lookup"><span data-stu-id="e2f78-110">The following scenario is typical:</span></span>

<span data-ttu-id="e2f78-111">A Contoso tem a sua conta global Partner (PGA) no Reino Unido.</span><span class="sxs-lookup"><span data-stu-id="e2f78-111">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="e2f78-112">A PGA é o seu negócio legal registado, e o seu ID MPN global é usado para gerir todos os negócios não transacionais.</span><span class="sxs-lookup"><span data-stu-id="e2f78-112">The PGA is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="e2f78-113">A Contoso também tem contas de localização partner (PLA) equivalentes a subsidiárias ou divisões em outro local no Reino Unido, França e EUA.</span><span class="sxs-lookup"><span data-stu-id="e2f78-113">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="e2f78-114">Na estrutura da Conta MPN, estas PLAs são representadas como IDs MPN de localização única.</span><span class="sxs-lookup"><span data-stu-id="e2f78-114">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="e2f78-115">As PLAs são utilizadas para negócios transacionais, como CSP ou programas de incentivos.</span><span class="sxs-lookup"><span data-stu-id="e2f78-115">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="e2f78-116">Os pagamentos estão ligados a locais específicos.</span><span class="sxs-lookup"><span data-stu-id="e2f78-116">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="e2f78-117">Há uma relação 1-1 entre um inquilino da CSP e uma identificação de localização MPN.</span><span class="sxs-lookup"><span data-stu-id="e2f78-117">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="Estrutura das localizações da MPN":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a><span data-ttu-id="e2f78-119">Pré-requisitos para adicionar uma nova conta para uma empresa de CSP</span><span class="sxs-lookup"><span data-stu-id="e2f78-119">Prerequisites in order to add a new account for a CSP business</span></span>

<span data-ttu-id="e2f78-120">Para adicionar uma nova conta de negócios da CSP, comece por garantir que cumpriu os pré-requisitos.</span><span class="sxs-lookup"><span data-stu-id="e2f78-120">To add a new CSP business account, start by ensuring that you have fulfilled the prerequisites.</span></span>

1. <span data-ttu-id="e2f78-121">Você deve ter uma identificação MPN de localização no país onde você quer fazer negócios com CSP.</span><span class="sxs-lookup"><span data-stu-id="e2f78-121">You must have a location MPN ID in the country where you want to do CSP business.</span></span> <span data-ttu-id="e2f78-122">Para criar uma nova localização MPN, leia "Adicionar uma localização MPN" abaixo.</span><span class="sxs-lookup"><span data-stu-id="e2f78-122">To create a new MPN location, read “Add an MPN location” below.</span></span>
  
1. <span data-ttu-id="e2f78-123">Para criar uma nova inscrição de Revendedor Indireto CSP, leia [Trabalhar com fornecedores indiretos](indirect-reseller-tasks-in-partner-center.md#get-started)</span><span class="sxs-lookup"><span data-stu-id="e2f78-123">To create a new CSP Indirect Reseller enrollment, read [Work with Indirect providers](indirect-reseller-tasks-in-partner-center.md#get-started)</span></span> 

>[!NOTE] 
 ><span data-ttu-id="e2f78-124">Lembre-se de assinar com as **novas** credenciais para a **nova** conta CSP.</span><span class="sxs-lookup"><span data-stu-id="e2f78-124">Remember to sign in with the **new** credentials for the **new** CSP account.</span></span> <span data-ttu-id="e2f78-125">Não use as suas credenciais existentes como Partner Center irá reconhecê-lo como tendo já uma conta.</span><span class="sxs-lookup"><span data-stu-id="e2f78-125">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

2. <span data-ttu-id="e2f78-126">Aceite o Acordo de Parceiro da Microsoft e ative a conta.</span><span class="sxs-lookup"><span data-stu-id="e2f78-126">Accept the Microsoft Partner Agreement and activate the account.</span></span>

1. <span data-ttu-id="e2f78-127">Se quiser inscrever-se como parceiro direct Bill, leia [requisitos para parceiros direct Bill](direct-partner-new-requirements.md)</span><span class="sxs-lookup"><span data-stu-id="e2f78-127">If you want to enroll as a Direct Bill partner, read [Requirements for Direct Bill partners](direct-partner-new-requirements.md)</span></span>

## <a name="view-your-mpn-locations"></a><span data-ttu-id="e2f78-128">Ver as suas localizações de MPN</span><span class="sxs-lookup"><span data-stu-id="e2f78-128">View your MPN locations</span></span>

1. <span data-ttu-id="e2f78-129">Inscreva-se no painel partner [Center](https://partner.microsoft.com/dashboard/home) com as suas credenciais de conta MPN.</span><span class="sxs-lookup"><span data-stu-id="e2f78-129">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/home) with your MPN account credentials.</span></span> <span data-ttu-id="e2f78-130">(As suas credenciais MPN podem ser diferentes das suas credenciais de CSP)</span><span class="sxs-lookup"><span data-stu-id="e2f78-130">(Your MPN credentials may be different from your CSP credentials)</span></span> 
 
1. <span data-ttu-id="e2f78-131">A partir do ícone **Definições,** selecione **definições de conta**, **perfil de organização,** **Legal**.</span><span class="sxs-lookup"><span data-stu-id="e2f78-131">From the **Settings** icon, select **Account settings**, **Organization profile**, **Legal**.</span></span> 

1. <span data-ttu-id="e2f78-132">No **separador Partner,** verifique se não existe uma mensagem de erro de banner a pedir-lhe para corrigir locais migrados a partir de PMC.</span><span class="sxs-lookup"><span data-stu-id="e2f78-132">On the **Partner** tab, verify that there isn't a banner error message asking you to fix migrated locations from PMC.</span></span>  <span data-ttu-id="e2f78-133">Se as suas localizações não foram configuradas corretamente em PMC, e ainda não transitaram para PC, precisa atualizar essas localizações.</span><span class="sxs-lookup"><span data-stu-id="e2f78-133">If your locations were not set up correctly in PMC, and have not transitioned yet to PC, you need to update those locations.</span></span>

:::image type="content" source="images/locations/location-two.png" alt-text="O Screencap mostra como atualizar a localização.":::
 
4.  <span data-ttu-id="e2f78-135">No ecrã de **localizações do PMC de revisão,** selecione **Update**.</span><span class="sxs-lookup"><span data-stu-id="e2f78-135">On the **Review PMC locations** screen, select **Update**.</span></span>
<span data-ttu-id="e2f78-136">Atualizar os seguintes campos:</span><span class="sxs-lookup"><span data-stu-id="e2f78-136">Update the following fields:</span></span>

- <span data-ttu-id="e2f78-137">**Campo de nomes**: Certifique-se de que o nome da localização da empresa está correto.</span><span class="sxs-lookup"><span data-stu-id="e2f78-137">**Name field**: Make sure that the name of the company location is correct.</span></span> <span data-ttu-id="e2f78-138">Se for apresentado um erro duplicado, tente mudar de, por exemplo, Contoso para Contoso, Inc.</span><span class="sxs-lookup"><span data-stu-id="e2f78-138">If a duplicate error is displayed, try changing from, for example, Contoso to Contoso, Inc.</span></span>

- <span data-ttu-id="e2f78-139">**Área de Entidade Jurídica**: Certifique-se de que escolheu a entidade jurídica a que a localização está ligada</span><span class="sxs-lookup"><span data-stu-id="e2f78-139">**Legal Entity field**: Make sure that you have chosen the legal entity the location is tied to</span></span>

- <span data-ttu-id="e2f78-140">**Linha de endereço 1 & 2 campos**: Certifique-se de que o endereço está correto</span><span class="sxs-lookup"><span data-stu-id="e2f78-140">**Address line 1 & 2 fields**: Make sure that the address is correct</span></span>

- <span data-ttu-id="e2f78-141">**Cidade & campos estado/província**: Certifique-se de que a combinação entre a cidade e o estado/província está correta.</span><span class="sxs-lookup"><span data-stu-id="e2f78-141">**City & State/Province fields**: Make sure the combination between the city and the state/province is correct.</span></span> <span data-ttu-id="e2f78-142">Há países onde será aplicado o menu suspenso para escolher o Estado/Província, e noutros países esse campo terá de ser inserido manualmente.</span><span class="sxs-lookup"><span data-stu-id="e2f78-142">There are countries where the dropdown menu for choosing the State/Province will apply, and in other countries that field will need to manually be inserted.</span></span>

- <span data-ttu-id="e2f78-143">**ZIP/ Código Postal :** Certifique-se de que o campo código postal está a corresponder ao seu País, Região, Cidade ou Endereço indicados.</span><span class="sxs-lookup"><span data-stu-id="e2f78-143">**ZIP/ Postal code field**: Make sure the Zip Code field is matching your indicated Country, Region, City, or Address.</span></span>

- <span data-ttu-id="e2f78-144">**Principais campos de informações de contacto**: Certifique-se de que os campos de primeiro e último nome estão preenchidos e que o endereço de e-mail indicado é um endereço de e-mail de trabalho e não pessoal (por exemplo, @outlook.com , @live.com etc.)</span><span class="sxs-lookup"><span data-stu-id="e2f78-144">**Primary contact information fields**: Make sure the first and last name fields are filled and that the e-mail address indicated is a work e-mail address and not a personal one (for example, @outlook.com, @live.com, etc.)</span></span>

- <span data-ttu-id="e2f78-145">**Campo de números de telefone**: Certifique-se de que o número de telefone NÃO inclui caracteres especiais, espaços ou código de país.</span><span class="sxs-lookup"><span data-stu-id="e2f78-145">**Phone number field**: Make sure that the Phone number does NOT include special characters, spaces, or country code.</span></span> <span data-ttu-id="e2f78-146">O valor introduzido no campo Número de Telefone conterá sempre um máximo de 10 caracteres.</span><span class="sxs-lookup"><span data-stu-id="e2f78-146">The value entered in the Phone Number field will always contain a maximum of 10 characters.</span></span>

5. <span data-ttu-id="e2f78-147">Se não houver uma mensagem de erro, então a partir de  **Definições**, selecione  **Definições** de Conta , **Perfil da Organização,** **Identificadores**.</span><span class="sxs-lookup"><span data-stu-id="e2f78-147">If there isn't an error message, then from  **Settings**, select  **Account Settings**, **Organization profile**, **Identifiers**.</span></span>

6. <span data-ttu-id="e2f78-148">Encontre o ID MPN com o Tipo "Localização" que corresponda ao país desta conta CSP e use-o para completar a associação.</span><span class="sxs-lookup"><span data-stu-id="e2f78-148">Find the MPN ID with Type "Location" that matches the country of this CSP account and use it to complete the association.</span></span>

7. <span data-ttu-id="e2f78-149">Se não conseguir encontrar o ID MPN de localização que corresponda à conta CSP que pretende utilizar, pode adicionar uma nova localização, que irá criar um novo ID MPN.</span><span class="sxs-lookup"><span data-stu-id="e2f78-149">If you can’t find the location MPN ID that matches the CSP account you want to use, you can add a new location, which will create a new MPN ID.</span></span> <span data-ttu-id="e2f78-150">Consulte **a localização mpn** abaixo.</span><span class="sxs-lookup"><span data-stu-id="e2f78-150">See **Add an MPN location** below.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="e2f78-151">Adicione uma localização MPN</span><span class="sxs-lookup"><span data-stu-id="e2f78-151">Add an MPN location</span></span>

1. <span data-ttu-id="e2f78-152">Inscreva-se usando a conta MPN no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="e2f78-152">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="e2f78-153">(As suas credenciais MPN podem ser diferentes das suas credenciais CSP) .</span><span class="sxs-lookup"><span data-stu-id="e2f78-153">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="e2f78-154">A conta MPN deve ter privilégios de Administração Global ou Administração de Contas.</span><span class="sxs-lookup"><span data-stu-id="e2f78-154">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="e2f78-155">A partir do **ícone Definições,** selecione as **definições de Conta** e, em seguida, selecione o perfil da **Organização**.</span><span class="sxs-lookup"><span data-stu-id="e2f78-155">From the **Settings icon**, select the **Account settings** and then select **Organization profile**.</span></span>

2. <span data-ttu-id="e2f78-156">Selecione **Legal** e, em seguida, no separador **Parceiro,** selecione **localizações de Negócios** e clique em **Adicionar uma localização.**</span><span class="sxs-lookup"><span data-stu-id="e2f78-156">Select **Legal** and then, on the **Partner** tab, select **Business locations,** and click on **Add a location.**</span></span>

3. <span data-ttu-id="e2f78-157">Forneça os dados necessários, incluindo o nome comercial, endereço e contato para a localização que pretende adicionar à sua empresa.</span><span class="sxs-lookup"><span data-stu-id="e2f78-157">Provide the required details including business name, address, and contact for the location that you want to add to your company.</span></span>
 
1. <span data-ttu-id="e2f78-158">Clique **em Adicionar localização**.</span><span class="sxs-lookup"><span data-stu-id="e2f78-158">Click **Add location**.</span></span> <span data-ttu-id="e2f78-159">Isto criará um novo ID MPN para o novo local que pode utilizar para transações e incentivos da CSP.</span><span class="sxs-lookup"><span data-stu-id="e2f78-159">This will create a new MPN ID for the new location which you can use for CSP transactions and incentives.</span></span>

:::image type="content" source="images/legal-biz.png" alt-text="Adicione um novo negócio legal":::

> [!NOTE]
> <span data-ttu-id="e2f78-161">Uma vez que uma localização é adicionada no Partner Center, não é possível removê-la.</span><span class="sxs-lookup"><span data-stu-id="e2f78-161">Once a location is added in Partner Center, you cannot remove it.</span></span> <span data-ttu-id="e2f78-162">Verá **MPN** no menu esquerdo do Partner Center se tiver usado o ID MPN correto para iniciar sins.</span><span class="sxs-lookup"><span data-stu-id="e2f78-162">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>


## <a name="delete-a-location"></a><span data-ttu-id="e2f78-163">Excluir uma localização</span><span class="sxs-lookup"><span data-stu-id="e2f78-163">Delete a location</span></span>

<span data-ttu-id="e2f78-164">Para eliminar uma localização da sua conta, terá de contactar o [Partner Support.](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b)</span><span class="sxs-lookup"><span data-stu-id="e2f78-164">To delete a location from your account, you will need to contact [Partner Support](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b).</span></span> <span data-ttu-id="e2f78-165">Certifique-se de que compreende o impacto que esta ação tem.</span><span class="sxs-lookup"><span data-stu-id="e2f78-165">Make sure that you understand the impact this action has.</span></span> <span data-ttu-id="e2f78-166">As localizações eliminadas não podem ser recuperadas e qualquer coisa ligada a esse id MPN específico deixará de ser reconhecida ou ativa para a sua empresa.</span><span class="sxs-lookup"><span data-stu-id="e2f78-166">Deleted locations cannot be retrieved and anything tied to that specific MPN id will no longer be recognized or be active for your company.</span></span>

## <a name="change-country-of-partner-global-account"></a><span data-ttu-id="e2f78-167">Mudar país de conta global partner</span><span class="sxs-lookup"><span data-stu-id="e2f78-167">Change country of Partner global account</span></span> 

1. <span data-ttu-id="e2f78-168">Inscreva-se usando a conta MPN no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="e2f78-168">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="e2f78-169">(As suas credenciais MPN podem ser diferentes das suas credenciais CSP) .</span><span class="sxs-lookup"><span data-stu-id="e2f78-169">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="e2f78-170">A conta MPN deve ter privilégios de Administração Global ou Administração de Contas.</span><span class="sxs-lookup"><span data-stu-id="e2f78-170">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

2. <span data-ttu-id="e2f78-171">No separador **Partner,** vá às localizações do **Negócios** e verifique a lista de locais para garantir que o local que deseja como entidade legal está listado.</span><span class="sxs-lookup"><span data-stu-id="e2f78-171">On the **Partner** tab, go to **Business locations** and check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> 
 
1. <span data-ttu-id="e2f78-172">Para adicionar uma localização, clique em **Adicionar uma localização** e, no voo para fora, forneça os detalhes necessários, incluindo o nome do negócio, endereço e contacto primário para a localização que pretende adicionar à sua empresa.</span><span class="sxs-lookup"><span data-stu-id="e2f78-172">To add a location, click **Add a location**, and, in the fly out, provide the required details including business name, address, and primary contact for the location that you want to add to your company.</span></span> 
 
1. <span data-ttu-id="e2f78-173">Selecione **Mude o seu país** junto ao **país/região** drop-down e siga os passos.</span><span class="sxs-lookup"><span data-stu-id="e2f78-173">Select **Change your country** next to the **Country/region** drop-down and follow the steps.</span></span> 

:::image type="content" source="images/lbp.png" alt-text="Os dados do perfil de negócio legal voam para fora":::

5. <span data-ttu-id="e2f78-175">Clique em **Guardar**.</span><span class="sxs-lookup"><span data-stu-id="e2f78-175">Click **Save**.</span></span>

6. <span data-ttu-id="e2f78-176">O país da conta global da MPN será alterado para o novo país legal.</span><span class="sxs-lookup"><span data-stu-id="e2f78-176">MPN global account country will be changed to the new legal country.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="e2f78-177">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="e2f78-177">Next steps</span></span>

- <span data-ttu-id="e2f78-178">Conheça o [processo de verificação.](verification-responses.md)</span><span class="sxs-lookup"><span data-stu-id="e2f78-178">Learn about the [verification process](verification-responses.md).</span></span>
