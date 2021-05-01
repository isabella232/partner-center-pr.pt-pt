---
title: Resolução de problemas co-venda de conectores de referências
ms.topic: how-to
ms.date: 09/21/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Aprenda respostas a perguntas comuns sobre a utilização de conectores co-venda. Leia este FAQ sobre como resolver problemas co-vender conectores.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 939654202a370f6d9ba15d9e62a11be44884b613
ms.sourcegitcommit: 1899307642f057070b1bdd647594fc46ba61fb08
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/30/2021
ms.locfileid: "108284218"
---
# <a name="troubleshoot-co-sell-referrals-connectors"></a><span data-ttu-id="a5a22-104">Resolução de problemas co-venda de conectores de referências</span><span class="sxs-lookup"><span data-stu-id="a5a22-104">Troubleshoot co-sell referrals connectors</span></span>

<span data-ttu-id="a5a22-105">**Aplica-se a**</span><span class="sxs-lookup"><span data-stu-id="a5a22-105">**Applies to**</span></span>

- <span data-ttu-id="a5a22-106">Dinâmica 365 CRM</span><span class="sxs-lookup"><span data-stu-id="a5a22-106">Dynamics 365 CRM</span></span>
- <span data-ttu-id="a5a22-107">Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="a5a22-107">Salesforce CRM</span></span>

<span data-ttu-id="a5a22-108">**Funções adequadas**</span><span class="sxs-lookup"><span data-stu-id="a5a22-108">**Appropriate roles**</span></span>

- <span data-ttu-id="a5a22-109">Administração de referências</span><span class="sxs-lookup"><span data-stu-id="a5a22-109">Referrals admin</span></span>
- <span data-ttu-id="a5a22-110">Administrador de sistema ou personalizador de sistema no CRM</span><span class="sxs-lookup"><span data-stu-id="a5a22-110">System admin or system customizer on the CRM</span></span>

 ## <a name="questions-and-answers-about-pre-requisites"></a><span data-ttu-id="a5a22-111">Perguntas e respostas sobre pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a5a22-111">Questions and answers about pre-requisites</span></span>

1. <span data-ttu-id="a5a22-112">Pode utilizar uma solução de conectores de referências para o seu ambiente?</span><span class="sxs-lookup"><span data-stu-id="a5a22-112">Can you use a trial co-sell referrals connectors solution for your environment?</span></span>

<span data-ttu-id="a5a22-113">Se estiver no ambiente de teste/encenação, pode optar pela solução experimental.</span><span class="sxs-lookup"><span data-stu-id="a5a22-113">If you are on the test/staging environment, you can opt for trial solution.</span></span> <span data-ttu-id="a5a22-114">A versão paga dos Conectores está disponível no AppSource por US$ 15/mês.</span><span class="sxs-lookup"><span data-stu-id="a5a22-114">The paid version of the Connectors is available in AppSource at US$ 15/month.</span></span> <span data-ttu-id="a5a22-115">Com a ligação paga, receberá 10K de chamadas API por dia.</span><span class="sxs-lookup"><span data-stu-id="a5a22-115">With the paid connection, you will be getting 10K API calls per day.</span></span> <span data-ttu-id="a5a22-116">Os Conectores são invólucros em cima das APIs de referência do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="a5a22-116">The Connectors are wrappers on top of Partner Center referral APIs.</span></span> <span data-ttu-id="a5a22-117">Sempre que as soluções de conector funcionam para um evento **Criar** ou **Atualizar** as oportunidades no Centro de Parceiros ou no lado crm, é feita uma chamada API.</span><span class="sxs-lookup"><span data-stu-id="a5a22-117">Whenever the connector solutions run for a **Create** or **Update** event on the opportunities on either Partner Center or the CRM side, an API call is made.</span></span>

2. <span data-ttu-id="a5a22-118">Que papel precisa para criar secções em ambiente CRM?</span><span class="sxs-lookup"><span data-stu-id="a5a22-118">What role do you need to create sections in CRM environment?</span></span>

<span data-ttu-id="a5a22-119">Os utilizadores que são administradores do sistema ou personalizadores de sistema podem aplicar alterações para todos.</span><span class="sxs-lookup"><span data-stu-id="a5a22-119">Users who are system admins or system customizers can apply changes for everyone.</span></span> <span data-ttu-id="a5a22-120">Todos os utilizadores de aplicações, no entanto, podem personalizar o sistema e até partilhar algumas das suas personalizações com outros.</span><span class="sxs-lookup"><span data-stu-id="a5a22-120">All app users, however,  can personalize the system and even share some of their customizations with others.</span></span> 

3. <span data-ttu-id="a5a22-121">Os vendedores de parceiros precisam de papéis especiais para trabalhar no Partner Center?</span><span class="sxs-lookup"><span data-stu-id="a5a22-121">Do partner sellers need special roles to work on Partner Center?</span></span>
 
<span data-ttu-id="a5a22-122">Os vendedores de parceiros devem ser atribuídos à função "Administração de Referências".</span><span class="sxs-lookup"><span data-stu-id="a5a22-122">Partner sellers must be assigned the “Referrals admin” role.</span></span> <span data-ttu-id="a5a22-123">Para mais informações, consulte [a visão geral das permissões.](create-user-accounts-and-set-permissions.md)</span><span class="sxs-lookup"><span data-stu-id="a5a22-123">For more information, see [Permissions overview](create-user-accounts-and-set-permissions.md).</span></span>

4. <span data-ttu-id="a5a22-124">Que campos precisam de ser criados primeiro no seu ambiente de CRM?</span><span class="sxs-lookup"><span data-stu-id="a5a22-124">What fields need to be set up first in your CRM environment?</span></span> 

<span data-ttu-id="a5a22-125">• Certifique-se de que a sua moeda é adequada à sua localização e que se encontra no seu ambiente crm com precisão.</span><span class="sxs-lookup"><span data-stu-id="a5a22-125">• Make sure your currency is appropriate to your location and is in your CRM environment accurately.</span></span> <span data-ttu-id="a5a22-126">• A sua equipa de vendas deve estar listada no seu ambiente de CRM como utilizadores de CRM.</span><span class="sxs-lookup"><span data-stu-id="a5a22-126">• Your sales team should be listed in your CRM environment as CRM users.</span></span>

5. <span data-ttu-id="a5a22-127">Que pré-requisitos são necessários para a criação de ambiente power automamate?</span><span class="sxs-lookup"><span data-stu-id="a5a22-127">What pre-requisites are required for Power Automate environment creation?</span></span>

<span data-ttu-id="a5a22-128">Para utilizar o ambiente Power Automamate, precisa:</span><span class="sxs-lookup"><span data-stu-id="a5a22-128">To use the Power Automate environment, you need:</span></span>

- <span data-ttu-id="a5a22-129">É necessária uma licença Power Automamate.</span><span class="sxs-lookup"><span data-stu-id="a5a22-129">A Power Automate license is required.</span></span>
- <span data-ttu-id="a5a22-130">É necessário um armazenamento mínimo de 1-GB.</span><span class="sxs-lookup"><span data-stu-id="a5a22-130">A minimum of 1-GB storage is required.</span></span>

6.  <span data-ttu-id="a5a22-131">Precisa de uma subscrição Dynamics 365 para utilizar a solução De Conectores Salesforce?</span><span class="sxs-lookup"><span data-stu-id="a5a22-131">Do you need a Dynamics 365 subscription to use Salesforce Connectors solution?</span></span>

<span data-ttu-id="a5a22-132">A solução Salesforce Connector é do tipo "Dynamics Flow" que suporta a sincronização com outros sistemas de CRM.</span><span class="sxs-lookup"><span data-stu-id="a5a22-132">The Salesforce Connector solution is of type “Dynamics Flow” that supports synchronizing with other CRM systems.</span></span> <span data-ttu-id="a5a22-133">A solução não requer que tenha uma instância Dynamics 365 ou uma subscrição.</span><span class="sxs-lookup"><span data-stu-id="a5a22-133">The solution doesn’t require you to have a Dynamics 365 instance or a subscription.</span></span> <span data-ttu-id="a5a22-134">Ao instalar a solução Salesforce, pode aparecer uma queda com o ambiente cds existente na sua empresa.</span><span class="sxs-lookup"><span data-stu-id="a5a22-134">While installing the Salesforce solution, a drop-down with existing CDS environment in your company may appear.</span></span> <span data-ttu-id="a5a22-135">Tens de selecionar esse ambiente.</span><span class="sxs-lookup"><span data-stu-id="a5a22-135">You need to select that environment.</span></span> <span data-ttu-id="a5a22-136">Além disso, se tiver o erro "Não conseguimos encontrar uma organização Dynamics 365 ligada ao utilizador inscrito", então terá de criar um novo ambiente para o conector.</span><span class="sxs-lookup"><span data-stu-id="a5a22-136">In addition, if you get the error "We couldn't find a Dynamics 365 organization connected to signed-in user", then you will need to create new environment for connector.</span></span>

## <a name="questions-and-answers-about-configuration"></a><span data-ttu-id="a5a22-137">Perguntas e respostas sobre configuração</span><span class="sxs-lookup"><span data-stu-id="a5a22-137">Questions and answers about configuration</span></span>

1. <span data-ttu-id="a5a22-138">O que deve fazer se enfrentar o seguinte erro enquanto ativa os fluxos na Plataforma De Automatização de Energia?</span><span class="sxs-lookup"><span data-stu-id="a5a22-138">What should you do if you face the following error while activating flows in Power Automate Platform?</span></span>

<span data-ttu-id="a5a22-139">Erro: O pedido ao Gestor de Recursos Azure falhou com erro: '{"error":{"code":"WorkflowTriggerNotFound","message":"O fluxo de trabalho 'e14d00f1-1fdf-4b1b-aaac-54a50606093d3' não foi encontrado."}}</span><span class="sxs-lookup"><span data-stu-id="a5a22-139">Error: Request to Azure Resource Manager failed with error: '{"error":{"code":"WorkflowTriggerNotFound","message":"The workflow 'e14d00f1-1fdf-4b1b-aaac-54a5064093d3' trigger 'manual' could not be found."}}'.</span></span> 

<span data-ttu-id="a5a22-140">Siga estes passos de resolução de problemas:</span><span class="sxs-lookup"><span data-stu-id="a5a22-140">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="a5a22-141">Apague a ligação do CDS e depois recrie as ligações do CDS.</span><span class="sxs-lookup"><span data-stu-id="a5a22-141">Delete the CDS connection and then recreate the CDS connections.</span></span>
- <span data-ttu-id="a5a22-142">Desligue o fluxo da criança e vá para fora</span><span class="sxs-lookup"><span data-stu-id="a5a22-142">Turn the child flow off and on</span></span> 
- <span data-ttu-id="a5a22-143">Elimine a solução e, em seguida, volte a instalar a solução.</span><span class="sxs-lookup"><span data-stu-id="a5a22-143">Delete solution and then reinstall the solution.</span></span> 

2.  <span data-ttu-id="a5a22-144">O que deve fazer se enfrentar o erro de "Iniciar in" ao adicionar um conector Partner Center na Plataforma De Automatização de Energia?</span><span class="sxs-lookup"><span data-stu-id="a5a22-144">What should you do if you face the "Sign in" error while adding a Partner Center connector in Power Automate Platform?</span></span>

:::image type="content" source="images/cosellconnectors/failure.png" alt-text="Mensagem de erro que requer inscrição":::

<span data-ttu-id="a5a22-146">Siga este passo de resolução de problemas:</span><span class="sxs-lookup"><span data-stu-id="a5a22-146">Follow this troubleshooting step:</span></span>

- <span data-ttu-id="a5a22-147">Utilize as credenciais do Partner Center para iniciar uma vez no ambiente de fluxo (flow.microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="a5a22-147">Use your Partner Center credentials to sign into the flow environment once (flow.microsoft.com).</span></span>


3. <span data-ttu-id="a5a22-148">O que deve fazer se receber o seguinte erro ao ativar o Centro de Parceiros para o fluxo de CRM na Plataforma de Automatização de Energia?</span><span class="sxs-lookup"><span data-stu-id="a5a22-148">What should you do if you receive the following error while activating the Partner Center to CRM flow in Power Automate Platform?</span></span>
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="Mensagem de erro que requer atualizações":::

<span data-ttu-id="a5a22-150">Siga estes passos de resolução de problemas:</span><span class="sxs-lookup"><span data-stu-id="a5a22-150">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="a5a22-151">Ativar primeiro os dois fluxos de crianças seguintes antes de ativar o Centro de Parceiros para o fluxo de CRM.</span><span class="sxs-lookup"><span data-stu-id="a5a22-151">Activate the following two child flows first before you activate the Partner Center to CRM flow.</span></span>
      - <span data-ttu-id="a5a22-152">Centro de Parceiros para CRM - Helper (Visualização insider)</span><span class="sxs-lookup"><span data-stu-id="a5a22-152">Partner Center to CRM - Helper (Insider Preview)</span></span>
      - <span data-ttu-id="a5a22-153">Partner Center Microsoft Co-sell Referral Updates to CRM (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="a5a22-153">Partner Center Microsoft Co-sell Referral Updates to CRM (Insider Preview)</span></span>

4. <span data-ttu-id="a5a22-154">O que deve fazer quando não é capaz de adicionar ligações ao fluxo quando tenta editar o fluxo?</span><span class="sxs-lookup"><span data-stu-id="a5a22-154">What should you do when you aren't able to add connections to the flow when you try to edit the flow?</span></span>

<span data-ttu-id="a5a22-155">Adiciona-se ligações ao fluxo enquanto o fluxo está em funcionamento e adiciona-se a cada fluxo separadamente.</span><span class="sxs-lookup"><span data-stu-id="a5a22-155">You add connections to the flow while the flow is running, and you add to each flow separately.</span></span>  <span data-ttu-id="a5a22-156">Se o diálogo para adicionar ligações não se abrir automaticamente durante a edição do fluxo, então pode editar cada um dos passos e sub etapas dos fluxos individualmente.</span><span class="sxs-lookup"><span data-stu-id="a5a22-156">If the dialog to add connections doesn't open up automatically while editing the flow, then you can edit each of the steps and sub steps of the flows individually.</span></span>

- <span data-ttu-id="a5a22-157">Selecione cada fluxo e edite-os individualmente.</span><span class="sxs-lookup"><span data-stu-id="a5a22-157">Select each flow and edit them individually.</span></span>
- <span data-ttu-id="a5a22-158">Expandir todos os passos no fluxo</span><span class="sxs-lookup"><span data-stu-id="a5a22-158">Expand all the steps in the flow</span></span> 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="Passos que precisam de ligações":::

- <span data-ttu-id="a5a22-160">Selecione os passos onde vê um ícone de aviso pedindo para associar ligações e adicione ligações.</span><span class="sxs-lookup"><span data-stu-id="a5a22-160">Select the steps where you see a warning icon asking to associate connections, and add connections.</span></span> 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="Editar passo a passo":::


5. <span data-ttu-id="a5a22-162">O que deve fazer se os fluxos da solução de Conectores de Referências co-vender não ligarem?</span><span class="sxs-lookup"><span data-stu-id="a5a22-162">What should you do if the flows of the Co-sell Referrals Connectors solution don’t turn on?</span></span>

<span data-ttu-id="a5a22-163">A.</span><span class="sxs-lookup"><span data-stu-id="a5a22-163">A.</span></span> <span data-ttu-id="a5a22-164">No Power Automamate, terá de editar fluxos na seguinte ordem e atualizá-los para utilizar as ligações corretas:</span><span class="sxs-lookup"><span data-stu-id="a5a22-164">In Power Automate, you'll need to edit flows in the following order and update them to use the correct connections:</span></span>

- <span data-ttu-id="a5a22-165">Registo Webhook do Partner Center (Visualização privilegiada)</span><span class="sxs-lookup"><span data-stu-id="a5a22-165">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="a5a22-166">Criar Co-venda Referral - Salesforce to Partner Center (Visualização insider)</span><span class="sxs-lookup"><span data-stu-id="a5a22-166">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="a5a22-167">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="a5a22-167">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="a5a22-168">Centro de Parceiros para Salesforce (Visualização de Insider)</span><span class="sxs-lookup"><span data-stu-id="a5a22-168">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="a5a22-169">Salesforce para Partner Center (Visualização insider)</span><span class="sxs-lookup"><span data-stu-id="a5a22-169">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="a5a22-170">Oportunidade Salesforce para Partner Center (Visualização insider)</span><span class="sxs-lookup"><span data-stu-id="a5a22-170">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="a5a22-171">Salesforce Microsoft Solutions to Partner Center (Visualização insider)</span><span class="sxs-lookup"><span data-stu-id="a5a22-171">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

 <span data-ttu-id="a5a22-172">B.</span><span class="sxs-lookup"><span data-stu-id="a5a22-172">B.</span></span> <span data-ttu-id="a5a22-173">Para cada um dos fluxos, selecione A opção **de utilizadores de executar apenas.**</span><span class="sxs-lookup"><span data-stu-id="a5a22-173">For each of flow, select **Run only users** option.</span></span> <span data-ttu-id="a5a22-174">Selecione **Utilizar a ligação** em vez de **fornecido pelo utilizador apenas por execução**.</span><span class="sxs-lookup"><span data-stu-id="a5a22-174">Select **Use connection** instead of **Provided by run-only user**.</span></span>  

:::image type="content" source="images/cosellconnectors/runonly.png" alt-text="Para ativar um fluxo":::


<span data-ttu-id="a5a22-176">C.</span><span class="sxs-lookup"><span data-stu-id="a5a22-176">C.</span></span> <span data-ttu-id="a5a22-177">Ativar estes fluxos abaixo mencionados:</span><span class="sxs-lookup"><span data-stu-id="a5a22-177">Activate these below mentioned flows:</span></span>

 - <span data-ttu-id="a5a22-178">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="a5a22-178">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>

- <span data-ttu-id="a5a22-179">Salesforce para Partner Center (Visualização insider)</span><span class="sxs-lookup"><span data-stu-id="a5a22-179">Salesforce to Partner Center (Insider Preview)</span></span>

    
<span data-ttu-id="a5a22-180">D.</span><span class="sxs-lookup"><span data-stu-id="a5a22-180">D.</span></span> <span data-ttu-id="a5a22-181">Ativar todos os fluxos restantes.</span><span class="sxs-lookup"><span data-stu-id="a5a22-181">Activate all the remaining flows.</span></span>

<span data-ttu-id="a5a22-182">E.</span><span class="sxs-lookup"><span data-stu-id="a5a22-182">E.</span></span> <span data-ttu-id="a5a22-183">No flow Partner Center Webhook Registration, selecione **Run**.</span><span class="sxs-lookup"><span data-stu-id="a5a22-183">At flow Partner Center Webhook Registration, select **Run**.</span></span> <span data-ttu-id="a5a22-184">Forneça o **url http** da primeira ação no Partner Center para o fluxo **Salesforce.**</span><span class="sxs-lookup"><span data-stu-id="a5a22-184">Provide the **http url** from the first action in **Partner Center to Salesforce** flow.</span></span> <span data-ttu-id="a5a22-185">Selecione todas as quatro opções em **Eventos para se registar** e selecione **sim** para Overwrite.</span><span class="sxs-lookup"><span data-stu-id="a5a22-185">Select all four options under **Events to register** and select **yes** for Overwrite.</span></span>

## <a name="questions-and-answers-about-runmaintenance"></a><span data-ttu-id="a5a22-186">Perguntas e respostas sobre Execução/Manutenção</span><span class="sxs-lookup"><span data-stu-id="a5a22-186">Questions and answers about Run/Maintenance</span></span>

1. <span data-ttu-id="a5a22-187">Como se consegue resolver falhas durante a execução do fluxo power automamate?</span><span class="sxs-lookup"><span data-stu-id="a5a22-187">How do you troubleshoot failures during Power Automate flow execution?</span></span>

<span data-ttu-id="a5a22-188">Para garantir que os fluxos de automatismo de potência funcionam como espera e para resolver falhas durante a execução, consulte [falhas de fluxo de correção](/power-automate/fix-flow-failures).</span><span class="sxs-lookup"><span data-stu-id="a5a22-188">To ensure that your Power Automate flows run as you expect and to troubleshoot failures during execution, refer to [Fix flow failures](/power-automate/fix-flow-failures).</span></span>

2. <span data-ttu-id="a5a22-189">O que deve fazer se vir referências que não são sincronizadas corretamente no Centro de Parceiros ou no ambiente de CRM?</span><span class="sxs-lookup"><span data-stu-id="a5a22-189">What should you do if you see referrals that aren't synchronized properly in Partner Center or CRM environment?</span></span>
 
<span data-ttu-id="a5a22-190">Para determinar o estado da sincronização de referência, **selecione Audit**.</span><span class="sxs-lookup"><span data-stu-id="a5a22-190">To determine the status of referral synchronization, select **Audit**.</span></span> 

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="Como sincronizar referências":::

<span data-ttu-id="a5a22-192">Certifique-se de que estão reunidas as seguintes condições:</span><span class="sxs-lookup"><span data-stu-id="a5a22-192">Ensure that the following conditions are met:</span></span>

- <span data-ttu-id="a5a22-193">O ID da solução é fornecido como parte da oportunidade.</span><span class="sxs-lookup"><span data-stu-id="a5a22-193">Solution ID is provided as part of the opportunity.</span></span>

- <span data-ttu-id="a5a22-194">É necessário um código de país de duas letras.</span><span class="sxs-lookup"><span data-stu-id="a5a22-194">Two letter country code is required.</span></span>

- <span data-ttu-id="a5a22-195">Quando a ajuda da Microsoft é selecionada para a oportunidade, são necessárias informações de contacto com o cliente.</span><span class="sxs-lookup"><span data-stu-id="a5a22-195">When help from Microsoft is selected for the opportunity, customer contact information is required.</span></span>

3. <span data-ttu-id="a5a22-196">Como garantir que uma referência sincronizará bidireccionalmente?</span><span class="sxs-lookup"><span data-stu-id="a5a22-196">How to ensure that a referral will synchronize bi-directionally?</span></span>

<span data-ttu-id="a5a22-197">Faça os seguintes passos:</span><span class="sxs-lookup"><span data-stu-id="a5a22-197">Do the following steps:</span></span>

- <span data-ttu-id="a5a22-198">Os vendedores de parceiros precisam de garantir que ativaram a opção **Sync com Partner Center** na secção CRM.</span><span class="sxs-lookup"><span data-stu-id="a5a22-198">Partner sellers need to ensure that they have enabled **Sync with Partner Center** option in the CRM section.</span></span>

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="Certifique-se de que ativou o Synch":::

- <span data-ttu-id="a5a22-200">Os vendedores precisam fornecer receitas e data de encerramento na qualificação de uma liderança.</span><span class="sxs-lookup"><span data-stu-id="a5a22-200">Sellers need to provide revenue and closing date when qualifying a lead.</span></span>

- <span data-ttu-id="a5a22-201">Se o ID de CRM for fornecido na fase de **criação** ou **atualização** da oportunidade de co-venda, mas uma oportunidade de chumbo com esse ID não for encontrada em CRM, então a atualização ou criação será ignorada.</span><span class="sxs-lookup"><span data-stu-id="a5a22-201">If CRM ID is provided in the **create** or **update** stage of co-sell opportunity, but a lead opportunity with that ID is not found in CRM, then update or create will be ignored.</span></span>

- <span data-ttu-id="a5a22-202">Certifique-se de que o campo de referência da moeda está configurado no ambiente salesforce.</span><span class="sxs-lookup"><span data-stu-id="a5a22-202">Ensure that referral currency field is configured on Salesforce environment.</span></span> 

4. <span data-ttu-id="a5a22-203">O que deve fazer se o conector ficar desligado e perder uma sincronização de referência.?</span><span class="sxs-lookup"><span data-stu-id="a5a22-203">What should you do if the connector gets disconnected and you miss a referral synchronization.?</span></span>

<span data-ttu-id="a5a22-204">Seguem-se algumas das opções que pode experimentar:</span><span class="sxs-lookup"><span data-stu-id="a5a22-204">Following are few of the options that you can try out:</span></span>

- <span data-ttu-id="a5a22-205">Verifique se o nome de utilizador ou a palavra-passe expirou para o utilizador do Partner Center com funções de administração de encaminhamento.</span><span class="sxs-lookup"><span data-stu-id="a5a22-205">Check whether username or password has expired for the Partner Center user with referral admin roles.</span></span>

- <span data-ttu-id="a5a22-206">Pode ir à oportunidade não sincronizada, fazer uma pequena atualização e observar se a referência foi sincronizada.</span><span class="sxs-lookup"><span data-stu-id="a5a22-206">You can go to the un-synchronized opportunity, make a minor update, and observe whether the referral has synchronized.</span></span>

- <span data-ttu-id="a5a22-207">Se os fluxos tiverem corrido e falhado, então selecione o fluxo e reencando a execução que falhou.</span><span class="sxs-lookup"><span data-stu-id="a5a22-207">If the flows have run and failed, then select the flow and re-submit the run that has failed.</span></span>

5. <span data-ttu-id="a5a22-208">O que deve fazer quando tiver acesso a erros negados?</span><span class="sxs-lookup"><span data-stu-id="a5a22-208">What should you do when you get access denied errors?</span></span>

<span data-ttu-id="a5a22-209">Certifique-se de que existem as funções apropriadas</span><span class="sxs-lookup"><span data-stu-id="a5a22-209">Make sure the appropriate roles exist</span></span>

- <span data-ttu-id="a5a22-210">Função de administrador de referência para o vendedor do Partner Center</span><span class="sxs-lookup"><span data-stu-id="a5a22-210">Referral Administrator role for Partner Center seller</span></span> 
 
- <span data-ttu-id="a5a22-211">Função de administrador de sistema ou personalizador de sistema na sua instância crm</span><span class="sxs-lookup"><span data-stu-id="a5a22-211">System Administrator or System Customizer role on your CRM instance</span></span>

- <span data-ttu-id="a5a22-212">Certifique-se de que o utilizador da conta de fluxo Power Automamate entra https://flow.microsoft.com em, pelo menos, uma vez antes</span><span class="sxs-lookup"><span data-stu-id="a5a22-212">Ensure that the Power Automate flow account user logs into https://flow.microsoft.com at least once beforehand</span></span>

6. <span data-ttu-id="a5a22-213">Se vir que **o código do país da conta do cliente** está em falta enquanto cria uma oportunidade de Co-venda, o que deve fazer?</span><span class="sxs-lookup"><span data-stu-id="a5a22-213">If you see that **Customer account country code** is missing while creating a Co-sell opportunity, what should you do?</span></span>

<span data-ttu-id="a5a22-214">Terá de adicionar o código de 2 letras ISO à conta do Cliente em CRM.</span><span class="sxs-lookup"><span data-stu-id="a5a22-214">You will need to add the ISO two-letter country code to the Customer account in CRM.</span></span>

7. <span data-ttu-id="a5a22-215">O que deve fazer se vir o erro que o **ID da solução é necessário** ao criar uma oportunidade de Co-venda?</span><span class="sxs-lookup"><span data-stu-id="a5a22-215">What should you do if you see the error that **Solution ID is required** while creating a Co-sell opportunity?</span></span>

<span data-ttu-id="a5a22-216">Para criar uma referência de co-venda, precisa de uma solução pronta para co-venda da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="a5a22-216">In order to create a co-sell referral, you need a Microsoft co-sell ready solution.</span></span> 

8. <span data-ttu-id="a5a22-217">O que deve fazer quando vê oportunidades de Co-venda criadas no Partner Center que não estão sincronizadas com CRM, mesmo que não existam erros de fluxo?</span><span class="sxs-lookup"><span data-stu-id="a5a22-217">What should you do when you see Co-sell opportunities created in Partner Center that aren't synchronized to CRM even though there are no flow errors?</span></span>

<span data-ttu-id="a5a22-218">Faça o seguinte:</span><span class="sxs-lookup"><span data-stu-id="a5a22-218">Do the following:</span></span>

- <span data-ttu-id="a5a22-219">Depois de ter criado um novo negócio de co-venda no Partner Center, verifique se o fluxo partner Center to Dynamics 365 é invocado (pode ser invocado várias vezes).</span><span class="sxs-lookup"><span data-stu-id="a5a22-219">After you have created a new co-sell deal in Partner Center, check if Partner Center to Dynamics 365 flow gets invoked (it might get invoked multiple times).</span></span>

- <span data-ttu-id="a5a22-220">Se o fluxo for invocado, verifique todos os fluxos invocados e identifique o fluxo que atualizaria o CRM.</span><span class="sxs-lookup"><span data-stu-id="a5a22-220">If the flow gets invoked, check all invoked flows, and identify the flow run which that would update the CRM.</span></span> <span data-ttu-id="a5a22-221">Pode seguir as ações e verificar se a atualizou o CRM ou se encontrou um problema.</span><span class="sxs-lookup"><span data-stu-id="a5a22-221">You can follow the actions and verify if it did update the CRM or encountered a problem.</span></span>

- <span data-ttu-id="a5a22-222">Consulte **o novo negócio** no Partner Center para ver se é preenchido com ID CRM.</span><span class="sxs-lookup"><span data-stu-id="a5a22-222">Check **New deal** in Partner Center to see if it gets populated with CRM ID.</span></span>

- <span data-ttu-id="a5a22-223">Certifique-se de que o negócio não está fechado acidentalmente como **Won** ou **Lost** in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="a5a22-223">Make sure that the deal is not accidentally closed as **Won** or **Lost** in Partner Center.</span></span>

## <a name="next-steps"></a><span data-ttu-id="a5a22-224">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="a5a22-224">Next steps</span></span>

- [<span data-ttu-id="a5a22-225">Gerir oportunidades potenciais</span><span class="sxs-lookup"><span data-stu-id="a5a22-225">Manage leads</span></span>](manage-leads.md)
 
- [<span data-ttu-id="a5a22-226">Gerir oportunidades de venda conjunta</span><span class="sxs-lookup"><span data-stu-id="a5a22-226">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
