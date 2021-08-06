---
title: Resolução de problemas co-venda de conectores de referências
ms.topic: how-to
ms.date: 09/21/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-referrals
description: Aprenda respostas a perguntas comuns sobre a utilização de conectores co-venda. Leia este FAQ sobre como resolver problemas co-vender conectores.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: af5f54f1bc4b03fcea0d5aed62f8541c5202166793ab189e355bb2e560fd9f00
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/06/2021
ms.locfileid: "115679975"
---
# <a name="troubleshoot-co-sell-referrals-connectors"></a>Resolução de problemas co-venda de conectores de referências

**Aplica-se a**: Dinâmica 365 CRM | Salesforce CRM

**Funções adequadas**: Administração de referências | Administrador de sistema ou personalizador de sistema no CRM

 ## <a name="questions-and-answers-about-pre-requisites"></a>Perguntas e respostas sobre pré-requisitos

1. Pode utilizar uma solução de conectores de referências para o seu ambiente?

Se estiver no ambiente de teste/encenação, pode optar pela solução experimental. A versão paga dos Conectores está disponível no AppSource por US$ 15/mês. Com a ligação paga, receberá 10K de chamadas API por dia. Os Conectores são invólucros em cima das APIs de referência do Partner Center. Sempre que as soluções de conector funcionam para um evento **Criar** ou **Atualizar** as oportunidades no Centro de Parceiros ou no lado crm, é feita uma chamada API.

2. Que papel precisa para criar secções em ambiente CRM?

Os utilizadores que são administradores do sistema ou personalizadores de sistema podem aplicar alterações para todos. Todos os utilizadores de aplicações, no entanto, podem personalizar o sistema e até partilhar algumas das suas personalizações com outros. 

3. Os vendedores de parceiros precisam de papéis especiais para trabalhar no Partner Center?
 
Os vendedores de parceiros devem ser atribuídos à função "Administração de Referências". Para mais informações, consulte [a visão geral das permissões.](create-user-accounts-and-set-permissions.md)

4. Que campos precisam de ser criados primeiro no seu ambiente de CRM? 

• Certifique-se de que a sua moeda é adequada à sua localização e que se encontra no seu ambiente crm com precisão. • A sua equipa de vendas deve estar listada no seu ambiente de CRM como utilizadores de CRM.

5. Que pré-requisitos são necessários para Power Automate criação ambiental?

Para utilizar o ambiente Power Automate, precisa:

- É necessária uma licença de Power Automate.
- É necessário um armazenamento mínimo de 1-GB.

6.  Precisa de uma subscrição Dynamics 365 para utilizar a solução De Conectores Salesforce?

A solução Salesforce Connector é do tipo "Dynamics Flow" que suporta a sincronização com outros sistemas de CRM. A solução não requer que tenha uma instância Dynamics 365 ou uma subscrição. Ao instalar a solução Salesforce, pode aparecer uma queda com o ambiente cds existente na sua empresa. Tens de selecionar esse ambiente. Além disso, se tiver o erro "Não conseguimos encontrar uma organização Dynamics 365 ligada ao utilizador inscrito", então terá de criar um novo ambiente para o conector.

## <a name="questions-and-answers-about-configuration"></a>Perguntas e respostas sobre configuração

1. O que deve fazer se enfrentar o seguinte erro ao ativar fluxos na Plataforma Power Automate?

Erro: O pedido ao Gestor de Recursos Azure falhou com erro: '{"error":{"code":"WorkflowTriggerNotFound","message":"O fluxo de trabalho 'e14d00f1-1fdf-4b1b-aaac-54a50606093d3' não foi encontrado."}} 

Siga estes passos de resolução de problemas:

- Apague a ligação do CDS e depois recrie as ligações do CDS.
- Desligue o fluxo da criança e vá para fora 
- Elimine a solução e, em seguida, volte a instalar a solução. 

2.  O que deve fazer se enfrentar o erro de "Iniciar sê-lo" ao mesmo tempo que adiciona um conector Partner Center na Plataforma Power Automate?

:::image type="content" source="images/cosellconnectors/failure.png" alt-text="Mensagem de erro que requer sing-in.":::

Siga este passo de resolução de problemas:

- Utilize as credenciais do Partner Center para iniciar uma vez no ambiente de fluxo (flow.microsoft.com).


3. O que deve fazer se receber o seguinte erro ao ativar o Centro de Parceiros para o fluxo de CRM na Plataforma Power Automate?
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="Mensagem de erro que requer atualizações.":::

Siga estes passos de resolução de problemas:

- Ativar primeiro os dois fluxos de crianças seguintes antes de ativar o Centro de Parceiros para o fluxo de CRM.
      - Centro de Parceiros para CRM - Helper (Visualização insider)
      - Partner Center Microsoft Co-sell Referral Updates to CRM (Insider Preview)

4. O que deve fazer quando não é capaz de adicionar ligações ao fluxo quando tenta editar o fluxo?

Adiciona-se ligações ao fluxo enquanto o fluxo está em funcionamento e adiciona-se a cada fluxo separadamente.  Se o diálogo para adicionar ligações não se abrir automaticamente durante a edição do fluxo, então pode editar cada um dos passos e sub etapas dos fluxos individualmente.

- Selecione cada fluxo e edite-os individualmente.
- Expandir todos os passos no fluxo 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="Passos que precisam de ligações.":::

- Selecione os passos onde vê um ícone de aviso pedindo para associar ligações e adicione ligações. 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="Editar fluxo passo a passo.":::


5. O que deve fazer se os fluxos da solução de Conectores de Referências co-vender não ligarem?

A. Em Power Automate, terá de editar fluxos na seguinte ordem e atualizá-los para utilizar as ligações corretas:

- Registo Webhook do Partner Center (Visualização privilegiada)
- Criar Co-venda Referral - Salesforce to Partner Center (Visualização insider)
- Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)
- Centro de Parceiros para Salesforce (Visualização de Insider)
- Salesforce para Partner Center (Visualização insider)
- Oportunidade Salesforce para Partner Center (Visualização insider)
- Salesforce Microsoft Solutions to Partner Center (Visualização insider)

 B. Para cada um dos fluxos, selecione A opção **de utilizadores de executar apenas.** Selecione **Utilizar a ligação** em vez de **fornecido pelo utilizador apenas por execução**.  

:::image type="content" source="images/cosellconnectors/runonly.png" alt-text="Para ativar um fluxo.":::


C. Ativar estes fluxos abaixo mencionados:

 - Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)

- Salesforce para Partner Center (Visualização insider)

    
D. Ativar todos os fluxos restantes.

E. No flow Partner Center Webhook Registration, selecione **Run**. Forneça o **url http** da primeira ação no Partner Center para o fluxo **Salesforce.** Selecione todas as quatro opções em **Eventos para se registar** e selecione **sim** para Overwrite.

## <a name="questions-and-answers-about-runmaintenance"></a>Perguntas e respostas sobre Execução/Manutenção

1. Como se consegue resolver falhas durante Power Automate execução do fluxo?

Para garantir que os fluxos de Power Automate funcionam como espera e para resolver falhas durante a execução, consulte [falhas de fluxo de correção](/power-automate/fix-flow-failures).

2. O que deve fazer se vir referências que não são sincronizadas corretamente no Centro de Parceiros ou no ambiente de CRM?
 
Para determinar o estado da sincronização de referência, **selecione Audit**. 

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="Como sincronizar referências.":::

Certifique-se de que estão reunidas as seguintes condições:

- O ID da solução é fornecido como parte da oportunidade.

- É necessário um código de país de duas letras.

- Quando a ajuda da Microsoft é selecionada para a oportunidade, são necessárias informações de contacto com o cliente.

3. Como garantir que uma referência sincronizará bidireccionalmente?

Faça os seguintes passos:

- Os vendedores de parceiros precisam de garantir que ativaram a opção **Sync com Partner Center** na secção CRM.

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="Certifique-se de que ativou o Synch.":::

- Os vendedores precisam fornecer receitas e data de encerramento na qualificação de uma liderança.

- Se o ID de CRM for fornecido na fase de **criação** ou **atualização** da oportunidade de co-venda, mas uma oportunidade de chumbo com esse ID não for encontrada em CRM, então a atualização ou criação será ignorada.

- Certifique-se de que o campo de referência da moeda está configurado no ambiente salesforce. 

4. O que deve fazer se o conector ficar desligado e perder uma sincronização de referência.?

Seguem-se algumas das opções que pode experimentar:

- Verifique se o nome de utilizador ou a palavra-passe expirou para o utilizador do Partner Center com funções de administração de encaminhamento.

- Pode ir à oportunidade não sincronizada, fazer uma pequena atualização e observar se a referência foi sincronizada.

- Se os fluxos tiverem corrido e falhado, então selecione o fluxo e reencando a execução que falhou.

5. O que deve fazer quando tiver acesso a erros negados?

Certifique-se de que existem as funções apropriadas

- Função de administrador de referência para o vendedor do Partner Center 
 
- Função de administrador de sistema ou personalizador de sistema na sua instância crm

- Certifique-se de que o Power Automate fluxo de entrada do utilizador em https://flow.microsoft.com pelo menos uma vez antes

6. Se vir que **o código do país da conta do cliente** está em falta enquanto cria uma oportunidade de Co-venda, o que deve fazer?

Terá de adicionar o código de 2 letras ISO à conta do Cliente em CRM.

7. O que deve fazer se vir o erro que o **ID da solução é necessário** ao criar uma oportunidade de Co-venda?

Para criar uma referência de co-venda, precisa de uma solução pronta para co-venda da Microsoft. 

8. O que deve fazer quando vê oportunidades de Co-venda criadas no Partner Center que não estão sincronizadas com CRM, mesmo que não existam erros de fluxo?

Faça o seguinte:

- Depois de ter criado um novo negócio de co-venda no Partner Center, verifique se o fluxo partner Center to Dynamics 365 é invocado (pode ser invocado várias vezes).

- Se o fluxo for invocado, verifique todos os fluxos invocados e identifique o fluxo que atualizaria o CRM. Pode seguir as ações e verificar se a atualizou o CRM ou se encontrou um problema.

- Consulte **o novo negócio** no Partner Center para ver se é preenchido com ID CRM.

- Certifique-se de que o negócio não está fechado acidentalmente como **Won** ou **Lost** in Partner Center.

## <a name="next-steps"></a>Passos seguintes

- [Gerir oportunidades potenciais](manage-leads.md)
 
- [Gerir oportunidades de venda conjunta](manage-co-sell-opportunities.md)
