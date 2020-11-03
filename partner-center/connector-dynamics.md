---
title: O conector de co-venda para Dynamics 365 CRM Partner Center
ms.topic: how-to
ms.date: 05/27/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Sincronizar as suas referências no Partner Center com o seu conector de co-venda para Dynamics 365 CRM. Os vendedores podem então co-vender com a Microsoft a partir dos seus sistemas CRM.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 8ea803e675ce7c2d21d680491bbdaedf792e631f
ms.sourcegitcommit: a8adb5f044f06bd684a5b7a06c8efe9f8b03d2db
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/14/2020
ms.locfileid: "92530314"
---
# <a name="co-sell-connector-for-dynamics-365-crm--overview"></a><span data-ttu-id="818a2-104">Conector de co-venda para Dynamics 365 CRM – Visão geral</span><span class="sxs-lookup"><span data-stu-id="818a2-104">Co-sell connector for Dynamics 365 CRM – Overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="818a2-105">Funções adequadas</span><span class="sxs-lookup"><span data-stu-id="818a2-105">Appropriate roles</span></span>

- <span data-ttu-id="818a2-106">Administração de referências</span><span class="sxs-lookup"><span data-stu-id="818a2-106">Referrals admin</span></span>
- <span data-ttu-id="818a2-107">Administrador de sistema ou personalizador de sistema no CRM</span><span class="sxs-lookup"><span data-stu-id="818a2-107">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="818a2-108">O conector partner Center co-sell permite que os seus vendedores co-vendam com a Microsoft a partir dos seus sistemas CRM.</span><span class="sxs-lookup"><span data-stu-id="818a2-108">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="818a2-109">Não terão de ser treinados para usar o Partner Center para gerir os negócios de co-venda.</span><span class="sxs-lookup"><span data-stu-id="818a2-109">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="818a2-110">Utilize os conectores Co-sell, para criar uma nova referência co-venda para contratar um vendedor da Microsoft, receber referências do vendedor da Microsoft, aceitar/recusar referências, modificar dados de negócio como valor de negócio e data de encerramento.</span><span class="sxs-lookup"><span data-stu-id="818a2-110">Use the Co-sell connectors, to create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span> <span data-ttu-id="818a2-111">Também pode receber quaisquer atualizações dos vendedores da Microsoft nestas ofertas de Co-venda.</span><span class="sxs-lookup"><span data-stu-id="818a2-111">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="818a2-112">Pode fazer todas as suas referências dentro do CRM à sua escolha e não no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="818a2-112">You can do all of your referrals work within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="818a2-113">A solução baseia-se na Solução de Automatização de Energia da Microsoft e utiliza APIs do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="818a2-113">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="818a2-114">Antes de instalar - pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="818a2-114">Before you install - pre-requisites</span></span>

|<span data-ttu-id="818a2-115">**Tópicos**</span><span class="sxs-lookup"><span data-stu-id="818a2-115">**Topics**</span></span>   |<span data-ttu-id="818a2-116">**Detalhes**</span><span class="sxs-lookup"><span data-stu-id="818a2-116">**Details**</span></span>   |<span data-ttu-id="818a2-117">**Ligações**</span><span class="sxs-lookup"><span data-stu-id="818a2-117">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="818a2-118">ID da rede de parceiros da Microsoft</span><span class="sxs-lookup"><span data-stu-id="818a2-118">Microsoft Partner Network ID</span></span> |<span data-ttu-id="818a2-119">Precisa de um ID MPN válido</span><span class="sxs-lookup"><span data-stu-id="818a2-119">You need a valid MPN ID</span></span>|<span data-ttu-id="818a2-120">Para se juntar à [MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="818a2-120">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="818a2-121">Cosell pronto</span><span class="sxs-lookup"><span data-stu-id="818a2-121">Cosell ready</span></span>|<span data-ttu-id="818a2-122">A sua solução IP/Serviços tem de ser co-vendida.</span><span class="sxs-lookup"><span data-stu-id="818a2-122">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="818a2-123">Venda com a Microsoft</span><span class="sxs-lookup"><span data-stu-id="818a2-123">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="818a2-124">Conta do Centro de Parceiros</span><span class="sxs-lookup"><span data-stu-id="818a2-124">Partner Center account</span></span>|<span data-ttu-id="818a2-125">O ID MPN associado ao inquilino do Centro De Parceiros deve ser o mesmo que o ID MPN associado à sua solução de Co-venda.</span><span class="sxs-lookup"><span data-stu-id="818a2-125">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="818a2-126">Verifique se consegue ver as suas referências de co-venda no portal Partner Center antes de implantar os conectores.</span><span class="sxs-lookup"><span data-stu-id="818a2-126">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="818a2-127">Gerir a sua conta</span><span class="sxs-lookup"><span data-stu-id="818a2-127">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="818a2-128">Funções de utilizador do Partner Center</span><span class="sxs-lookup"><span data-stu-id="818a2-128">Partner Center user roles</span></span>|<span data-ttu-id="818a2-129">O empregado que vai instalar e usar os conectores deve ser um administrador de referências</span><span class="sxs-lookup"><span data-stu-id="818a2-129">The employee who will install and use the connectors must be a Referrals admin</span></span>|<span data-ttu-id="818a2-130">[Assign users roles and permissions](create-user-accounts-and-set-permissions.md) (Atribuir funções e permissões de utilizador)</span><span class="sxs-lookup"><span data-stu-id="818a2-130">[Assign users roles and permissions](create-user-accounts-and-set-permissions.md)</span></span>| |<span data-ttu-id="818a2-131">Dinâmica 365 CRM</span><span class="sxs-lookup"><span data-stu-id="818a2-131">Dynamics 365 CRM</span></span>|<span data-ttu-id="818a2-132">A função de utilizador crm é administrador do sistema ou personalizador do sistema</span><span class="sxs-lookup"><span data-stu-id="818a2-132">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="818a2-133">Atribuir funções na Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="818a2-133">Assign roles in Dynamics 365</span></span>](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="818a2-134">Conta de fluxo de automatização de energia</span><span class="sxs-lookup"><span data-stu-id="818a2-134">Power Automate Flow Account</span></span>|<span data-ttu-id="818a2-135">Uma conta ativa [de Automação](https://flow.microsoft.com) de Energia para o administrador do Sistema CRM ou personalizador do sistema.</span><span class="sxs-lookup"><span data-stu-id="818a2-135">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="818a2-136">Este utilizador deve iniciar sustação na [Power Automamate](https://flow.microsoft.com) pelo menos uma vez antes da instalação.</span><span class="sxs-lookup"><span data-stu-id="818a2-136">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a><span data-ttu-id="818a2-137">Instalar Referências do Centro de Parceiros Sincronização para Dinâmica 365 (Solução de Automatização de Potência)</span><span class="sxs-lookup"><span data-stu-id="818a2-137">Install Partner Center Referrals Synchronization for Dynamics 365 (Power Automate Solution)</span></span>

1. <span data-ttu-id="818a2-138">Vá ao [Power Automamate](https://flow.microsoft.com) e selecione **Ambientes** no canto superior direito.</span><span class="sxs-lookup"><span data-stu-id="818a2-138">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="818a2-139">Este passo irá mostrar-lhe as instâncias de CRM disponíveis.</span><span class="sxs-lookup"><span data-stu-id="818a2-139">This step will show you the available CRM instances.</span></span>

2. <span data-ttu-id="818a2-140">Selecione a instância CRM apropriada a partir da queda no canto superior direito.</span><span class="sxs-lookup"><span data-stu-id="818a2-140">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="818a2-141">Selecione **Soluções** na barra de navegação esquerda.</span><span class="sxs-lookup"><span data-stu-id="818a2-141">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="818a2-142">Clique no link **Open AppSource** no menu superior.</span><span class="sxs-lookup"><span data-stu-id="818a2-142">Click on the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Open AppSource":::

5. <span data-ttu-id="818a2-144">Procure por **Conectores de Referências do Centro de Parceiros para Dinâmicas365** no ecrã pop-up.</span><span class="sxs-lookup"><span data-stu-id="818a2-144">Search for **Partner Center Referrals Connectors for Dynamics365** in the pop-up screen.</span></span>  

6. <span data-ttu-id="818a2-145">Clique no botão **Get it now** e, em seguida, **Continue** .</span><span class="sxs-lookup"><span data-stu-id="818a2-145">Click the **Get it now** button and then **Continue** .</span></span>

7. <span data-ttu-id="818a2-146">Isto abre a página onde pode selecionar o ambiente CRM (Dynamics 365) para instalar a aplicação.</span><span class="sxs-lookup"><span data-stu-id="818a2-146">This opens the page where you can select the CRM (Dynamics 365) environment to install application.</span></span>  <span data-ttu-id="818a2-147">Concorde com os termos e condições.</span><span class="sxs-lookup"><span data-stu-id="818a2-147">Agree to terms and conditions.</span></span>

8. <span data-ttu-id="818a2-148">Em seguida, é direcionado para a página **Gerir as suas soluções.**</span><span class="sxs-lookup"><span data-stu-id="818a2-148">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="818a2-149">Navegue para "Partner Center Referrals" utilizando os botões de seta na parte inferior da página.</span><span class="sxs-lookup"><span data-stu-id="818a2-149">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="818a2-150">**A instalação programada** deve aparecer ao lado da solução de referências do Centro parceiro.</span><span class="sxs-lookup"><span data-stu-id="818a2-150">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="818a2-151">A instalação levará 10-15 minutos.</span><span class="sxs-lookup"><span data-stu-id="818a2-151">Installation will take 10-15 minutes.</span></span> 

9. <span data-ttu-id="818a2-152">Assim que a instalação estiver concluída, volte a navegar para [o Power Automamate](https://flow.microsoft.com) e selecione **Soluções** da área de navegação à esquerda.</span><span class="sxs-lookup"><span data-stu-id="818a2-152">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="818a2-153">Note que **a Sincronização de Referências do Centro de Parceiros para a Dinâmica 365** está disponível na lista de Soluções.</span><span class="sxs-lookup"><span data-stu-id="818a2-153">Notice that **Partner Center Referrals Synchronization for Dynamics 365** is available in the Solutions list.</span></span>

10. <span data-ttu-id="818a2-154">Selecione **Partner Center Referencias Synchronization for Dynamics 365** .</span><span class="sxs-lookup"><span data-stu-id="818a2-154">Select **Partner Center Referrals Synchronization for Dynamics 365** .</span></span> <span data-ttu-id="818a2-155">Estão disponíveis os seguintes fluxos e entidades power-automamate:</span><span class="sxs-lookup"><span data-stu-id="818a2-155">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="CRMs disponíveis":::

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="818a2-157">Melhores práticas: teste antes de ir ao vivo</span><span class="sxs-lookup"><span data-stu-id="818a2-157">Best practice: test before you go live</span></span>

<span data-ttu-id="818a2-158">Antes de instalar, configurar e personalizar a solução Power Automamate no ambiente de produção, certifique-se de testar a solução numa fase de CRM de encenação.</span><span class="sxs-lookup"><span data-stu-id="818a2-158">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="818a2-159">Instale a solução Microsoft Power Automate num ambiente de preparação/instância CRM.</span><span class="sxs-lookup"><span data-stu-id="818a2-159">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>
- <span data-ttu-id="818a2-160">Faça uma cópia da solução e execute a sua configuração e faça personalizações de fluxo power-automatizado no ambiente de preparação.</span><span class="sxs-lookup"><span data-stu-id="818a2-160">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>
- <span data-ttu-id="818a2-161">Teste a solução numa fase de encenação/CRM.</span><span class="sxs-lookup"><span data-stu-id="818a2-161">Test the solution on a staging/CRM instance.</span></span> 
- <span data-ttu-id="818a2-162">Quanto ao sucesso, importa como solução gerida para o caso de produção.</span><span class="sxs-lookup"><span data-stu-id="818a2-162">On success, import as managed solution to the production instance.</span></span> 

## <a name="configure-the-solution"></a><span data-ttu-id="818a2-163">Configure a solução</span><span class="sxs-lookup"><span data-stu-id="818a2-163">Configure the solution</span></span>

1. <span data-ttu-id="818a2-164">Depois de ter instalado a solução no seu caso CRM, volte a navegar para [Power Automamate](https://flow.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="818a2-164">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="818a2-165">A partir do **drop-down Do Ambiente** no canto superior direito, selecione a instância CRM onde instalou a solução Power Automamate.</span><span class="sxs-lookup"><span data-stu-id="818a2-165">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>

3. <span data-ttu-id="818a2-166">Terá de criar ligações que associem as três contas de utilizador:</span><span class="sxs-lookup"><span data-stu-id="818a2-166">You'll need to create connections that associate the three user accounts:</span></span>

   - <span data-ttu-id="818a2-167">Utilizador do Partner Center com credenciais de administração de referências</span><span class="sxs-lookup"><span data-stu-id="818a2-167">Partner Center user with referrals admin credentials</span></span>

   - <span data-ttu-id="818a2-168">Eventos do Centro de Parceiros</span><span class="sxs-lookup"><span data-stu-id="818a2-168">Partner Center Events</span></span>

   - <span data-ttu-id="818a2-169">Administração CRM com o Power Automamate flui na solução.</span><span class="sxs-lookup"><span data-stu-id="818a2-169">CRM admin with the Power Automate flows in the solution.</span></span>

      1. <span data-ttu-id="818a2-170">Selecione **Ligações** da barra de navegação esquerda e selecione a solução "Partner Center Referrals" da lista.</span><span class="sxs-lookup"><span data-stu-id="818a2-170">Select **Connections** from the left navigation bar and select the “Partner Center Referrals” solution from the list.</span></span>

      2. <span data-ttu-id="818a2-171">Criar uma ligação clicando **Criar uma ligação** .</span><span class="sxs-lookup"><span data-stu-id="818a2-171">Create a connection by clicking **Create a connection** .</span></span>

         :::image type="content" source="images/cosellconnectors/createconnection.png" alt-text="Criar ligação":::

      3. <span data-ttu-id="818a2-173">Procure **referências ao Centro de Parceiros (pré-visualização)** na barra de pesquisa no canto superior direito.</span><span class="sxs-lookup"><span data-stu-id="818a2-173">Search for **Partner Center Referrals (preview)** in the search bar on the top-right corner.</span></span>

      4. <span data-ttu-id="818a2-174">Crie uma ligação para o utilizador do Centro de Parceiros com o papel de credenciais da administração de referências.</span><span class="sxs-lookup"><span data-stu-id="818a2-174">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

      5. <span data-ttu-id="818a2-175">Em seguida, crie uma ligação Partner Center Events para o seu utilizador Partner Center com as credenciais de administração de referências.</span><span class="sxs-lookup"><span data-stu-id="818a2-175">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

      6. <span data-ttu-id="818a2-176">Criar uma ligação para o Serviço Comum de Dados (ambiente atual) para o utilizador administrador de CRM.</span><span class="sxs-lookup"><span data-stu-id="818a2-176">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>

4. <span data-ttu-id="818a2-177">Para associar os fluxos power automamate com as ligações, edite cada um dos fluxos power automate para ligar ao Common Data Service e às Referências do Centro de Parceiros.</span><span class="sxs-lookup"><span data-stu-id="818a2-177">To associate the Power Automate flows with the connections, edit each of the Power Automate flows to connect to Common Data Service and Partner Center Referrals.</span></span> <span data-ttu-id="818a2-178">Guarde as alterações.</span><span class="sxs-lookup"><span data-stu-id="818a2-178">Save the changes.</span></span>

5. <span data-ttu-id="818a2-179">**Ligue** os fluxos de automatização de energia.</span><span class="sxs-lookup"><span data-stu-id="818a2-179">**Turn on** the Power Automate flows.</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="818a2-180">Utilize APIs webhook para se registar para eventos de mudança de recursos</span><span class="sxs-lookup"><span data-stu-id="818a2-180">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="818a2-181">As APIs do Partner Center Webhook permitem-lhe registar-se para eventos de alteração de recursos.</span><span class="sxs-lookup"><span data-stu-id="818a2-181">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="818a2-182">Estes eventos de alteração são enviados para o seu url como posts HTTP.</span><span class="sxs-lookup"><span data-stu-id="818a2-182">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="818a2-183">Para registar o seu url, selecione **Partner Center Webhook Registr (Insider Preview)** Power Automamate flow.</span><span class="sxs-lookup"><span data-stu-id="818a2-183">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="818a2-184">Adicione ligações para (a.) Utilizador do Partner Center com credenciais de administração de referências (b.) Eventos do Centro de Parceiros, conforme destacado abaixo</span><span class="sxs-lookup"><span data-stu-id="818a2-184">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Acionador":::

3. <span data-ttu-id="818a2-186">Quando fizer estas atualizações, verá</span><span class="sxs-lookup"><span data-stu-id="818a2-186">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhooks":::

4. <span data-ttu-id="818a2-188">Guarde as alterações e selecione **Ligue- se** .</span><span class="sxs-lookup"><span data-stu-id="818a2-188">Save your changes and select **Turn on** .</span></span>

   <span data-ttu-id="818a2-189">Para permitir que os webhooks do Partner Center ouçam as alterações do evento, faça os seguintes passos:</span><span class="sxs-lookup"><span data-stu-id="818a2-189">To enable Partner Center webhooks to listen to event changes, do the following steps:</span></span>

5. <span data-ttu-id="818a2-190">Selecione **Partner Center para Dynamics 365 (Visualização insider)** .</span><span class="sxs-lookup"><span data-stu-id="818a2-190">Select **Partner Center to Dynamics 365 (Insider Preview)** .</span></span>

6. <span data-ttu-id="818a2-191">Selecione o ícone **Editar** e selecione **Quando um pedido HTTP for recebido** .</span><span class="sxs-lookup"><span data-stu-id="818a2-191">Select the **Edit** icon and select **When a HTTP request is received** .</span></span>

7. <span data-ttu-id="818a2-192">Selecione o ícone **Copy** para copiar o URL HTTP POST fornecido.</span><span class="sxs-lookup"><span data-stu-id="818a2-192">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/cosellconnectors/copyurl.png" alt-text="Copiar URL":::

8. <span data-ttu-id="818a2-194">Selecione agora o "Partner Center Webhook Registration (Insider Preview)" Power Automamate flow e selecione **Run** .</span><span class="sxs-lookup"><span data-stu-id="818a2-194">Now select the “Partner Center Webhook Registration (Insider Preview)” Power Automate flow and select **Run** .</span></span>

9. <span data-ttu-id="818a2-195">Certifique-se de que a janela "Run Flow" se abre no painel direito e clique em **Continuar** .</span><span class="sxs-lookup"><span data-stu-id="818a2-195">Ensure that the “Run Flow” window opens on the right-hand pane and click **Continue** .</span></span>

10. <span data-ttu-id="818a2-196">Introduza os seguintes detalhes:</span><span class="sxs-lookup"><span data-stu-id="818a2-196">Enter the following details:</span></span>

    1. <span data-ttu-id="818a2-197">**Http Trigger Endpoint** : URL copiado do passo anterior</span><span class="sxs-lookup"><span data-stu-id="818a2-197">**Http Trigger Endpoint** : URL copied from earlier step</span></span>

    2. <span data-ttu-id="818a2-198">**Eventos para Registar** : "referenciação criada" e "referenciada"</span><span class="sxs-lookup"><span data-stu-id="818a2-198">**Events to Register** : “referral-created” and “referral-updated”</span></span>

    3. <span data-ttu-id="818a2-199">**Substitua os pontos finais do gatilho existentes se estiver presente:** Sim (Isto substitui quaisquer pontos finais existentes.)</span><span class="sxs-lookup"><span data-stu-id="818a2-199">**Overwrite existing trigger endpoints if present** : Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="818a2-200">Selecione **Executar** e, em seguida, selecione **Fazer.**</span><span class="sxs-lookup"><span data-stu-id="818a2-200">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="818a2-201">O webhook pode agora ouvir criar e atualizar eventos.</span><span class="sxs-lookup"><span data-stu-id="818a2-201">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="818a2-202">Personalizar etapas de sincronização</span><span class="sxs-lookup"><span data-stu-id="818a2-202">Customize synchronization steps</span></span>

<span data-ttu-id="818a2-203">Quando as referências de Co-venda são sincronizadas entre o Partner Center e o seu sistema CRM, os campos sincronizados no Partner Center PC estão listados aqui.</span><span class="sxs-lookup"><span data-stu-id="818a2-203">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="818a2-204">Muitas vezes os sistemas de CRM são altamente personalizados.</span><span class="sxs-lookup"><span data-stu-id="818a2-204">Often CRM systems are highly customized.</span></span> <span data-ttu-id="818a2-205">Pode personalizar os fluxos power automamate.</span><span class="sxs-lookup"><span data-stu-id="818a2-205">You can customize the Power Automate flows.</span></span> <span data-ttu-id="818a2-206">Siga o guia de mapeamento de campo e, se necessário, faça as alterações adequadas nos passos dos fluxos power automamate.</span><span class="sxs-lookup"><span data-stu-id="818a2-206">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="818a2-207">Os centros de parceiros da Microsoft para mapeamentos CRM são fornecidos, mas com base no seu ambiente CRM, pode optar por personalizar ainda mais os campos.</span><span class="sxs-lookup"><span data-stu-id="818a2-207">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="818a2-208">Vários passos de cada um dos fluxos power automamate podem ser personalizados com base nas suas necessidades.</span><span class="sxs-lookup"><span data-stu-id="818a2-208">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="818a2-209">Seguem-se exemplos de personalizações disponíveis:</span><span class="sxs-lookup"><span data-stu-id="818a2-209">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="818a2-210">Para personalizar os campos para criar ou atualizar eventos no Centro de Parceiros para sincronização de referência CRM:</span><span class="sxs-lookup"><span data-stu-id="818a2-210">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span> 

    <span data-ttu-id="818a2-211">a.</span><span class="sxs-lookup"><span data-stu-id="818a2-211">a.</span></span> <span data-ttu-id="818a2-212">Selecione Partner Center para Dynamics 365 (Insider Preview) ou Partner Center to Salesforce (Preview Insider).</span><span class="sxs-lookup"><span data-stu-id="818a2-212">Select Partner Center to Dynamics 365 (Insider Preview) or Partner Center to Salesforce (Insider Preview).</span></span>

    <span data-ttu-id="818a2-213">b.</span><span class="sxs-lookup"><span data-stu-id="818a2-213">b.</span></span> <span data-ttu-id="818a2-214">**Selecione Editar** para editar/personalizar o fluxo power automamate.</span><span class="sxs-lookup"><span data-stu-id="818a2-214">Select **Edit** to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="818a2-215">c.</span><span class="sxs-lookup"><span data-stu-id="818a2-215">c.</span></span> <span data-ttu-id="818a2-216">Selecione **(Âmbito) Sincronizar o chumbo ou a oportunidade** .</span><span class="sxs-lookup"><span data-stu-id="818a2-216">Select **(Scope) Synchronize the lead or opportunity** .</span></span>

2. <span data-ttu-id="818a2-217">Para personalizar mapeamentos de campo crm (baseado no guia de mapeamentos de campo) para criar eventos, selecione **Se é nova oportunidade partilhada, então** .</span><span class="sxs-lookup"><span data-stu-id="818a2-217">To customize CRM field mappings (based on field mappings guide) for create events, select **If it’s new Shared opportunity, then** .</span></span> <span data-ttu-id="818a2-218">Selecione o subpass **se sim** e, em seguida, expandir **Criando uma nova oportunidade no CRM** .</span><span class="sxs-lookup"><span data-stu-id="818a2-218">Select the substep **if yes** and then expand **Creating a new opportunity in the CRM** .</span></span> <span data-ttu-id="818a2-219">Pode editar os mapeamentos nesta secção utilizando o Guia de Mapeamento de Campo.</span><span class="sxs-lookup"><span data-stu-id="818a2-219">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

    <span data-ttu-id="818a2-220">d.</span><span class="sxs-lookup"><span data-stu-id="818a2-220">d.</span></span> <span data-ttu-id="818a2-221">Para personalizar mapeamentos de campo de CRM (baseados no guia de mapeamentos de campo) para eventos de atualização, clique no passo "(Âmbito) Sincronizar o chumbo ou oportunidade".</span><span class="sxs-lookup"><span data-stu-id="818a2-221">For customizing CRM field mappings (based on field mappings guide) for update events, click on the step “(Scope) Synchronize the lead or opportunity”.</span></span>

    <span data-ttu-id="818a2-222">e.</span><span class="sxs-lookup"><span data-stu-id="818a2-222">e.</span></span> <span data-ttu-id="818a2-223">Selecione **Se é uma atualização para uma oportunidade, então** .</span><span class="sxs-lookup"><span data-stu-id="818a2-223">Select **If it’s an update to an opportunity, then** .</span></span> <span data-ttu-id="818a2-224">Selecione o subpass **se sim** e, em seguida, expandir Se a diferença entre **os objetos de oportunidade no Partner Center e CRM, então** .</span><span class="sxs-lookup"><span data-stu-id="818a2-224">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then** .</span></span>  

    <span data-ttu-id="818a2-225">f.</span><span class="sxs-lookup"><span data-stu-id="818a2-225">f.</span></span> <span data-ttu-id="818a2-226">Selecione **Se sim** seguido com **a atualização oportunidade existente**</span><span class="sxs-lookup"><span data-stu-id="818a2-226">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="818a2-227">Para personalizar os campos de sincronização de referência de CRM para PC para eventos de atualização:</span><span class="sxs-lookup"><span data-stu-id="818a2-227">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

    <span data-ttu-id="818a2-228">a.</span><span class="sxs-lookup"><span data-stu-id="818a2-228">a.</span></span> <span data-ttu-id="818a2-229">**Selecione Editar** para editar/personalizar o fluxo power automamate.</span><span class="sxs-lookup"><span data-stu-id="818a2-229">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="818a2-230">b.</span><span class="sxs-lookup"><span data-stu-id="818a2-230">b.</span></span> <span data-ttu-id="818a2-231">Selecione **(Âmbito) Sincronizar a oportunidade** .</span><span class="sxs-lookup"><span data-stu-id="818a2-231">Select **(Scope) Synchronize the opportunity** .</span></span>

    <span data-ttu-id="818a2-232">c.</span><span class="sxs-lookup"><span data-stu-id="818a2-232">c.</span></span> <span data-ttu-id="818a2-233">Para personalizar mapeamentos de campo de CRM para eventos de atualização, selecione **Se houver diferença entre os objetos de chumbo no Partner Center e CRM, então** .</span><span class="sxs-lookup"><span data-stu-id="818a2-233">To customize CRM field mappings for update events, select **If there is difference between the lead objects in Partner Center and CRM, then** .</span></span> 

    <span data-ttu-id="818a2-234">d.</span><span class="sxs-lookup"><span data-stu-id="818a2-234">d.</span></span> <span data-ttu-id="818a2-235">Selecione o sub-passo **se sim** e, em seguida, expandir o passo Atualizar uma referência **com dados de oportunidade** .</span><span class="sxs-lookup"><span data-stu-id="818a2-235">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data** .</span></span>

   <span data-ttu-id="818a2-236">Pode editar os mapeamentos nesta secção com base no Guia de Mapeamento de Campo.</span><span class="sxs-lookup"><span data-stu-id="818a2-236">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="818a2-237">Para personalizar os campos de sincronização de referência de CRM para PC para criar eventos?</span><span class="sxs-lookup"><span data-stu-id="818a2-237">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   <span data-ttu-id="818a2-238">a.</span><span class="sxs-lookup"><span data-stu-id="818a2-238">a.</span></span> <span data-ttu-id="818a2-239">**Selecione Editar** para editar/personalizar o fluxo power automamate.</span><span class="sxs-lookup"><span data-stu-id="818a2-239">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   <span data-ttu-id="818a2-240">b.</span><span class="sxs-lookup"><span data-stu-id="818a2-240">b.</span></span> <span data-ttu-id="818a2-241">Selecione **(Âmbito) Referências sincronizadas.**</span><span class="sxs-lookup"><span data-stu-id="818a2-241">Select **(Scope) Synchronizing Referrals.**</span></span>

   <span data-ttu-id="818a2-242">c.</span><span class="sxs-lookup"><span data-stu-id="818a2-242">c.</span></span> <span data-ttu-id="818a2-243">Para personalizar mapeamentos de campo de CRM (baseados no guia de mapeamentos de campo) para criar eventos, **selecione Create Microsoft Referral** .</span><span class="sxs-lookup"><span data-stu-id="818a2-243">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral** .</span></span>

   <span data-ttu-id="818a2-244">Pode editar os mapeamentos nesta secção com base no Guia de Mapeamento de Campo.</span><span class="sxs-lookup"><span data-stu-id="818a2-244">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="818a2-245">Sincronização de co-venda bidis de ponta a ponta</span><span class="sxs-lookup"><span data-stu-id="818a2-245">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="818a2-246">Uma vez instalada, configurada e personalizada a solução Power Automate, pode testar a sincronização de referências de Co-venda entre a Dynamics 365 e o Partner Center.</span><span class="sxs-lookup"><span data-stu-id="818a2-246">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Dynamics 365 and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="818a2-247">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="818a2-247">Pre-requisites</span></span>

<span data-ttu-id="818a2-248">Para sincronizar as referências através do Partner Center e Dynamics 365 CRM, a solução Power Automamate demarca claramente os campos de referência específicos da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="818a2-248">To synchronize the referrals across Partner Center and Dynamics 365 CRM, the Power Automate solution clearly demarcates Microsoft-specific referral fields.</span></span> <span data-ttu-id="818a2-249">Esta identificação dá às suas equipas de vendedor a possibilidade de decidir quais as referências que querem partilhar com a Microsoft para co-venda.</span><span class="sxs-lookup"><span data-stu-id="818a2-249">This identification gives your seller teams  the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="818a2-250">Um conjunto de campos personalizados está disponível como parte da entidade **Opportunity.**</span><span class="sxs-lookup"><span data-stu-id="818a2-250">A set of custom fields is available as part of the **Opportunity** entity.</span></span> <span data-ttu-id="818a2-251">Um utilizador de administração CRM terá de criar uma secção de CRM separada com os campos personalizados **Opportunity.**</span><span class="sxs-lookup"><span data-stu-id="818a2-251">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="818a2-252">Os seguintes campos personalizados devem fazer parte da secção CRM:</span><span class="sxs-lookup"><span data-stu-id="818a2-252">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="818a2-253">**Sincronizar com o Partner Center** : Se sincronizar a oportunidade com o Microsoft Partner Center</span><span class="sxs-lookup"><span data-stu-id="818a2-253">**Sync with Partner Center** : Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="818a2-254">**Identificador** de referência : Um campo de identificação apenas de leitura para referência do Microsoft Partner Center</span><span class="sxs-lookup"><span data-stu-id="818a2-254">**Referral Identifier** : A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="818a2-255">**Link de referência** : Um link apenas de leitura para a referência no Microsoft Partner Center</span><span class="sxs-lookup"><span data-stu-id="818a2-255">**Referral Link** : A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="818a2-256">**Como pode a Microsoft ajudar?** : Ajuda necessária da Microsoft para a referenciação</span><span class="sxs-lookup"><span data-stu-id="818a2-256">**How can Microsoft help?** : Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="818a2-257">**Produtos** : Lista de produtos associados a esta oportunidade</span><span class="sxs-lookup"><span data-stu-id="818a2-257">**Products** : List of products associated with this opportunity</span></span>

- <span data-ttu-id="818a2-258">**Auditoria** : Um rasto de auditoria só de leitura para sincronização com referências do Partner Center</span><span class="sxs-lookup"><span data-stu-id="818a2-258">**Audit** : A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="818a2-259">CENÁRIOS:</span><span class="sxs-lookup"><span data-stu-id="818a2-259">SCENARIOS:</span></span>

1. <span data-ttu-id="818a2-260">Sincronização de encaminhamento quando a referência é criada ou atualizada em CRM e sincronizada no Partner Center:</span><span class="sxs-lookup"><span data-stu-id="818a2-260">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="818a2-261">Inscreva-se no ambiente Dynamics 365 CRM com o utilizador que tenha visibilidade na secção **Oportunidade** do CRM.</span><span class="sxs-lookup"><span data-stu-id="818a2-261">Sign into your Dynamics 365 CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="818a2-262">Certifique-se de que a seguinte secção está presente quando criar uma "Nova Oportunidade" no ambiente Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="818a2-262">Ensure that the following section is present when you create a “New Opportunity” in Dynamics 365 environment</span></span>

      :::image type="content" source="images/cosellconnectors/opportunity.png" alt-text="Secção de Oportunidade de Amostra mostrando informações do Microsoft Partner Center na Dynamics 365.":::

   3. <span data-ttu-id="818a2-264">Para sincronizar esta oportunidade com o Microsoft Partner Center, certifique-se de que define os seguintes campos na vista do cartão:</span><span class="sxs-lookup"><span data-stu-id="818a2-264">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

      - <span data-ttu-id="818a2-265">**Sincronização com o Centro de Parceiros** : Sim</span><span class="sxs-lookup"><span data-stu-id="818a2-265">**Sync with Partner Center** : Yes</span></span>

      - <span data-ttu-id="818a2-266">**Como pode a Microsoft ajudar?** : Selecione a partir do seguinte:</span><span class="sxs-lookup"><span data-stu-id="818a2-266">**How can Microsoft help?** : Select from the following:</span></span>

         :::image type="content" source="images/cosellconnectors/help.png" alt-text="Secção de Oportunidade de Amostra em Dynamics 365 que mostra opções de ajuda do Microsoft Partner Center ao lado de um campo chamado Como pode o Microsoft Help?":::

      - <span data-ttu-id="818a2-268">**Produtos** : IDs de solução do produto</span><span class="sxs-lookup"><span data-stu-id="818a2-268">**Products** : Solution IDs of the product</span></span>

   4. <span data-ttu-id="818a2-269">Uma vez criada a oportunidade na Dynamics 365 com a opção **Sync with Partner Center** definida para **Sim,** aguarde 10 minutos e, em seguida, inscreva-se na sua conta Partner Center.</span><span class="sxs-lookup"><span data-stu-id="818a2-269">Once the opportunity is created in Dynamics 365 with **Sync with Partner Center** option set to **Yes** , wait 10 minutes, and then sign into your Partner Center account.</span></span> <span data-ttu-id="818a2-270">As suas referências serão sincronizadas com a Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="818a2-270">Your referrals will be synchronized with Dynamics 365.</span></span>

   5. <span data-ttu-id="818a2-271">Da mesma forma, para uma oportunidade que teve a opção "Sync with Partner Center" definida como "Sim", se atualizar a oportunidade na Dynamics 365 CRM, as alterações serão sincronizadas na sua conta Partner Center.</span><span class="sxs-lookup"><span data-stu-id="818a2-271">Likewise, for an opportunity that had “Sync with Partner Center” option set to “Yes”, if you update the opportunity in Dynamics 365 CRM, the changes will be synchronized in your Partner Center account.</span></span>

   6. <span data-ttu-id="818a2-272">As oportunidades sincronizadas com sucesso com o Partner Center serão identificadas com ✔icon in Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="818a2-272">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Dynamics 365.</span></span>

2. <span data-ttu-id="818a2-273">Sincronização de referência quando a referência é criada ou atualizada no Microsoft Partner Center e sincronizada no ambiente Dynamics 365:</span><span class="sxs-lookup"><span data-stu-id="818a2-273">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Dynamics 365 environment:</span></span>

   1. <span data-ttu-id="818a2-274">Inscreva-se no painel do Centro de [Parceiros.](https://partner.microsoft.com/dashboard/home)</span><span class="sxs-lookup"><span data-stu-id="818a2-274">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

   2. <span data-ttu-id="818a2-275">Selecione **Referências** no menu à esquerda.</span><span class="sxs-lookup"><span data-stu-id="818a2-275">Select **Referrals** from the left-hand menu.</span></span>

   3. <span data-ttu-id="818a2-276">Crie uma nova referência de Co-venda do Partner Center clicando na opção "New deal".</span><span class="sxs-lookup"><span data-stu-id="818a2-276">Create a new Co-sell referral from Partner Center by clicking “New deal” option.</span></span>

   4. <span data-ttu-id="818a2-277">Inscreva-se no ambiente Dynamics 365 CRM.</span><span class="sxs-lookup"><span data-stu-id="818a2-277">Sign into your Dynamics 365 CRM environment.</span></span>

   5. <span data-ttu-id="818a2-278">Navegue para **oportunidades abertas.**</span><span class="sxs-lookup"><span data-stu-id="818a2-278">Navigate to **Open Opportunities** .</span></span> <span data-ttu-id="818a2-279">A referência criada no Microsoft Partner Center está agora sincronizada na Dynamics 365 CRM.</span><span class="sxs-lookup"><span data-stu-id="818a2-279">The referral created in Microsoft Partner Center is now synchronized in Dynamics 365 CRM.</span></span>

   6. <span data-ttu-id="818a2-280">Quando seleciona uma referência sincronizada, os dados da visualização do cartão são preenchidos.</span><span class="sxs-lookup"><span data-stu-id="818a2-280">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="818a2-281">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="818a2-281">Next steps</span></span>

- [<span data-ttu-id="818a2-282">Gerir oportunidades potenciais</span><span class="sxs-lookup"><span data-stu-id="818a2-282">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="818a2-283">Gerir oportunidades de venda conjunta</span><span class="sxs-lookup"><span data-stu-id="818a2-283">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="818a2-284">Mais sobre a plataforma Microsoft Power Automate?</span><span class="sxs-lookup"><span data-stu-id="818a2-284">More about Microsoft Power Automate platform?</span></span>](/power-automate/)

- [<span data-ttu-id="818a2-285">Webhooks do Partner Center</span><span class="sxs-lookup"><span data-stu-id="818a2-285">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)