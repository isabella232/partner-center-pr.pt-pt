---
title: O conector de co-venda para Dynamics 365 CRM Partner Center
description: Sincronizar referências no Partner Center com o seu conector de co-venda para Dynamics 365 CRM. Em seguida, pode co-vender com a Microsoft a partir do seu sistema CRM.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-referrals
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.date: 09/27/2021
ms.openlocfilehash: 4b89db5a93ce40eff73bc22d47e82841997d499f
ms.sourcegitcommit: d731813da1d31519dc2dc583d17899e5cf4ec1b2
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/27/2021
ms.locfileid: "129072370"
---
# <a name="co-sell-connector-for-dynamics-365-crm-overview"></a>Conector de co-venda para visão geral da Dynamics 365 CRM

**Funções adequadas**: Administração de referências | Administrador de sistema ou personalizador de sistema no CRM

Os conectores do Partner Center permitem que os seus vendedores co-vendam com a Microsoft a partir dos sistemas do seu sistema de relacionamento com o cliente (CRM). Não terão de ser treinados para usar o Partner Center para gerir negócios de co-venda. Utilize os conectores co-venda para criar uma nova referência de co-venda para:

- Engatar um vendedor da Microsoft
- Receber referências do vendedor da Microsoft
- Aceitar ou recusar referências
- Modificar dados de negócios como o valor do negócio e a data de encerramento 
 
Também pode receber quaisquer atualizações dos vendedores da Microsoft nestas ofertas de co-venda. Pode gerir todas as suas referências no CRM à sua escolha e não no Partner Center.

A solução baseia-se em Power Automate e utiliza APIs do Partner Center.

## <a name="prerequisites"></a>Pré-requisitos

Antes de instalar a solução, certifique-se de que cumpre os seguintes requisitos.

| Tópicos   | Detalhes   | Ligações   |
|--------------|--------------------|------|
| Microsoft Partner Network (MPN) ID |Precisa de uma identificação de MPN válida. | [Junte-se à Rede de Parceiros](https://partner.microsoft.com/) |
| Co-venda pronta|A sua solução IP/Serviços tem de ser co-vendida. | [Venda com a Microsoft](https://partner.microsoft.com/membership/sell-with-microsoft) |
| Conta do Centro de Parceiros | O ID MPN associado ao inquilino do Centro De Parceiros deve ser o mesmo que o MPN ID associado à sua solução de co-venda. Verifique se consegue ver as suas referências de co-venda no portal Partner Center antes de implementar os conectores. | [Gerir a sua conta](create-user-accounts-and-set-permissions.md) |
| Funções de utilizador do Partner Center | O empregado que instalar e utilizar os conectores deve ser um administrador de referências.|[Assign users roles and permissions](create-user-accounts-and-set-permissions.md) (Atribuir funções e permissões de utilizador) |
| Dinâmica 365 CRM|A função de utilizador crm é administração do sistema ou personalização do sistema.|[Atribuir funções na Dynamics 365](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization) |
| conta de fluxo Power Automate|Criar um novo ambiente de produção com base de dados para testes, encenação e produção. Se tiver um ambiente de produção existente com base de dados, pode ser reutilizado. O utilizador que vai instalar a solução de conector deve ter uma licença Power Automate e acesso a este ambiente. Pode monitorizar o progresso e obter mais informações em [Power Automate](https://flow.microsoft.com/) se a instalação falhar. Selecione **Ver histórico** em **Soluções**. | [Criar ou gerir o ambiente](/power-platform/admin/create-environment#create-an-environment-with-a-database) |

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a>Instalar Sincronização de referências do Centro de Parceiros para dinâmicas 365 (solução Power Automate)

1. Vá a [Power Automate](https://flow.microsoft.com)e selecione **Ambientes** no canto superior direito. Este passo irá mostrar-lhe as instâncias de CRM disponíveis.

2. Selecione a instância crm apropriada da lista de recuos no canto superior direito.

3. Selecione **Soluções** à esquerda.

4. Selecione o link **Open AppSource** no menu superior.

   :::image type="content" source="images/cosellconnectors/open-appsource.png" alt-text="Screenshot que mostra Open AppSource.":::

5. Procure por **Conectores de Referências do Centro de Parceiros para Dinâmicas 365** no ecrã pop-up.  

6. Selecione o botão **Get-it now** e, em seguida, selecione **Continue**.

7. Aparece uma página onde pode selecionar o ambiente CRM (Dynamics 365) para instalar a aplicação. Concorde com os termos e condições.

8. Pode monitorizar o progresso e, se a instalação falhar, poderá obter mais detalhes em Power Automate selecionando **Ver histórico** em **Soluções**.

9. Depois de concluída a instalação, volte a [Power Automate](https://flow.microsoft.com) e selecione **Soluções** à esquerda. **Partner Center Referencias Synchronization for Dynamics 365** está agora disponível na lista **de Soluções.**

10. Selecione **Partner Center Referencias Synchronization for Dynamics 365**. Estão disponíveis os seguintes fluxos e entidades Power Automate.

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="Screenshot que mostra CRMs disponíveis.":::

## <a name="test-before-you-go-live"></a>Teste antes de ir ao vivo

Antes de instalar, configurar e personalizar a solução Power Automate no ambiente de produção, teste a solução numa fase de CRM de encenação. Vai precisar de:

- Instale a solução Power Automate num ambiente de preparação de CRM.
- Configure e personalize a solução Power Automate num ambiente de preparação.
- Teste a solução numa fase de CRM de encenação.
- Após um teste bem sucedido, importa como solução gerida para o caso de produção.

## <a name="configure-the-solution"></a>Configure a solução

1. Depois de ter instalado a solução no seu caso crm, volte a [Power Automate](https://flow.microsoft.com/).

2. A partir da lista de **suspensos ambientes** no canto superior direito, selecione a instância CRM onde instalou a solução Power Automate.

3. Terá de criar ligações que associem as três contas de utilizador:

   - Utilizador do Partner Center com credenciais de administração de referências
   - Eventos do Centro de Parceiros
   - Administração de CRM com o Power Automate flui na solução

   a. Selecione **Ligações** à esquerda e selecione a solução **'Referências do Centro parceiro'** da lista.

   b. Criar uma ligação selecionando **Criar uma ligação**.

      :::image type="content" source="images/cosellconnectors/dynamics-1.png" alt-text="Screenshot que mostra Criar uma ligação.":::

   c. Procure **referências ao Centro de Parceiros (pré-visualização)** na barra de pesquisa no canto superior direito.

   d. Crie uma ligação para o utilizador do Centro de Parceiros com o papel de credenciais da administração de referências.

   e. Em seguida, crie uma ligação Partner Center Events para o seu utilizador Partner Center com as credenciais de administração de referências.

   f. Criar uma ligação para o Serviço Comum de Dados (ambiente atual) para o utilizador administrador de CRM.
     
   exemplo, Depois de ter adicionado todas as ligações, deverá ver as seguintes ligações no seu ambiente.

      :::image type="content" source="images/cosellconnectors/dynamics-2.png" alt-text="Screenshot que mostra ligações.":::

## <a name="edit-the-connections"></a>Editar as ligações

1. Volte à página **Soluções** e selecione **Solução Padrão.** Selecione **Referência de Ligação (pré-visualização)** selecionando **All**.

   :::image type="content" source="images/connection-reference-video.gif" alt-text="Screenshot que mostra a edição das ligações.":::

2. Edite cada uma das ligações individualmente selecionando o ícone elipse. Adicione as ligações relevantes.

   :::image type="content" source="images/cosellconnectors/dynamics-4.png" alt-text="Screenshot que mostra ligações listadas.":::

3. Volte à página Soluções, selecione **Partner Center Referrals Synchronization for Dynamics 365**, e ligue o fluxo selecionando o ícone de elipses ao lado de cada fluxo na seguinte sequência.  Se encontrar problemas enquanto liga o fluxo, consulte os passos de [personalização](connector-dynamics.md#customize-synchronization-steps) e [os passos de resolução de problemas](connectors-troubleshoot.md).

   Ligue os fluxos na seguinte sequência:

   a. Registo Webhook do Partner Center (Visualização privilegiada)
   
   b. [Personalizar] Criar ou obter detalhes do fluxo Dynamics 365
   
   c. Criar Co-venda Referência - Dinâmica 365 para Partner Center (Visualização insider)
   
   d. Centro de Parceiros para Dinâmica 365 - Ajudante (Visualização insider)
   
   e. Partner Center Microsoft Co-sell Referral Updates to Dynamics 365 (Visualização insider)
   
   f. Centro de Parceiros para Dinâmica 365 (Visualização insider)
   
   exemplo, Dinâmica 365 para Partner Center (Visualização insider)
   
   h. Dinâmica 365 Oportunidade para Partner Center (Visualização insider)
   
   i. Dinâmica 365 Soluções Microsoft para Partner Center (Visualização insider)
 
## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Utilize apis webhook para se registar para eventos de mudança de recursos

Pode utilizar as APIs do Partner Center webhook para se registar para eventos de mudança de recursos. Estes eventos de alteração são enviados para o seu URL como posts HTTP.

1. Selecione **Partner Center para Dynamics 365 (Visualização insider)**.

2. Selecione o ícone **Editar** e selecione **Quando um pedido HTTP for recebido**.

3. Selecione o ícone **Copy** para copiar o URL HTTP POST fornecido.

   :::image type="content" source="images/webhook-video.gif" alt-text="Screenshot que mostra a utilização de webhooks para registar alterações de recursos.":::

4. Selecione o **Registo webhook do Centro de Parceiros (Visualização de Insider)** Power Automate fluxo e, em seguida, selecione **Executar**.

5. Certifique-se de que a janela **de fluxo de funcionação** se abre no painel direito e selecione **Continue**.

6. Introduza os seguintes detalhes:

   - **Http Trigger Endpoint**: Este URL foi copiado de um passo anterior.
   - **Eventos a Registar**: Selecione todos os eventos disponíveis ( criados por **encaminhamento,** **referenciação,** **criados por referências relacionadas** e **atualizados com referências relacionadas).**
   - **Substitua os pontos finais do gatilho existentes se estiver presente?** Apenas um URL pode ser registado para um determinado evento webhook.

7. Selecione **executar o fluxo** e, em seguida, selecione **Fazer.**

O webhook pode agora ouvir, criar e atualizar eventos.

## <a name="customize-synchronization-steps"></a>Personalizar etapas de sincronização

Os sistemas CRM são altamente personalizados e pode personalizar a solução Power Automate com base na sua configuração crm. Quando as referências de co-venda são sincronizadas entre o Partner Center e o seu sistema CRM, os campos sincronizados no Pc partner Center estão listados no [guia de mapeamento de campo personalizado](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S).

Siga o guia de mapeamento de campo e, se necessário, faça as alterações apropriadas em [Personalizar] Criar ou Obter Detalhes a partir de variáveis de fluxo ou ambiente **dynamics 365.** Não atualize quaisquer outros fluxos na solução Power Automate porque pode afetar futuras atualizações de soluções.

Estão disponíveis as seguintes personalizações:

- **Mostrar a marca de verificação no nome de oportunidade**: Por padrão, será apresentada uma marca de verificação ao lado do nome de oportunidade para indicar que a sincronização entre Partner Center e Dynamics 365 CRM está a acontecer com sucesso. Da mesma forma, será exibida uma marca cruzada se a sincronização falhar. Para evitar adicionar uma marca de verificação ou cruz no nome de oportunidade, desaveie o valor atual da marca de **verificação do Display na** variável ambiente de nome de oportunidade para Nº.
- **Valor do negócio**: Por defeito, o valor da oferta do Partner Center será sincronizado de e para `estimatedvalue` o CRM. Se tiver um campo diferente no CRM para que o valor do negócio se sincronize a partir de:

  - Atualize o nome do campo **de valor do Negócio** na variável ambiente Dynamics 365 com o nome de campo do CRM. Certifique-se de que fornece o nome do campo, não o seu nome de exibição.
  - Editar **[Personalizar] Criar ou Obter Detalhes a partir do fluxo Dynamics 365**, e ir para **criar ou atualizar oportunidade** em CRM e atualizar Criar uma nova **oportunidade** e atualizar as ações de **oportunidade existentes** para atribuir o valor **DealValue** ao campo correto no CRM. Além disso, remova a atribuição **DealValue** do campo **Receita Estimada.**

- **Código de país da conta do cliente**: Tem de fornecer um código de países de duas letras (ISO 3166) quando criar uma nova referência. Por predefinição, o código de país será sincronizado de e para o campo **address1_country** da conta no CRM. Se tiver um campo diferente no CRM para que o código do país sincronize a partir de:

  - Para um campo de código de país não ligado na conta que contém um código de duas letras, atualize o nome do código de país de **conta de cliente** na variável ambiente Dynamics 365 com o nome de campo do CRM. Certifique-se de que fornece o nome do campo, não o seu nome de exibição. Editar **[Personalizar] Criar ou Obter Detalhes a partir do fluxo Dynamics 365,** e ir para **criar ou obter conta de cliente** na ação CRM para atribuir um valor **país** ao campo correto no CRM. Além disso, **remova** a atribuição de valor país do **campo Endereço 1: Campo país/região.**

  - Para um campo de código de país baseado em procura na conta, adicione um novo campo personalizado na conta e a povoe-o automaticamente com um código de país de duas letras (ISO 3166) com base no valor selecionado no campo baseado em procura e vice-versa. Siga os passos anteriores para o campo de código country não-ookup para sincronizar um novo campo personalizado do CRM de e para o Partner Center.

- **Campos de oportunidades**: Se existirem campos obrigatórios em **Opportunity** que precisam de ser povoados, **edite [Personalizar] Criar ou Obter Detalhes da Dinâmica 365 flow** e ir para **Criar ou atualizar oportunidade** no CRM e atualizar Criar uma **nova ação de oportunidade** para atribuir valores aos campos obrigatórios com base nos requisitos do seu negócio.
- **Campos de chumbo**: Se existirem campos obrigatórios em **Chumbo** que precisam de ser povoados, **edite [Personalizar] Criar ou Obter Detalhes da Dinâmica 365 flow** e ir para Criar ou atualizar **chumbo** no CRM e atualizar Criar uma **nova ação de chumbo** para atribuir valores aos campos obrigatórios com base nos requisitos do seu negócio.
- **Conta do cliente**: Quando uma nova referência é sincronizada do Partner Center para o CRM, a solução Power Automate tenta procurar uma conta existente no CRM utilizando o nome da empresa do cliente e o código postal. Se não encontrar uma, uma nova conta de cliente será criada no CRM. Para atualizar os critérios de pesquisa e novos detalhes de criação de conta, **editar [Personalizar] Criar ou Obter Detalhes a partir do fluxo Dynamics 365** e ir para **criar ou obter conta de cliente** na ação de conta de clientes CRM e **Criar.**

## <a name="update-environment-variable"></a>Atualizar variável de ambiente

Para atualizar um valor variável ambiental:

1. Aceda à página **Soluções** e selecione **Solução Padrão**. Selecione **a Variável ambiente** selecionando **All**.

2. Selecione a variável ambiente para o valor que precisa de ser atualizado e **selecione Editar** utilizando o ícone elipse.

3. Atualizar **O Valor Atual** (não atualizar o Valor **Padrão)** utilizando a opção De Novo **Valor** e fornecendo o valor. O valor deve corresponder ao tipo de dados da variável. Por exemplo, o tipo de dados Sim ou Não aceitará o valor Sim ou Não.

   :::image type="content" source="images/cosellconnectors/environment-variables-video.gif" alt-text="Screenshot que mostra atualização variáveis ambientais.":::

## <a name="end-to-end-bidirectional-co-sell-referral-synchronization"></a>Sincronização bidirecional de ponta a ponta

Depois de instalar, configurar e personalizar a solução Power Automate, pode testar a sincronização de referências de co-venda entre a Dynamics 365 e o Partner Center.

### <a name="prerequisites"></a>Pré-requisitos

Para sincronizar as referências através do Partner Center e dynamics 365 CRM, a solução Power Automate demarca claramente os campos de referência específicos da Microsoft. Esta identificação dá às suas equipas de vendedores a capacidade de decidir quais as referências que querem partilhar com a Microsoft para co-venda.

Um conjunto de campos e objetos personalizados será adicionado como parte da instalação da solução. Um utilizador de administração CRM terá de criar uma secção de CRM separada com os campos personalizados **Opportunity.**

Os seguintes campos personalizados devem fazer parte da secção CRM:

- **Sincronizar com o Partner Center**: Se sincronizar a oportunidade com o Partner Center. Por padrão, o valor deste campo é Nº e precisa de ser explicitamente definido para Sim pelo seu vendedor para partilhar uma oportunidade com a Microsoft. As novas referências partilhadas do Partner Center para o CRM terão este valor de campo definido para Sim.
- **Identificador de referência**: Um campo de identificação apenas de leitura para a referenciação do Centro de Parceiros.
- **Link de referência**: Uma ligação apenas de leitura para a referência no Centro de Parceiros.
- **Como pode a Microsoft ajudar?** Para criar uma referência de co-venda, selecione a ajuda adequada necessária à Microsoft. Um contacto com o cliente deve ser associado à oportunidade de criar uma referência de co-venda. Para criar uma referência não-co-venda, não selecione este campo. Uma referência não co-venda pode ser convertida para uma referência de co-venda a qualquer momento, selecionando a opção adequada para ajuda.
- **Visibilidade de referência do Microsoft Partner Center**: Selecione a visibilidade para a referenciação do Centro de Parceiros. Ao torná-lo visível para os vendedores da Microsoft, uma referência não co-venda pode ser convertida para co-vender. Quando a ajuda da Microsoft é necessária, a referência é visível para os vendedores da Microsoft por padrão. Depois deste campo ser marcado como visível, não pode ser revertido.
- **Microsoft CRM Identifier**: Quando uma referência de co-venda é criada e aceite pela Microsoft, este campo será preenchido com o identificador CRM da Microsoft.
- **Produtos: Obsoleto**: Não utilize este campo nem o adicione à secção CRM. Está disponível apenas para retrocompatibilidade. Utilize, em vez disso, soluções partner center.
- **Auditoria**: Um rasto de auditoria apenas para sincronização com referências do Partner Center.
- **Microsoft Partner Center Solutions**: Um objeto personalizado para associar soluções prontas de co-venda ou soluções Microsoft com a oportunidade. Uma ou mais soluções podem ser adicionadas ou removidas da oportunidade. É obrigatório adicionar pelo menos uma solução de co-venda pronta ou a solução Microsoft para a oportunidade antes de a partilhar com a Microsoft. Para associar este objeto à oportunidade, atualize o formulário **Oportunidade** no CRM.

  Selecione o separador apropriado no formulário **Oportunidade** e adicione uma subrede como mostrado aqui.

  :::image type="content" source="images/cosellconnectors/dynamics-6.png" alt-text="Screenshot que mostra o formulário Opportunity.":::

  :::image type="content" source="images/cosellconnectors/dynamics-7.png" alt-text="Screenshot que mostra Microsoft Solutions.":::

- Depois de adicionar soluções Microsoft, pode pré-vender detalhes da solução pronta para que os seus vendedores não tenham de as adicionar. Para adicionar um novo detalhe de solução, vá ao objeto Detalhes da solução da Microsoft no CRM e selecione **Add Record** para adicionar uma entrada ou utilizar **Excel upload** para adicionar várias entradas.

  :::image type="content" source="images/cosellconnectors/dynamics-solution-1.png" alt-text="Screenshot que mostra novos detalhes da solução da Microsoft.":::

## <a name="scenarios"></a>Cenários

### <a name="referral-synchronization-when-referral-is-created-or-updated-in-the-crm-and-synced-in-partner-center"></a>Sincronização de encaminhamento quando a referenciação é criada ou atualizada no CRM e sincronizada no Partner Center

   1. Inscreva-se no ambiente Dynamics 365 CRM com o utilizador que tem visibilidade na secção **Oportunidade** do CRM.

   2. Certifique-se de que a secção **Microsoft Partner Center** está presente quando criar uma nova oportunidade no ambiente Dynamics 365.

      :::image type="content" source="images/cosellconnectors/dynamics-solution-2.png" alt-text="Screenshot que mostra nova oportunidade.":::

   3. Para sincronizar esta oportunidade com o Partner Center, certifique-se de que define os seguintes campos na vista do cartão:

      - **Como pode a Microsoft ajudar?**: Para criar uma referência de co-venda, selecione uma opção de ajuda apropriada.

         :::image type="content" source="images/cosellconnectors/dynamics-solution-3.png" alt-text="Screenshot que mostra como obter campos apropriados na vista do cartão.":::

      - **Contacto com o Cliente**: Para criar uma referência de co-venda, adicione um contacto do cliente à oportunidade.
      - **Sincronização com o Centro de Parceiros:** Sim.
      - **Microsoft Solutions**: Para partilhar uma referência com a Microsoft, adicione uma solução de co-venda válida pronta ou microsoft à oportunidade.

        :::image type="content" source="images/cosellconnectors/dynamics-solution-4.png" alt-text="Screenshot que mostra O ID da Solução.":::

   4. Depois de a oportunidade ser criada na Dynamics 365 com a opção **Sync With Partner Center** definida para Sim, aguarde 10 minutos. Em seguida, inscreva-se na sua conta partner Center. As suas referências serão sincronizadas com a Dynamics 365 e **o Referral Identifier**. **O Link de Referência** será preenchido. Se houver uma falha, o campo **de Auditoria** será preenchido com informações de erro.

      1. Da mesma forma, para uma oportunidade que teve a opção **Sync With Partner Center** definida para Sim, se atualizar a oportunidade em Dynamics 365 CRM, as alterações serão sincronizadas na sua conta Partner Center.

      2. As oportunidades sincronizadas com sucesso com o Partner Center serão identificadas com ✔icon in Dynamics 365.

### <a name="referral-synchronization-when-the-referral-is-created-or-updated-in-partner-center-and-synchronized-in-the-dynamics-365-environment"></a>Sincronização de referência quando a referência é criada ou atualizada no Partner Center e sincronizada no ambiente Dynamics 365

   1. Inscreva-se no [painel do Partner Center](https://partner.microsoft.com/dashboard/home).

   2. Selecione o azulejo **de referências.**

   3. Crie uma nova referência de co-venda do Partner Center selecionando a opção **New deal.**

   4. Inscreva-se no ambiente Dynamics 365 CRM.

   5. Ir para **oportunidades abertas.** A referência criada no Partner Center está agora sincronizada em Dynamics 365 CRM.

   6. Quando seleciona uma referência sincronizada, os dados da visualização do cartão são preenchidos.

## <a name="next-steps"></a>Passos seguintes

- [Gerir oportunidades potenciais](manage-leads.md)

- [Gerir oportunidades de venda conjunta](manage-co-sell-opportunities.md)

- [Mais sobre a plataforma microsoft Power Automate](/power-automate/)

- [Webhooks do Centro de Parceiros](/partner-center/develop/partner-center-webhooks)
