---
title: O conector de co-venda para Salesforce CRM Partner Center
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Sincronizar as suas referências no Partner Center com o seu Salesforce CRM. Os vendedores podem então co-vender com a Microsoft a partir dos seus sistemas CRM.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.date: 06/28/2021
ms.openlocfilehash: f8cb4cd2488e55ab64cf7b7cdce4a3e950b266de
ms.sourcegitcommit: 6a6e8f9af0a58b32770c7fce9f567dd4795b9797
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/29/2021
ms.locfileid: "113029125"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a>Conector de co-venda para Salesforce CRM - visão geral

**Funções adequadas**: Administração de referências | Administrador de sistema ou personalizador de sistema no CRM

O conector partner Center co-sell permite que os seus vendedores co-vendam com a Microsoft a partir dos seus sistemas CRM. Não terão de ser treinados para usar o Partner Center para gerir os negócios de co-venda. Utilizando os conectores Co-sell, pode criar uma nova referência de Co-venda para contratar um vendedor da Microsoft, receber referências do vendedor da Microsoft, aceitar/recusar referências, modificar dados de negócios como o valor do negócio e a data de encerramento.  Também pode receber quaisquer atualizações dos vendedores da Microsoft nestas ofertas de Co-venda. Pode fazer todas as suas referências enquanto trabalha dentro do CRM à sua escolha e não no Partner Center.

A solução baseia-se na Solução de Automatização de Energia da Microsoft e utiliza APIs do Partner Center.

## <a name="before-you-install---pre-requisites"></a>Antes de instalar - pré-requisitos

|**Tópicos**|**Detalhes**|**Ligações**|
|--------------|--------------------|------|
|ID da rede de parceiros da Microsoft |Precisa de um ID MPN válido|Para se juntar à [MPN](https://partner.microsoft.com/)|
|Co-vender pronto|A sua solução IP/Serviços tem de ser co-vendida.|[Venda com a Microsoft](https://partner.microsoft.com/membership/sell-with-microsoft)|
|Conta do Centro de Parceiros|O ID MPN associado ao inquilino do Centro De Parceiros deve ser o mesmo que o ID MPN associado à sua solução de Co-venda. Verifique se consegue ver as suas referências de co-venda no portal Partner Center antes de implantar os conectores.|[Gerir a sua conta](create-user-accounts-and-set-permissions.md)|
|Funções de utilizador do Partner Center|O empregado que vai instalar e usar os conectores deve ser um administrador de referências|[Assign users roles and permissions](create-user-accounts-and-set-permissions.md) (Atribuir funções e permissões de utilizador)|
|Salesforce CRM|A função de utilizador crm é administrador do sistema ou personalizador do sistema|[Atribuir funções na Salesforce CRM](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|Conta de fluxo de automatização de energia|Criar um novo ambiente de produção com base de dados para testes, encenação e produção. Se tiver um ambiente de produção existente com base de dados, pode ser reutilizado. O utilizador que vai instalar a solução de conector deve ter uma licença Power Automamate e acesso a este ambiente. Pode monitorizar o progresso e obter mais informações no [Power Automamate](https://flow.microsoft.com/) se a instalação falhar. Selecione **Ver histórico** em **Soluções**.|[Criar ou gerir o ambiente](/power-platform/admin/create-environment#create-an-environment-with-a-database)|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a>Instalação do Pacote Salesforce para Campos Personalizados da Microsoft

Para sincronizar as referências através do Partner Center e da Salesforce CRM, a solução Power Automamate precisa de identificar claramente os campos de referência específicos da Microsoft. Esta demarcação proporciona às equipas de vendedores parceiros a capacidade de decidir quais as referências que querem partilhar com a Microsoft para co-venda.

1. Na Salesforce, ative **notas** e adicione-as à lista de oportunidades relacionadas. [Referência](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

1. Ativar **as equipas de Oportunidade** seguindo os passos:
    - Na configuração, utilize a caixa **De localização Rápida** para localizar as Definições da Equipa de Oportunidade.
    - Defina as definições conforme necessário. [Referência](https://help.salesforce.com/articleView?id=sf.opp_team_manage.htm&type=5)

1. No Salesforce, instale campos e objetos personalizados utilizando o [instalador de embalagens.](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV) Utilize este instalador para instalar a embalagem em qualquer empresa.

    >[!NOTE]
    >Se estiver a instalar-se numa caixa de areia, deve substituir a parte inicial do URL por `http://test.salesforce.com` .

1. Na Salesforce, adicione as Soluções Microsoft à lista relacionada com a **Oportunidade.** Uma vez adicionado, selecione o ícone da **chave** inglesa e atualize propriedades

## <a name="best-practice-test-before-you-go-live"></a>Melhores Práticas: Teste antes de ir ao vivo

Antes de instalar, configurar e personalizar a solução Power Automamate no ambiente de produção, certifique-se de testar a solução numa fase de CRM de encenação.

- Instale a solução Microsoft Power Automate num ambiente de preparação/instância CRM.

- Faça uma cópia da solução e execute a sua configuração e faça personalizações de fluxo power-automatizado no ambiente de preparação.

- Teste a solução numa fase de encenação/CRM.

- No que diz respeito ao sucesso, a importação como solução gerida para o caso de produção.

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a>Instalar Referências do Centro de Parceiros Sincronização para Salesforce CRM

1. Vá ao [Power Automamate](https://flow.microsoft.com) e selecione **Ambientes** no canto superior direito. Isto irá mostrar-lhe as instâncias de CRM disponíveis.

1. Selecione a instância crm apropriada da lista de recuos no canto superior direito.

1. Selecione **Soluções** na barra de navegação esquerda.

1. Selecione o link **Open AppSource** no menu superior.

   :::image type="content" source="images/cosellconnectors/open-appsource.png" alt-text="Open AppSource":::

1. Procure por **Conectores de Referências do Centro de Parceiros para Salesforce** no ecrã pop-up.  

   :::image type="content" source="images/salesforce/salesforce-get-it-now.png" alt-text="Screenshot de Get It Now.":::

1. Selecione o botão **Get it now** e, em seguida, selecione **Continue**.

1. Na página seguinte, selecione o ambiente DE CRM salesforce para instalar a aplicação. Concorde com os termos e condições.

1. Em seguida, é direcionado para a página **Gerir as suas soluções.**  Navegue para "Partner Center Referrals" utilizando os botões de seta na parte inferior da página. **A instalação programada** deve aparecer ao lado da solução de referências do Centro parceiro. A instalação levará 10-15 minutos.

1. Depois de concluída a instalação, volte a navegar para [o Power Automamate](https://flow.microsoft.com) e selecione **Soluções** da área de navegação à esquerda. Note que **a Sincronização de Referências do Partner Center para a Salesforce** já está disponível na lista de Soluções.

1. Selecione **Partner Center Referrals Synchronization for Salesforce**. Estão disponíveis os seguintes fluxos e entidades power-automamate:

   :::image type="content" source="images/cosellconnectors/partner-center-referrals-synchronization.png" alt-text="Fluxos de salesforce":::

## <a name="configure-the-solution"></a>Configure a solução

1. Depois de ter instalado a solução no seu caso CRM, volte a navegar para [Power Automamate](https://flow.microsoft.com/).

1. A partir do **drop-down dos Ambientes** no canto superior direito, selecione a instância CRM onde instalou a solução Power Automamate.

1. Terá de criar ligações que associem as três contas de utilizador:

   - Utilizador do Partner Center com credenciais de administração de referências
   - Eventos do Centro de Parceiros
   - Administração CRM com o Power Automamate flui na solução

   1. Selecione **Ligações** da barra de navegação esquerda e selecione a solução **de Referências do Centro parceiro** da lista.

   1. Criar uma ligação selecionando **Criar uma ligação**.

        :::image type="content" source="images/cosellconnectors/dynamics-1.png" alt-text="Screenshot que mostra Criar uma ligação.":::

   1. Procure **referências ao Centro de Parceiros (pré-visualização)** na barra de pesquisa no canto superior direito.

   1. Crie uma ligação para o utilizador do Centro de Parceiros com o papel de credenciais da administração de referências.

   1. Em seguida, crie uma ligação Partner Center Events para o seu utilizador Partner Center com as credenciais de administração de referências.

   1. Criar uma ligação para o Salesforce para o utilizador administrador crm.
  
   1. Crie uma ligação para o Microsoft Dataverse para o utilizador administrador crm.

   1. Depois de ter adicionado todas as Ligações, deverá ver as seguintes ligações no seu ambiente:

        :::image type="content" source="images/cosellconnectors/salesforce-connections.png" alt-text="Screenshot que mostra como observar ligações.":::

### <a name="edit-the-connections"></a>Editar as ligações

1. Volte à página **Soluções** e selecione **Solução Padrão.** Selecione **Referência de Ligação (pré-visualização)** clicando **em Tudo**.

   :::image type="content" source="images/connection-reference-video.gif" alt-text="Screenshot que mostra a edição das ligações.":::

1. Edite cada uma das Ligações individualmente selecionando o ícone elipse. Adicione as ligações relevantes.

   :::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="O atht screenshot mostra como editar conectores.":::

1. Ligue os fluxos na seguinte sequência:
   - Registo Webhook do Partner Center (Visualização privilegiada)
   - [Personalizar] Criar ou obter detalhes da Salesforce
   - Criar Co-vender Referral-Salesforce ao Partner Center (Visualização insider)
   - Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)  
   - Centro de Parceiros para Salesforce (Visualização de Insider)
   - Salesforce para Partner Center (Visualização insider)
   - Oportunidade Salesforce para Partner Center (Visualização insider)
   - Salesforce Microsoft Solutions to Partner Center (Visualização insider)

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Utilize APIs webhook para se registar para eventos de mudança de recursos

Pode utilizar as APIs do Partner Center webhook para se registar para eventos de mudança de recursos. Estes eventos de alteração são enviados para o seu URL como posts HTTP.

1. Selecione **Partner Center para Salesforce CRM (Visualização insider)**.

1. Selecione o **ícone Editar** e selecione **Quando um pedido HTTP for recebido**.

1. Selecione o ícone **Copy** para copiar o **URL HTTP POST** fornecido .

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="Screenshot que mostra como copiar o URL.":::

1. Selecione o fluxo de automatização de automatização do **Centro de Parceiros (Visualização de Insider)** e, em seguida, selecione **Executar**.

1. Certifique-se de que a janela **de fluxo de funcionação** se abre no painel direito e selecione **Continue**.

1. Introduza os seguintes detalhes:

   - **Http Trigger Endpoint**: Este URL foi copiado de um passo anterior.
   - **Eventos a Registar**: Selecione todos os eventos disponíveis **(criados por encaminhamento,** **referenciação,** **criados por referências relacionadas** e **atualizados com referências relacionadas).**
   - **Substitua os pontos finais do gatilho existentes se estiver presente?** Apenas um URL pode ser registado para um determinado evento webhook.

1. Selecione **fluxo de execução** e, em seguida, selecione **Fazer**.

O webhook pode agora ouvir, criar e atualizar eventos.

## <a name="customize-synchronization-steps"></a>Personalizar etapas de sincronização

Os sistemas CRM são altamente personalizados e pode personalizar a solução Power Automate com base na sua configuração CRM. Quando as referências de co-venda são sincronizadas entre o Partner Center e o seu sistema CRM, os campos sincronizados no Pc partner Center estão listados no [guia de mapeamento de campo personalizado](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S).

Siga o guia de mapeamento de campo e, se necessário, faça as alterações apropriadas em **[Personalizar] Criar ou Obter Detalhes de salesforce** ou variáveis ambientais. Não atualize quaisquer outros fluxos na solução Power Automamate porque pode afetar futuras atualizações de soluções.

Estão disponíveis as seguintes personalizações:

- **Mostrar a marca de verificação no nome de oportunidade**: Por predefinição, será apresentada uma marca de verificação ao lado do nome de oportunidade para indicar que a sincronização entre o Partner Center e o Salesforce CRM está a acontecer com sucesso. Da mesma forma, será exibida uma marca cruzada se a sincronização falhar. Para evitar adicionar uma marca de verificação ou cruz no nome de oportunidade, desave o valor atual da marca de **verificação do Display na** variável ambiente de nome de oportunidade para Nº.

- **Nome artístico:**

  - **Nome de palco ativo**: Este é o palco do oleoduto de venda de uma oportunidade na Salesforce.  Representa uma fase ativa e equivale a uma referência em estado aceite no Partner Center. Esta pode ser a próxima etapa do oleoduto de vendas após o estágio em espera. A fase de vendas da Moving Opportunity fora do palco on-hold em estágio ativo aceitará a referência no Partner Center e as alterações começarão a sincronizar.

  - **Nome do palco em espera**: Nome do palco no oleoduto de venda de uma oportunidade na Salesforce. Representa um palco em espera. Novas referências de co-venda partilhadas pela Microsoft que ainda não são aceites serão definidas para esta fase na Salesforce. Quaisquer alterações efetuadas numa oportunidade enquanto estiver em fase de espera não sincronizarão com o Partner Center. A fase de vendas da Moving Opportunity fora deste palco em espera aceitará a referência no Partner Center e as mudanças começarão a sincronizar.

- **Código de país de conta** de cliente : É obrigatório fornecer um código de país de duas letras (ISO 3166) quando criar uma nova remessa. Por padrão, o código de país será sincronizado de e para o campo **BillingCountry** da conta na Salesforce. Se tiver um campo diferente na Salesforce para o código do país sincronizar a partir de:

  - Para um campo de código de país não-anzol na conta que contém um código de duas letras:

    - Atualize o nome de campo **do Código de País** de Conta de Cliente na variável ambiente Salesforce com o nome de campo do CRM. Certifique-se de que fornece o nome do campo e não o seu nome de exibição.

    - Editar **[Personalizar] Criar ou Obter Detalhes da Salesforce,** e ir para criar ou obter conta de cliente em ação **CRM** para atribuir um valor **país** ao campo correto no CRM. Além disso, **remova** a atribuição de valor country do **BillingCountry**.

  - Para um campo de código de país baseado em procura na conta:

    - Adicione um novo campo personalizado na conta e preencha-o automaticamente com um código de país de duas letras (ISO 3166) com base no valor selecionado no campo baseado em procura e vice-versa.

    - Siga os passos anteriores para o campo de código country não-anzol para sincronizar um novo campo personalizado do CRM de e para o Partner Center.

- **Valor do negócio**: Por padrão, o valor da oferta do Partner Center será sincronizado de e para **o Valor** no CRM. Se tiver um campo diferente no CRM para que o valor do negócio se sincronize a partir de:

  - Atualize o nome do campo **de valor do Negócio** na variável ambiente Salesforce com o nome de campo do CRM. Certifique-se de que fornece o nome do campo e não o seu nome de exibição.

  - Editar **[Personalizar] Criar ou Obter Detalhes da Salesforce** e ir para **criar ou atualizar oportunidade** em CRM e atualizar tanto Criar uma nova **oportunidade** e atualizar as ações de **oportunidade existentes** para atribuir o **DealValue** ao campo correto em Salesforce.

- **Código de moeda de valor de** negócio : Nome do campo de código de moeda de valor de negócio na Salesforce. Este nome de API de campo será usado para obter o código de moeda de valor de negócio da Opportunity ao criar ou atualizar a referência no Microsoft Partner Center. Se o campo de código de moeda de valor de negócio for diferente do campo padrão **CurrencyIsoCode,** atualize o valor atual desta variável ambiente.

  - Atualize o nome do campo **de valor do Negócio** na variável ambiente Salesforce com o nome de campo do CRM. Certifique-se de que fornece o nome do campo e não o seu nome de exibição.

  - Editar **[Personalizar] Criar ou Obter Detalhes da Salesforce** e ir para **criar ou atualizar oportunidade** em CRM e atualizar tanto Criar uma nova **oportunidade** e atualizar as ações de **oportunidade existentes** para atribuir o **DealValueCurrency** ao campo correto em Salesforce.

- **Oportunidade de Co-venda sincronizada**: Se definido para **sim,** apenas as oportunidades de co-venda e partilha de gasodutos serão sincronizadas do Partner Center para o Salesforce. Se definido para **não,** leads, co-sell e pipeline sharing oportunidades serão sincronizados de Partner Center para Salesforce. Esta variável não tem qualquer impacto nas oportunidades sincronizadas da Salesforce para partner Center.

## <a name="update-environment-variable"></a>Atualizar variável de ambiente

Para atualizar um valor variável ambiental:

1. Aceda à página **Soluções** e selecione **Solução Padrão**. Selecione **a Variável ambiente** selecionando **Tudo**.

1. Selecione a variável ambiente para o valor que precisa de ser atualizado e **selecione Editar** utilizando o ícone elipse.

1. Atualizar **Valor Corrente** (não atualizar Valor **Padrão)** utilizando a opção De Novo **Valor** e fornecendo o valor. O valor deve corresponder ao tipo de dados da variável. Por exemplo, o tipo de dados Sim ou Não aceitará o valor Sim ou Não.

   :::image type="content" source="images/cosellconnectors/environment-variables-video.gif" alt-text="Screenshot que mostra atualização variáveis ambientais.":::

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a>Sincronização de co-venda bidis de ponta a ponta

Depois de instalar, configurar e personalizar a solução Power Automate, pode testar a sincronização de referências de Co-venda entre o Salesforce CRM e o Partner Center.

### <a name="pre-requisites"></a>Pré-requisitos

Para sincronizar as referências através do Partner Center e da Salesforce CRM, a solução Power Automamate precisa de demarcar claramente os campos de referência específicos da Microsoft. Esta identificação proporciona às suas equipas de vendedores a capacidade de decidir quais as referências que querem partilhar com a Microsoft para co-venda.

Um conjunto de campos personalizados está disponível como parte da Sincronização de Referências do Partner Center para **a** solução de soluções de CRM Salesforce. Um utilizador de administração CRM terá de criar uma secção de CRM separada com os campos personalizados **Opportunity.**

Os seguintes campos personalizados devem fazer parte da secção CRM:

- **Sincronizar com o Partner Center**: Se sincronizar a oportunidade com o Partner Center. Por padrão, o valor deste campo é Não e precisa de ser explicitamente definido para Sim pelo seu vendedor para partilhar uma oportunidade com a Microsoft. Novas referências partilhadas do Partner Center para CRM terão este valor de campo definido para Sim.

- **Identificador de referência**: Um campo de identificação apenas de leitura para a referência do Microsoft Partner Center.

- **Link de referência**: Um link apenas de leitura para a referência no Microsoft Partner Center.

- **Como pode a Microsoft ajudar:** Ajuda necessária da Microsoft para a referenciação. Para criar uma referência de co-venda, selecione a ajuda adequada necessária à Microsoft. Um contacto com o cliente deve ser associado à oportunidade de criar uma referência de co-venda. Para criar uma referência não co-venda, não selecione este campo. Uma referência não co-venda pode ser convertida para uma referência de co-venda a qualquer momento, selecionando a opção adequada para a ajuda exigida.

- **Visibilidade de referência do Microsoft Partner Center**: Selecione a visibilidade para a referenciação do Partner Center. Ao torná-lo visível para os vendedores da Microsoft, uma referência não-co-venda pode ser convertida para co-vender. Quando a ajuda da Microsoft é necessária, a referência é visível para os vendedores da Microsoft por padrão. Depois deste campo ser marcado como visível, não pode ser revertido.

- **Identificador de CRM da Microsoft**: Quando uma referência de co-venda é criada e aceite pela Microsoft, este campo será preenchido com o identificador CRM da Microsoft.

- **Microsoft Partner Center Solutions**: Um objeto personalizado para associar soluções prontas de co-venda ou soluções Microsoft com a oportunidade. Uma ou mais soluções podem ser adicionadas ou removidas da oportunidade. É obrigatório adicionar pelo menos uma solução de co-venda pronta ou a solução Microsoft para a oportunidade antes de a partilhar com a Microsoft. Para associar este objeto à oportunidade, atualize o formulário **Oportunidade** no CRM.

- **Auditoria**: Um rasto de auditoria só de leitura para sincronização com referências do Partner Center

### <a name="scenarios"></a>CENÁRIOS

1. Sincronização de encaminhamento quando a referência é criada ou atualizada em CRM e sincronizada no Partner Center:

   1. Inscreva-se no seu ambiente de CRM Salesforce com o utilizador que tenha visibilidade na secção **Oportunidade** do CRM.

   1. Certifique-se de que a secção, **o Microsoft Partner Center** está presente quando criar uma nova **oportunidade** no ambiente CRM salesforce.

   1. As oportunidades sincronizadas com sucesso com o Partner Center serão identificadas com ✔ ícone no Salesforce CRM.
      :::image type="content" source="images/salesforce/salesforce-environment.png" alt-text="Screenshot do ambiente Salesforce.":::

   1. Para sincronizar esta oportunidade com o Microsoft Partner Center, certifique-se de que define os seguintes campos na vista do cartão:

      - **Como pode a Microsoft ajudar?**: Para criar uma referência de co-venda, selecione uma opção de ajuda apropriada.

        :::image type="content" source="images/salesforce/salesforce-help-option.png" alt-text="Screenshot que mostra como obter campos apropriados na vista do cartão.":::

      - **Sincronização com o Centro de Parceiros**: Sim
      - **Contacto com o Cliente**: Para criar uma referência de co-venda, adicione um contacto do cliente à oportunidade.
      - **Microsoft Solutions**: Para partilhar uma referência com a Microsoft, adicione uma solução de co-venda válida pronta ou microsoft à oportunidade.

   1. Depois de definir a oportunidade **Sync com a** opção Partner Center para **Sim,** aguarde 10 minutos, inscreva-se na sua conta Partner Center. As suas referências serão sincronizadas com o Salesforce CRM, e o Link de Referência será preenchido. Se houver uma falha, o campo de Auditoria será preenchido com informações de erro.

   1. Da mesma forma, quando a opção **Sync with Partner Center** estiver definida como **Sim**, se atualizar a oportunidade no Salesforce CRM, as alterações sincronizar-se-ão com a sua conta Partner Center.

2. Sincronização de referência quando a referência é criada ou atualizada no Microsoft Partner Center e sincronizada no ambiente de CRM da Salesforce:

    1. Inscreva-se no painel do Centro de [Parceiros.](https://partner.microsoft.com/dashboard/home)

    1. Selecione **Referências** no menu à esquerda.

    1. Crie uma nova referência de Co-venda do Partner Center clicando na opção "New deal".

    1. Inscreva-se no seu ambiente de CRM Salesforce.

    1. Navegue para **oportunidades abertas.** A referência criada no Microsoft Partner Center está agora sincronizada na Salesforce CRM.

    1. Quando seleciona uma referência sincronizada, os dados da visualização do cartão são preenchidos.

       :::image type="content" source="images/salesforce/salesforce-casino.png" alt-text="Screenshot da página de oportunidades Salesforce.":::

>[!NOTE]
>**Precisa de ajuda com a implantação?**
>Para assistência com a sua implementação de conector de referência de co-venda, pode contratar um Consultor Técnico de Parceiros. Podem prestar assistência à implantação e boas práticas para uma implementação bem sucedida.
>
>Para mais informações, consulte [Como Submeter um pedido de pré-venda técnica e serviços de implantação](technical-benefits.md)

## <a name="next-steps"></a>Passos seguintes

- [Gerir oportunidades potenciais](manage-leads.md)

- [Gerir oportunidades de venda conjunta](manage-co-sell-opportunities.md)

- [Webhooks do Centro de Parceiros](/partner-center/develop/partner-center-webhooks)
