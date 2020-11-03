---
title: Personalize a experiência fora da caixa de um dispositivo
ms.topic: how-to
ms.date: 04/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Antes de entregar o novo dispositivo de um cliente, pode utilizar perfis do Windows Autopilot para personalizar ou configurar previamente a experiência fora de caixa do dispositivo (OOBE).
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: 0ae61db0ca040afe67faa3a0883ea033b8f67562
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/22/2020
ms.locfileid: "92529839"
---
# <a name="use-windows-autopilot-profiles-on-new-devices-to-customize-a-customers-out-of-box-experience"></a><span data-ttu-id="4b09b-103">Utilizar perfis do Windows Autopilot em novos dispositivos para personalizar a experiência inicial de um cliente</span><span class="sxs-lookup"><span data-stu-id="4b09b-103">Use Windows Autopilot profiles on new devices to customize a customer's out-of-box experience</span></span>

<span data-ttu-id="4b09b-104">**Aplica-se a**</span><span class="sxs-lookup"><span data-stu-id="4b09b-104">**Applies to**</span></span>

- <span data-ttu-id="4b09b-105">Parceiros de conta direta da CSP, fornecedores indiretos e revendedores indiretos</span><span class="sxs-lookup"><span data-stu-id="4b09b-105">CSP direct-bill partners, indirect providers, and indirect resellers</span></span>

<span data-ttu-id="4b09b-106">**Funções adequadas**</span><span class="sxs-lookup"><span data-stu-id="4b09b-106">**Appropriate roles**</span></span>

- <span data-ttu-id="4b09b-107">Agente administrativo</span><span class="sxs-lookup"><span data-stu-id="4b09b-107">Admin agent</span></span>
- <span data-ttu-id="4b09b-108">Administrador global</span><span class="sxs-lookup"><span data-stu-id="4b09b-108">Global admin</span></span>
- <span data-ttu-id="4b09b-109">Agente comercial</span><span class="sxs-lookup"><span data-stu-id="4b09b-109">Sales agent</span></span>
- <span data-ttu-id="4b09b-110">Administração de gestão de utilizadores</span><span class="sxs-lookup"><span data-stu-id="4b09b-110">User management admin</span></span>

<span data-ttu-id="4b09b-111">Se gerir os dispositivos do cliente, poderá ter de personalizar a experiência fora da caixa (OOBE) para os utilizadores do cliente.</span><span class="sxs-lookup"><span data-stu-id="4b09b-111">If you manage customer devices, you may need to customize the out-of-box experience (OOBE) for the customer's users.</span></span> <span data-ttu-id="4b09b-112">Pode configurar novos dispositivos com perfis Do Windows Autopilot antes de entregar os dispositivos aos clientes e aplicar novos perfis aos dispositivos que os clientes já adquiriram.</span><span class="sxs-lookup"><span data-stu-id="4b09b-112">You can pre-configure new devices with Windows Autopilot profiles before delivering the devices to customers and apply new profiles to devices customers have already purchased.</span></span> 

<span data-ttu-id="4b09b-113">Note que os OEMs começaram a incluir uma etiqueta de envio no exterior da caixa do dispositivo Autopilot que mostra o ID da chave de produto do dispositivo **(PKID)** .</span><span class="sxs-lookup"><span data-stu-id="4b09b-113">Note that OEMs have started including a shipping label on the outside of the Autopilot device box that shows the device's **Product Key ID (PKID)** .</span></span>  <span data-ttu-id="4b09b-114">Este código de barras lídimensional e legível proporciona aos parceiros a jusante uma forma de registar dispositivos para o Autopilot sem ter de desboxar o(s) dispositivo(s) e recolher o ID do dispositivo por meios alternativos.</span><span class="sxs-lookup"><span data-stu-id="4b09b-114">This 1-dimensional, readable barcode provides downstream partners with a way to register devices for Autopilot without having to unbox the device(s) and harvest the device ID by alternative means.</span></span>

<span data-ttu-id="4b09b-115">Este artigo explica como criar e aplicar perfis de piloto automático em dispositivos no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="4b09b-115">This article explains how to create and apply Autopilot profiles to devices in Partner Center.</span></span>

<span data-ttu-id="4b09b-116">Se ainda não está familiarizado com o Autopilot, reveja as informações nestes artigos:</span><span class="sxs-lookup"><span data-stu-id="4b09b-116">If you're not already familiar with Autopilot, review the information in these articles:</span></span>

- [<span data-ttu-id="4b09b-117">Visão geral do Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="4b09b-117">Overview of Windows Autopilot</span></span>](/windows/deployment/windows-10-auto-pilot)
- [<span data-ttu-id="4b09b-118">Guia de referência de implantação de piloto automático</span><span class="sxs-lookup"><span data-stu-id="4b09b-118">Autopilot deployment reference guide</span></span>](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a><span data-ttu-id="4b09b-119">Descrição geral</span><span class="sxs-lookup"><span data-stu-id="4b09b-119">Overview</span></span>

<span data-ttu-id="4b09b-120">Com a funcionalidade Piloto Automático do Windows no Partner Center, pode criar perfis personalizados para aplicar aos dispositivos do cliente.</span><span class="sxs-lookup"><span data-stu-id="4b09b-120">With the Windows Autopilot feature in Partner Center, you can create custom profiles to apply to customer devices.</span></span> <span data-ttu-id="4b09b-121">As seguintes definições de perfil estavam disponíveis no momento da publicação deste artigo:</span><span class="sxs-lookup"><span data-stu-id="4b09b-121">The following profile settings were available at the time this article was published:</span></span>

- <span data-ttu-id="4b09b-122">Ignore as definições de privacidade.</span><span class="sxs-lookup"><span data-stu-id="4b09b-122">Skip privacy settings.</span></span> <span data-ttu-id="4b09b-123">Esta definição opcional de perfil autopiloto permite que as organizações não perguntem sobre as definições de privacidade durante o processo OOBE.</span><span class="sxs-lookup"><span data-stu-id="4b09b-123">This optional Autopilot profile setting enables organizations to not ask about privacy settings during the OOBE process.</span></span>

- <span data-ttu-id="4b09b-124">Desative a criação de conta de administração local no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4b09b-124">Disable local admin account creation on the device.</span></span> <span data-ttu-id="4b09b-125">As organizações podem decidir se o utilizador que configura o dispositivo deve ter acesso ao administrador uma vez que o processo esteja concluído.</span><span class="sxs-lookup"><span data-stu-id="4b09b-125">Organizations can decide whether the user setting up the device should have administrator access once the process is complete.</span></span>

- <span data-ttu-id="4b09b-126">Configurar automaticamente o dispositivo para o trabalho ou para a escola.</span><span class="sxs-lookup"><span data-stu-id="4b09b-126">Automatically set up device for work or school.</span></span> <span data-ttu-id="4b09b-127">Todos os dispositivos registados no Autopilot serão automaticamente considerados trabalho ou dispositivos escolares, pelo que esta questão não será feita durante o processo OOBE.</span><span class="sxs-lookup"><span data-stu-id="4b09b-127">All devices registered with Autopilot will automatically be considered work or school devices, so this question will not be asked during the OOBE process.</span></span>

- <span data-ttu-id="4b09b-128">Skip Cortana, OneDrive e páginas de configuração de registo OEM.</span><span class="sxs-lookup"><span data-stu-id="4b09b-128">Skip Cortana, OneDrive, and OEM registration setup pages.</span></span> <span data-ttu-id="4b09b-129">Todos os dispositivos registados no Autopilot saltarão automaticamente estas páginas durante o processo de experiência fora de caixa (OOBE).</span><span class="sxs-lookup"><span data-stu-id="4b09b-129">All devices registered with Autopilot will automatically skip these pages during the out-of-box experience (OOBE) process.</span></span>

- <span data-ttu-id="4b09b-130">Ignore o Contrato de Licença de Utilizador Final (EULA).</span><span class="sxs-lookup"><span data-stu-id="4b09b-130">Skip End User License Agreement (EULA).</span></span> <span data-ttu-id="4b09b-131">A partir da versão 1709 do Windows 10, as organizações podem decidir saltar a página EULA apresentada durante o processo OOBE.</span><span class="sxs-lookup"><span data-stu-id="4b09b-131">Starting in Windows 10 version 1709, organizations can decide to skip the EULA page presented during the OOBE process.</span></span> <span data-ttu-id="4b09b-132">Consulte o [despedimento do Windows Autopilot EULA](#windows-autopilot-eula-dismissal) abaixo para obter informações importantes a considerar sobre saltar a página EULA durante a configuração do Windows.</span><span class="sxs-lookup"><span data-stu-id="4b09b-132">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

<span data-ttu-id="4b09b-133">Aplicam-se as seguintes permissões e limitações de gestão de perfis e dispositivos:</span><span class="sxs-lookup"><span data-stu-id="4b09b-133">The following profile and device management permissions and limitations apply:</span></span>

- <span data-ttu-id="4b09b-134">Os parceiros CSP podem continuar a gerir os perfis do Autopilot de clientes existentes com os quais têm relações de revendedores, mesmo que os clientes tenham removido os privilégios de administração delegada dos parceiros.</span><span class="sxs-lookup"><span data-stu-id="4b09b-134">CSP partners can continue to manage Autopilot profiles for existing customers with whom they have reseller relationships, even if the customers have removed the partner's delegated administration privileges.</span></span>

- <span data-ttu-id="4b09b-135">Pode gerir dispositivos existentes dos clientes que adicionou.</span><span class="sxs-lookup"><span data-stu-id="4b09b-135">You can manage existing devices for your customers that you have added.</span></span>

- <span data-ttu-id="4b09b-136">Não pode gerir dispositivos que o seu cliente carregou para a Microsoft Store para Empresas ou para o Portal do Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="4b09b-136">You can't manage devices your customer has uploaded to Microsoft Store for Business or the Microsoft Intune Portal.</span></span>

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a><span data-ttu-id="4b09b-137">Criar e gerir perfis de piloto automático no Partner Center</span><span class="sxs-lookup"><span data-stu-id="4b09b-137">Create and manage Autopilot profiles in Partner Center</span></span>

<span data-ttu-id="4b09b-138">No Partner Center, pode criar perfis de implementação do Windows Autopilot e aplicá-los em dispositivos.</span><span class="sxs-lookup"><span data-stu-id="4b09b-138">In Partner Center, you can create Windows Autopilot deployment profiles and apply them to devices.</span></span>

>[!NOTE]
><span data-ttu-id="4b09b-139">Só os agentes administrativos podem criar e aplicar perfis.</span><span class="sxs-lookup"><span data-stu-id="4b09b-139">Only admin agents can create and apply profiles.</span></span>

### <a name="create-a-new-autopilot-profile"></a><span data-ttu-id="4b09b-140">Criar um novo perfil de piloto automático</span><span class="sxs-lookup"><span data-stu-id="4b09b-140">Create a new Autopilot profile</span></span>

1. <span data-ttu-id="4b09b-141">Selecione **clientes** do menu Partner Center e, em seguida, selecione o cliente para o qual está a criar o perfil Autopilot.</span><span class="sxs-lookup"><span data-stu-id="4b09b-141">Select **Customers** from the Partner Center menu and then select the customer you're creating the Autopilot profile for.</span></span>

2. <span data-ttu-id="4b09b-142">Na página de pormenor do cliente, selecione **Dispositivos** .</span><span class="sxs-lookup"><span data-stu-id="4b09b-142">On the customer's detail page, select **Devices** .</span></span>

3. <span data-ttu-id="4b09b-143">Nos **perfis do Windows Autopilot** selecione Adicionar novo **perfil** .</span><span class="sxs-lookup"><span data-stu-id="4b09b-143">Under **Windows Autopilot profiles** select **Add new profile** .</span></span>

4. <span data-ttu-id="4b09b-144">Introduza o nome e a descrição do perfil e, em seguida, configufique as definições OOBE.</span><span class="sxs-lookup"><span data-stu-id="4b09b-144">Enter the profile's name and description and then configure the OOBE settings.</span></span> <span data-ttu-id="4b09b-145">Escolha entre:</span><span class="sxs-lookup"><span data-stu-id="4b09b-145">Choose from:</span></span>  

   - <span data-ttu-id="4b09b-146">Salte as definições de privacidade na configuração</span><span class="sxs-lookup"><span data-stu-id="4b09b-146">Skip privacy settings in setup</span></span>

   - <span data-ttu-id="4b09b-147">Desativar a conta de administração local na configuração</span><span class="sxs-lookup"><span data-stu-id="4b09b-147">Disable local admin account in setup</span></span>
  
   - <span data-ttu-id="4b09b-148">Salte automaticamente as páginas na configuração</span><span class="sxs-lookup"><span data-stu-id="4b09b-148">Automatically skip pages in setup</span></span><br>
        <span data-ttu-id="4b09b-149">(Inclui *configuração automaticamente selecionada para o trabalho ou escola* e as páginas de *configuração de registo Skip Cortana, OneDrive e OEM)*</span><span class="sxs-lookup"><span data-stu-id="4b09b-149">(Includes *Automatically select setup for work or school* and *Skip Cortana, OneDrive, and OEM registration setup pages* )</span></span>
  
   - <span data-ttu-id="4b09b-150">Ignorar o contrato de licença de utilizador final (EULA)</span><span class="sxs-lookup"><span data-stu-id="4b09b-150">Skip end user license agreement (EULA)</span></span><br> 
       >[!IMPORTANT] 
       ><span data-ttu-id="4b09b-151">Consulte o [despedimento do Windows Autopilot EULA](#windows-autopilot-eula-dismissal) abaixo para obter informações importantes a considerar sobre saltar a página EULA durante a configuração do Windows.</span><span class="sxs-lookup"><span data-stu-id="4b09b-151">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

5. <span data-ttu-id="4b09b-152">**Selecione Enviar por terminada.**</span><span class="sxs-lookup"><span data-stu-id="4b09b-152">Select **Submit** when finished.</span></span>

### <a name="apply-an-autopilot-profile-to-customer-devices"></a><span data-ttu-id="4b09b-153">Aplicar um perfil autopiloto nos dispositivos do cliente</span><span class="sxs-lookup"><span data-stu-id="4b09b-153">Apply an Autopilot profile to customer devices</span></span>

>[!NOTE]
><span data-ttu-id="4b09b-154">As instruções abaixo assumem que já adicionou os dispositivos do cliente ao Partner Center e que pode aceder à sua lista de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="4b09b-154">The instructions below assume that you've already added the customer's devices to Partner Center and that you can access their device list.</span></span> <span data-ttu-id="4b09b-155">Se ainda não adicionou os dispositivos do cliente, siga as instruções dos [dispositivos Add para a conta de um cliente](#add-devices-to-a-customers-account) e siga os passos abaixo.</span><span class="sxs-lookup"><span data-stu-id="4b09b-155">If you haven't already added the customer's devices, follow the instructions in [Add devices to a customer's account](#add-devices-to-a-customers-account) and then follow the steps below.</span></span>

<span data-ttu-id="4b09b-156">Depois de criar um perfil autopiloto para um cliente, pode aplicá-lo aos dispositivos do cliente.</span><span class="sxs-lookup"><span data-stu-id="4b09b-156">After you create an Autopilot profile for a customer, you can apply it to the customer's devices.</span></span>

1. <span data-ttu-id="4b09b-157">Selecione **clientes** do menu Partner Center e, em seguida, selecione o cliente para o quais criou o perfil Autopilot.</span><span class="sxs-lookup"><span data-stu-id="4b09b-157">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="4b09b-158">Na página de pormenor do cliente, selecione **Dispositivos** .</span><span class="sxs-lookup"><span data-stu-id="4b09b-158">On the customer's detail page, select **Devices** .</span></span>

3. <span data-ttu-id="4b09b-159">Em **Aplicar perfis a dispositivos** selecione os dispositivos ou grupos de dispositivos a que pretende adicionar perfis e, em seguida, selecione Aplicar o **perfil** .</span><span class="sxs-lookup"><span data-stu-id="4b09b-159">Under **Apply profiles to devices** select the devices or device groups you want to add profiles to and then select **Apply profile** .</span></span> <span data-ttu-id="4b09b-160">O perfil que acabou de aplicar aparece na coluna **Profile.**</span><span class="sxs-lookup"><span data-stu-id="4b09b-160">The profile you just applied appears in the **Profile** column.</span></span>

4. <span data-ttu-id="4b09b-161">Siga os passos abaixo para verificar se o perfil será aplicado com sucesso no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4b09b-161">Follow the steps below to verify that the profile will be applied successfully to the device.</span></span>

    <span data-ttu-id="4b09b-162">a.</span><span class="sxs-lookup"><span data-stu-id="4b09b-162">a.</span></span>  <span data-ttu-id="4b09b-163">Ligue um dispositivo à rede e ligue-o.</span><span class="sxs-lookup"><span data-stu-id="4b09b-163">Connect a device to the network and turn it on.</span></span>

    <span data-ttu-id="4b09b-164">b.</span><span class="sxs-lookup"><span data-stu-id="4b09b-164">b.</span></span>  <span data-ttu-id="4b09b-165">Verifique se aparecem os ecrãs OOBE apropriados (se houver).</span><span class="sxs-lookup"><span data-stu-id="4b09b-165">Verify that the appropriate OOBE screens (if any) appear.</span></span>

    <span data-ttu-id="4b09b-166">c.</span><span class="sxs-lookup"><span data-stu-id="4b09b-166">c.</span></span>  <span data-ttu-id="4b09b-167">Quando o processo OOBE parar, reinicie o dispositivo nas definições predefinidos da sua fábrica para o preparar para um novo utilizador.</span><span class="sxs-lookup"><span data-stu-id="4b09b-167">When the OOBE process stops, reset the device to its factory default settings to prepare it for a new user.</span></span>

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a><span data-ttu-id="4b09b-168">Remova um perfil de piloto automático do dispositivo de um cliente</span><span class="sxs-lookup"><span data-stu-id="4b09b-168">Remove an Autopilot profile from a customer's device</span></span>

1. <span data-ttu-id="4b09b-169">Selecione **clientes** do menu Partner Center e, em seguida, selecione o cliente para o quais criou o perfil Autopilot.</span><span class="sxs-lookup"><span data-stu-id="4b09b-169">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="4b09b-170">Na página de pormenor do cliente, selecione **Dispositivos** .</span><span class="sxs-lookup"><span data-stu-id="4b09b-170">On the customer's detail page, select **Devices** .</span></span>

3. <span data-ttu-id="4b09b-171">Em **Aplicar perfis a dispositivos** selecione os dispositivos de onde pretende remover o perfil e, em seguida, selecione Remover o **perfil** .</span><span class="sxs-lookup"><span data-stu-id="4b09b-171">Under **Apply profiles to devices** select the devices you want to remove the profile from and then select **Remove profile** .</span></span>

   >[!NOTE]
   ><span data-ttu-id="4b09b-172">Remover um perfil de um dispositivo não elimina o perfil da sua lista.</span><span class="sxs-lookup"><span data-stu-id="4b09b-172">Removing a profile from a device does not delete the profile from your list.</span></span> <span data-ttu-id="4b09b-173">Se pretender eliminar um perfil, siga as instruções em [Atualizar ou elimine um perfil de Piloto Automático](#update-or-delete-an-autopilot-profile).</span><span class="sxs-lookup"><span data-stu-id="4b09b-173">If you want to delete a profile, follow the instructions in [Update or delete an Autopilot profile](#update-or-delete-an-autopilot-profile).</span></span>

### <a name="update-or-delete-an-autopilot-profile"></a><span data-ttu-id="4b09b-174">Atualizar ou eliminar um perfil de piloto automático</span><span class="sxs-lookup"><span data-stu-id="4b09b-174">Update or delete an Autopilot profile</span></span>

<span data-ttu-id="4b09b-175">Se um cliente quiser alterar a experiência fora da caixa depois de ter enviado os dispositivos para eles, pode alterar o perfil no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="4b09b-175">If a customer wants to change the out-of-box experience after you've shipped the devices to them, you can change the profile in Partner Center.</span></span>

<span data-ttu-id="4b09b-176">Quando o dispositivo do cliente se ligar à internet, irá descarregar a versão de perfil mais recente durante o processo OOBE.</span><span class="sxs-lookup"><span data-stu-id="4b09b-176">When the customer's device connects to the internet, it will download the latest profile version during the OOBE process.</span></span> <span data-ttu-id="4b09b-177">Além disso, sempre que um cliente restaurar um dispositivo nas suas definições padrão de fábrica, o dispositivo irá novamente descarregar a versão de perfil mais recente durante o processo OOBE.</span><span class="sxs-lookup"><span data-stu-id="4b09b-177">Also, any time a customer restores a device to its factory default settings, the device will again download the latest profile version during the OOBE process.</span></span>

1. <span data-ttu-id="4b09b-178">Selecione **clientes** do menu Partner Center e, em seguida, selecione o cliente que quer que você mude um perfil de Piloto Automático.</span><span class="sxs-lookup"><span data-stu-id="4b09b-178">Select **Customers** from the Partner Center menu and then select the customer who wants you to change an Autopilot profile.</span></span>

2. <span data-ttu-id="4b09b-179">Na página de pormenor do cliente, selecione **Dispositivos** .</span><span class="sxs-lookup"><span data-stu-id="4b09b-179">On the customer's detail page, select **Devices** .</span></span>

3. <span data-ttu-id="4b09b-180">Nos **perfis do Windows Autopilot** selecione o perfil necessário para atualizar.</span><span class="sxs-lookup"><span data-stu-id="4b09b-180">Under **Windows Autopilot profiles** select the profile you need to update.</span></span> <span data-ttu-id="4b09b-181">Faça as alterações necessárias e, em seguida, **selecione Enviar por isso.**</span><span class="sxs-lookup"><span data-stu-id="4b09b-181">Make the required changes and then select **Submit** .</span></span>

<span data-ttu-id="4b09b-182">Para eliminar este perfil, **selecione Eliminar** o perfil do canto superior direito da página.</span><span class="sxs-lookup"><span data-stu-id="4b09b-182">To delete this profile, select **Delete profile** from the upper right corner of the page.</span></span>

### <a name="add-devices-to-a-customers-account"></a><span data-ttu-id="4b09b-183">Adicionar dispositivos à conta de um cliente</span><span class="sxs-lookup"><span data-stu-id="4b09b-183">Add devices to a customer's account</span></span>

>[!NOTE]
><span data-ttu-id="4b09b-184">Os agentes de vendas e os agentes administrativos podem adicionar dispositivos à conta de um cliente.</span><span class="sxs-lookup"><span data-stu-id="4b09b-184">Sales agents and admin agents can add devices to a customer's account.</span></span>

<span data-ttu-id="4b09b-185">Antes de poder aplicar perfis autopilotos personalizados aos dispositivos do cliente, tem de conseguir aceder à lista de dispositivos do cliente.</span><span class="sxs-lookup"><span data-stu-id="4b09b-185">Before you can apply custom Autopilot profiles to customer devices, you must be able to access the customer's device list.</span></span>

<span data-ttu-id="4b09b-186">Se pretender utilizar o nome OEM, número de série e combinação de modelos, esteja ciente destas limitações:</span><span class="sxs-lookup"><span data-stu-id="4b09b-186">If you plan to use the OEM name, serial number, and model combination, be aware of these limitations:</span></span>

- <span data-ttu-id="4b09b-187">Este tuple funciona apenas para dispositivos mais recentes (hashes 4k, por exemplo) e não é suportado para hashes de 128b (RS2 e dispositivos anteriores).</span><span class="sxs-lookup"><span data-stu-id="4b09b-187">This tuple works only for newer devices (4k hashes, for example) and is not supported for 128b hashes (RS2 and prior devices).</span></span>

- <span data-ttu-id="4b09b-188">O registo de tuple é sensível a casos, pelo que os dados do ficheiro devem corresponder aos nomes do modelo e do fabricante ***exatamente*** conforme fornecido pelo fornecedor OEM (fornecedor de hardware).</span><span class="sxs-lookup"><span data-stu-id="4b09b-188">The tuple registration is case sensitive, so the data in the file must match the model and manufacturer names ***exactly*** as provided by the OEM provider (hardware provider).</span></span>

<span data-ttu-id="4b09b-189">Siga as instruções abaixo para adicionar dispositivos à conta de um cliente no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="4b09b-189">Follow the instructions below to add devices to a customer's account in Partner Center.</span></span>

1. <span data-ttu-id="4b09b-190">Selecione **clientes** do menu Partner Center e, em seguida, selecione o cliente cujos dispositivos pretende gerir.</span><span class="sxs-lookup"><span data-stu-id="4b09b-190">Select **Customers** from the Partner Center menu and then select the customer whose devices you want to manage.</span></span>

2. <span data-ttu-id="4b09b-191">Na página de pormenor do cliente, selecione **Dispositivos** .</span><span class="sxs-lookup"><span data-stu-id="4b09b-191">On the customer's detail page, select **Devices** .</span></span>

3. <span data-ttu-id="4b09b-192">Em **Aplicar perfis a dispositivos** selecione Adicionar **dispositivos** .</span><span class="sxs-lookup"><span data-stu-id="4b09b-192">Under **Apply profiles to devices** select **Add devices** .</span></span>

4. <span data-ttu-id="4b09b-193">Introduza um nome para a lista de **dispositivos** e, em seguida, selecione Procurar para carregar a lista do cliente (em formato de ficheiro .csv) para o Partner Center.</span><span class="sxs-lookup"><span data-stu-id="4b09b-193">Enter a name for the device list and then select **Browse** to upload the customer's list (in .csv file format) to Partner Center.</span></span>

    >[!NOTE]
    ><span data-ttu-id="4b09b-194">Devia ter recebido este ficheiro .csv com a compra do seu dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4b09b-194">You should have received this .csv file with your device purchase.</span></span> <span data-ttu-id="4b09b-195">Se não recebeu um ficheiro .csv, pode criar um, seguindo os passos na [adição de dispositivos ao Windows Autopilot](/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span><span class="sxs-lookup"><span data-stu-id="4b09b-195">If you didn't receive a .csv file, you can create one yourself by following the steps in [Adding devices to Windows Autopilot](/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span></span>  

5. <span data-ttu-id="4b09b-196">Faça o upload do ficheiro .csv e, em seguida, **selecione Guardar** .</span><span class="sxs-lookup"><span data-stu-id="4b09b-196">Upload the .csv file and then select **Save** .</span></span>

<span data-ttu-id="4b09b-197">Se receber uma mensagem de erro ao tentar carregar o ficheiro .csv, verifique o formato do ficheiro.</span><span class="sxs-lookup"><span data-stu-id="4b09b-197">If you get an error message while trying to upload the .csv file, check the format of the file.</span></span> <span data-ttu-id="4b09b-198">Pode utilizar apenas o hash de hardware ou o nome do OEM, o número de série e o modelo (nessa ordem das colunas) ou o ID do Produto do Windows.</span><span class="sxs-lookup"><span data-stu-id="4b09b-198">You can use the hardware hash only, or the OEM name, serial number, and model (in that column order), or the Windows Product ID.</span></span> <span data-ttu-id="4b09b-199">Também pode utilizar o ficheiro .csv da amostra fornecido a partir do link ao lado dos dispositivos Add para criar uma lista de **dispositivos.**</span><span class="sxs-lookup"><span data-stu-id="4b09b-199">You can also use the sample .csv file provided from the link next to **Add devices** to create a device list.</span></span>

<span data-ttu-id="4b09b-200">O seu ficheiro .csv deve ser parecido com isto:</span><span class="sxs-lookup"><span data-stu-id="4b09b-200">Your .csv file should look something like this:</span></span>

> <span data-ttu-id="4b09b-201">**Número de série do dispositivo,ID do produto do Windows,Hash de Hardware,Nome do fabricante,Modelo de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="4b09b-201">**Device Serial Number,Windows Product ID,Hardware Hash,Manufacturer name,Device model**</span></span>

> <span data-ttu-id="4b09b-202">**{serialNumber},,,Microsoft Corporation,Surface Laptop**</span><span class="sxs-lookup"><span data-stu-id="4b09b-202">**{serialNumber},,,Microsoft Corporation,Surface Laptop**</span></span>

>[!NOTE]
> <span data-ttu-id="4b09b-203">"Nome do fabricante" e "Modelo do Dispositivo" são sensíveis a maiôs.</span><span class="sxs-lookup"><span data-stu-id="4b09b-203">"Manufacturer name" and "Device model" are case-sensitive.</span></span>

<span data-ttu-id="4b09b-204">Se não souber qual o valor a colocar para o nome do Fabricante e modelo de dispositivo, pode executá-lo no dispositivo para recolher os valores corretos:</span><span class="sxs-lookup"><span data-stu-id="4b09b-204">If you don't know what value to put for Manufacturer name and Device Model, you can run this on the device to gather the correct values:</span></span>

<pre><code>md c:\\HWID

Set-Location c:\\HWID

Set-ExecutionPolicy -Scope Process -ExecutionPolicy Unrestricted

Install-Script -Name Get-WindowsAutoPilotInfo

Get-WindowsAutoPilotInfo.ps1 -OutputFile AutoPilotHWID.csv -Partner -Force
</code></pre>

## <a name="windows-autopilot-eula-dismissal"></a><span data-ttu-id="4b09b-205">Despedimento do Windows Autopilot EULA</span><span class="sxs-lookup"><span data-stu-id="4b09b-205">Windows Autopilot EULA dismissal</span></span>

### <a name="important-information"></a><span data-ttu-id="4b09b-206">INFORMAÇÃO IMPORTANTE</span><span class="sxs-lookup"><span data-stu-id="4b09b-206">IMPORTANT INFORMATION</span></span>

<span data-ttu-id="4b09b-207">O Windows Autopilot permite-lhe configurar instalações personalizadas do Windows em dispositivos que gere para os seus clientes.</span><span class="sxs-lookup"><span data-stu-id="4b09b-207">Windows Autopilot allows you to configure customized installations of Windows on devices you manage for your customers.</span></span> <span data-ttu-id="4b09b-208">Se for autorizado a fazê-lo pelo cliente, pode suprimir ou ocultar certos ecrãs de configuração que normalmente são apresentados aos utilizadores ao configurar o Windows, incluindo o ecrã de aceitação do EULA (End User License Agreement).</span><span class="sxs-lookup"><span data-stu-id="4b09b-208">If authorized to do so by the customer, you can suppress or hide certain set-up screens that are normally presented to users when setting up Windows, including the EULA (End User License Agreement) acceptance screen.</span></span>

<span data-ttu-id="4b09b-209">Ao utilizar esta função, concorda que suprimir ou ocultar quaisquer ecrãs concebidos para fornecer aos utilizadores um aviso ou aceitação de termos significa que obteve consentimento e autorização suficientes do seu cliente para ocultar termos, e que, em nome do seu cliente (seja uma organização ou um utilizador individual como o caso pode ser), consentir com quaisquer avisos e aceitar quaisquer termos aplicáveis ao seu cliente.</span><span class="sxs-lookup"><span data-stu-id="4b09b-209">By using this function, you agree that suppressing or hiding any screens that are designed to provide users with notice or acceptance of terms means that you have obtained sufficient consent and authorization from your customer to hide terms, and that you, on behalf of your customer (whether an organization or an individual user as the case may be), consent to any notices and accept any terms that are applicable to your customer.</span></span> <span data-ttu-id="4b09b-210">Isto inclui o acordo com os termos e condições da licença ou aviso que seriam apresentados ao utilizador se não a suprimir ou esconder usando esta ferramenta.</span><span class="sxs-lookup"><span data-stu-id="4b09b-210">This includes agreement to the terms and conditions of the license or notice that would be presented to the user if you did not suppress or hide it using this tool.</span></span> <span data-ttu-id="4b09b-211">O seu cliente não poderá utilizar o software Windows nesses dispositivos se o cliente não tiver adquirido validamente uma licença para o software da Microsoft ou dos seus distribuidores licenciados.</span><span class="sxs-lookup"><span data-stu-id="4b09b-211">Your customer may not use the Windows software on those devices if the customer has not validly acquired a license for the software from Microsoft or its licensed distributors.</span></span>