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
ms.openlocfilehash: 74894671966ac0409f6366f33c91ddadfae1ba4c
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276982"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a><span data-ttu-id="8c531-104">Conector de co-venda para Salesforce CRM - visão geral</span><span class="sxs-lookup"><span data-stu-id="8c531-104">Co-sell connector for Salesforce CRM - overview</span></span>

<span data-ttu-id="8c531-105">**Funções adequadas**: Administração de referências | Administrador de sistema ou personalizador de sistema no CRM</span><span class="sxs-lookup"><span data-stu-id="8c531-105">**Appropriate roles**: Referrals admin | System admin or system customizer on the CRM</span></span>

<span data-ttu-id="8c531-106">O conector partner Center co-sell permite que os seus vendedores co-vendam com a Microsoft a partir dos seus sistemas CRM.</span><span class="sxs-lookup"><span data-stu-id="8c531-106">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="8c531-107">Não terão de ser treinados para usar o Partner Center para gerir os negócios de co-venda.</span><span class="sxs-lookup"><span data-stu-id="8c531-107">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="8c531-108">Utilizando os conectores Co-sell, pode criar uma nova referência de Co-venda para contratar um vendedor da Microsoft, receber referências do vendedor da Microsoft, aceitar/recusar referências, modificar dados de negócios como o valor do negócio e a data de encerramento.</span><span class="sxs-lookup"><span data-stu-id="8c531-108">Using the Co-sell connectors, you can create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span>  <span data-ttu-id="8c531-109">Também pode receber quaisquer atualizações dos vendedores da Microsoft nestas ofertas de Co-venda.</span><span class="sxs-lookup"><span data-stu-id="8c531-109">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="8c531-110">Pode fazer todas as suas referências enquanto trabalha dentro do CRM à sua escolha e não no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="8c531-110">You can do all of your referrals work while working within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="8c531-111">A solução baseia-se na Solução de Automatização de Energia da Microsoft e utiliza APIs do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="8c531-111">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="8c531-112">Antes de instalar - pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8c531-112">Before you install - pre-requisites</span></span>

|<span data-ttu-id="8c531-113">**Tópicos**</span><span class="sxs-lookup"><span data-stu-id="8c531-113">**Topics**</span></span>   |<span data-ttu-id="8c531-114">**Detalhes**</span><span class="sxs-lookup"><span data-stu-id="8c531-114">**Details**</span></span>   |<span data-ttu-id="8c531-115">**Ligações**</span><span class="sxs-lookup"><span data-stu-id="8c531-115">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="8c531-116">ID da rede de parceiros da Microsoft</span><span class="sxs-lookup"><span data-stu-id="8c531-116">Microsoft Partner Network ID</span></span> |<span data-ttu-id="8c531-117">Precisa de um ID MPN válido</span><span class="sxs-lookup"><span data-stu-id="8c531-117">You need a valid MPN ID</span></span>|<span data-ttu-id="8c531-118">Para se juntar à [MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="8c531-118">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="8c531-119">Co-vender pronto</span><span class="sxs-lookup"><span data-stu-id="8c531-119">Co-sell ready</span></span>|<span data-ttu-id="8c531-120">A sua solução IP/Serviços tem de ser co-vendida.</span><span class="sxs-lookup"><span data-stu-id="8c531-120">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="8c531-121">Venda com a Microsoft</span><span class="sxs-lookup"><span data-stu-id="8c531-121">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="8c531-122">Conta do Centro de Parceiros</span><span class="sxs-lookup"><span data-stu-id="8c531-122">Partner Center account</span></span>|<span data-ttu-id="8c531-123">O ID MPN associado ao inquilino do Centro De Parceiros deve ser o mesmo que o ID MPN associado à sua solução de Co-venda.</span><span class="sxs-lookup"><span data-stu-id="8c531-123">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="8c531-124">Verifique se consegue ver as suas referências de co-venda no portal Partner Center antes de implantar os conectores.</span><span class="sxs-lookup"><span data-stu-id="8c531-124">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="8c531-125">Gerir a sua conta</span><span class="sxs-lookup"><span data-stu-id="8c531-125">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="8c531-126">Funções de utilizador do Partner Center</span><span class="sxs-lookup"><span data-stu-id="8c531-126">Partner Center user roles</span></span>|<span data-ttu-id="8c531-127">O empregado que vai instalar e usar os conectores deve ser um administrador de referências</span><span class="sxs-lookup"><span data-stu-id="8c531-127">The employee who will install and use the connectors must be a Referrals admin</span></span>|<span data-ttu-id="8c531-128">[Assign users roles and permissions](create-user-accounts-and-set-permissions.md) (Atribuir funções e permissões de utilizador)</span><span class="sxs-lookup"><span data-stu-id="8c531-128">[Assign users roles and permissions](create-user-accounts-and-set-permissions.md)</span></span>|
|<span data-ttu-id="8c531-129">Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="8c531-129">Salesforce CRM</span></span>|<span data-ttu-id="8c531-130">A função de utilizador crm é administrador do sistema ou personalizador do sistema</span><span class="sxs-lookup"><span data-stu-id="8c531-130">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="8c531-131">Atribuir funções na Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="8c531-131">Assign roles in Salesforce CRM</span></span>](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|<span data-ttu-id="8c531-132">Conta de fluxo de automatização de energia</span><span class="sxs-lookup"><span data-stu-id="8c531-132">Power Automate Flow Account</span></span>|<span data-ttu-id="8c531-133">Uma conta ativa [de Automação](https://flow.microsoft.com) de Energia para o administrador do Sistema CRM ou personalizador do sistema.</span><span class="sxs-lookup"><span data-stu-id="8c531-133">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="8c531-134">Este utilizador deve iniciar sustação na [Power Automamate](https://flow.microsoft.com) pelo menos uma vez antes da instalação.</span><span class="sxs-lookup"><span data-stu-id="8c531-134">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a><span data-ttu-id="8c531-135">Instalação do Pacote Salesforce para Campos Personalizados da Microsoft</span><span class="sxs-lookup"><span data-stu-id="8c531-135">Installation of Salesforce Package for Microsoft Custom Fields</span></span> 

<span data-ttu-id="8c531-136">Para sincronizar as referências através do Partner Center e da Salesforce CRM, a solução Power Automamate precisa de identificar claramente os campos de referência específicos da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="8c531-136">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly identify Microsoft-specific referral fields.</span></span> <span data-ttu-id="8c531-137">Esta demarcação proporciona às equipas de vendedores parceiros a capacidade de decidir quais as referências que querem partilhar com a Microsoft para co-venda.</span><span class="sxs-lookup"><span data-stu-id="8c531-137">This demarcation provides partner seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

1. <span data-ttu-id="8c531-138">Na Salesforce, ative **notas** e adicione-as à lista de oportunidades relacionadas.</span><span class="sxs-lookup"><span data-stu-id="8c531-138">In Salesforce, activate **Notes** and add it to the opportunities related list.</span></span> 
[<span data-ttu-id="8c531-139">Referência</span><span class="sxs-lookup"><span data-stu-id="8c531-139">Reference</span></span>](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

2. <span data-ttu-id="8c531-140">Ativar **as equipas de Oportunidade** seguindo os passos:</span><span class="sxs-lookup"><span data-stu-id="8c531-140">Activate **Opportunity teams** by following the steps:</span></span> 
    - <span data-ttu-id="8c531-141">Na configuração, utilize a caixa **De localização Rápida** para localizar as Definições da Equipa de Oportunidade.</span><span class="sxs-lookup"><span data-stu-id="8c531-141">In Setup, use the **Quick Find** box to locate Opportunity Team Settings.</span></span>
    - <span data-ttu-id="8c531-142">Defina as definições conforme necessário.</span><span class="sxs-lookup"><span data-stu-id="8c531-142">Define the settings as needed.</span></span>
[<span data-ttu-id="8c531-143">Referência</span><span class="sxs-lookup"><span data-stu-id="8c531-143">Reference</span></span>](https://help.salesforce.com/articleView?id=teamselling_enabling.htm&type=5]) 

3. <span data-ttu-id="8c531-144">No Salesforce, instale campos e objetos personalizados utilizando o [instalador de embalagens.](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV)</span><span class="sxs-lookup"><span data-stu-id="8c531-144">In Salesforce, install custom fields and objects using the [package installer](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV).</span></span> <span data-ttu-id="8c531-145">Utilize isto para instalar a embalagem em qualquer empresa.</span><span class="sxs-lookup"><span data-stu-id="8c531-145">Use this to install the package into any company.</span></span>

>[!NOTE]
><span data-ttu-id="8c531-146">Se estiver a instalar numa caixa de areia, deve substituir a parte inicial do URL por http://test.salesforce.com</span><span class="sxs-lookup"><span data-stu-id="8c531-146">If you are installing into a sandbox, you must replace the initial portion of the URL with http://test.salesforce.com</span></span>

4. <span data-ttu-id="8c531-147">Na Salesforce, adicione as Soluções Microsoft à lista relacionada com a **Oportunidade.**</span><span class="sxs-lookup"><span data-stu-id="8c531-147">In Salesforce, add Microsoft Solutions to the **Opportunity** related list.</span></span> <span data-ttu-id="8c531-148">Uma vez adicionado, selecione o ícone da **chave** inglesa e atualize propriedades</span><span class="sxs-lookup"><span data-stu-id="8c531-148">Once added, select the **wrench** icon and update properties</span></span>

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="8c531-149">Melhores Práticas: Teste antes de ir ao vivo</span><span class="sxs-lookup"><span data-stu-id="8c531-149">Best Practice: Test before you go live</span></span>

<span data-ttu-id="8c531-150">Antes de instalar, configurar e personalizar a solução Power Automamate no ambiente de produção, certifique-se de testar a solução numa fase de CRM de encenação.</span><span class="sxs-lookup"><span data-stu-id="8c531-150">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="8c531-151">Instale a solução Microsoft Power Automate num ambiente de preparação/instância CRM.</span><span class="sxs-lookup"><span data-stu-id="8c531-151">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>

- <span data-ttu-id="8c531-152">Faça uma cópia da solução e execute a sua configuração e faça personalizações de fluxo power-automatizado no ambiente de preparação.</span><span class="sxs-lookup"><span data-stu-id="8c531-152">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>

- <span data-ttu-id="8c531-153">Teste a solução numa fase de encenação/CRM.</span><span class="sxs-lookup"><span data-stu-id="8c531-153">Test the solution on a staging/CRM instance.</span></span>

- <span data-ttu-id="8c531-154">No que diz respeito ao sucesso, a importação como solução gerida para o caso de produção.</span><span class="sxs-lookup"><span data-stu-id="8c531-154">On success, import as a managed solution to the production instance.</span></span>

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a><span data-ttu-id="8c531-155">Instalar Referências do Centro de Parceiros Sincronização para Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="8c531-155">Install Partner Center Referrals Synchronization for Salesforce CRM</span></span>

1. <span data-ttu-id="8c531-156">Vá ao [Power Automamate](https://flow.microsoft.com) e selecione **Ambientes** no canto superior direito.</span><span class="sxs-lookup"><span data-stu-id="8c531-156">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="8c531-157">Isto irá mostrar-lhe as instâncias de CRM disponíveis.</span><span class="sxs-lookup"><span data-stu-id="8c531-157">This will show you the available CRM instances.</span></span>

2. <span data-ttu-id="8c531-158">Selecione a instância CRM apropriada a partir da queda no canto superior direito.</span><span class="sxs-lookup"><span data-stu-id="8c531-158">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="8c531-159">Selecione **Soluções** na barra de navegação esquerda.</span><span class="sxs-lookup"><span data-stu-id="8c531-159">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="8c531-160">Selecione o link **Open AppSource** no menu superior.</span><span class="sxs-lookup"><span data-stu-id="8c531-160">Select the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Abrir AppSource.":::

5. <span data-ttu-id="8c531-162">Procure por **Conectores de Referências do Centro de Parceiros para Salesforce** no ecrã pop-up.</span><span class="sxs-lookup"><span data-stu-id="8c531-162">Search for **Partner Center Referrals Connectors for Salesforce** in the pop-up screen.</span></span>  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="A força de vendas.":::

6. <span data-ttu-id="8c531-164">Selecione o botão **Get-lo agora** e, em seguida, **Continue**.</span><span class="sxs-lookup"><span data-stu-id="8c531-164">Select the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="8c531-165">Isto abre a página onde pode selecionar o ambiente de CRM salesforce para instalar a aplicação.</span><span class="sxs-lookup"><span data-stu-id="8c531-165">This opens the page where you can select the Salesforce CRM  environment to install application.</span></span>  <span data-ttu-id="8c531-166">Concorde com os termos e condições.</span><span class="sxs-lookup"><span data-stu-id="8c531-166">Agree to terms and conditions.</span></span>

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="CRMs disponíveis.":::

8. <span data-ttu-id="8c531-168">Em seguida, é direcionado para a página **Gerir as suas soluções.**</span><span class="sxs-lookup"><span data-stu-id="8c531-168">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="8c531-169">Navegue para "Partner Center Referrals" utilizando os botões de seta na parte inferior da página.</span><span class="sxs-lookup"><span data-stu-id="8c531-169">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="8c531-170">**A instalação programada** deve aparecer ao lado da solução de referências do Centro parceiro.</span><span class="sxs-lookup"><span data-stu-id="8c531-170">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="8c531-171">A instalação levará 10-15 minutos.</span><span class="sxs-lookup"><span data-stu-id="8c531-171">Installation will take 10-15 minutes.</span></span>

9. <span data-ttu-id="8c531-172">Assim que a instalação estiver concluída, volte a navegar para [o Power Automamate](https://flow.microsoft.com) e selecione **Soluções** da área de navegação à esquerda.</span><span class="sxs-lookup"><span data-stu-id="8c531-172">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="8c531-173">Note que **a Sincronização de Referências do Partner Center para a Salesforce** está disponível na lista de Soluções.</span><span class="sxs-lookup"><span data-stu-id="8c531-173">Notice that **Partner Center Referrals Synchronization for Salesforce** is available in the Solutions list.</span></span>

10. <span data-ttu-id="8c531-174">Selecione **Partner Center Referrals Synchronization for Salesforce**.</span><span class="sxs-lookup"><span data-stu-id="8c531-174">Select **Partner Center Referrals Synchronization for Salesforce**.</span></span> <span data-ttu-id="8c531-175">Estão disponíveis os seguintes fluxos e entidades power-automamate:</span><span class="sxs-lookup"><span data-stu-id="8c531-175">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/salesforce10.png" alt-text="A força de vendas flui.":::



## <a name="configure-the-solution"></a><span data-ttu-id="8c531-177">Configure a solução</span><span class="sxs-lookup"><span data-stu-id="8c531-177">Configure the solution</span></span>

1. <span data-ttu-id="8c531-178">Depois de ter instalado a solução no seu caso CRM, volte a navegar para [Power Automamate](https://flow.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="8c531-178">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="8c531-179">A partir do **drop-down Do Ambiente** no canto superior direito, selecione a instância CRM onde instalou a solução Power Automamate.</span><span class="sxs-lookup"><span data-stu-id="8c531-179">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>
3. <span data-ttu-id="8c531-180">Terá de criar ligações que associem as três contas de utilizador:</span><span class="sxs-lookup"><span data-stu-id="8c531-180">You will need to create connections that associate the three user accounts:</span></span>
    - <span data-ttu-id="8c531-181">Utilizador do Partner Center com credenciais de administração de referências</span><span class="sxs-lookup"><span data-stu-id="8c531-181">Partner Center user with referrals admin credentials</span></span>
    - <span data-ttu-id="8c531-182">Eventos do Centro de Parceiros</span><span class="sxs-lookup"><span data-stu-id="8c531-182">Partner Center Events</span></span>
    - <span data-ttu-id="8c531-183">Administração CRM com o Power Automamate flui na solução.</span><span class="sxs-lookup"><span data-stu-id="8c531-183">CRM admin with the Power Automate flows in the solution.</span></span>
4. <span data-ttu-id="8c531-184">Selecione **Ligações** da barra de navegação esquerda e selecione a solução "Partner Center Referrals" da lista.</span><span class="sxs-lookup"><span data-stu-id="8c531-184">Select **Connections** from the left navigation bar and select the "Partner Center Referrals" solution from the list.</span></span>

5. <span data-ttu-id="8c531-185">Criar uma ligação clicando **Criar uma ligação**.</span><span class="sxs-lookup"><span data-stu-id="8c531-185">Create a connection by clicking **Create a connection**.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce12.png" alt-text="Criar ligação.":::

- <span data-ttu-id="8c531-187">Procure referências ao Centro de Parceiros (pré-visualização) na barra de pesquisa no canto superior direito.</span><span class="sxs-lookup"><span data-stu-id="8c531-187">Search for Partner Center Referrals (preview) in the search bar on the top-right corner.</span></span>

- <span data-ttu-id="8c531-188">Crie uma ligação para o utilizador do Centro de Parceiros com o papel de credenciais da administração de referências.</span><span class="sxs-lookup"><span data-stu-id="8c531-188">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

-  <span data-ttu-id="8c531-189">Em seguida, crie uma ligação Partner Center Events para o seu utilizador Partner Center com as credenciais de administração de referências.</span><span class="sxs-lookup"><span data-stu-id="8c531-189">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

- <span data-ttu-id="8c531-190">Criar uma ligação para o Salesforce para o utilizador administrador crm.</span><span class="sxs-lookup"><span data-stu-id="8c531-190">Create a connection for Salesforce for the CRM administrator user.</span></span>

-  <span data-ttu-id="8c531-191">Uma vez adicionadas todas as Ligações, deverá ver as seguintes Ligações no seu ambiente:</span><span class="sxs-lookup"><span data-stu-id="8c531-191">Once you have all the Connections added, you should see the following Connections in your environment:</span></span>

 :::image type="content" source="images/cosellconnectors/salesforce13.png" alt-text="Observe as ligações.":::

### <a name="edit-the-connections"></a><span data-ttu-id="8c531-193">Editar as ligações</span><span class="sxs-lookup"><span data-stu-id="8c531-193">Edit the connections</span></span>

1. <span data-ttu-id="8c531-194">Volte à página Soluções e selecione **Solução Padrão.**</span><span class="sxs-lookup"><span data-stu-id="8c531-194">Return to the Solutions page and select **Default Solution**.</span></span>  <span data-ttu-id="8c531-195">Selecione **Referência de Ligação (pré-visualização)** clicando **em Tudo**.</span><span class="sxs-lookup"><span data-stu-id="8c531-195">Select **Connection Reference (preview)** by clicking **All**.</span></span>
 
:::image type="content" source="images/cosellconnectors/salesforce14.png" alt-text="Iniciar a edição do conector.":::

2. <span data-ttu-id="8c531-197">Edite cada uma das Ligações individualmente selecionando o ícone de três pontos.</span><span class="sxs-lookup"><span data-stu-id="8c531-197">Edit each of the Connections individually by selecting the three dots icon.</span></span> <span data-ttu-id="8c531-198">Adicione as ligações relevantes.</span><span class="sxs-lookup"><span data-stu-id="8c531-198">Add the relevant connections.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="Editar conectores.":::

3. <span data-ttu-id="8c531-200">Ligue os fluxos na seguinte sequência:</span><span class="sxs-lookup"><span data-stu-id="8c531-200">Turn on the flows in the following sequence:</span></span>

- <span data-ttu-id="8c531-201">Registo Webhook do Partner Center (Visualização privilegiada)</span><span class="sxs-lookup"><span data-stu-id="8c531-201">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="8c531-202">Criar Co-venda Referral - Salesforce to Partner Center (Visualização insider)</span><span class="sxs-lookup"><span data-stu-id="8c531-202">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="8c531-203">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="8c531-203">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="8c531-204">Centro de Parceiros para Salesforce (Visualização de Insider)</span><span class="sxs-lookup"><span data-stu-id="8c531-204">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="8c531-205">Salesforce para Partner Center (Visualização insider)</span><span class="sxs-lookup"><span data-stu-id="8c531-205">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="8c531-206">Oportunidade Salesforce para Partner Center (Visualização insider)</span><span class="sxs-lookup"><span data-stu-id="8c531-206">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="8c531-207">Salesforce Microsoft Solutions to Partner Center (Visualização insider)</span><span class="sxs-lookup"><span data-stu-id="8c531-207">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="8c531-208">Utilize APIs webhook para se registar para eventos de mudança de recursos</span><span class="sxs-lookup"><span data-stu-id="8c531-208">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="8c531-209">As APIs do Partner Center Webhook permitem-lhe registar-se para eventos de alteração de recursos.</span><span class="sxs-lookup"><span data-stu-id="8c531-209">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="8c531-210">Estes eventos de alteração são enviados para o seu url como posts HTTP.</span><span class="sxs-lookup"><span data-stu-id="8c531-210">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="8c531-211">Para registar o seu url, selecione **Partner Center Webhook Registr (Insider Preview)** Power Automamate flow.</span><span class="sxs-lookup"><span data-stu-id="8c531-211">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="8c531-212">Adicione ligações para (a.) Utilizador do Partner Center com credenciais de administração de referências (b.) Eventos do Centro de Parceiros, conforme destacado abaixo</span><span class="sxs-lookup"><span data-stu-id="8c531-212">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="O gatilho.":::

3. <span data-ttu-id="8c531-214">Quando fizer estas atualizações, verá</span><span class="sxs-lookup"><span data-stu-id="8c531-214">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhooks.":::

4. <span data-ttu-id="8c531-216">Guarde as alterações e selecione **Ligue- se**.</span><span class="sxs-lookup"><span data-stu-id="8c531-216">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="8c531-217">Para permitir que os webhooks do Partner Center ouçam as alterações do evento, execute os seguintes passos:</span><span class="sxs-lookup"><span data-stu-id="8c531-217">To enable Partner Center webhooks to listen to event changes, perform the following steps:</span></span>

5. <span data-ttu-id="8c531-218">Selecione **Partner Center para Salesforce CRM (Visualização insider)**.</span><span class="sxs-lookup"><span data-stu-id="8c531-218">Select **Partner Center to Salesforce CRM (Insider Preview)**.</span></span>

6. <span data-ttu-id="8c531-219">Selecione o ícone **Editar** e selecione **Quando um pedido HTTP for recebido**.</span><span class="sxs-lookup"><span data-stu-id="8c531-219">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="8c531-220">Selecione o ícone **Copy** para copiar o URL HTTP POST fornecido.</span><span class="sxs-lookup"><span data-stu-id="8c531-220">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="Copiar URL.":::

8. <span data-ttu-id="8c531-222">Selecione agora o "Partner Center Webhook Registration (Insider Preview)" Power Automamate flow e selecione **Run**.</span><span class="sxs-lookup"><span data-stu-id="8c531-222">Now select the "Partner Center Webhook Registration (Insider Preview)" Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="8c531-223">Certifique-se de que a janela "Run Flow" se abre no painel direito e selecione **Continue**.</span><span class="sxs-lookup"><span data-stu-id="8c531-223">Ensure that the "Run Flow" window opens on the right-hand pane and select **Continue**.</span></span>

10. <span data-ttu-id="8c531-224">Introduza os seguintes detalhes:</span><span class="sxs-lookup"><span data-stu-id="8c531-224">Enter the following details:</span></span>

    1. <span data-ttu-id="8c531-225">**Http Trigger Endpoint**: URL copiado do passo anterior</span><span class="sxs-lookup"><span data-stu-id="8c531-225">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="8c531-226">**Eventos para Registar**: "referenciação criada" e "referenciada"</span><span class="sxs-lookup"><span data-stu-id="8c531-226">**Events to Register**: "referral-created" and "referral-updated"</span></span>

    3. <span data-ttu-id="8c531-227">**Substitua os pontos finais do gatilho existentes se estiver presente:** Sim (Isto substitui quaisquer pontos finais existentes.)</span><span class="sxs-lookup"><span data-stu-id="8c531-227">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="8c531-228">Selecione **Executar** e, em seguida, selecione **Fazer.**</span><span class="sxs-lookup"><span data-stu-id="8c531-228">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="8c531-229">O webhook pode agora ouvir criar e atualizar eventos.</span><span class="sxs-lookup"><span data-stu-id="8c531-229">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="8c531-230">Personalizar etapas de sincronização</span><span class="sxs-lookup"><span data-stu-id="8c531-230">Customize synchronization steps</span></span>

<span data-ttu-id="8c531-231">Quando as referências de Co-venda são sincronizadas entre o Partner Center e o seu sistema CRM, os campos sincronizados no Partner Center PC estão listados aqui.</span><span class="sxs-lookup"><span data-stu-id="8c531-231">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="8c531-232">Muitas vezes os sistemas de CRM são altamente personalizados.</span><span class="sxs-lookup"><span data-stu-id="8c531-232">Often CRM systems are highly customized.</span></span> <span data-ttu-id="8c531-233">Pode personalizar os fluxos power automamate.</span><span class="sxs-lookup"><span data-stu-id="8c531-233">You can customize the Power Automate flows.</span></span> <span data-ttu-id="8c531-234">Siga o guia de mapeamento de campo e, se necessário, faça as alterações adequadas nos passos dos fluxos power automamate.</span><span class="sxs-lookup"><span data-stu-id="8c531-234">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="8c531-235">Os centros de parceiros da Microsoft para mapeamentos CRM são fornecidos, mas com base no seu ambiente CRM, pode optar por personalizar ainda mais os campos.</span><span class="sxs-lookup"><span data-stu-id="8c531-235">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="8c531-236">Vários passos de cada um dos fluxos power automamate podem ser personalizados com base nas suas necessidades.</span><span class="sxs-lookup"><span data-stu-id="8c531-236">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="8c531-237">Seguem-se exemplos de personalizações disponíveis:</span><span class="sxs-lookup"><span data-stu-id="8c531-237">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="8c531-238">Para personalizar os campos para criar ou atualizar eventos no Centro de Parceiros para sincronização de referência CRM:</span><span class="sxs-lookup"><span data-stu-id="8c531-238">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span>

   1. <span data-ttu-id="8c531-239">Selecione Partner Center para Salesforce CRM (Visualização insider).</span><span class="sxs-lookup"><span data-stu-id="8c531-239">Select Partner Center to Salesforce CRM (Insider Preview).</span></span>

   2. <span data-ttu-id="8c531-240">**Selecione Editar** para editar/personalizar o fluxo power automamate.</span><span class="sxs-lookup"><span data-stu-id="8c531-240">Select **Edit** to edit/customize the Power Automate flow.</span></span>

   3. <span data-ttu-id="8c531-241">Selecione **(Âmbito) Sincronizar o chumbo ou a oportunidade**.</span><span class="sxs-lookup"><span data-stu-id="8c531-241">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="8c531-242">Para personalizar mapeamentos de campo de CRM para criar eventos, selecione **Se é nova oportunidade partilhada, então**.</span><span class="sxs-lookup"><span data-stu-id="8c531-242">To customize CRM field mappings for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="8c531-243">Selecione o sub-passo **se sim** e, em seguida, expanda **criando uma nova oportunidade no CRM**.</span><span class="sxs-lookup"><span data-stu-id="8c531-243">Select the sub-step **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="8c531-244">Pode editar os mapeamentos nesta secção utilizando o Guia de Mapeamento de Campo.</span><span class="sxs-lookup"><span data-stu-id="8c531-244">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

   1. <span data-ttu-id="8c531-245">Para personalizar mapeamentos de campo crm para eventos de atualização, selecione o passo "(Scope) Sincronizar o chumbo ou a oportunidade".</span><span class="sxs-lookup"><span data-stu-id="8c531-245">To customize CRM field mappings for update events, select the step "(Scope) Synchronize the lead or opportunity".</span></span>

   2. <span data-ttu-id="8c531-246">Selecione **Se é uma atualização para uma oportunidade, então**.</span><span class="sxs-lookup"><span data-stu-id="8c531-246">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="8c531-247">Selecione o sub-passo **se sim** e, em seguida, expandir Se a diferença entre **os objetos de oportunidade no Partner Center e CRM, então**.</span><span class="sxs-lookup"><span data-stu-id="8c531-247">Select the sub-step **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

   3. <span data-ttu-id="8c531-248">Selecione **Se sim** seguido com **a atualização oportunidade existente**</span><span class="sxs-lookup"><span data-stu-id="8c531-248">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="8c531-249">Para personalizar os campos de sincronização de referência de CRM para PC para eventos de atualização:</span><span class="sxs-lookup"><span data-stu-id="8c531-249">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

   1. <span data-ttu-id="8c531-250">**Selecione Editar** para editar/personalizar o fluxo power automamate.</span><span class="sxs-lookup"><span data-stu-id="8c531-250">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="8c531-251">Selecione **(Âmbito) Sincronizar a oportunidade**.</span><span class="sxs-lookup"><span data-stu-id="8c531-251">Select **(Scope) Synchronize the opportunity**.</span></span>

   3. <span data-ttu-id="8c531-252">Para personalizar mapeamentos de campo de CRM (baseados no guia de mapeamentos de campo) para eventos de atualização, selecione **Se houver diferença entre os objetos de chumbo no Partner Center e CRM, então**.</span><span class="sxs-lookup"><span data-stu-id="8c531-252">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span>

   4. <span data-ttu-id="8c531-253">Selecione o sub-passo **se sim** e, em seguida, expandir o passo Atualizar uma referência **com dados de oportunidade**.</span><span class="sxs-lookup"><span data-stu-id="8c531-253">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="8c531-254">Pode editar os mapeamentos nesta secção com base no Guia de Mapeamento de Campo.</span><span class="sxs-lookup"><span data-stu-id="8c531-254">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="8c531-255">Para personalizar os campos de sincronização de referência de CRM para PC para criar eventos?</span><span class="sxs-lookup"><span data-stu-id="8c531-255">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   1. <span data-ttu-id="8c531-256">**Selecione Editar** para editar/personalizar o fluxo power automamate.</span><span class="sxs-lookup"><span data-stu-id="8c531-256">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="8c531-257">Selecione **(Âmbito) Referências sincronizadas.**</span><span class="sxs-lookup"><span data-stu-id="8c531-257">Select **(Scope) Synchronizing Referrals.**</span></span>

   3. <span data-ttu-id="8c531-258">Para personalizar mapeamentos de campo de CRM (baseados no guia de mapeamentos de campo) para criar eventos, **selecione Create Microsoft Referral**.</span><span class="sxs-lookup"><span data-stu-id="8c531-258">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

<span data-ttu-id="8c531-259">Pode editar os mapeamentos nesta secção com base no Guia de Mapeamento de Campo.</span><span class="sxs-lookup"><span data-stu-id="8c531-259">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>


## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="8c531-260">Sincronização de co-venda bidis de ponta a ponta</span><span class="sxs-lookup"><span data-stu-id="8c531-260">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="8c531-261">Uma vez instalada, configurada e personalizada a solução Power Automate, pode testar a sincronização de referências de Co-venda entre o Salesforce CRM e o Partner Center.</span><span class="sxs-lookup"><span data-stu-id="8c531-261">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Salesforce CRM and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="8c531-262">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8c531-262">Pre-requisites</span></span>

<span data-ttu-id="8c531-263">Para sincronizar as referências através do Partner Center e da Salesforce CRM, a solução Power Automamate precisa de demarcar claramente os campos de referência específicos da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="8c531-263">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="8c531-264">Esta identificação proporciona às suas equipas de vendedores a capacidade de decidir quais as referências que querem partilhar com a Microsoft para co-venda.</span><span class="sxs-lookup"><span data-stu-id="8c531-264">This identification provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="8c531-265">Um conjunto de campos personalizados está disponível como parte da Sincronização de Referências do Partner Center para **a** solução de soluções de CRM Salesforce.</span><span class="sxs-lookup"><span data-stu-id="8c531-265">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM solution **Opportunity** entity.</span></span> <span data-ttu-id="8c531-266">Um utilizador de administração CRM terá de criar uma secção de CRM separada com os campos personalizados **Opportunity.**</span><span class="sxs-lookup"><span data-stu-id="8c531-266">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="8c531-267">Os seguintes campos personalizados devem fazer parte da secção CRM:</span><span class="sxs-lookup"><span data-stu-id="8c531-267">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="8c531-268">**Sincronizar com o Partner Center**: Se sincronizar a oportunidade com o Microsoft Partner Center</span><span class="sxs-lookup"><span data-stu-id="8c531-268">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="8c531-269">**Identificador** de referência : Um campo de identificação apenas de leitura para referência do Microsoft Partner Center</span><span class="sxs-lookup"><span data-stu-id="8c531-269">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="8c531-270">**Link de referência**: Um link apenas de leitura para a referência no Microsoft Partner Center</span><span class="sxs-lookup"><span data-stu-id="8c531-270">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="8c531-271">**Como pode a Microsoft ajudar:** Ajuda necessária da Microsoft para a referenciação</span><span class="sxs-lookup"><span data-stu-id="8c531-271">**How can Microsoft help**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="8c531-272">**Produtos**: Lista de produtos associados a esta oportunidade</span><span class="sxs-lookup"><span data-stu-id="8c531-272">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="8c531-273">**Auditoria**: Um rasto de auditoria só de leitura para sincronização com referências do Partner Center</span><span class="sxs-lookup"><span data-stu-id="8c531-273">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="8c531-274">CENÁRIOS:</span><span class="sxs-lookup"><span data-stu-id="8c531-274">SCENARIOS:</span></span>

1. <span data-ttu-id="8c531-275">Sincronização de encaminhamento quando a referência é criada ou atualizada em CRM e sincronizada no Partner Center:</span><span class="sxs-lookup"><span data-stu-id="8c531-275">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="8c531-276">Inscreva-se no seu ambiente de CRM Salesforce com o utilizador que tenha visibilidade na secção **Oportunidade** do CRM.</span><span class="sxs-lookup"><span data-stu-id="8c531-276">Sign into your Salesforce CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="8c531-277">Certifique-se de que a secção seguinte está presente quando criar uma "Nova Oportunidade" no ambiente CRM da Salesforce</span><span class="sxs-lookup"><span data-stu-id="8c531-277">Ensure that the following section is present when you create a "New Opportunity" in Salesforce CRM environment</span></span>

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Ambiente de salesforce.":::

   3. <span data-ttu-id="8c531-279">Para sincronizar esta oportunidade com o Microsoft Partner Center, certifique-se de que define os seguintes campos na vista do cartão:</span><span class="sxs-lookup"><span data-stu-id="8c531-279">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

       - <span data-ttu-id="8c531-280">"Sincronização com Centro de Parceiros": Sim</span><span class="sxs-lookup"><span data-stu-id="8c531-280">"Sync with Partner Center": Yes</span></span>
       - <span data-ttu-id="8c531-281">"Como pode a Microsoft ajudar?": Selecione a partir das seguintes opções:</span><span class="sxs-lookup"><span data-stu-id="8c531-281">"How can Microsoft help?": Select from the following options:</span></span>
       - <span data-ttu-id="8c531-282">Produtos: IDs de solução do produto</span><span class="sxs-lookup"><span data-stu-id="8c531-282">Products: Solution IDs of the product</span></span>

   4. <span data-ttu-id="8c531-283">Depois de definir a oportunidade  **Sync com Partner Center** para **Sim,** aguarde 10 minutos, inscreva-se na sua conta Partner Center.</span><span class="sxs-lookup"><span data-stu-id="8c531-283">Once you have set the opportunity  **Sync with Partner Center** option to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="8c531-284">As suas referências serão sincronizadas com a Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="8c531-284">Your referrals will be synchronized with Salesforce CRM.</span></span>

   5. <span data-ttu-id="8c531-285">Quando a opção "Sync with Partner Center" estiver definida como "Sim", se atualizar a oportunidade no Salesforce CRM, as alterações sincronizar-se-ão com a sua conta Partner Center.</span><span class="sxs-lookup"><span data-stu-id="8c531-285">When the "Sync with Partner Center" option is set to "Yes", if you update the opportunity in Salesforce CRM, the changes will synchronize with your Partner Center account.</span></span>

   6. <span data-ttu-id="8c531-286">As oportunidades sincronizadas com sucesso com o Partner Center serão identificadas com ✔icon na Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="8c531-286">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Salesforce CRM.</span></span>

2. <span data-ttu-id="8c531-287">Sincronização de referência quando a referência é criada ou atualizada no Microsoft Partner Center e sincronizada no ambiente de CRM da Salesforce:</span><span class="sxs-lookup"><span data-stu-id="8c531-287">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Salesforce CRM environment:</span></span>

    1. <span data-ttu-id="8c531-288">Inscreva-se no painel do Centro de [Parceiros.](https://partner.microsoft.com/dashboard/home)</span><span class="sxs-lookup"><span data-stu-id="8c531-288">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    2. <span data-ttu-id="8c531-289">Selecione **Referências** no menu à esquerda.</span><span class="sxs-lookup"><span data-stu-id="8c531-289">Select **Referrals** from the left-hand menu.</span></span>

    3. <span data-ttu-id="8c531-290">Crie uma nova referência de Co-venda do Partner Center clicando na opção "New deal".</span><span class="sxs-lookup"><span data-stu-id="8c531-290">Create a new Co-sell referral from Partner Center by clicking "New deal" option.</span></span>

    4. <span data-ttu-id="8c531-291">Inscreva-se no seu ambiente de CRM Salesforce.</span><span class="sxs-lookup"><span data-stu-id="8c531-291">Sign into your Salesforce CRM environment.</span></span>

    5. <span data-ttu-id="8c531-292">Navegue para **oportunidades abertas.**</span><span class="sxs-lookup"><span data-stu-id="8c531-292">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="8c531-293">A referência criada no Microsoft Partner Center está agora sincronizada na Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="8c531-293">The referral created in Microsoft Partner Center is now synchronized in Salesforce CRM.</span></span>

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Ecrã de oportunidade de salesforce.":::

    6. <span data-ttu-id="8c531-295">Quando seleciona uma referência sincronizada, os dados da visualização do cartão são preenchidos.</span><span class="sxs-lookup"><span data-stu-id="8c531-295">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="8c531-296">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="8c531-296">Next steps</span></span>

- [<span data-ttu-id="8c531-297">Gerir oportunidades potenciais</span><span class="sxs-lookup"><span data-stu-id="8c531-297">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="8c531-298">Gerir oportunidades de venda conjunta</span><span class="sxs-lookup"><span data-stu-id="8c531-298">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="8c531-299">Webhooks do Centro de Parceiros</span><span class="sxs-lookup"><span data-stu-id="8c531-299">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)
