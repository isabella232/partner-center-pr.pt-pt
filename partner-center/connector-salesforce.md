---
title: O conector de co-venda para Salesforce CRM Partner Center
ms.topic: how-to
ms.date: 01/06/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Sincronizar as suas referências no Partner Center com o seu Salesforce CRM. Os vendedores podem então co-vender com a Microsoft a partir dos seus sistemas CRM.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 68b8bdf7a88c1ca8d063cf3198fc49bf87552edb
ms.sourcegitcommit: de2ac2eea26426ae8f962d29ab50b68850318ce6
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/07/2021
ms.locfileid: "97960956"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a><span data-ttu-id="61058-104">Conector de co-venda para Salesforce CRM - visão geral</span><span class="sxs-lookup"><span data-stu-id="61058-104">Co-sell connector for Salesforce CRM - overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="61058-105">Funções adequadas</span><span class="sxs-lookup"><span data-stu-id="61058-105">Appropriate roles</span></span>

- <span data-ttu-id="61058-106">Administração de referências</span><span class="sxs-lookup"><span data-stu-id="61058-106">Referrals admin</span></span>
- <span data-ttu-id="61058-107">Administrador de sistema ou personalizador de sistema no CRM</span><span class="sxs-lookup"><span data-stu-id="61058-107">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="61058-108">O conector partner Center co-sell permite que os seus vendedores co-vendam com a Microsoft a partir dos seus sistemas CRM.</span><span class="sxs-lookup"><span data-stu-id="61058-108">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="61058-109">Não terão de ser treinados para usar o Partner Center para gerir os negócios de co-venda.</span><span class="sxs-lookup"><span data-stu-id="61058-109">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="61058-110">Utilizando os conectores Co-sell, pode criar uma nova referência de Co-venda para contratar um vendedor da Microsoft, receber referências do vendedor da Microsoft, aceitar/recusar referências, modificar dados de negócios como o valor do negócio e a data de encerramento.</span><span class="sxs-lookup"><span data-stu-id="61058-110">Using the Co-sell connectors, you can create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span>  <span data-ttu-id="61058-111">Também pode receber quaisquer atualizações dos vendedores da Microsoft nestas ofertas de Co-venda.</span><span class="sxs-lookup"><span data-stu-id="61058-111">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="61058-112">Pode fazer todas as suas referências enquanto trabalha dentro do CRM à sua escolha e não no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="61058-112">You can do all of your referrals work while working within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="61058-113">A solução baseia-se na Solução de Automatização de Energia da Microsoft e utiliza APIs do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="61058-113">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="61058-114">Antes de instalar - pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="61058-114">Before you install - pre-requisites</span></span>

|<span data-ttu-id="61058-115">**Tópicos**</span><span class="sxs-lookup"><span data-stu-id="61058-115">**Topics**</span></span>   |<span data-ttu-id="61058-116">**Detalhes**</span><span class="sxs-lookup"><span data-stu-id="61058-116">**Details**</span></span>   |<span data-ttu-id="61058-117">**Ligações**</span><span class="sxs-lookup"><span data-stu-id="61058-117">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="61058-118">ID da rede de parceiros da Microsoft</span><span class="sxs-lookup"><span data-stu-id="61058-118">Microsoft Partner Network ID</span></span> |<span data-ttu-id="61058-119">Precisa de um ID MPN válido</span><span class="sxs-lookup"><span data-stu-id="61058-119">You need a valid MPN ID</span></span>|<span data-ttu-id="61058-120">Para se juntar à [MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="61058-120">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="61058-121">Co-vender pronto</span><span class="sxs-lookup"><span data-stu-id="61058-121">Co-sell ready</span></span>|<span data-ttu-id="61058-122">A sua solução IP/Serviços tem de ser co-vendida.</span><span class="sxs-lookup"><span data-stu-id="61058-122">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="61058-123">Venda com a Microsoft</span><span class="sxs-lookup"><span data-stu-id="61058-123">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="61058-124">Conta do Centro de Parceiros</span><span class="sxs-lookup"><span data-stu-id="61058-124">Partner Center account</span></span>|<span data-ttu-id="61058-125">O ID MPN associado ao inquilino do Centro De Parceiros deve ser o mesmo que o ID MPN associado à sua solução de Co-venda.</span><span class="sxs-lookup"><span data-stu-id="61058-125">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="61058-126">Verifique se consegue ver as suas referências de co-venda no portal Partner Center antes de implantar os conectores.</span><span class="sxs-lookup"><span data-stu-id="61058-126">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="61058-127">Gerir a sua conta</span><span class="sxs-lookup"><span data-stu-id="61058-127">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="61058-128">Funções de utilizador do Partner Center</span><span class="sxs-lookup"><span data-stu-id="61058-128">Partner Center user roles</span></span>|<span data-ttu-id="61058-129">O empregado que vai instalar e usar os conectores deve ser um administrador de referências</span><span class="sxs-lookup"><span data-stu-id="61058-129">The employee who will install and use the connectors must be a Referrals admin</span></span>|<span data-ttu-id="61058-130">[Assign users roles and permissions](create-user-accounts-and-set-permissions.md) (Atribuir funções e permissões de utilizador)</span><span class="sxs-lookup"><span data-stu-id="61058-130">[Assign users roles and permissions](create-user-accounts-and-set-permissions.md)</span></span>|
|<span data-ttu-id="61058-131">Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="61058-131">Salesforce CRM</span></span>|<span data-ttu-id="61058-132">A função de utilizador crm é administrador do sistema ou personalizador do sistema</span><span class="sxs-lookup"><span data-stu-id="61058-132">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="61058-133">Atribuir funções na Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="61058-133">Assign roles in Salesforce CRM</span></span>](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|<span data-ttu-id="61058-134">Conta de fluxo de automatização de energia</span><span class="sxs-lookup"><span data-stu-id="61058-134">Power Automate Flow Account</span></span>|<span data-ttu-id="61058-135">Uma conta ativa [de Automação](https://flow.microsoft.com) de Energia para o administrador do Sistema CRM ou personalizador do sistema.</span><span class="sxs-lookup"><span data-stu-id="61058-135">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="61058-136">Este utilizador deve iniciar sustação na [Power Automamate](https://flow.microsoft.com) pelo menos uma vez antes da instalação.</span><span class="sxs-lookup"><span data-stu-id="61058-136">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a><span data-ttu-id="61058-137">Instalação do Pacote Salesforce para Campos Personalizados da Microsoft</span><span class="sxs-lookup"><span data-stu-id="61058-137">Installation of Salesforce Package for Microsoft Custom Fields</span></span> 

<span data-ttu-id="61058-138">Para sincronizar as referências através do Partner Center e da Salesforce CRM, a solução Power Automamate precisa de identificar claramente os campos de referência específicos da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="61058-138">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly identify Microsoft specific referral fields.</span></span> <span data-ttu-id="61058-139">Esta demarcação proporciona às equipas de vendedores parceiros a capacidade de decidir quais as referências que querem partilhar com a Microsoft para co-venda.</span><span class="sxs-lookup"><span data-stu-id="61058-139">This demarcation provides partner seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

1. <span data-ttu-id="61058-140">Na Salesforce, ative **notas** e adicione-as à lista de oportunidades relacionadas.</span><span class="sxs-lookup"><span data-stu-id="61058-140">In Salesforce, activate **Notes** and add it to the opportunities related list.</span></span> 
[<span data-ttu-id="61058-141">Referência</span><span class="sxs-lookup"><span data-stu-id="61058-141">Reference</span></span>](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

2. <span data-ttu-id="61058-142">Ativar **as equipas de Oportunidade** seguindo os passos:</span><span class="sxs-lookup"><span data-stu-id="61058-142">Activate **Opportunity teams** by following the steps:</span></span> 
    - <span data-ttu-id="61058-143">Na configuração, utilize a caixa **De localização Rápida** para localizar as Definições da Equipa de Oportunidade.</span><span class="sxs-lookup"><span data-stu-id="61058-143">In Setup, use the **Quick Find** box to locate Opportunity Team Settings.</span></span>
    - <span data-ttu-id="61058-144">Defina as definições conforme necessário.</span><span class="sxs-lookup"><span data-stu-id="61058-144">Define the settings as needed.</span></span>
[<span data-ttu-id="61058-145">Referência</span><span class="sxs-lookup"><span data-stu-id="61058-145">Reference</span></span>](https://help.salesforce.com/articleView?id=teamselling_enabling.htm&type=5]) 

3. <span data-ttu-id="61058-146">No Salesforce, instale campos e objetos personalizados utilizando o instalador de pacotes abaixo.</span><span class="sxs-lookup"><span data-stu-id="61058-146">In Salesforce, install custom fields and objects using package installer below.</span></span>
  
<span data-ttu-id="61058-147">Vá [aqui](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV) para instalar o pacote em qualquer empresa.</span><span class="sxs-lookup"><span data-stu-id="61058-147">Go [here](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV) to install the package into any company.</span></span>


<span data-ttu-id="61058-148">Nota: Se estiver a instalar-se numa caixa de areia, deve substituir a parte inicial do URL por http://test.salesforce.com</span><span class="sxs-lookup"><span data-stu-id="61058-148">Note: If you are installing into a sandbox you must replace the initial portion of the URL with http://test.salesforce.com</span></span>

4. <span data-ttu-id="61058-149">Na Salesforce, adicione as Soluções Microsoft à lista relacionada com a **Oportunidade.**</span><span class="sxs-lookup"><span data-stu-id="61058-149">In Salesforce, add Microsoft Solutions to the **Opportunity** related list.</span></span> <span data-ttu-id="61058-150">Uma vez adicionado, clique no ícone da **chave** inglesa e atualize propriedades</span><span class="sxs-lookup"><span data-stu-id="61058-150">Once added, click on the **wrench** icon and update properties</span></span>

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="61058-151">Melhores Práticas: Teste antes de ir ao vivo</span><span class="sxs-lookup"><span data-stu-id="61058-151">Best Practice: Test before you go live</span></span>

<span data-ttu-id="61058-152">Antes de instalar, configurar e personalizar a solução Power Automamate no ambiente de produção, certifique-se de testar a solução numa fase de CRM de encenação.</span><span class="sxs-lookup"><span data-stu-id="61058-152">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="61058-153">Instale a solução Microsoft Power Automate num ambiente de preparação/instância CRM.</span><span class="sxs-lookup"><span data-stu-id="61058-153">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>

- <span data-ttu-id="61058-154">Faça uma cópia da solução e execute a sua configuração e faça personalizações de fluxo power-automatizado no ambiente de preparação.</span><span class="sxs-lookup"><span data-stu-id="61058-154">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>

- <span data-ttu-id="61058-155">Teste a solução numa fase de encenação/CRM.</span><span class="sxs-lookup"><span data-stu-id="61058-155">Test the solution on a staging/CRM instance.</span></span>

- <span data-ttu-id="61058-156">No que diz respeito ao sucesso, a importação como solução gerida para o caso de produção.</span><span class="sxs-lookup"><span data-stu-id="61058-156">On success, import as a managed solution to the production instance.</span></span>

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a><span data-ttu-id="61058-157">Instalar Referências do Centro de Parceiros Sincronização para Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="61058-157">Install Partner Center Referrals Synchronization for Salesforce CRM</span></span>

1. <span data-ttu-id="61058-158">Vá ao [Power Automamate](https://flow.microsoft.com) e selecione **Ambientes** no canto superior direito.</span><span class="sxs-lookup"><span data-stu-id="61058-158">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="61058-159">Isto irá mostrar-lhe as instâncias de CRM disponíveis.</span><span class="sxs-lookup"><span data-stu-id="61058-159">This will show you the available CRM instances.</span></span>

2. <span data-ttu-id="61058-160">Selecione a instância CRM apropriada a partir da queda no canto superior direito.</span><span class="sxs-lookup"><span data-stu-id="61058-160">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="61058-161">Selecione **Soluções** na barra de navegação esquerda.</span><span class="sxs-lookup"><span data-stu-id="61058-161">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="61058-162">Clique no link **Open AppSource** no menu superior.</span><span class="sxs-lookup"><span data-stu-id="61058-162">Click on the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Open AppSource":::

5. <span data-ttu-id="61058-164">Procure por **Conectores de Referências do Centro de Parceiros para Salesforce** no ecrã pop-up.</span><span class="sxs-lookup"><span data-stu-id="61058-164">Search for **Partner Center Referrals Connectors for Salesforce** in the pop-up screen.</span></span>  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Salesforce":::

6. <span data-ttu-id="61058-166">Clique no botão **Get it now** e, em seguida, **Continue**.</span><span class="sxs-lookup"><span data-stu-id="61058-166">Click the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="61058-167">Isto abre a página onde pode selecionar o ambiente de CRM salesforce para instalar a aplicação.</span><span class="sxs-lookup"><span data-stu-id="61058-167">This opens the page where you can select the Salesforce CRM  environment to install application.</span></span>  <span data-ttu-id="61058-168">Concorde com os termos e condições.</span><span class="sxs-lookup"><span data-stu-id="61058-168">Agree to terms and conditions.</span></span>

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="CRMs disponíveis":::

8. <span data-ttu-id="61058-170">Em seguida, é direcionado para a página **Gerir as suas soluções.**</span><span class="sxs-lookup"><span data-stu-id="61058-170">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="61058-171">Navegue para "Partner Center Referrals" utilizando os botões de seta na parte inferior da página.</span><span class="sxs-lookup"><span data-stu-id="61058-171">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="61058-172">**A instalação programada** deve aparecer ao lado da solução de referências do Centro parceiro.</span><span class="sxs-lookup"><span data-stu-id="61058-172">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="61058-173">A instalação levará 10-15 minutos.</span><span class="sxs-lookup"><span data-stu-id="61058-173">Installation will take 10-15 minutes.</span></span>

9. <span data-ttu-id="61058-174">Assim que a instalação estiver concluída, volte a navegar para [o Power Automamate](https://flow.microsoft.com) e selecione **Soluções** da área de navegação à esquerda.</span><span class="sxs-lookup"><span data-stu-id="61058-174">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="61058-175">Note que **a Sincronização de Referências do Partner Center para a Salesforce** está disponível na lista de Soluções.</span><span class="sxs-lookup"><span data-stu-id="61058-175">Notice that **Partner Center Referrals Synchronization for Salesforce** is available in the Solutions list.</span></span>

10. <span data-ttu-id="61058-176">Selecione **Partner Center Referrals Synchronization for Salesforce**.</span><span class="sxs-lookup"><span data-stu-id="61058-176">Select **Partner Center Referrals Synchronization for Salesforce**.</span></span> <span data-ttu-id="61058-177">Estão disponíveis os seguintes fluxos e entidades power-automamate:</span><span class="sxs-lookup"><span data-stu-id="61058-177">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/salesforce10.png" alt-text="Fluxos de salesforce":::



## <a name="configure-the-solution"></a><span data-ttu-id="61058-179">Configure a solução</span><span class="sxs-lookup"><span data-stu-id="61058-179">Configure the solution</span></span>

1. <span data-ttu-id="61058-180">Depois de ter instalado a solução no seu caso CRM, volte a navegar para [Power Automamate](https://flow.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="61058-180">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="61058-181">A partir do **drop-down Do Ambiente** no canto superior direito, selecione a instância CRM onde instalou a solução Power Automamate.</span><span class="sxs-lookup"><span data-stu-id="61058-181">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>
3. <span data-ttu-id="61058-182">Terá de criar ligações que associem as três contas de utilizador:</span><span class="sxs-lookup"><span data-stu-id="61058-182">You will need to create connections that associate the three user accounts:</span></span>
    - <span data-ttu-id="61058-183">Utilizador do Partner Center com credenciais de administração de referências</span><span class="sxs-lookup"><span data-stu-id="61058-183">Partner Center user with referrals admin credentials</span></span>
    - <span data-ttu-id="61058-184">Eventos do Centro de Parceiros</span><span class="sxs-lookup"><span data-stu-id="61058-184">Partner Center Events</span></span>
    - <span data-ttu-id="61058-185">Administração CRM com o Power Automamate flui na solução.</span><span class="sxs-lookup"><span data-stu-id="61058-185">CRM admin with the Power Automate flows in the solution.</span></span>
4. <span data-ttu-id="61058-186">Selecione **Ligações** da barra de navegação esquerda e selecione a solução "Partner Center Referrals" da lista.</span><span class="sxs-lookup"><span data-stu-id="61058-186">Select **Connections** from the left navigation bar and select the "Partner Center Referrals" solution from the list.</span></span>

5. <span data-ttu-id="61058-187">Criar uma ligação clicando **Criar uma ligação**.</span><span class="sxs-lookup"><span data-stu-id="61058-187">Create a connection by clicking **Create a connection**.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce12.png" alt-text="Criar ligação":::

- <span data-ttu-id="61058-189">Procure referências ao Centro de Parceiros (pré-visualização) na barra de pesquisa no canto superior direito.</span><span class="sxs-lookup"><span data-stu-id="61058-189">Search for Partner Center Referrals (preview) in the search bar on the top right corner.</span></span>

- <span data-ttu-id="61058-190">Crie uma ligação para o utilizador do Centro de Parceiros com o papel de credenciais da administração de referências.</span><span class="sxs-lookup"><span data-stu-id="61058-190">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

-  <span data-ttu-id="61058-191">Em seguida, crie uma ligação Partner Center Events para o seu utilizador Partner Center com as credenciais de administração de referências.</span><span class="sxs-lookup"><span data-stu-id="61058-191">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

- <span data-ttu-id="61058-192">Criar uma ligação para o Salesforce para o utilizador administrador crm.</span><span class="sxs-lookup"><span data-stu-id="61058-192">Create a connection for Salesforce for the CRM administrator user.</span></span>

-  <span data-ttu-id="61058-193">Uma vez adicionadas todas as Ligações, deverá ver as seguintes Ligações no seu ambiente:</span><span class="sxs-lookup"><span data-stu-id="61058-193">Once you have all the Connections added, you should see the following Connections in your environment:</span></span>

 :::image type="content" source="images/cosellconnectors/salesforce13.png" alt-text="Observar ligações":::

### <a name="edit-the-connections"></a><span data-ttu-id="61058-195">Editar as ligações</span><span class="sxs-lookup"><span data-stu-id="61058-195">Edit the connections</span></span>

1. <span data-ttu-id="61058-196">Volte à página Soluções e selecione **Solução Padrão.**</span><span class="sxs-lookup"><span data-stu-id="61058-196">Return to the Solutions page and select **Default Solution**.</span></span>  <span data-ttu-id="61058-197">Selecione **Referência de Ligação (pré-visualização)** clicando **em Tudo**.</span><span class="sxs-lookup"><span data-stu-id="61058-197">Select **Connection Reference (preview)** by clicking **All**.</span></span>
 
:::image type="content" source="images/cosellconnectors/salesforce14.png" alt-text="Iniciar a edição do conector":::

2. <span data-ttu-id="61058-199">Edite cada uma das Ligações uma a uma selecionando o ícone de três pontos.</span><span class="sxs-lookup"><span data-stu-id="61058-199">Edit each of the Connections one by one by selecting the three dots icon.</span></span> <span data-ttu-id="61058-200">Adicione as ligações relevantes.</span><span class="sxs-lookup"><span data-stu-id="61058-200">Add the relevant connections.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="Editar conectores":::

3. <span data-ttu-id="61058-202">Ligue os fluxos na seguinte sequência:</span><span class="sxs-lookup"><span data-stu-id="61058-202">Turn on the flows in the following sequence:</span></span>

- <span data-ttu-id="61058-203">Registo Webhook do Partner Center (Visualização privilegiada)</span><span class="sxs-lookup"><span data-stu-id="61058-203">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="61058-204">Criar Co-venda Referral - Salesforce to Partner Center (Visualização insider)</span><span class="sxs-lookup"><span data-stu-id="61058-204">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="61058-205">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="61058-205">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="61058-206">Centro de Parceiros para Salesforce (Visualização de Insider)</span><span class="sxs-lookup"><span data-stu-id="61058-206">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="61058-207">Salesforce para Partner Center (Visualização insider)</span><span class="sxs-lookup"><span data-stu-id="61058-207">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="61058-208">Oportunidade Salesforce para Partner Center (Visualização insider)</span><span class="sxs-lookup"><span data-stu-id="61058-208">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="61058-209">Salesforce Microsoft Solutions to Partner Center (Visualização insider)</span><span class="sxs-lookup"><span data-stu-id="61058-209">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="61058-210">Utilize APIs webhook para se registar para eventos de mudança de recursos</span><span class="sxs-lookup"><span data-stu-id="61058-210">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="61058-211">As APIs do Partner Center Webhook permitem-lhe registar-se para eventos de alteração de recursos.</span><span class="sxs-lookup"><span data-stu-id="61058-211">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="61058-212">Estes eventos de alteração são enviados para o seu url como posts HTTP.</span><span class="sxs-lookup"><span data-stu-id="61058-212">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="61058-213">Para registar o seu url, selecione **Partner Center Webhook Registr (Insider Preview)** Power Automamate flow.</span><span class="sxs-lookup"><span data-stu-id="61058-213">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="61058-214">Adicione ligações para (a.) Utilizador do Partner Center com credenciais de administração de referências (b.) Eventos do Centro de Parceiros, conforme destacado abaixo</span><span class="sxs-lookup"><span data-stu-id="61058-214">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Acionador":::

3. <span data-ttu-id="61058-216">Quando fizer estas atualizações, verá</span><span class="sxs-lookup"><span data-stu-id="61058-216">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhooks":::

4. <span data-ttu-id="61058-218">Guarde as alterações e selecione **Ligue- se**.</span><span class="sxs-lookup"><span data-stu-id="61058-218">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="61058-219">Para permitir que os webhooks do Partner Center ouçam as alterações do evento, execute os seguintes passos:</span><span class="sxs-lookup"><span data-stu-id="61058-219">To enable Partner Center webhooks to listen to event changes, perform the following steps:</span></span>

5. <span data-ttu-id="61058-220">Selecione **Partner Center para Salesforce CRM (Visualização insider)**.</span><span class="sxs-lookup"><span data-stu-id="61058-220">Select **Partner Center to Salesforce CRM (Insider Preview)**.</span></span>

6. <span data-ttu-id="61058-221">Selecione o ícone **Editar** e selecione **Quando um pedido HTTP for recebido**.</span><span class="sxs-lookup"><span data-stu-id="61058-221">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="61058-222">Selecione o ícone **Copy** para copiar o URL HTTP POST fornecido.</span><span class="sxs-lookup"><span data-stu-id="61058-222">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="Copiar URL":::

8. <span data-ttu-id="61058-224">Selecione agora o "Partner Center Webhook Registration (Insider Preview)" Power Automamate flow e selecione **Run**.</span><span class="sxs-lookup"><span data-stu-id="61058-224">Now select the "Partner Center Webhook Registration (Insider Preview)" Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="61058-225">Certifique-se de que a janela "Run Flow" se abre no painel direito e clique em **Continuar**.</span><span class="sxs-lookup"><span data-stu-id="61058-225">Ensure that the "Run Flow" window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="61058-226">Introduza os seguintes detalhes:</span><span class="sxs-lookup"><span data-stu-id="61058-226">Enter the following details:</span></span>

    1. <span data-ttu-id="61058-227">**Http Trigger Endpoint**: URL copiado do passo anterior</span><span class="sxs-lookup"><span data-stu-id="61058-227">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="61058-228">**Eventos para Registar**: "referenciação criada" e "referenciada"</span><span class="sxs-lookup"><span data-stu-id="61058-228">**Events to Register**: "referral-created" and "referral-updated"</span></span>

    3. <span data-ttu-id="61058-229">**Substitua os pontos finais do gatilho existentes se estiver presente:** Sim (Isto substitui quaisquer pontos finais existentes.)</span><span class="sxs-lookup"><span data-stu-id="61058-229">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="61058-230">Selecione **Executar** e, em seguida, selecione **Fazer.**</span><span class="sxs-lookup"><span data-stu-id="61058-230">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="61058-231">O webhook pode agora ouvir criar e atualizar eventos.</span><span class="sxs-lookup"><span data-stu-id="61058-231">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="61058-232">Personalizar etapas de sincronização</span><span class="sxs-lookup"><span data-stu-id="61058-232">Customize synchronization steps</span></span>

<span data-ttu-id="61058-233">Quando as referências de Co-venda são sincronizadas entre o Partner Center e o seu sistema CRM, os campos sincronizados no Partner Center PC estão listados aqui.</span><span class="sxs-lookup"><span data-stu-id="61058-233">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="61058-234">Muitas vezes os sistemas de CRM são altamente personalizados.</span><span class="sxs-lookup"><span data-stu-id="61058-234">Often CRM systems are highly customized.</span></span> <span data-ttu-id="61058-235">Pode personalizar os fluxos power automamate.</span><span class="sxs-lookup"><span data-stu-id="61058-235">You can customize the Power Automate flows.</span></span> <span data-ttu-id="61058-236">Siga o guia de mapeamento de campo e, se necessário, faça as alterações adequadas nos passos dos fluxos power automamate.</span><span class="sxs-lookup"><span data-stu-id="61058-236">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="61058-237">Os centros de parceiros da Microsoft para mapeamentos CRM são fornecidos, mas com base no seu ambiente CRM, pode optar por personalizar ainda mais os campos.</span><span class="sxs-lookup"><span data-stu-id="61058-237">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="61058-238">Vários passos de cada um dos fluxos power automamate podem ser personalizados com base nas suas necessidades.</span><span class="sxs-lookup"><span data-stu-id="61058-238">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="61058-239">Seguem-se exemplos de personalizações disponíveis:</span><span class="sxs-lookup"><span data-stu-id="61058-239">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="61058-240">Para personalizar os campos para criar ou atualizar eventos no Centro de Parceiros para sincronização de referência CRM:</span><span class="sxs-lookup"><span data-stu-id="61058-240">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span>

   1. <span data-ttu-id="61058-241">Selecione Partner Center para Salesforce CRM (Visualização insider).</span><span class="sxs-lookup"><span data-stu-id="61058-241">Select Partner Center to Salesforce CRM (Insider Preview).</span></span>

   2. <span data-ttu-id="61058-242">**Selecione Editar** para editar/personalizar o fluxo power automamate.</span><span class="sxs-lookup"><span data-stu-id="61058-242">Select **Edit** to edit/customize the Power Automate flow.</span></span>

   3. <span data-ttu-id="61058-243">Selecione **(Âmbito) Sincronizar o chumbo ou a oportunidade**.</span><span class="sxs-lookup"><span data-stu-id="61058-243">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="61058-244">Para personalizar mapeamentos de campo de CRM para criar eventos, selecione **Se é nova oportunidade partilhada, então**.</span><span class="sxs-lookup"><span data-stu-id="61058-244">To customize CRM field mappings for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="61058-245">Selecione o sub-passo **se sim** e, em seguida, expanda **criando uma nova oportunidade no CRM**.</span><span class="sxs-lookup"><span data-stu-id="61058-245">Select the sub-step **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="61058-246">Pode editar os mapeamentos nesta secção utilizando o Guia de Mapeamento de Campo.</span><span class="sxs-lookup"><span data-stu-id="61058-246">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

   1. <span data-ttu-id="61058-247">Para personalizar mapeamentos de campo CRM para eventos de atualização, clique no passo "(Scope) Sincronizar o chumbo ou a oportunidade".</span><span class="sxs-lookup"><span data-stu-id="61058-247">To customize CRM field mappings for update events, click on the step "(Scope) Synchronize the lead or opportunity".</span></span>

   2. <span data-ttu-id="61058-248">Selecione **Se é uma atualização para uma oportunidade, então**.</span><span class="sxs-lookup"><span data-stu-id="61058-248">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="61058-249">Selecione o subpass **se sim** e, em seguida, expandir Se a diferença entre **os objetos de oportunidade no Partner Center e CRM, então**.</span><span class="sxs-lookup"><span data-stu-id="61058-249">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

   3. <span data-ttu-id="61058-250">Selecione **Se sim** seguido com **a atualização oportunidade existente**</span><span class="sxs-lookup"><span data-stu-id="61058-250">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="61058-251">Para personalizar os campos de sincronização de referência de CRM para PC para eventos de atualização:</span><span class="sxs-lookup"><span data-stu-id="61058-251">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

   1. <span data-ttu-id="61058-252">**Selecione Editar** para editar/personalizar o fluxo power automamate.</span><span class="sxs-lookup"><span data-stu-id="61058-252">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="61058-253">Selecione **(Âmbito) Sincronizar a oportunidade**.</span><span class="sxs-lookup"><span data-stu-id="61058-253">Select **(Scope) Synchronize the opportunity**.</span></span>

   3. <span data-ttu-id="61058-254">Para personalizar mapeamentos de campo de CRM (baseados no guia de mapeamentos de campo) para eventos de atualização, selecione **Se houver diferença entre os objetos de chumbo no Partner Center e CRM, então**.</span><span class="sxs-lookup"><span data-stu-id="61058-254">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span>

   4. <span data-ttu-id="61058-255">Selecione o sub-passo **se sim** e, em seguida, expandir o passo Atualizar uma referência **com dados de oportunidade**.</span><span class="sxs-lookup"><span data-stu-id="61058-255">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="61058-256">Pode editar os mapeamentos nesta secção com base no Guia de Mapeamento de Campo.</span><span class="sxs-lookup"><span data-stu-id="61058-256">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="61058-257">Para personalizar os campos de sincronização de referência de CRM para PC para criar eventos?</span><span class="sxs-lookup"><span data-stu-id="61058-257">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   1. <span data-ttu-id="61058-258">**Selecione Editar** para editar/personalizar o fluxo power automamate.</span><span class="sxs-lookup"><span data-stu-id="61058-258">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="61058-259">Selecione **(Âmbito) Referências sincronizadas.**</span><span class="sxs-lookup"><span data-stu-id="61058-259">Select **(Scope) Synchronizing Referrals.**</span></span>

   3. <span data-ttu-id="61058-260">Para personalizar mapeamentos de campo de CRM (baseados no guia de mapeamentos de campo) para criar eventos, **selecione Create Microsoft Referral**.</span><span class="sxs-lookup"><span data-stu-id="61058-260">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

<span data-ttu-id="61058-261">Pode editar os mapeamentos nesta secção com base no Guia de Mapeamento de Campo.</span><span class="sxs-lookup"><span data-stu-id="61058-261">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>


## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="61058-262">Sincronização de co-venda bidis de ponta a ponta</span><span class="sxs-lookup"><span data-stu-id="61058-262">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="61058-263">Uma vez instalada, configurada e personalizada a solução Power Automate, pode testar a sincronização de referências de Co-venda entre o Salesforce CRM e o Partner Center.</span><span class="sxs-lookup"><span data-stu-id="61058-263">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Salesforce CRM and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="61058-264">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="61058-264">Pre-requisites</span></span>

<span data-ttu-id="61058-265">Para sincronizar as referências através do Partner Center e da Salesforce CRM, a solução Power Automamate precisa de demarcar claramente os campos de referência específicos da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="61058-265">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="61058-266">Esta identificação proporciona às suas equipas de vendedores a capacidade de decidir quais as referências que querem partilhar com a Microsoft para co-venda.</span><span class="sxs-lookup"><span data-stu-id="61058-266">This identification provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="61058-267">Um conjunto de campos personalizados está disponível como parte da Sincronização de Referências do Partner Center para **a** solução de soluções de CRM Salesforce.</span><span class="sxs-lookup"><span data-stu-id="61058-267">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM solution **Opportunity** entity.</span></span> <span data-ttu-id="61058-268">Um utilizador de administração CRM terá de criar uma secção de CRM separada com os campos personalizados **Opportunity.**</span><span class="sxs-lookup"><span data-stu-id="61058-268">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="61058-269">Os seguintes campos personalizados devem fazer parte da secção CRM:</span><span class="sxs-lookup"><span data-stu-id="61058-269">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="61058-270">**Sincronizar com o Partner Center**: Se sincronizar a oportunidade com o Microsoft Partner Center</span><span class="sxs-lookup"><span data-stu-id="61058-270">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="61058-271">**Identificador** de referência : Um campo de identificação apenas de leitura para referência do Microsoft Partner Center</span><span class="sxs-lookup"><span data-stu-id="61058-271">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="61058-272">**Link de referência**: Um link apenas de leitura para a referência no Microsoft Partner Center</span><span class="sxs-lookup"><span data-stu-id="61058-272">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="61058-273">**Como pode a Microsoft ajudar:** Ajuda necessária da Microsoft para a referenciação</span><span class="sxs-lookup"><span data-stu-id="61058-273">**How can Microsoft help**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="61058-274">**Produtos**: Lista de produtos associados a esta oportunidade</span><span class="sxs-lookup"><span data-stu-id="61058-274">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="61058-275">**Auditoria**: Um rasto de auditoria só de leitura para sincronização com referências do Partner Center</span><span class="sxs-lookup"><span data-stu-id="61058-275">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="61058-276">CENÁRIOS:</span><span class="sxs-lookup"><span data-stu-id="61058-276">SCENARIOS:</span></span>

1. <span data-ttu-id="61058-277">Sincronização de encaminhamento quando a referência é criada ou atualizada em CRM e sincronizada no Partner Center:</span><span class="sxs-lookup"><span data-stu-id="61058-277">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="61058-278">Inscreva-se no seu ambiente de CRM Salesforce com o utilizador que tenha visibilidade na secção **Oportunidade** do CRM.</span><span class="sxs-lookup"><span data-stu-id="61058-278">Sign into your Salesforce CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="61058-279">Certifique-se de que a secção seguinte está presente quando criar uma "Nova Oportunidade" no ambiente CRM da Salesforce</span><span class="sxs-lookup"><span data-stu-id="61058-279">Ensure that the following section is present when you create a "New Opportunity" in Salesforce CRM environment</span></span>

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Ambiente salesforce":::

   3. <span data-ttu-id="61058-281">Para sincronizar esta oportunidade com o Microsoft Partner Center, certifique-se de que define os seguintes campos na vista do cartão:</span><span class="sxs-lookup"><span data-stu-id="61058-281">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

       - <span data-ttu-id="61058-282">"Sincronização com Centro de Parceiros": Sim</span><span class="sxs-lookup"><span data-stu-id="61058-282">"Sync with Partner Center": Yes</span></span>
       - <span data-ttu-id="61058-283">"Como pode a Microsoft ajudar?": Selecione a partir das seguintes opções:</span><span class="sxs-lookup"><span data-stu-id="61058-283">"How can Microsoft help?": Select from the following options:</span></span>
       - <span data-ttu-id="61058-284">Produtos: IDs de solução do produto</span><span class="sxs-lookup"><span data-stu-id="61058-284">Products: Solution IDs of the product</span></span>

   4. <span data-ttu-id="61058-285">Depois de definir a oportunidade  **Sync com Partner Center** para **Sim,** aguarde 10 minutos, inscreva-se na sua conta Partner Center.</span><span class="sxs-lookup"><span data-stu-id="61058-285">Once you have set the opportunity  **Sync with Partner Center** option to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="61058-286">As suas referências serão sincronizadas com a Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="61058-286">Your referrals will be synchronized with Salesforce CRM.</span></span>

   5. <span data-ttu-id="61058-287">Quando a opção "Sync with Partner Center" estiver definida como "Sim", se atualizar a oportunidade no Salesforce CRM, as alterações sincronizar-se-ão com a sua conta Partner Center.</span><span class="sxs-lookup"><span data-stu-id="61058-287">When the "Sync with Partner Center" option is set to "Yes", if you update the opportunity in Salesforce CRM, the changes will synchronize with your Partner Center account.</span></span>

   6. <span data-ttu-id="61058-288">As oportunidades sincronizadas com sucesso com o Partner Center serão identificadas com ✔icon na Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="61058-288">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Salesforce CRM.</span></span>

2. <span data-ttu-id="61058-289">Sincronização de referência quando a referência é criada ou atualizada no Microsoft Partner Center e sincronizada no ambiente de CRM da Salesforce:</span><span class="sxs-lookup"><span data-stu-id="61058-289">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Salesforce CRM environment:</span></span>

    1. <span data-ttu-id="61058-290">Inscreva-se no painel do Centro de [Parceiros.](https://partner.microsoft.com/dashboard/home)</span><span class="sxs-lookup"><span data-stu-id="61058-290">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    2. <span data-ttu-id="61058-291">Selecione **Referências** no menu à esquerda.</span><span class="sxs-lookup"><span data-stu-id="61058-291">Select **Referrals** from the left-hand menu.</span></span>

    3. <span data-ttu-id="61058-292">Crie uma nova referência de Co-venda do Partner Center clicando na opção "New deal".</span><span class="sxs-lookup"><span data-stu-id="61058-292">Create a new Co-sell referral from Partner Center by clicking "New deal" option.</span></span>

    4. <span data-ttu-id="61058-293">Inscreva-se no seu ambiente de CRM Salesforce.</span><span class="sxs-lookup"><span data-stu-id="61058-293">Sign into your Salesforce CRM environment.</span></span>

    5. <span data-ttu-id="61058-294">Navegue para **oportunidades abertas.**</span><span class="sxs-lookup"><span data-stu-id="61058-294">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="61058-295">A referência criada no Microsoft Partner Center está agora sincronizada na Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="61058-295">The referral created in Microsoft Partner Center is now synchronized in Salesforce CRM.</span></span>

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Tela de oportunidade de salesforce":::

    6. <span data-ttu-id="61058-297">Quando seleciona uma referência sincronizada, os dados da visualização do cartão são preenchidos.</span><span class="sxs-lookup"><span data-stu-id="61058-297">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="61058-298">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="61058-298">Next steps</span></span>

- [<span data-ttu-id="61058-299">Gerir oportunidades potenciais</span><span class="sxs-lookup"><span data-stu-id="61058-299">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="61058-300">Gerir oportunidades de venda conjunta</span><span class="sxs-lookup"><span data-stu-id="61058-300">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="61058-301">Webhooks do Partner Center</span><span class="sxs-lookup"><span data-stu-id="61058-301">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)
