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
ms.openlocfilehash: fa9b35343e1251cfce5caff107de8dff344f4e68
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148419"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a>Conector de co-venda para Salesforce CRM - visão geral

**Funções adequadas**: Administração de referências | Administrador de sistema ou personalizador de sistema no CRM

O conector partner Center co-sell permite que os seus vendedores co-vendam com a Microsoft a partir dos seus sistemas CRM. Não terão de ser treinados para usar o Partner Center para gerir os negócios de co-venda. Utilizando os conectores Co-sell, pode criar uma nova referência de Co-venda para contratar um vendedor da Microsoft, receber referências do vendedor da Microsoft, aceitar/recusar referências, modificar dados de negócios como o valor do negócio e a data de encerramento.  Também pode receber quaisquer atualizações dos vendedores da Microsoft nestas ofertas de Co-venda. Pode fazer todas as suas referências enquanto trabalha dentro do CRM à sua escolha e não no Partner Center. 

A solução baseia-se na Solução de Automatização de Energia da Microsoft e utiliza APIs do Partner Center.

## <a name="before-you-install---pre-requisites"></a>Antes de instalar - pré-requisitos

|**Tópicos**   |**Detalhes**   |**Ligações**   |
|--------------|--------------------|------|
|ID da rede de parceiros da Microsoft |Precisa de um ID MPN válido|Para se juntar à [MPN](https://partner.microsoft.com/)|
|Co-vender pronto|A sua solução IP/Serviços tem de ser co-vendida.|[Venda com a Microsoft](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|Conta do Centro de Parceiros|O ID MPN associado ao inquilino do Centro De Parceiros deve ser o mesmo que o ID MPN associado à sua solução de Co-venda. Verifique se consegue ver as suas referências de co-venda no portal Partner Center antes de implantar os conectores.|[Gerir a sua conta](create-user-accounts-and-set-permissions.md)|
|Funções de utilizador do Partner Center|O empregado que vai instalar e usar os conectores deve ser um administrador de referências|[Assign users roles and permissions](create-user-accounts-and-set-permissions.md) (Atribuir funções e permissões de utilizador)|
|Salesforce CRM|A função de utilizador crm é administrador do sistema ou personalizador do sistema|[Atribuir funções na Salesforce CRM](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|Conta de fluxo de automatização de energia|Uma conta ativa [de Automação](https://flow.microsoft.com) de Energia para o administrador do Sistema CRM ou personalizador do sistema. Este utilizador deve iniciar sustação na [Power Automamate](https://flow.microsoft.com) pelo menos uma vez antes da instalação.|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a>Instalação do Pacote Salesforce para Campos Personalizados da Microsoft 

Para sincronizar as referências através do Partner Center e da Salesforce CRM, a solução Power Automamate precisa de identificar claramente os campos de referência específicos da Microsoft. Esta demarcação proporciona às equipas de vendedores parceiros a capacidade de decidir quais as referências que querem partilhar com a Microsoft para co-venda.

1. Na Salesforce, ative **notas** e adicione-as à lista de oportunidades relacionadas. 
[Referência](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

2. Ativar **as equipas de Oportunidade** seguindo os passos: 
    - Na configuração, utilize a caixa **De localização Rápida** para localizar as Definições da Equipa de Oportunidade.
    - Defina as definições conforme necessário.
[Referência](https://help.salesforce.com/articleView?id=teamselling_enabling.htm&type=5]) 

3. No Salesforce, instale campos e objetos personalizados utilizando o [instalador de embalagens.](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV) Utilize isto para instalar a embalagem em qualquer empresa.

>[!NOTE]
>Se estiver a instalar numa caixa de areia, deve substituir a parte inicial do URL por http://test.salesforce.com

4. Na Salesforce, adicione as Soluções Microsoft à lista relacionada com a **Oportunidade.** Uma vez adicionado, selecione o ícone da **chave** inglesa e atualize propriedades

## <a name="best-practice-test-before-you-go-live"></a>Melhores Práticas: Teste antes de ir ao vivo

Antes de instalar, configurar e personalizar a solução Power Automamate no ambiente de produção, certifique-se de testar a solução numa fase de CRM de encenação.

- Instale a solução Microsoft Power Automate num ambiente de preparação/instância CRM.

- Faça uma cópia da solução e execute a sua configuração e faça personalizações de fluxo power-automatizado no ambiente de preparação.

- Teste a solução numa fase de encenação/CRM.

- No que diz respeito ao sucesso, a importação como solução gerida para o caso de produção.

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a>Instalar Referências do Centro de Parceiros Sincronização para Salesforce CRM

1. Vá ao [Power Automamate](https://flow.microsoft.com) e selecione **Ambientes** no canto superior direito. Isto irá mostrar-lhe as instâncias de CRM disponíveis.

2. Selecione a instância CRM apropriada a partir da queda no canto superior direito.

3. Selecione **Soluções** na barra de navegação esquerda.

4. Selecione o link **Open AppSource** no menu superior.

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Open AppSource":::

5. Procure por **Conectores de Referências do Centro de Parceiros para Salesforce** no ecrã pop-up.  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Salesforce":::

6. Selecione o botão **Get-lo agora** e, em seguida, **Continue**.

7. Isto abre a página onde pode selecionar o ambiente de CRM salesforce para instalar a aplicação.  Concorde com os termos e condições.

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="CRMs disponíveis":::

8. Em seguida, é direcionado para a página **Gerir as suas soluções.**  Navegue para "Partner Center Referrals" utilizando os botões de seta na parte inferior da página. **A instalação programada** deve aparecer ao lado da solução de referências do Centro parceiro. A instalação levará 10-15 minutos.

9. Assim que a instalação estiver concluída, volte a navegar para [o Power Automamate](https://flow.microsoft.com) e selecione **Soluções** da área de navegação à esquerda. Note que **a Sincronização de Referências do Partner Center para a Salesforce** está disponível na lista de Soluções.

10. Selecione **Partner Center Referrals Synchronization for Salesforce**. Estão disponíveis os seguintes fluxos e entidades power-automamate:

    :::image type="content" source="images/cosellconnectors/salesforce10.png" alt-text="Fluxos de salesforce":::



## <a name="configure-the-solution"></a>Configure a solução

1. Depois de ter instalado a solução no seu caso CRM, volte a navegar para [Power Automamate](https://flow.microsoft.com/).

2. A partir do **drop-down Do Ambiente** no canto superior direito, selecione a instância CRM onde instalou a solução Power Automamate.
3. Terá de criar ligações que associem as três contas de utilizador:
    - Utilizador do Partner Center com credenciais de administração de referências
    - Eventos do Centro de Parceiros
    - Administração CRM com o Power Automamate flui na solução.
4. Selecione **Ligações** da barra de navegação esquerda e selecione a solução "Partner Center Referrals" da lista.

5. Criar uma ligação clicando **Criar uma ligação**.

:::image type="content" source="images/cosellconnectors/salesforce12.png" alt-text="Criar ligação":::

- Procure referências ao Centro de Parceiros (pré-visualização) na barra de pesquisa no canto superior direito.

- Crie uma ligação para o utilizador do Centro de Parceiros com o papel de credenciais da administração de referências.

-  Em seguida, crie uma ligação Partner Center Events para o seu utilizador Partner Center com as credenciais de administração de referências.

- Criar uma ligação para o Salesforce para o utilizador administrador crm.

-  Uma vez adicionadas todas as Ligações, deverá ver as seguintes Ligações no seu ambiente:

 :::image type="content" source="images/cosellconnectors/salesforce13.png" alt-text="Observar ligações":::

### <a name="edit-the-connections"></a>Editar as ligações

1. Volte à página Soluções e selecione **Solução Padrão.**  Selecione **Referência de Ligação (pré-visualização)** clicando **em Tudo**.
 
:::image type="content" source="images/cosellconnectors/salesforce14.png" alt-text="Iniciar a edição do conector":::

2. Edite cada uma das Ligações individualmente selecionando o ícone de três pontos. Adicione as ligações relevantes.

:::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="Editar conectores":::

3. Ligue os fluxos na seguinte sequência:

- Registo Webhook do Partner Center (Visualização privilegiada)
- Criar Co-venda Referral - Salesforce to Partner Center (Visualização insider)
- Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)
- Centro de Parceiros para Salesforce (Visualização de Insider)
- Salesforce para Partner Center (Visualização insider)
- Oportunidade Salesforce para Partner Center (Visualização insider)
- Salesforce Microsoft Solutions to Partner Center (Visualização insider)

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Utilize APIs webhook para se registar para eventos de mudança de recursos

As APIs do Partner Center Webhook permitem-lhe registar-se para eventos de alteração de recursos. Estes eventos de alteração são enviados para o seu url como posts HTTP.

1. Para registar o seu url, selecione **Partner Center Webhook Registr (Insider Preview)** Power Automamate flow.

2. Adicione ligações para (a.) Utilizador do Partner Center com credenciais de administração de referências (b.) Eventos do Centro de Parceiros, conforme destacado abaixo

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Acionador":::

3. Quando fizer estas atualizações, verá

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhooks":::

4. Guarde as alterações e selecione **Ligue- se**.

   Para permitir que os webhooks do Partner Center ouçam as alterações do evento, execute os seguintes passos:

5. Selecione **Partner Center para Salesforce CRM (Visualização insider)**.

6. Selecione o ícone **Editar** e selecione **Quando um pedido HTTP for recebido**.

7. Selecione o ícone **Copy** para copiar o URL HTTP POST fornecido.

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="Copiar URL":::

8. Selecione agora o "Partner Center Webhook Registration (Insider Preview)" Power Automamate flow e selecione **Run**.

9. Certifique-se de que a janela "Run Flow" se abre no painel direito e selecione **Continue**.

10. Introduza os seguintes detalhes:

    1. **Http Trigger Endpoint**: URL copiado do passo anterior

    2. **Eventos para Registar**: "referenciação criada" e "referenciada"

    3. **Substitua os pontos finais do gatilho existentes se estiver presente:** Sim (Isto substitui quaisquer pontos finais existentes.)

11. Selecione **Executar** e, em seguida, selecione **Fazer.**

O webhook pode agora ouvir criar e atualizar eventos.

## <a name="customize-synchronization-steps"></a>Personalizar etapas de sincronização

Quando as referências de Co-venda são sincronizadas entre o Partner Center e o seu sistema CRM, os campos sincronizados no Partner Center PC estão listados aqui.

Muitas vezes os sistemas de CRM são altamente personalizados. Pode personalizar os fluxos power automamate. Siga o guia de mapeamento de campo e, se necessário, faça as alterações adequadas nos passos dos fluxos power automamate.  Os centros de parceiros da Microsoft para mapeamentos CRM são fornecidos, mas com base no seu ambiente CRM, pode optar por personalizar ainda mais os campos.

Vários passos de cada um dos fluxos power automamate podem ser personalizados com base nas suas necessidades. Seguem-se exemplos de personalizações disponíveis:

1. Para personalizar os campos para criar ou atualizar eventos no Centro de Parceiros para sincronização de referência CRM:

   1. Selecione Partner Center para Salesforce CRM (Visualização insider).

   2. **Selecione Editar** para editar/personalizar o fluxo power automamate.

   3. Selecione **(Âmbito) Sincronizar o chumbo ou a oportunidade**.

2. Para personalizar mapeamentos de campo de CRM para criar eventos, selecione **Se é nova oportunidade partilhada, então**. Selecione o sub-passo **se sim** e, em seguida, expanda **criando uma nova oportunidade no CRM**. Pode editar os mapeamentos nesta secção utilizando o Guia de Mapeamento de Campo.

   1. Para personalizar mapeamentos de campo crm para eventos de atualização, selecione o passo "(Scope) Sincronizar o chumbo ou a oportunidade".

   2. Selecione **Se é uma atualização para uma oportunidade, então**. Selecione o sub-passo **se sim** e, em seguida, expandir Se a diferença entre **os objetos de oportunidade no Partner Center e CRM, então**.  

   3. Selecione **Se sim** seguido com **a atualização oportunidade existente**

3. Para personalizar os campos de sincronização de referência de CRM para PC para eventos de atualização:

   1. **Selecione Editar** para editar/personalizar o fluxo power automamate.

   2. Selecione **(Âmbito) Sincronizar a oportunidade**.

   3. Para personalizar mapeamentos de campo de CRM (baseados no guia de mapeamentos de campo) para eventos de atualização, selecione **Se houver diferença entre os objetos de chumbo no Partner Center e CRM, então**.

   4. Selecione o sub-passo **se sim** e, em seguida, expandir o passo Atualizar uma referência **com dados de oportunidade**.

   Pode editar os mapeamentos nesta secção com base no Guia de Mapeamento de Campo.

4. Para personalizar os campos de sincronização de referência de CRM para PC para criar eventos?

   1. **Selecione Editar** para editar/personalizar o fluxo power automamate.

   2. Selecione **(Âmbito) Referências sincronizadas.**

   3. Para personalizar mapeamentos de campo de CRM (baseados no guia de mapeamentos de campo) para criar eventos, **selecione Create Microsoft Referral**.

Pode editar os mapeamentos nesta secção com base no Guia de Mapeamento de Campo.


## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a>Sincronização de co-venda bidis de ponta a ponta

Uma vez instalada, configurada e personalizada a solução Power Automate, pode testar a sincronização de referências de Co-venda entre o Salesforce CRM e o Partner Center.

### <a name="pre-requisites"></a>Pré-requisitos

Para sincronizar as referências através do Partner Center e da Salesforce CRM, a solução Power Automamate precisa de demarcar claramente os campos de referência específicos da Microsoft. Esta identificação proporciona às suas equipas de vendedores a capacidade de decidir quais as referências que querem partilhar com a Microsoft para co-venda.

Um conjunto de campos personalizados está disponível como parte da Sincronização de Referências do Partner Center para **a** solução de soluções de CRM Salesforce. Um utilizador de administração CRM terá de criar uma secção de CRM separada com os campos personalizados **Opportunity.**

Os seguintes campos personalizados devem fazer parte da secção CRM:

- **Sincronizar com o Partner Center**: Se sincronizar a oportunidade com o Microsoft Partner Center

- **Identificador** de referência : Um campo de identificação apenas de leitura para referência do Microsoft Partner Center

- **Link de referência**: Um link apenas de leitura para a referência no Microsoft Partner Center

- **Como pode a Microsoft ajudar:** Ajuda necessária da Microsoft para a referenciação

- **Produtos**: Lista de produtos associados a esta oportunidade

- **Auditoria**: Um rasto de auditoria só de leitura para sincronização com referências do Partner Center

### <a name="scenarios"></a>CENÁRIOS:

1. Sincronização de encaminhamento quando a referência é criada ou atualizada em CRM e sincronizada no Partner Center:

   1. Inscreva-se no seu ambiente de CRM Salesforce com o utilizador que tenha visibilidade na secção **Oportunidade** do CRM.

   2. Certifique-se de que a secção seguinte está presente quando criar uma "Nova Oportunidade" no ambiente CRM da Salesforce

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Ambiente salesforce":::

   3. Para sincronizar esta oportunidade com o Microsoft Partner Center, certifique-se de que define os seguintes campos na vista do cartão:

       - "Sincronização com Centro de Parceiros": Sim
       - "Como pode a Microsoft ajudar?": Selecione a partir das seguintes opções:
       - Produtos: IDs de solução do produto

   4. Depois de definir a oportunidade  **Sync com Partner Center** para **Sim,** aguarde 10 minutos, inscreva-se na sua conta Partner Center. As suas referências serão sincronizadas com a Salesforce CRM.

   5. Quando a opção "Sync with Partner Center" estiver definida como "Sim", se atualizar a oportunidade no Salesforce CRM, as alterações sincronizar-se-ão com a sua conta Partner Center.

   6. As oportunidades sincronizadas com sucesso com o Partner Center serão identificadas com ✔icon na Salesforce CRM.

2. Sincronização de referência quando a referência é criada ou atualizada no Microsoft Partner Center e sincronizada no ambiente de CRM da Salesforce:

    1. Inscreva-se no painel do Centro de [Parceiros.](https://partner.microsoft.com/dashboard/home)

    2. Selecione **Referências** no menu à esquerda.

    3. Crie uma nova referência de Co-venda do Partner Center clicando na opção "New deal".

    4. Inscreva-se no seu ambiente de CRM Salesforce.

    5. Navegue para **oportunidades abertas.** A referência criada no Microsoft Partner Center está agora sincronizada na Salesforce CRM.

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Tela de oportunidade de salesforce":::

    6. Quando seleciona uma referência sincronizada, os dados da visualização do cartão são preenchidos.

## <a name="next-steps"></a>Passos seguintes

- [Gerir oportunidades potenciais](manage-leads.md)

- [Gerir oportunidades de venda conjunta](manage-co-sell-opportunities.md)

- [Webhooks do Centro de Parceiros](/partner-center/develop/partner-center-webhooks)
