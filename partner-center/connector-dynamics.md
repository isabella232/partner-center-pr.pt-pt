---
title: O conector de co-venda para Dynamics 365 CRM Partner Center
description: Sincronizar referências no Partner Center com o seu conector de co-venda para Dynamics 365 CRM. Os vendedores podem então co-vender com a Microsoft a partir dos seus sistemas CRM.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.date: 03/01/2021
ms.openlocfilehash: 1b0f8f12cf60db0dcc03aae24316e869cbf34376
ms.sourcegitcommit: d7fbaff51c7ac29fbf700d7f7fdef798fd97c6fa
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/10/2021
ms.locfileid: "102619414"
---
# <a name="co-sell-connector-for-dynamics-365-crm--overview"></a>Conector de co-venda para Dynamics 365 CRM – Visão geral

### <a name="appropriate-roles"></a>Funções adequadas

- Administração de referências
- Administrador de sistema ou personalizador de sistema no CRM

O conector Partner Center Co-sell permite que os seus vendedores co-vendam com a Microsoft a partir dos seus sistemas CRM. Não terão de ser treinados para usar o Partner Center para gerir os negócios de co-venda. Utilize os conectores Co-sell, para criar uma nova referência co-venda para contratar um vendedor da Microsoft, receber referências do vendedor da Microsoft, aceitar/recusar referências, modificar dados de negócio como valor de negócio e data de encerramento. Também pode receber quaisquer atualizações dos vendedores da Microsoft nestas ofertas de Co-venda. Pode gerir todas as suas referências no CRM à sua escolha e não no Partner Center. 

A solução baseia-se na Solução de Automatização de Energia da Microsoft e utiliza APIs do Partner Center.

## <a name="before-you-install---pre-requisites"></a>Antes de instalar - pré-requisitos

|**Tópicos**   |**Detalhes**   |**Ligações**   |
|--------------|--------------------|------|
|ID da rede de parceiros da Microsoft |Precisa de um ID MPN válido|Para se juntar à [MPN](https://partner.microsoft.com/)|
|Co-vender pronto|A sua solução IP/Serviços tem de ser co-vendida.|[Venda com a Microsoft](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|Conta do Centro de Parceiros|O ID MPN associado ao inquilino do Centro De Parceiros deve ser o mesmo que o ID MPN associado à sua solução de Co-venda. Verifique se consegue ver as suas referências de co-venda no portal Partner Center antes de implantar os conectores.|[Gerir a sua conta](create-user-accounts-and-set-permissions.md)|
|Funções de utilizador do Partner Center|O empregado que vai instalar e usar os conectores deve ser um administrador de referências|[Assign users roles and permissions](create-user-accounts-and-set-permissions.md) (Atribuir funções e permissões de utilizador)| 
|Dinâmica 365 CRM|A função de utilizador crm é administrador do sistema ou personalizador do sistema|[Atribuir funções na Dynamics 365](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|Conta de fluxo de automatização de energia|Criar um novo ambiente de produção com base de dados para teste/encenação e produção. Se tiver um ambiente de produção existente com base de dados, pode ser reutilizada. O utilizador que vai instalar a solução de conector precisa de ter licença Power Automamate e acesso a este ambiente. Pode monitorizar o progresso e obter mais detalhes caso a instalação falhe no [PowerUto,](https://flow.microsoft.com/) clicando em Ver histórico em Soluções.|[Criar ou gerir o ambiente](/power-platform/admin/create-environment#create-an-environment-with-a-database)|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a>Instalar Referências do Centro de Parceiros Sincronização para Dinâmica 365 (Solução de Automatização de Potência)

1. Vá ao [Power Automamate](https://flow.microsoft.com) e selecione **Ambientes** no canto superior direito. Este passo irá mostrar-lhe as instâncias de CRM disponíveis.

2. Selecione a instância CRM apropriada a partir da queda no canto superior direito.

3. Selecione **Soluções** na barra de navegação esquerda.

4. Clique no link **Open AppSource** no menu superior.

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Open AppSource":::

5. Procure por **Conectores de Referências do Centro de Parceiros para Dinâmicas365** no ecrã pop-up.  

6. Clique no botão **Get it now** e, em seguida, **Continue**.

7. Isto abre a página onde pode selecionar o ambiente CRM (Dynamics 365) para instalar a aplicação.  Concorde com os termos e condições.

8. Pode monitorizar o progresso e obter mais detalhes caso a instalação falhe no PowerUto, clicando em **Ver histórico** em **Soluções**.
 

9. Assim que a instalação estiver concluída, volte a navegar para [o Power Automamate](https://flow.microsoft.com) e selecione **Soluções** da área de navegação à esquerda. Note que **a Sincronização de Referências do Centro de Parceiros para a Dinâmica 365** está disponível na lista de Soluções.

10. Selecione **Partner Center Referencias Synchronization for Dynamics 365**. Estão disponíveis os seguintes fluxos e entidades power-automamate:

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="CRMs disponíveis":::

## <a name="best-practice-test-before-you-go-live"></a>Melhores práticas: teste antes de ir ao vivo

Antes de instalar, configurar e personalizar a solução Power Automamate no ambiente de produção, certifique-se de testar a solução numa fase de CRM de encenação.

- Instale a solução Microsoft Power Automate num ambiente de preparação/instância CRM.
- Configure e personalize a solução Microsoft Power Automamate em ambiente de encenação.
- Teste a solução numa fase de encenação/CRM. 
- Quanto ao sucesso, importa como solução gerida para o caso de produção. 

## <a name="configure-the-solution"></a>Configure a solução

1. Depois de ter instalado a solução no seu caso CRM, volte a navegar para [Power Automamate](https://flow.microsoft.com/).


2. A partir do **drop-down Do Ambiente** no canto superior direito, selecione a instância CRM onde instalou a solução Power Automamate.

3. Terá de criar ligações que associem as três contas de utilizador:

   - Utilizador do Partner Center com credenciais de administração de referências

   - Eventos do Centro de Parceiros

   - Administração CRM com o Power Automamate flui na solução.

      1. Selecione **Ligações** da barra de navegação esquerda e selecione a solução **de Referências do Centro parceiro** da lista.

      2. Criar uma ligação clicando **Criar uma ligação**.

         :::image type="content" source="images/cosellconnectors/dynamics-1.png" alt-text="Criar ligação":::

      3. Procure **referências ao Centro de Parceiros (pré-visualização)** na barra de pesquisa no canto superior direito.

      4. Crie uma ligação para o utilizador do Centro de Parceiros com o papel de credenciais da administração de referências.

      5. Em seguida, crie uma ligação Partner Center Events para o seu utilizador Partner Center com as credenciais de administração de referências.

      6. Criar uma ligação para o Serviço Comum de Dados (ambiente atual) para o utilizador administrador de CRM.
     
      7. Uma vez adicionadas todas as Ligações, deverá ver as seguintes Ligações no seu ambiente:

         :::image type="content" source="images/cosellconnectors/dynamics-2.png" alt-text="Ligações":::
   
## <a name="edit-the-connections"></a>Editar as ligações

1. Volte à página **Soluções** e selecione **Solução Padrão.** Selecione **Referência de Ligação (pré-visualização)** clicando **em Tudo**.

   :::image type="content" source="images/connection-reference-video.gif" alt-text="Edição das ligações":::

2. Edite cada uma das Ligações uma a uma selecionando o ícone de três pontos. Adicione as ligações relevantes.

   :::image type="content" source="images/cosellconnectors/dynamics-4.png" alt-text="Ligações listadas"::: 

3.  Volte à página Soluções, selecione Partner Center Referrals Synchronization for Dynamics 365 e ligue o fluxo clicando em três pontos ícone ao lado de cada fluxo na seguinte sequência. Se encontrar problemas ao ligar o fluxo, consulte [os passos](connector-dynamics.md#customize-synchronization-steps) de personalização e [os passos de resolução de problemas](connectors-troubleshoot.md). 

Ligue os fluxos na seguinte sequência:

- Registo Webhook do Partner Center (Visualização privilegiada)
- Criar Co-venda Referência - Dinâmica 365 para Partner Center (Visualização insider)
- [Personalizar] Criar ou obter detalhes do fluxo Dynamics 365 
- Centro de Parceiros para Dinâmica 365 - Ajudante (Visualização insider)
- Partner Center Microsoft Co-sell Referral Updates to Dynamics 365 (Visualização insider)
- Centro de Parceiros para Dinâmica 365 (Visualização insider)
- Dinâmica 365 para Partner Center (Visualização insider)
- Dinâmica 365 Oportunidade para Partner Center (Visualização insider)
- Dinâmica 365 Soluções Microsoft para Partner Center (Visualização insider)
 

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Utilize APIs webhook para se registar para eventos de mudança de recursos

As APIs do Partner Center Webhook permitem-lhe registar-se para eventos de alteração de recursos. Estes eventos de alteração são enviados para o seu url como posts HTTP.

1. Selecione **Partner Center para Dynamics 365 (Visualização insider)**.

2. Selecione o ícone **Editar** e selecione **Quando um pedido HTTP for recebido**.

3. Selecione o ícone **Copy** para copiar o URL HTTP POST fornecido.

   :::image type="content" source="images/webhook-video.gif" alt-text="Use webhooks para registar alterações de recursos":::

4. Selecione o fluxo de automatização do "Partner Center Webhook "Insider Preview)" e, em seguida, selecione **Executar**.

5. Certifique-se de que a janela "Run Flow" se abre no painel direito e clique em **Continuar**.

6. Introduza os seguintes detalhes:

   - **Http Trigger Endpoint**: URL copiado do passo anterior

   - **Eventos a Registar**: Selecione todos os eventos disponíveis ("referenciação-criada", "referenciada", "relacionada com referências criadas", "relacionadas com a referenciação")

   -**Sobrepor os pontos finais do gatilho existentes se estiver presente**: Sim, é importante notar que apenas um URL pode ser registado para um determinado evento webhook. É importante notar que apenas um URL pode ser registado para um determinado evento webhook. 

7. Selecione **Executar** e, em seguida, selecione **Fazer.**

O webhook pode agora ouvir criar e atualizar eventos.

## <a name="customize-synchronization-steps"></a>Personalizar etapas de sincronização

Os sistemas CRM são altamente personalizados e pode personalizar a solução Power Automate com base na sua configuração CRM.  Quando as referências de Co-venda são sincronizadas entre o Partner Center e o seu sistema CRM, os campos sincronizados no Partner Center PC estão listados no [guia de mapeamento de campo personalizado.](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S)

Siga o guia de mapeamento de campo e, se necessário, faça as alterações apropriadas em [Personalizar] Criar ou Obter Detalhes a partir de variáveis de fluxo ou ambiente **Dynamics 365.** Recomenda-se que não atualize quaisquer outros fluxos na solução Power Automamate, uma vez que pode ter impacto em futuras atualizações de soluções. 

Seguem-se as personalizações disponíveis:

- Ver marca no nome Opportunity: Por predefinição, será apresentada uma marca de verificação ao lado do nome Opportunity para indicar que a sincronização entre Partner Center e Dynamics 365 CRM está a acontecer com sucesso. Da mesma forma, será exibida uma marca cruzada se a sincronização falhar. Para evitar adicionar verificação ou marca cruzada no nome Opportunity, desaveie o valor atual da marca de verificação do Display na variável ambiente de nome de oportunidade para Nº.

- Valor do negócio: Por padrão, o valor da oferta do Partner Center será sincronizado de e para o **valor estimado** em CRM. Se tiver um campo diferente em CRM para o valor da transações para sincronizar a partir de:

  a. Atualizar O nome do campo de valor do negócio na variável ambiente Dynamics 365 com o nome de campo do CRM. Note que deve fornecer o nome do campo e não o seu nome de exibição.

  b. Editar **[Personalizar] Criar ou Obter Detalhes a partir do fluxo Dynamics 365**  e navegar para **criar ou atualizar** oportunidade em CRM e atualizar Criar uma nova **oportunidade** e atualizar as ações de **oportunidade existentes** para atribuir valor **DealValue** ao campo correto em CRM. Além disso, remova a **atribuição DealValue** do campo **Receitas Estimadas.**

- Código de país de conta de cliente: É obrigatório fornecer um código de país de duas letras (ISO 3166) ao criar uma nova remessa. Por predefinição, o código de país será sincronizado de e para o campo address1_country da Conta em CRM. Se tiver um campo diferente em CRM para o código do país sincronizar a partir de:

   a. Para um campo de código de país não-procurada em Conta que contenha código de duas letras:

   - Atualizar nome de campo de código de conta de cliente na variável ambiente Dynamics 365 com o nome de campo do CRM. Note que deve fornecer o nome do campo e não o seu nome de exibição.

   - Editar **[Personalizar] Criar ou Obter Detalhes a partir do fluxo Dynamics 365**  e navegar para criar ou obter conta de cliente em ação CRM para atribuir valor country ao campo correto em CRM. Além disso, remova a atribuição de valor do país do Endereço 1: Campo país/região.

   b. Para um campo de código de país baseado em procura na conta:

   - Adicione um novo campo personalizado em Conta e preencha-o automaticamente com código de país de duas letras (ISO 3166) com base no valor selecionado no campo baseado em procura e vice-versa.

   - Siga os passos acima para o campo de código do país não-lookup para sincronizar novo campo personalizado de CRM de e para o Partner Center.

- Campos de oportunidade: Se existirem campos obrigatórios em Opportunity que precisam de ser povoados **editar [Personalizar] Criar ou Obter Detalhes da Dinâmica 365 fluem**  e navegar para **criar ou atualizar oportunidade** em CRM e atualizar Criar uma nova **ação de oportunidade** para atribuir valores aos campos obrigatórios com base nos requisitos do seu negócio.

- Campos de chumbo: Se existirem campos obrigatórios no Lead que precisam de ser povoados **editar [Personalizar] Criar ou Obter Detalhes da Dinâmica 365 fluir**  e navegar para **criar ou atualizar chumbo** em CRM e atualizar Criar uma nova **ação de chumbo** para atribuir valores aos campos obrigatórios com base nos requisitos do seu negócio.

- Conta do Cliente: Quando uma nova referência é sincronizada do Partner Center para CRM, a solução Power Automamate tenta procurar uma conta existente em CRM utilizando o nome da empresa do cliente e o código postal. Se não encontrar uma, será criada uma nova conta de cliente em CRM. Para atualizar os critérios de pesquisa e novos detalhes de criação de conta, **editar [Personalizar] Criar ou Obter Detalhes a partir do fluxo Dynamics 365** e navegar para **criar ou obter conta de cliente** em CRM e Criar **ação de conta de cliente.**

## <a name="update-environment-variable"></a>Atualizar variável de ambiente

Para atualizar um valor variável ambiental:

1. Aceda à página **Soluções** e selecione **Solução Padrão.** Selecione **Variável ambiente** clicando em Tudo.

2. Selecione a variável ambiente para o valor que precisa de ser atualizado e clique em **Editar** usando três pontos ícone.

3. Atualizar **Valor Corrente** (não atualizar Valor Predefinido) utilizando nova opção de **valor** e fornecer o valor. O valor deve coincidir com o tipo de Dados da variável para, por exemplo, Sim/Nenhum tipo de dados aceitará ou sim ou não.

   :::image type="content" source="images/environment-variables-video.gif" alt-text="Atualizar variáveis ambientais":::

- Sincronização de co-venda bidis de ponta a ponta

Uma vez instalada, configurada e personalizada a solução Power Automate, pode testar a sincronização de referências de Co-venda entre a Dynamics 365 e o Partner Center.

### <a name="pre-requisites"></a>Pré-requisitos

Para sincronizar as referências através do Partner Center e Dynamics 365 CRM, a solução Power Automamate demarca claramente os campos de referência específicos da Microsoft. Esta identificação dá às suas equipas de vendedor a possibilidade de decidir quais as referências que querem partilhar com a Microsoft para co-venda.

Um conjunto de campos e objetos personalizados será adicionado como parte da instalação da solução. Um utilizador de administração CRM terá de criar uma secção de CRM separada com os campos personalizados **Opportunity.**

Os seguintes campos personalizados devem fazer parte da secção CRM:

- **Sincronizar com o Partner Center**: Se sincronizar a oportunidade com o Microsoft Partner Center. Por padrão, o valor deste campo é Não e precisa de ser explicitamente definido para Sim pelo seu vendedor para partilhar uma oportunidade com a Microsoft. Novas referências partilhadas do Partner Center para CRM terão este valor de campo definido para Sim.

- **Identificador** de referência : Um campo de identificação apenas de leitura para referência do Microsoft Partner Center

- **Link de referência**: Um link apenas de leitura para a referência no Microsoft Partner Center
- **Como pode a Microsoft ajudar?** Para criar uma referência de co-venda, selecione a ajuda adequada necessária à Microsoft. Um contacto com o cliente deve ser associado à Oportunidade de criar uma referência de co-venda. Para criar uma referência não co-venda deixe este campo não selecionado. Uma referência não co-venda pode ser convertida para uma referência de co-venda a qualquer momento, selecionando a opção de ajuda adequada exigida.

- **Visibilidade de referência do Microsoft Partner Center**: Selecione a visibilidade para o Microsoft Partner Center Referral. Ao torná-lo visível para os vendedores da Microsoft, uma referência não co-venda pode ser convertida para co-vender. Quando a ajuda da Microsoft é necessária, a referência é visível para os vendedores da Microsoft por padrão. Uma vez marcado como visível este campo não pode ser revertido.

- **Identificador de CRM da Microsoft**: Quando uma referência de co-venda é criada e aceite pela Microsoft, este campo será preenchido com o identificador CRM da Microsoft.

- **Produtos: Obsoleto** – não utilize este campo ou adicione-o à secção CRM, está disponível apenas para retrocompatibilidade. Utilize, em vez disso, soluções do Microsoft Partner Center.

- **Auditoria**: Um rasto de auditoria só de leitura para sincronização com referências do Partner Center

- **Microsoft Partner Center Solutions**: Um objeto personalizado para associar soluções prontas de Co-venda ou soluções Microsoft com a oportunidade. Uma ou mais soluções podem ser adicionadas e/ou removidas da Oportunidade. É obrigatório adicionar pelo menos uma solução de Co-venda pronta ou microsoft à Oportunidade antes de partilhá-la com a Microsoft. Para associar este objeto ao Opportunity, atualize o formulário Oportunidade em CRM:

  Selecione o separador apropriado no formulário Opportunity e adicione uma sub-grelha como mostrado abaixo:

  :::image type="content" source="images/cosellconnectors/dynamics-6.png" alt-text="Forma de oportunidade":::

  :::image type="content" source="images/cosellconnectors/dynamics-7.png" alt-text="{alt-text}":::

- Depois de adicionar as Soluções Microsoft, pode pré-povoar detalhes de soluções prontas para que os seus vendedores não tenham de as adicionar. Para adicionar um novo detalhe de solução, vá ao objeto Microsoft Solution Details em CRM e clique no **Add Record** para adicionar uma entrada ou utilizar o upload **do Excel** para adicionar várias entradas.

  :::image type="content" source="images/dynamic-1a.png" alt-text="Detalhes da solução":::

### <a name="scenarios"></a>Cenários:

1. Sincronização de encaminhamento quando a referência é criada ou atualizada em CRM e sincronizada no Partner Center:

   1. Inscreva-se no ambiente Dynamics 365 CRM com o utilizador que tenha visibilidade na secção **Oportunidade** do CRM.

   2. Certifique-se de que a secção Microsoft Partner Center está presente quando criar uma "Nova Oportunidade" no ambiente Dynamics 365

   :::image type="content" source="images/dynamic-2a.png" alt-text="Nova oportunidade"::: 

   3. Para sincronizar esta oportunidade com o Partner Center, certifique-se de que define os seguintes campos na vista do cartão:

      - **Como pode a Microsoft ajudar?**: Para criar uma referência de Co-venda selecione uma opção de ajuda apropriada.

         :::image type="content" source="images/dynamic-3a.png" alt-text="Como obter campos apropriados na vista do cartão":::

      - **Contacto com o Cliente**: Para criar uma referência de Co-venda, adicione um contacto do cliente ao Opportunity.

      - **Sincronização com o Centro de Parceiros**: Sim

      - Microsoft Solutions: Para partilhar uma referência com a Microsoft, adicione uma solução de Co-venda válida pronta ou microsoft ao Opportunity.
       
      
      :::image type="content" source="images/dynamic-4a.png" alt-text="ID da Solução":::

   4. Uma vez criada a oportunidade na Dynamics 365 com a opção Sync com Partner Center definida para Sim, aguarde 10 minutos e, em seguida, inscreva-se na sua conta Partner Center. As suas referências serão sincronizadas com a Dynamics 365 e o Referral Identifier. O Link de Referência será preenchido. Em caso de falha, o campo de auditoria será preenchido com informações de erro.
     
    5. Da mesma forma, para uma oportunidade que teve a opção "Sync with Partner Center" definida como "Sim", se atualizar a oportunidade na Dynamics 365 CRM, as alterações serão sincronizadas na sua conta Partner Center.

    6. As oportunidades sincronizadas com sucesso com o Partner Center serão identificadas com ✔icon in Dynamics 365.

2. Sincronização de referência quando a referência é criada ou atualizada no Microsoft Partner Center e sincronizada no ambiente Dynamics 365:

   1. Inscreva-se no painel do Centro de [Parceiros.](https://partner.microsoft.com/dashboard/home)

   2. Selecione **Referências** no menu à esquerda.

   3. Crie uma nova referência de Co-venda do Partner Center selecionando a opção **New deal.**

   4. Inscreva-se no ambiente Dynamics 365 CRM.

   5. Navegue para **oportunidades abertas.** A referência criada no Microsoft Partner Center está agora sincronizada na Dynamics 365 CRM.

   6. Quando seleciona uma referência sincronizada, os dados da visualização do cartão são preenchidos.

## <a name="next-steps"></a>Passos seguintes

- [Gerir oportunidades potenciais](manage-leads.md)

- [Gerir oportunidades de venda conjunta](manage-co-sell-opportunities.md)

- [Mais sobre a plataforma Microsoft Power Automate?](/power-automate/)

- [Webhooks do Centro de Parceiros](/partner-center/develop/partner-center-webhooks)
