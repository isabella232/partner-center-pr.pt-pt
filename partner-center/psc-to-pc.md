---
title: Migrar do Partner Sales Connect (PSC)
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como os parceiros da Microsoft podem migrar do Partner Sales Connect (PSC) para Partner Center e criar ou gerir ofertas enviadas pelos vendedores da Microsoft.
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 12/07/2020
ms.openlocfilehash: 495d9899db36d0e4911647b337a99105a063236c
ms.sourcegitcommit: 79d2f00c352db61252e523f45abf93fe2a2742a5
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/04/2021
ms.locfileid: "102124827"
---
# <a name="guide-to-co-selling-in-partner-center-pc-for-partners-migrating-from-partner-sales-connect-psc"></a>Guia para co-venda no Partner Center (PC) para parceiros que migram do Partner Sales Connect (PSC)

**Funções adequadas**

- Administrador de conta
- Administração de referências
- Vendedor de Vendas de Parceiros (PSC)
- Administrador de Vendas de Parceiros (PSC)
- Gestor de negócios Partner Sales Connect (PSC)

Este artigo fornece orientação para os parceiros que migram do Partner Sales Connect para Partner Center para que possam continuar a criar e gerir ofertas de co-venda no Partner Center.

>[!Note]
> Se está aqui porque viu um estandarte no PSC sobre a migração, está no lugar certo. Este guia não é aplicável para a Solution Assessment (SA) e para os parceiros comerciais de licenciamento da OEM que gerem as suas ofertas em PSC.

>[!Important]
> A partir de 1 de abril de 2021 a sua empresa não poderá criar ou editar negócios no PSC. **Você ainda será capaz de descarregar os dados de ofertas existentes usando a capacidade de exportação a granel em PSC. Você também pode [migrar ofertas abertas](psc-to-pc.md#psc-deals-migration) de PSC para Partner Center após esta data.** <br><br> Se houver ofertas em que está a trabalhar ativamente que contenham soluções elegíveis de incentivo de CO-sell IP, tem duas opções: <br><br> 1. Marque o negócio como ganho e complete o registo de negócio no PSC antes de 31 de março de 2021. <br> 2. [Migrar as ofertas](psc-to-pc.md#psc-deals-migration) para o Partner Center para que tenha mais tempo para trabalhar no negócio e iniciar o registo de negócios.

Como sabem, **a empresa perderá acesso ao PSC depois de 30 de abril de 2021**. No entanto, ainda encontrará tudo o que pretende fazer no Partner Center, como criar ofertas de co-venda, gerir as suas ofertas e atuar em ofertas enviadas pelos vendedores da Microsoft.

Haverá diferenças, no entanto. A seguinte orientação pode ajudar a tornar a sua transição para o Partner Center mais suave e simples.

## <a name="before-you-move-things-you-need-to-know"></a>Antes de te mexeres, as coisas que precisas de saber

### <a name="if-you-are-a-psc-admin"></a>Se você é um administrador psc

- Precisa de um e-mail de trabalho para iniciar sinscê-lo no [Partner Center.](https://partner.microsoft.com/)
- Crie a sua conta com a ajuda da [administração](permissions-overview.md)da conta Partner Center .
- Saiba como co-vender no Partner Center lendo este documento.
- Configurar contas de utilizador no Partner Center para todos os seus utilizadores de PSC (funções de Administrador, Gestor de Acordos e Vendedor) e atribuir-lhes [funções de administração de encaminhamento](permissions-overview.md).

>[!IMPORTANT]
> Certifique-se de que o ID MPN mostrado no banner do PSC está disponível na lista de localizações mpn no Partner Center.

:::image type="content" source="images/pscmigration/mpnidcheck.png" alt-text="Imagem mostrando o banner do PSC onde os parceiros podem encontrar o ID MPN.":::

 Para verificar se o ID MPN aparece como uma localização MPN do Partner Center, inscreva-se no painel de [instrumentos](https://partner.microsoft.com/dashboard)Partner Center, em seguida, selecione **Definições** (o ícone De engrenagem) no canto superior direito do ecrã, seguido de **Definições** de Conta . No menu de navegação à esquerda do segundo nível, selecione **Localizações** para ver a lista de todos os IDs e locais mpn associados à conta Partner Center.

### <a name="if-you-are-a-psc-deal-manager-or-seller"></a>Se você é um gestor de negócios psc ou vendedor

- Precisa de um e-mail de trabalho para iniciar sincê-lo no painel de instrumentos do Centro [de Parceiros.](https://partner.microsoft.com/dashboard)
- Se estiver a utilizar uma conta não-trabalho no PSC ou o seu email de trabalho for para uma empresa diferente da empresa parceira, contacte o administrador do PSC para obter ajuda de configuração de conta.
- Consulte o seu administrador do PSC se a configuração da sua conta Partner Center está completa independentemente da conta que utiliza para iniciar sê-lo no PSC.
- Verifique se tem acesso ao Partner Center e à secção de Referências.
- Leia este documento para compreender os fluxos de trabalho e as alterações no Centro de Parceiros.

## <a name="as-an-admin-in-psc-these-are-your-next-steps"></a>Como administrador no PSC, estes são os seus próximos passos

A partir do menu de navegação à esquerda do Centro Parceiro, selecione a opção **Referências.** Confirme que pode aceder às páginas de Referências.

  >[!Note]
  > Poderá ter de assinar fora do Partner Center e voltar a inscrever-se para refrescar as suas credenciais de acesso às páginas de Referências.

Se não vir a opção **de Referências** no menu Partner Center ou páginas relacionadas com referências, contacte a [administração](permissions-overview.md) da conta da sua empresa e peça-lhe que lhe dê acesso à opção **de Referências** e área relacionada.

Para encontrar a administração da conta da sua empresa:

1. Selecione **as definições** de conta do ícone de engrenagem no topo-direito do painel Partner Center.

1. Selecione **a gestão** do utilizador a partir do segundo nível, menu de navegação à esquerda.

1. No topo da lista de utilizadores, selecione o menu de entrega do **filtro.** Alterar a opção **para Administração conta.**

   A página apresentará todos os administradores da conta com os respetivos endereços de e-mail. Envie um e-mail a um deles e peça-lhes que atribuam o papel de administrador de referências para a sua conta de trabalho.

  :::image type="content" source="images/pscmigration/account-admin.png" alt-text="Imagem mostrando os administradores de conta na página de gestão de utilizadores de definições de parceiros.":::

>[!Important]
>- Se a sua função envolve apenas gerir utilizadores no PSC, peça ao administrador de conta da sua empresa para lhe atribuir o papel [de administrador](permissions-overview.md#manage-mpn-membership-and-your-company) de conta no Partner Center. 
>- Se o seu papel também inclui gerir oportunidades de co-venda, peça para ser atribuído o papel [de administrador de referências.](permissions-overview.md#manage-referrals)
> - É uma boa ideia também nomear uma liderança de gestão de mudança entre os administradores do PSC. Ao fazê-lo, todos os administradores do PSC terão de contactar individualmente os administradores de conta partner Center. Em vez disso, o chumbo da gestão da mudança pode então ser a pessoa principal a trabalhar com a administração da conta partner Center.

## <a name="user-migration"></a>Migração de utilizadores

Depois de configurar a sua conta no Partner Center, utilize o assistente de migração do utilizador na página de oportunidades de co-venda para atribuir automaticamente funções do Partner Center aos colaboradores da sua empresa.

>[!Note]
> A migração de utilizadores só pode ser realizada por administradores de [conta](permissions-overview.md#manage-mpn-membership-and-your-company) da sua empresa. Se não tiver a função de administrador de conta, encontre um administrador de conta que possa ajudar a configurar as contas do utilizador com a ajuda do assistente de migração do utilizador.

:::image type="content" source="images/pscmigration/psc-user-migration.png" alt-text="Imagem mostrando o assistente de migração do utilizador.":::

Os administradores de conta verão um link de assistente de migração de utilizadores do PSC na página de oportunidades de co-venda ao lado do guia de referências. Podem iniciar a migração do utilizador selecionando o link. Para iniciar a migração do utilizador, os administradores podem selecionar o link. Podem executar este passo de migração do utilizador várias vezes até que todos os utilizadores sejam atribuídos papéis adequados no Partner Center.

A tabela de migração do utilizador tem os seguintes detalhes:

- Conta de utilizador - ID de e-mail do funcionário
- Conta parceira do PSC - A conta a que o trabalhador está associado no PSC
- Função de utilizador do PSC - Uma das três funções atribuídas no PSC.
- Localização PC MPN - Local para o qual o utilizador receberá funções relevantes para PC. A conta parceira do PSC MPN é usada para encontrar a localização MPN equivalente no Partner Center para atribuir permissões. Toda a organização denota o vOrg MPN ID.
- Função de utilizador do PC - Os colaboradores são atribuídos funções com base nas suas funções de utilizador do PSC. A administração no PSC será atribuída a funções de administração de referências no PC. Será atribuído ao vendedor a função de utilizador de referências no PC. Saiba mais sobre os papéis do PC e o que os utilizadores com estas funções podem fazer no centro parceiro [aqui](permissions-overview.md#manage-referrals)
- PC AAD Tenant - o inquilino a que os utilizadores estão designados no Partner Center
- Estado - Existem três Estados possíveis para o estado da migração
    - **Não migrado** - O utilizador não tem qualquer função de referência para PC atribuída
    - **Migrado** - O utilizador foi migrado com sucesso com papel relevante atribuído como mostrado na tabela
    - **Erro** - Incapaz de completar a migração devido a algum erro

Às vezes, a migração pode falhar e resultar em erros. Eis algumas razões pelas quais uma migração pode causar um erro e algumas das formas de resolver a questão:

1. Os utilizadores de CPS podem estar a utilizar uma conta não-trabalho.

2. O utilizador do PSC pode estar a utilizar uma conta de um domínio diferente daquele que utiliza no Partner Center.

   Para resolver erros relacionados com os cenários 1 e 2, peça ao utilizador para se inscrever no Partner Center utilizando a sua conta de trabalho anexada ao seu inquilino Azure AD. O seu [administrador global](permissions-overview.md#manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles) pode ajudar.
   
   Para encontrar o seu administrador global: 
   - Inscreva-se no painel de [instrumentos](https://partner.microsoft.com/dashboard) Partner Center e selecione **as definições** de conta do ícone de engrenagem no topo direito.
   - Selecione **a gestão** do utilizador a partir da barra de navegação do segundo nível, à esquerda.
   - No topo da lista de utilizadores, selecione o menu de entrega do **filtro** e altere a opção para **administração Global.** Em seguida, a página exibe todos os administradores globais com os respetivos endereços de e-mail. Peça a um deles que atribua o papel de administrador de encaminhamento para a sua conta de trabalho.
   
      O administrador global pode criar uma nova conta de utilizador no seu inquilino AZure AD ou atribuir o acesso do utilizador ao outros utilizadores de conta de domínio. Uma vez configuradas as contas para todos os gestores e utilizadores de negócios do PSC, eles precisam de iniciar sação no Partner Center, selecionar **Referências** do menu de navegação à esquerda e confirmar que podem ver a página de Referências.

3. O utilizador já tem uma função de encaminhamento atribuída no Partner Center.
    - Pode verificar o papel existente do utilizador. No canto superior direito do Partner Center, selecione **Definições** (o ícone de engrenagem) e, em **seguida, as definições de Conta**. Quando vir um segundo menu de navegação à esquerda, selecione **a gestão do utilizador** e procure o utilizador.

## <a name="psc-deals-migration"></a>PSC Negoceia migração

Depois de ter concluído a migração de utilizadores, utilize o assistente de migração de ofertas na página de oportunidades de co-venda para trazer todas as ofertas abertas elegíveis do PSC para PC. **O link de migração de negócios será visível apenas com todo o âmbito de organização no Partner Center.** Haverá um link chamado **"migração de acordos psc"** no topo direito da página de Oportunidades de Co-venda, que abrirá o assistente de migração do negócio.

Leia esta secção antes de iniciar a migração do negócio.

**Elegível para migração**

Apenas algumas ofertas são elegíveis para migração de CPC para PC. Este assistente de migração foi construído para ajudar os parceiros a levarem as suas ofertas para o Partner Center, onde ainda estão a trabalhar ativamente com os seus clientes para fechar o negócio. **Apenas os negócios que estão em estado aberto criados a partir de 1 de janeiro de 2020 com detalhes válidos da conta de parceiro (ID MPN válido) e não submetidos a registo de negócios são elegíveis para migração.**

**Não elegível para migração**

- Acordos de avaliação de soluções não são elegíveis para migração de negócios
- Negócios de licenciamento da OEM não são elegíveis para migração de negócios
- Qualquer acordo que tenha sido marcado como ganho no PSC não é elegível para migração. O registo de negócios se for elegível para as transações marcadas como ganhos deve ser concluído no PSC.

## <a name="pre-requisites-for-deal-migration"></a>Pré-requisitos para a migração de negócios

Antes de iniciar a migração do negócio a partir do PC, siga as instruções abaixo para estabelecer os acordos no PSC para uma migração bem sucedida.

1. Todos os membros da equipa de vendas da sua empresa que trabalham nos negócios abertos são informados sobre esta migração.
2. Os membros da equipa de vendas são treinados para usar o Partner Center para a gestão de negócios.
3. Os negócios têm todas as informações necessárias, conforme descrito abaixo.
    - Detalhes da empresa do cliente, incluindo nome e endereço
    - Dados de contato do cliente se for um negócio de co-venda
    - Pelo menos uma solução
    - Pelo menos um membro da equipa com todos os detalhes - primeiro nome, apelido, ID de e-mail e número de telefone
    - Valor do negócio
    - Data de fecho de negócio estimada
    - Notas de parceiro

Você pode usar as capacidades de descarregamento e upload em massa no PSC para adicionar todos os detalhes em falta no negócio para todas as ofertas elegíveis.

>[!Note]
> A migração de acordos terá êxito, mesmo que os pré-requisitos acima referidos não sejam cumpridos. Mas não pode alterar o estado do negócio se algum dos campos acima mencionados exigidos no Partner Center não estiver disponível. Em seguida, terá de introduzir todas as informações necessárias que faltam nos negócios no Partner Center para começar a trabalhar neles. **É fortemente aconselhável limpar as ofertas elegíveis no CPS antes de migrar para o Partner Center.**

A migração de negócios no Partner Center é construída como uma experiência de clique. Tudo o que precisa fazer é clicar no botão **"Ofertas migratórias"** assim que a sua empresa estiver pronta para migrar as ofertas elegíveis. **Não pode escolher os acordos que pretende migrar do PSC. Se não quiser migrar quaisquer ofertas para o Partner Center, transloque-os para o estado fechado no PSC antes de iniciar a migração.**

>[!Note]
> Após o início da migração, **pode levar até 24 horas para os negócios serem migrados.**

Uma vez concluída a migração, a mensagem do banner terá o estatuto alterado para ser completada com um link para o relatório de migração. Faça o download do relatório para ver os detalhes das ofertas que foram migradas do PSC para pc.

O relatório inclui os detalhes abaixo.

1. **Partner Center engagement ID** - O identificador único no Partner Center para todos os negócios em um noivado. Existem duas ofertas - uma para o parceiro e outra para a Microsoft num compromisso de co-venda no Partner Center.
2. **Partner Center referenciação ID** - O identificador único no Partner Center para o negócio pertencente ao parceiro.
3. **Nome do negócio** - Identificador dado ao negócio no PSC.
4. **Identificação de acordo com o PSC** - O identificador único no PSC para o negócio.
5. **Erros** - para indicar se há algum erro durante a migração de um negócio específico.

Todos os negócios que foram migrados com sucesso não serão visíveis no PSC. Pode continuar a trabalhar nas ofertas migradas no PC, incluindo completar o registo de negócios no PC. Não haverá alterações nas interações com os vendedores da Microsoft para co-vender ofertas.

As ofertas migradas do PSC estarão disponíveis nos separadores de Entrada e Saída com base na origem do negócio. Todas as ofertas partilhadas pela sua empresa estarão disponíveis no separador Outbound e as ofertas iniciadas pela Microsoft estarão disponíveis no separador Entrada do Partner Center. Haverá dois tipos de acordos que serão criados após a migração.

1. **Co-vender ofertas** - Ofertas que são marcadas como co-venda no PSC serão criadas como co-vender ofertas no Partner Center.
2. **Ofertas lideradas por parceiros** - Ofertas que não estejam marcadas como co-venda serão criadas como ofertas lideradas por parceiros no Partner Center. As ofertas lideradas por parceiros são visíveis para os vendedores da Microsoft e podem ser atualizadas para co-vender ofertas antes de atingir o estado terminal (won, lost). Além disso, os acordos liderados por parceiros são elegíveis para registo de negócios se houver uma solução elegível de incentivo no negócio.

>[!Important]
> Se houver erros devidos aos quais algumas ofertas não puderam ser migradas, **pode relançar a migração do negócio clicando no botão "Acordos migratórios".** Só será ativado se houver algumas negociações elegíveis ainda por migrar. Isto também será útil se estiver na fase de transição onde alguns novos negócios estão a ser criados no PSC após o início da migração de acordos.

Uma vez que todos os negócios são migrados com sucesso, haverá banner mostrando **"No deals to migrar"** com o botão **"Migrar acordos"** a ser **desativado.**

Após completar a migração dos utilizadores e/ou a migração de negócios, utilize as seguintes orientações para decidir a estratégia de migração:

Se a sua empresa tiver um Partner Development Manager (PDM) - Quando a sua conta Partner Center estiver configurada e os seus utilizadores tiverem movimentos e permissões, pode mover as suas atividades de Co-venda para Partner Center. Informe o PDM para fazer a troca em vez de esperar até que a sua migração complete o prazo, o que permitirá que todas as suas novas ofertas fluam para o Partner Center.

>[!Note]
>Uma vez feita esta troca, só poderá atuar sobre as ofertas ativas existentes no PSC. Não pode criar novas ofertas nem receber quaisquer ofertas de vendedores da Microsoft no PSC.

Se a sua empresa não tiver um PDM - Certifique-se de que todas as contas de utilizador são configuradas e verificadas por todos os utilizadores. Será notificado através de um e-mail e de um banner no PSC sobre a data exata em que pode começar a Co-vender no Partner Center. Lembre-se que ainda terá de gerir os negócios ativos existentes no PSC.

>[!Important]
> Tem até 30 de abril de 2021 para registar os negócios que estão marcados como ganhos.

## <a name="next-steps-for-psc-admins-psc-deal-managers-and-psc-sellers"></a>Próximos passos para administradores de PSC, gestores de acordos de PSC e vendedores de PSC

Saiba como co-vender no Partner Center.
Este é um passo importante, que o ajudará a estar preparado para a Co-venda no Partner Center. Compreenda os fluxos de trabalho e as mudanças no Partner Center para que possa efetivamente Co-vender imediatamente. Comece por ler completamente este documento. Um bom conjunto de recursos também está disponível na [galeria de experiências Co-sell.](https://aka.ms/cosellexperience)

## <a name="major-differences-between-psc-and-pc-workflows"></a>Grandes diferenças entre fluxos de trabalho do CPE e do PC

|**Cenário**|**Conexão de vendas de parceiros**|**Partner Center**|
|-----|:-----|:-----|
|Funções de utilizador|O PSC tem funções de administrador, gestor de negócios e vendedor.|O PC tem [apenas função de administração de referência](permissions-overview.md#manage-referrals) que dá tanto a leitura como a escrita permissão para todos os negócios.|
|Convidando a Microsoft a fazer um acordo de co-venda|Iniciado pelo vendedor da Microsoft, não há pedido explícito por parte do parceiro.|O parceiro terá de fazer um [pedido explícito](manage-co-sell-opportunities.md#add-solutions) se uma ajuda do vendedor da Microsoft for necessária para um negócio. O Microsoft Seller tem a opção de recusar o pedido.|
|Validade|Não há noção de um acordo expirado.|As transações de entrada de sócios expiram em 14 dias se não forem aceites pelo parceiro. O mesmo acontece com os negócios de saída de parceiros onde podem entrar em estado de expiração se o vendedor da Microsoft não agir sobre eles em 14 dias.|
|Detalhes do vendedor da Microsoft|Visível assim que um acordo é criado.|Os detalhes do Microsoft Seller só são partilhados com o Partner se o vendedor aceitar explicitamente o convite para co-venda do parceiro.|
|[Gasoduto privado](manage-co-sell-opportunities.md#types-of-co-sell-opportunities)|Não disponível.|Os parceiros podem partilhar o seu pipeline sem dar visibilidade aos vendedores da Microsoft.|
|Soluções|As soluções pertencentes a apenas uma lista de preços podem ser adicionadas a um negócio.|O parceiro pode adicionar soluções que pertençam às [seguintes](manage-co-sell-opportunities.md#add-solutions) listas. a) As suas próprias soluções b) Soluções do catálogo de primeira parte da Microsoft (semelhante ao papel de Transaction Deal no PSC) e c) Co-vender soluções de outros parceiros de terceiros (semelhantes ao papel isv Deal no PSC).|
|Atribuição de acordo|Só o vendedor designado pode ver e agir sobre os negócios.|Os membros da equipa podem ser adicionados a um acordo para especificar as pessoas que trabalham num acordo, não há nenhum bloqueio de outros administradores de encaminhamento de visualização ou atuação nesses negócios.|
|Organização de clientes|Entrada de texto em formulário gratuito.|Pode pesquisar a organização do [cliente](manage-co-sell-opportunities.md#select-your-customer) contra a [base de dados D&B](https://www.dnb.com/) digitando apenas alguns caracteres. O nome e endereço legais são automaticamente preenchidos com base na escolha.|
|Contacto com o cliente|Não é obrigatório.|Não é obrigatório para a partilha de gasodutos privados. Obrigatório se o vendedor da Microsoft for convidado a participar num pedido de Co-venda.|
|API pública|Não disponível.|[A API pública](/partner/develop/referrals) para gerir programáticamente referências do Partner Center.|

## <a name="map-the-fields-in-psc-to-the-corresponding-fields-in-partner-center"></a>Mapear os campos em PSC para os campos correspondentes no Partner Center

Esta secção compara (ou "mapas") imagens selecionadas mostradas para o CPS com a visualização correspondente na secção de oportunidades de co-venda do Partner Center.

Verá círculos numerados, amarelos ou vermelhos em cada par de imagens:

- **O que significam círculos amarelos?** Círculos numerados e amarelos aparecem primeiro em cada imagem do PSC. Em seguida, encontrará uma imagem do Partner Center abaixo com muitos dos mesmos números.

   Para ver como cada campo ou atributo nos mapas do PSC ao seu homólogo no Partner Center, combine os círculos numerados juntos nas duas imagens relacionadas. Por exemplo, combine o "1" numerado, amarelo no primeiro, imagem de PSC para o "1" numerado, amarelo "1" no segundo, imagem do Partner Center abaixo.

- **O que significa um círculo vermelho?** Se vir um círculo vermelho numa imagem, isso indica que o campo DEC não está disponível no Partner Center.

Os mapeamentos de campo do Centro PSC-para-Parceiro são mostrados para as seguintes áreas:

1. Página inicial do PSC mapeada para o Centro de Parceiros co-vender oportunidades padrão padrão
1. Vista da grelha do PSC mapeada para a vista de negócio do Partner Center
1. Detalhes do negócio do PSC visualizam mapeada para a visão de detalhes do negócio do Centro parceiro
1. Visualização de produtos de adicionar PSC mapeada para a visão de soluções de adicionar parceiro
1. Visualização de gestão de utilizador do PSC mapeada para a visão de gestão do utilizador do Partner Center
1. Visualização da atribuição de funções de utilizador do PSC mapeada para a visão de atribuição de funções do Partner Center
1. Ver notificações de PSC mapeadas para a visão de notificações do Centro parceiro

### <a name="1---psc-home-page-mapped-to-the-partner-center-co-sell-opportunities-default-view"></a>1 - Página inicial do PSC mapeada para a vista padrão de oportunidades de Co-venda do Partner Center

Compare os círculos correspondentes e numerados entre a imagem superior do PSC e a imagem do Partner Center abaixo. Os números correspondentes mostram onde pode encontrar a funcionalidade ou atributo relacionado com o PSC no Partner Center. Os círculos vermelhos indicam que não existe um campo de partner center correspondente.  

:::image type="content" source="images/pscmigration/homepage.png" alt-text="Imagem mostrando os mapeamentos de campo entre a página inicial do Partner Sales Connect e a visão padrão de Oportunidades de Co-venda no Partner Center." lightbox="images/pscmigration/home-page-expanded.png":::

### <a name="2---psc-grid-view-mapped-to-the-partner-center-deal-view"></a>2 - Vista da grelha do PSC mapeada para a vista de negócio do Partner Center

Compare os círculos correspondentes e numerados entre a imagem superior do PSC e a imagem do Partner Center abaixo. Os números correspondentes mostram onde pode encontrar a funcionalidade ou atributo relacionado com o PSC no Partner Center. Os círculos vermelhos indicam que não existe um campo de partner center correspondente.  

> [!NOTE]
> Outras considerações aparecem abaixo das imagens.

:::image type="content" source="images/pscmigration/gridview.png" alt-text="Imagem mostrando os mapeamentos de campo entre a vista da grelha de vendas de parceiros (PSC) e a vista de negócio do Partner Center." lightbox="images/pscmigration/grid-view-expanded.png":::

**Considerações especiais:**

- Não há nenhuma vista de lista no Partner Center como a do PSC.  Todas as ofertas são listadas com base na data mais recente recebida ou criada com a informação do cliente e o tipo de negócio. O primeiro negócio na vista é selecionado por padrão. A maioria dos valores que são apresentados no formato de tabela do PSC estão disponíveis na visão detalhada do negócio no PC.
- O papel do negócio não é um campo obrigatório no PC. Não é exibido ou capturado em nenhum dos fluxos de trabalho. É derivado automaticamente do lado do vendedor da Microsoft com base nas soluções adicionadas ao negócio.
- A última data modificada não é apresentada na página de detalhes de encaminhamento no PC. Os parceiros podem usar a funcionalidade de tipo para classificar as ofertas com base na última data atualizada.

### <a name="3---psc-deal-details-view-mapped-to-partner-center"></a>3 - Detalhes do negócio do PSC visualizam mapeado para o Partner Center

Compare os círculos correspondentes e numerados na imagem superior (PSC) com a imagem do Partner Center abaixo. Os números correspondentes mostram onde pode encontrar a funcionalidade ou atributo relacionado com o PSC no Partner Center. Os círculos vermelhos indicam que não há campo ou área correspondente no Centro de Parceiros.

> [!NOTE]
> Outras considerações aparecem abaixo das imagens.

:::image type="content" source="images/pscmigration/dealdetails.png" alt-text="Imagem mostrando os mapeamentos de campo entre a visão de detalhes de negócio do Partner Sales Connect (PSC) e a visão de detalhes do negócio do Partner Center." lightbox="images/pscmigration/deal-details-expanded.png":::

**Considerações especiais:**

- Os parceiros podem editar um negócio selecionando o botão de edição na vista de detalhes do negócio do parceiro (6). Uma vez selecionado o botão de edição, todos os campos tornar-se-ão editáveis. Em seguida, tem a opção de guardar ou cancelar as edições feitas no negócio.
- Não há opção para fechar o negócio como duplicado no Partner Center.
- O Resultado do Cliente não está disponível no Partner Center. Todos os detalhes relacionados com as interações do cliente podem ser atualizados na secção Notas no PC.
- A data de fecho estimada da solução só está disponível para ofertas OEM IOT no Partner Center. Estas informações não são apresentadas para outros tipos de negócio.
- O programa de licenciamento não é necessário no PC. Esta informação é auto-inferida com base nas soluções selecionadas no negócio.

>[!Note]
>Qualquer negócio marcado como ganho ou perdido não pode ser editado depois. Tenha cuidado ao mover um acordo para um destes estados terminais.

### <a name="4---psc-add-products-view-mapped-to-the-partner-center-add-solutions-view"></a>4 - Vista psc 'Adicionar produtos' mapeada para a visão 'Adicionar soluções' do Centro Parceiro

Compare os círculos correspondentes e numerados na imagem superior (PSC) com a imagem do Partner Center abaixo. Os números correspondentes mostram onde pode encontrar a funcionalidade ou atributo relacionado com o PSC no Partner Center. Os círculos vermelhos indicam que não há campo ou área correspondente no Centro de Parceiros.
  
:::image type="content" source="images/pscmigration/products.png" alt-text="Imagem mostrando os mapeamentos de campo entre o Partner Sales Connect (PSC) adicionar a vista de produtos e o Centro de Parceiros adicionar visão de soluções." lightbox="images/pscmigration/products-expanded.png":::

### <a name="5---user-management-in-psc-versus-partner-center"></a>5 - Gestão de utilizadores em PSC versus Partner Center

Compare os círculos correspondentes e numerados na imagem superior (PSC) com a imagem do Partner Center abaixo. Os números correspondentes mostram onde pode encontrar a funcionalidade ou atributo relacionado com o PSC no Partner Center. Os círculos vermelhos indicam que não há campo ou área correspondente no Centro de Parceiros.  

 :::image type="content" source="images/pscmigration/usermanagement.png" alt-text="Imagem mostrando os mapeamentos de campo entre a casa de gestão do utilizador Partner Sales Connect (PSC) e a vista da página de gestão do utilizador do Partner Center dentro da área de definições de conta."  lightbox="images/pscmigration/user-management-expanded.png":::

### <a name="6---user-role-assignment-in-psc-versus-partner-center"></a>6 - Atribuição de função de utilizador no PSC versus Partner Center

Compare os círculos correspondentes e numerados na imagem superior (PSC) com a imagem do Partner Center abaixo. Os números correspondentes mostram onde pode encontrar a funcionalidade ou atributo relacionado com o PSC no Partner Center. Os círculos vermelhos indicam que não há campo ou área correspondente no Centro de Parceiros.  

:::image type="content" source="images/pscmigration/roles.png" alt-text="Imagem mostrando os mapeamentos de campo entre a visão de atribuição de funções Partner Sales Connect (PSC) e a vista de atribuição de funções do Partner Center." lightbox="images/pscmigration/roles-expanded.png":::

**Considerações especiais:**

- O papel equivalente para a administração do PSC é o papel de administrador de conta no Partner Center.
- Há apenas um papel no Partner Center para co-vender gestão de negócios. Este papel é o papel de administrador de referência.

### <a name="7---notifications-in-psc-versus-partner-center"></a>7 - Notificações no PSC versus Partner Center

Compare os círculos correspondentes e numerados na imagem superior (PSC) com a imagem do Partner Center abaixo. Os números correspondentes mostram onde pode encontrar a funcionalidade ou atributo relacionado com o PSC no Partner Center. Os círculos vermelhos indicam que não há campo ou área correspondente no Centro de Parceiros.  

:::image type="content" source="images/pscmigration/notifications.png" alt-text="Imagem mostrando o mapeamento entre as notificações Partner Sales Connect (PSC) e a visualização de notificações do Partner Center."  lightbox="images/pscmigration/notifications-expanded.png":::

## <a name="moving-from-psc-to-partner-center---frequently-asked-questions"></a>Passar de PSC para Partner Center - Perguntas frequentes

As seguintes secções respondem a perguntas frequentes sobre a migração.

### <a name="1---what-should-i-do-if-i-dont-have-access-to-partner-center"></a>1 - O que devo fazer se não tiver acesso ao Partner Center?

Pode contactar os seus administradores listados na página "Não ter acesso" para obter as funções atribuídas. Necessitará da [função de administrador de encaminhamento](permissions-overview.md#manage-referrals) para ler e escrever permissão ao abrigo da secção de referências. Se está a gerir apenas perfis de negócio, então vai precisar do perfil de negócios no centro de parceiros.

:::image type="content" source="images/pscmigration/noaccess.png" alt-text="Imagem mostrando a experiência de não acesso no Partner Center.":::

### <a name="2---who-can-grant-me-access-to-the-referrals-section-in-partner-center"></a>2 - Quem me pode conceder acesso à secção de Referências no Centro de Parceiros?

O administrador da sua [conta](permissions-overview.md#manage-mpn-membership-and-your-company) pode dar-lhe acesso ao separador Referências. Para encontrar o administrador da sua conta, selecione **as definições** de Conta do ícone de engrenagem no topo-direito do [painel](https://partner.microsoft.com/dashboard)Partner Center . Em seguida, selecione **a gestão** do utilizador a partir da barra de navegação deixada no segundo nível. No topo da lista de utilizadores, selecione o menu de entrega do **filtro** e altere a opção de **administração de conta**. A página apresentará todos os administradores da conta com os respetivos endereços de e-mail. Peça a um deles que atribua o papel de administrador de encaminhamento para a sua conta de trabalho.

### <a name="3---the-new-deal-button-is-greyed-out-for-our-account-what-should-i-do-to-start-creating-deals"></a>3 - O botão +new deal está acinzentado para a nossa conta. O que devo fazer para começar a criar acordos?

Isto só acontece se não houver soluções prontas de Co-venda anexadas à organização MPN que está a utilizar no Partner Center. Contacte o seu PDM para que o MPN ID das suas soluções é corrigido ou crie um bilhete de apoio que mencione o problema: "Novo botão de negócio acinzentado após a migração do PSC."

### <a name="4---can-i-assign-deals-to-a-specific-person-from-our-organization-like-psc"></a>4 - Posso atribuir ofertas a uma pessoa específica da nossa organização como o PSC?

Pode atribuir membros da equipa a um acordo específico. Não impede outros administradores de visualização ou atuação nesses negócios.

### <a name="5---is-there-a-view-of-all-the-deals-assigned-to-me"></a>5 - Existe uma visão de todos os negócios que me foram atribuídos?

Pode utilizar a funcionalidade favorito, que é um separador ao nível do utilizador. Pode marcar todas as ofertas que lhe são atribuídas como favoritas para ter um acesso rápido às ofertas.

### <a name="6---is-there-a-read-only-view-for-the-deals"></a>6 - Existe uma visão apenas de leitura para os negócios?

Não, não há uma visão apenas de leitura dos negócios na secção de referências. Todos os administradores de referência terão leitura completa e escreverão acesso a todos os negócios.

### <a name="7---how-can-i-register-a-deal-after-marking-it-as-won"></a>7 - Como posso registar um acordo depois de o marcar como ganho?

Se o negócio cumprir os critérios abaixo, mostraremos um pop-up para iniciar o [registo do negócio.](./register-deals.md)

- Há uma solução elegível de incentivo anexa ao negócio.
- O vendedor da Microsoft é convidado a participar no negócio, ou convidaram-no para o negócio.
- O cartão Microsoft está no estado Aceite ou Ganho no Partner Center.

### <a name="8---i-get-an-error-message-when-i-select-the-new-deal-registration-button-in-the-deal-registration-section-how-can-i-register-my-deals"></a>8 - Recebo uma mensagem de erro quando seleciono o botão "+New deal registration" na secção De Registo de Negócios. Como posso registar os meus acordos?

O botão **de registo +New deal** deve ser utilizado apenas pelos parceiros que estão registados no programa de ligação ISV para registar um acordo sem oportunidade de co-venda correspondente no Partner Center. Para registar negócios com uma oportunidade de co-venda, um pop-up será exibido quando o negócio for marcado como ganho e se cumprir os critérios de registo do negócio.

### <a name="9---is-adding-a-customer-organization-mandatory"></a>9 - A adição de uma organização de clientes é obrigatória?

Sim, adicionar uma [organização de clientes](./manage-co-sell-opportunities.md#select-your-customer) é obrigatório no Partner Center. Comece por procurar o local onde o cliente está. Com base nos detalhes que tem; você pode ser específico, incluindo o nome exato do edifício ou apenas dar detalhes da cidade. A pesquisa da organização irá buscar todas as entidades legais que correspondem ao nome que inseriu para que não tenha de inserir nenhum endereço. Todos os detalhes são preenchidos automaticamente com base na organização selecionada.

### <a name="10---are-customer-contact-details-mandatory"></a>10 - Os dados de contacto do cliente são obrigatórios?

Depende do [tipo de acordo](./manage-co-sell-opportunities.md#types-of-co-sell-opportunities) que está a criar. Se estiver apenas a partilhar o seu oleoduto e não necessitar de ajuda da organização de vendas da Microsoft, pode optar por não dar detalhes de contacto com o cliente. Se estiver a co-vender onde está ativamente à procura de ajuda do vendedor da Microsoft, terá de fornecer os dados de contacto do cliente. Deve obter o consentimento explícito do cliente antes de criar um pedido de co-venda no centro de parceiros.

### <a name="11---how-many-solutions-can-i-add-to-a-deal"></a>11 - Quantas soluções posso acrescentar a um acordo?

Pode adicionar até 50 soluções (análogas aos 'produtos' do PSC) a um acordo. Ao contrário do PSC, pode misturar soluções a partir de suas próprias soluções elegíveis co-venda, SKUs de primeira parte da Microsoft e outras soluções elegíveis de terceiros. Não há nenhuma função de negócio que deve ser selecionado ou disponível no centro parceiro. Para o Microsoft SKUs, pode opcionalmente adicionar quantidade e preço para cada SKU que é adicionado ao negócio.

### <a name="12---when-will-i-get-to-know-the-microsoft-seller-details-after-creating-a-deal"></a>12 - Quando vou conhecer os detalhes do vendedor da Microsoft depois de criar um acordo?

Os vendedores da Microsoft são atribuídos apenas depois de corresponderem ao requisito de ajuda exato indicado enquanto criam o negócio com a personalidade do vendedor relevante no lado da Microsoft. Mesmo após a atribuição, os vendedores da Microsoft terão a opção de aceitar ou rejeitar o convite de co-venda. Só se um convite de co-venda for aceite por um vendedor, o negócio será atualizado com os dados de contacto do vendedor da Microsoft. O SLA para os vendedores da Microsoft agirem no negócio é de 14 dias. É o mesmo SLA que os sócios têm de agir sobre o negócio antes de entrar em estado caducado.

### <a name="13---where-can-i-find-the-opportunity-id"></a>13 - Onde posso encontrar a oportunidade de imposição?

O ID de oportunidade no PSC é o mesmo que o ID do negócio no PC. Pode encontrar a identificação do negócio ao lado do nome do negócio quando abrir qualquer negócio.

### <a name="14---how-can-my-pdm-get-access-to-pc"></a>14 - Como é que o meu PDM pode ter acesso ao PC?

O Partner Center não pode ser acedido pelos seus PDMs diretamente ao contrário do PSC. Existem múltiplas opções para ativar essa capacidade, que são mencionadas abaixo.

- OCP Insights - Se os PDMs estiverem apenas a ver as ofertas e os progressos relacionados com eles, podem usar o portal OCP Insights para obter a sua visão da organização. Esta é uma ferramenta interna e disponível apenas para PDMs. Note que os insights OCP não estão disponíveis para os utilizadores da sua empresa.
- Utilizador convidado no Partner Center - Pode adicionar a sua conta PDM @microsoft.com como utilizador convidado no centro de parceiros e atribuir-lhes funções de administração de encaminhamento para que possam visualizar e agir em referências.
- Criar um [novo utilizador](./create-user-accounts-and-set-permissions.md#add-a-new-user) no seu inquilino - Pode criar um novo utilizador no seu próprio inquilino e partilhar esses detalhes com o PDM para que possam ver e agir em referências semelhantes a outros utilizadores de referência na sua conta.

## <a name="finding-the-correct-mpn-id-if-your-account-in-psc-is-not-associated-with-a-valid-mpn"></a>Encontrar o ID MPN correto se a sua conta no PSC não estiver associada a um MPN válido

Se está aqui porque viu um banner no PSC mencionando "problema de associação MPN inválido do PSC", está no lugar certo. A sua conta pode ter sido ligada a um ID MPN inválido devido às seguintes razões

- A sua empresa não tem uma conta no Partner Center.
- O seu PDM cometeu um erro ao introduzir o ID mpn da sua conta nos sistemas internos que ligam a sua conta DESEC à sua conta Partner Center (MPNID).
- A sua empresa não completou a migração do Partner Membership Center (PMC) para PC.

Primeiro, encontre o ID MPN correto seguindo os passos abaixo

- Faça login na sua conta Partner Center
- Utilize as orientações indicadas na documentação das [definições](./partner-center-account-setup.md#locate-your-mpn-id) de conta para localizar o ID MPN.

Abaixo está uma imagem mostrando a localização exata onde você pode encontrar o seu Parceiro Centro MPN ID

:::image type="content" source="images/pscmigration/findingMPNID.png" alt-text="Imagem mostrando as definições da conta onde o parceiro pode encontrar o seu ID MPN."  lightbox="images/pscmigration/findingMPNID.png":::

Seguinte

- Se tiver um PDM, peça-lhes que o seu ID MPN é corrigido com o ID MPN correto da sua conta de centro de parceiros.
- Se não tiver um PDM, envie um e-mail para o endereço indicado no banner do PSC com as informações da conta do CPS mostradas no banner do PSC e o ID MPN correto da sua conta de centro de parceiros.

## <a name="resources-to-help-you-create-and-manage-your-deals-in-partner-center"></a>Recursos para ajudá-lo a criar e gerir as suas ofertas no Partner Center

Se ainda não leu os tópicos de ajuda de co-venda, os seguintes recursos irão ajudá-lo a gerir negócios no centro de parceiros.

|**Para fazer isto**   |**Leia isto**   |
|-----------------------|:-----------------------|
|Compreender os separadores e a navegação na página de oportunidades de co-venda|[Navegando na secção de co-venda](./manage-co-sell-opportunities.md#navigating-the-co-sell-section)|
|Selecionando uma organização de clientes da lista D&B |[Selecione o seu cliente](./manage-co-sell-opportunities.md#select-your-customer)|
|Modificação dos campos na secção de detalhes do negócio|[Detalhes do negócio](./manage-co-sell-opportunities.md#deal-details)|
|Adicionar os membros da sua equipa a uma equipa de negócios|[Adicione os seus colaboradores](./manage-co-sell-opportunities.md#add-team-members)|
|Respondendo a um acordo de co-venda|[Gerir ofertas de co-venda](./manage-co-sell-opportunities.md#responding-to-a-co-sell-opportunity)
|Registar ofertas que ganhou no Partner Center |[Registar um novo acordo](./register-deals.md)
|Obtenha insights de referência e descubra como estão as suas referências |[Informações de referências](./referral-insights.md)
|Criar e gerir o perfil de negócios|[Gerir perfil empresarial](./create-a-marketing-profile.md)
|Gerencie pistas para o seu perfil de negócio |[Gerir oportunidades potenciais](./manage-leads.md)|

## <a name="next-steps"></a>Passos seguintes


- [Partner Sales Connect to Partner Center workbook](https://partner.microsoft.com/resources/detail/partner-sales-connect-to-partner-center-transition-workbook-pptx) - livro para alinhar os processos e funções de vendas dos parceiros com novos processos de vendas via Partner Center vs. Partner Sales Connect.
- [Partner Center co-sell operating guide](https://partner.microsoft.com/resources/detail/co-sell-operating-model-guide-pptx) - orientação para identificar um modelo operativo via Partner Center para gerir leads ou co-vender oportunidades e registar ofertas.
- [Deck de gestão](https://partner.microsoft.com/resources/detail/referral-management-in-partner-center-pptx) de encaminhamento - instrução passo a passo visualizada para gerir leads e co-vender oportunidades através do Partner Center.
- [Publicar e gerir no mercado comercial](https://partner.microsoft.com/resources/detail/publishing-and-managing-co-sell-offers-in-commercial-marketplace-pptx) - instrução visualizada passo a passo para criar, gerir e publicar ofertas através do Partner Center no mercado comercial.