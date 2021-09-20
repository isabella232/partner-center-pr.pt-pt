---
title: Migração de Ligação de Vendas de Parceiros (PSC) para Parceiros IOT
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-referrals
description: Saiba como os parceiros microsoft IOT podem migrar de Ligação de Vendas de Parceiros (PSC) para Partner Center e criar ou gerir ofertas.
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 07/07/2021
ms.openlocfilehash: 2b05046118c83c0d398272da68054a8a0c9c48e4
ms.sourcegitcommit: 731a5e2725a72ecdae40189a3f52ab6b4a4c8058
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/19/2021
ms.locfileid: "127987640"
---
# <a name="guide-to-create-and-manage-iot-deals-in-partner-center-pc-for-iot-partners-migrating-from-partner-sales-connect-psc"></a>Guia para criar e gerir ofertas de IOT no Partner Center (PC) para parceiros IOT migrando de Parceiros Sales Ligação (PSC)

**Funções adequadas**: Administração de contas | Administração de referências | | de vendedores de Ligação de vendas de parceiros (PSC) | de administração de Ligação de vendas de parceiros (PSC) Gestor de negócios de Ligação de vendas de parceiros (PSC)

Este artigo fornece orientações para os parceiros IOT migrarem de Partner Sales Ligação (PSC) para Partner Center (PC) para que possam continuar a criar e gerir ofertas no Partner Center.

>[!Note]
> Este guia **aplica-se apenas aos parceiros de negócios da IOT** que gerem as suas ofertas em PSC.

>[!Important]
> A partir de 15 de agosto de 2021, a sua empresa não poderá criar ou editar negócios no PSC. **Você ainda será capaz de baixar os dados de ofertas existentes usando a capacidade de exportação a granel em PSC. Você também pode [migrar ofertas abertas](partner-sales-connect-to-partner-center-iot.md#psc-deals-migration) de PSC para Partner Center após esta data.**

Como sabe, **a sua empresa perderá acesso ao PSC após 30 de agosto de 2021**. No entanto, ainda encontrará tudo o que pretende fazer no Partner Center, como criar e gerir negócios.

Haverá diferenças, no entanto. A seguinte orientação pode ajudar a tornar a sua transição para o Partner Center mais suave e simples.

## <a name="before-you-move-things-you-need-to-know"></a>Antes de te mexeres, as coisas que precisas de saber

### <a name="if-you-are-a-psc-admin"></a>Se você é um administrador psc

- Precisa de um e-mail de trabalho para iniciar sinscê-lo no [Partner Center.](https://partner.microsoft.com/)
- Configurar a sua conta com a ajuda da [conta](permissions-overview.md)partner Center.
- Aprenda a criar e gerir ofertas de IOT no Partner Center lendo este documento.
- Configurar contas de utilizador no Partner Center para todos os seus utilizadores de PSC (funções de Administrador, Gestor de Acordos e Vendedor) e atribuí-las a [funções de administrador de encaminhamento ou de encaminhamento](permissions-overview.md)de utilizadores .

### <a name="if-you-are-a-psc-deal-manager-or-seller"></a>Se você é um gestor de negócios psc ou vendedor

- Precisa de um e-mail de trabalho para iniciar [sinscê-lo](https://partner.microsoft.com/dashboard)no painel do Centro de Parceiros.
- Se estiver a utilizar uma conta não-trabalho no PSC ou o seu email de trabalho for para uma empresa diferente da empresa parceira, contacte o seu administrador do PSC para obter ajuda de configuração de conta.
- Consulte o seu administrador do PSC se a configuração da sua conta Partner Center estiver concluída independentemente da conta que utiliza para iniciar sê-lo no PSC.
- Verifique se tem acesso ao Centro de Parceiros e à secção de Referências.
- Leia este documento para compreender os fluxos de trabalho e as alterações no Centro de Parceiros.

## <a name="as-an-admin-in-psc-these-are-your-next-steps"></a>Como administrador no PSC, estes são os seus próximos passos

A partir do menu de navegação à esquerda do Centro Parceiro, selecione a opção **Referências.** Confirme que pode aceder à página de Oportunidades de Co-venda.

  >[!Note]
  > Poderá ter de assinar fora do Partner Center e voltar a inscrever-se para refrescar as suas credenciais de acesso às páginas de Referências.

Se não vir a opção **de Referências** no menu Partner Center ou páginas relacionadas com referências, contacte a [administração](permissions-overview.md) da conta da sua empresa e peça-lhe que lhe dê acesso à opção **de Referências** e área relacionada.

Para encontrar a conta da sua empresa admin:

1. Selecione **as definições** de conta do ícone de engrenagem no topo-direito do painel Partner Center.

1. Selecione **a gestão** do utilizador do segundo nível, menu de navegação à esquerda.

1. No topo da lista de utilizadores, selecione o menu de entrega do **filtro.** Alterar a opção **para Administração conta.**

   A página apresentará todos os administradores da conta com os respetivos endereços de e-mail. Envie um e-mail a um deles e peça-lhes que atribuam a função de administração de referências para a sua conta de trabalho.

  :::image type="content" source="images/pscmigration/account-admin.gif" alt-text="Imagem mostrando os administradores de conta na página de gestão do utilizador de definições de parceiro.":::

>[!Important]
>- Se a sua função envolve apenas gerir utilizadores em PSC, peça ao administrador de conta da sua empresa para lhe atribuir o papel [de administrador](permissions-overview.md#manage-mpn-membership-and-your-company) de conta no Partner Center de acordo com a política da sua empresa.
>- Se o seu papel também inclui gerir negócios iot, peça para ser atribuído o [cargo de administrador de referências ou encaminha](permissions-overview.md#manage-referrals) a função de utilizador conforme apropriado.
> - É uma boa ideia também nomear uma liderança de gestão de mudança entre os administradores do PSC. Ao fazê-lo, todos os administradores do PSC terão de contactar individualmente os administradores de conta partner center. Em vez disso, o chumbo da gestão da mudança pode então ser a pessoa principal a trabalhar com a administração da conta partner Center.

## <a name="user-migration"></a>Migração de utilizadores

Depois de configurar a sua conta no Partner Center, utilize o assistente de migração do utilizador na página de oportunidades de co-venda para atribuir automaticamente funções do Partner Center aos colaboradores da sua empresa.

>[!Note]
> A migração do utilizador só pode ser realizada por administradores de [conta](permissions-overview.md#manage-mpn-membership-and-your-company) da sua empresa. Se não tiver a função de administrador de conta, encontre um administrador de conta que possa ajudar a configurar as contas do utilizador com a ajuda do assistente de migração do utilizador.

:::image type="content" source="images/pscmigration/user-migration.gif" alt-text="Imagem mostrando o assistente de migração do utilizador.":::

Os administradores de conta verão um link de assistente de migração de utilizadores do PSC na página de oportunidades de co-venda ao lado do guia de referências. Podem iniciar a migração do utilizador selecionando o link. Para iniciar a migração do utilizador, os administradores podem selecionar o link. Podem executar este passo de migração do utilizador várias vezes até que todos os utilizadores sejam atribuídos papéis adequados no Partner Center.

A tabela de migração do utilizador tem os seguintes detalhes:

- Conta de utilizador - ID de e-mail do funcionário
- Conta parceira do PSC - A conta a que o trabalhador está associado no PSC
- Função de utilizador do PSC - Uma das três funções atribuídas no PSC.
- Localização PC MPN - A localização para a qual o utilizador receberá funções relevantes do Partner Center (PC). A conta parceira do PSC MPN é usada para encontrar a localização MPN equivalente no Partner Center para atribuir permissões. Toda a organização denota o vOrg MPN ID.
- Função de utilizador do PC - Os colaboradores são atribuídos funções com base nas suas funções de utilizador do PSC. A administração em PSC será atribuída a funções de administrador de referências no Partner Center. O vendedor será atribuído a referências à função de utilizador no Partner Center. Saiba mais sobre as funções do Partner Center e o que os utilizadores com estas funções podem fazer na [Atribuição de funções e permissões para os utilizadores de uma empresa que precisam de trabalhar no Partner Center.](permissions-overview.md#manage-referrals)
- Pc AAD Tenant - o inquilino Microsoft Azure Ative Directory (Azure AD) a que os utilizadores são designados no Partner Center
- Estado - Existem três Estados possíveis para o estado da migração
    - **Não migrado** - O utilizador não tem qualquer função de referência do Partner Center atribuída
    - **Migrado** - O utilizador foi migrado com sucesso com papel relevante atribuído como mostrado na tabela
    - **Erro** - Incapaz de completar a migração devido a algum erro

Às vezes, a migração pode falhar e resultar em erros. Eis algumas razões pelas quais uma migração pode causar um erro e algumas das formas de resolver a questão:

1. Os utilizadores de CPS podem estar a utilizar uma conta não-trabalho.

2. O utilizador do PSC pode estar a utilizar uma conta de um domínio diferente daquele que utiliza no Partner Center.

   Para resolver erros relacionados com os cenários 1 e 2, peça ao utilizador para se inscrever no Partner Center utilizando a sua conta de trabalho anexada ao seu inquilino Azure AD. O seu [administrador global](permissions-overview.md#manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles) pode ajudar.
   
   Para encontrar o seu administrador global: 
   1. Inscreva-se no painel de [instrumentos](https://partner.microsoft.com/dashboard) Do Centro de Parceiros e selecione **as definições** de conta do ícone de engrenagem no topo-direito.
   2. Selecione a **gestão** do utilizador a partir da barra de navegação do segundo nível, esquerda.
   3. No topo da lista de utilizadores, selecione o menu de entrega do **Filtro** e altere a opção para **administração Global.** A página apresenta então todos os administradores globais com os respetivos endereços de e-mail. Peça a um deles que atribua o papel de administrador de encaminhamento para a sua conta de trabalho.
   
      O administrador global pode criar uma nova conta de utilizador no seu inquilino AZure AD ou atribuir acesso ao utilizador convidado aos outros utilizadores de conta de domínio. Uma vez configuradas as contas para todos os gestores e utilizadores de negócios do PSC, eles precisam de iniciar sação no Partner Center, selecionar **Referências** do menu de navegação à esquerda e confirmar que podem ver a página de Referências.

3. O utilizador já tem uma função de encaminhamento atribuída no Partner Center.
    - Pode verificar o papel existente do utilizador. No canto superior direito do Partner Center, selecione **Definições** (o ícone de engrenagem) e, em **seguida, as definições de Conta**. Quando vir um segundo menu de navegação à esquerda, selecione **a gestão do Utilizador** e procure o utilizador.

## <a name="psc-deals-migration"></a>PSC negoceia migração

Depois de ter concluído a migração de utilizadores, use o assistente de migração de ofertas na página de oportunidades de co-venda para levar todas as ofertas abertas elegíveis do PSC para o Partner Center. **O link de migração de negócios será visível apenas para os administradores de encaminhamento com todo o âmbito de organização no Partner Center.** Existirá uma ligação com o nome **“migração de ofertas PSC”** no canto superior direito da página de oportunidades de venda conjunta, que abrirá o assistente de migração de ofertas.

Leia esta secção antes de iniciar a migração do negócio.

**Elegível para migração**

Apenas algumas ofertas são elegíveis para migração do PSC para o Partner Center. Este assistente de migração foi construído para ajudar os parceiros a levarem as suas ofertas para o Partner Center, onde ainda estão a trabalhar ativamente com os seus clientes para fechar o negócio. **Apenas os negócios que estão em estado aberto criados a partir de 1 de janeiro de 2020 com dados válidos da conta de parceiro (ID MPN válido) são elegíveis para migração.**

## <a name="pre-requisites-for-deal-migration"></a>Pré-requisitos para a migração de acordos

Antes de iniciar a migração do acordo do Partner Center, siga as instruções abaixo para estabelecer os acordos no PSC para uma migração bem sucedida.

- Todos os membros da equipa de vendas da sua empresa que trabalham nos negócios abertos são informados sobre esta migração.
- Os membros da equipa de vendas são treinados para usar o Partner Center para a gestão de negócios.
- Os negócios têm todas as informações necessárias, conforme descrito abaixo.
    - Detalhes da empresa do cliente, incluindo nome e endereço
    - Pelo menos uma solução
    - Pelo menos um membro da equipa com todos os detalhes - primeiro nome, apelido, ID de e-mail e número de telefone
    - Valor do negócio
    - Data de fecho do negócio estimada
    - Notas de parceiro

Você pode usar as capacidades de descarregamento e upload em massa no PSC para adicionar todos os detalhes em falta no negócio para todas as ofertas elegíveis.

>[!Note]
> A migração de acordos terá êxito, mesmo que os pré-requisitos acima referidos não sejam cumpridos. Mas não pode alterar o estado do negócio se algum dos campos acima mencionados exigidos no Partner Center não estiver disponível. Em seguida, terá de introduzir todas as informações necessárias que faltam nos negócios no Partner Center para começar a trabalhar nelas. **É fortemente aconselhável limpar as ofertas elegíveis no PSC antes de os migrar para o Partner Center.**

A migração de negócios no Partner Center é construída como uma experiência de um clique. Tudo o que precisa de fazer é clicar no botão **"Acordos migratórios"** assim que a sua empresa estiver pronta para migrar as ofertas elegíveis. **Não pode escolher os acordos que pretende migrar do PSC. Se não quiser migrar quaisquer negócios para o Partner Center, transloque-os para o estado fechado no PSC antes de iniciar a migração.**

>[!Note]
> Após o início da migração, **pode levar até 24 horas para os negócios serem migrados.**

Uma vez concluída a migração, a mensagem do banner terá o estado alterado para ser completada com um link para o relatório de migração. Faça o download do relatório para ver os detalhes das ofertas que foram migradas do PSC para o Partner Center.

O relatório inclui os detalhes abaixo.

- **Partner Center engagement ID** - O identificador único no Partner Center para todos os negócios em um noivado. Existem duas ofertas - uma para o parceiro e outra para a Microsoft num compromisso de co-venda no Partner Center.
- **Partner Center referenciação ID** - O identificador único no Partner Center para o negócio pertencente ao parceiro.
- **Nome do negócio** - Identificador dado ao negócio no PSC.
- **Identificação de acordo com o PSC** - O identificador único no PSC para o negócio.
- **Erros** - para indicar se há algum erro durante a migração de um negócio específico.

Todos os acordos que foram migrados com sucesso não serão visíveis no PSC. Pode continuar a trabalhar nos negócios migrados no Partner Center.

As ofertas migradas do PSC estarão disponíveis no separador Outbound da página de Oportunidades de Co-venda. Todos os negócios serão criados como acordos liderados por parceiros. São visíveis para os vendedores da Microsoft.

>[!Important]
> Se houver erros devidos aos quais algumas ofertas não puderam ser migradas, **pode relançar a migração do negócio clicando no botão "Acordos migratórios".** Só será ativado se houver algumas negociações elegíveis ainda por migrar. Isto também será útil se estiver na fase de transição onde alguns novos negócios estão a ser criados no PSC após o início da migração de acordos.

Uma vez que todos os negócios são migrados com sucesso, haverá banner mostrando **"No deals to migrar"** com o botão **"Migrar acordos"** a ser **desativado.**

## <a name="next-steps"></a>Passos seguintes

Aprenda a criar e gerir ofertas de IOT no Partner Center.
Este é um passo importante, que o ajudará a estar preparado para a gestão de negócios da IOT no Partner Center. Compreenda os fluxos de trabalho e as mudanças no Partner Center para que possa efetivamente criar e gerir negócios. Comece por ler completamente este documento.

## <a name="differences-between-psc-and-pc-workflows"></a>Diferenças entre fluxos de trabalho de CPE e PC

|**Cenário**|**Ligação de Vendas de Parceiros**|**Partner Center**|
|-----|:-----|:-----|
|Funções de utilizador|O PSC tem funções de administrador, gestor de negócios e vendedor.|O Partner Center tem funções [de administração e encaminhamento](permissions-overview.md#manage-referrals) de funções de utilizador que dão tanto permissão de leitura como de escrita com base no âmbito de localização.|
|Detalhes do vendedor da Microsoft|Visível assim que um acordo é criado.|Os detalhes do Microsoft Seller não são visíveis para os parceiros, uma vez que o tipo de negócio é liderado por parceiros.
|Soluções|Qualquer número de soluções podem ser adicionadas ao negócio.|O parceiro pode adicionar um máximo de 50 soluções ao negócio.
|Atribuição de acordo|Só o vendedor designado pode ver e agir sobre os negócios.|Os utilizadores de referência adicionados à secção de equipa de um negócio podem ver e agir sobre o negócio. Os administradores de encaminhamento para a localização da MPN para as quais o negócio foi criado podem ver e agir sobre o negócio.|
|Organização de clientes|Entrada de texto de formulário gratuito.|Pode pesquisar a organização do [cliente](manage-co-sell-opportunities.md#select-your-customer) contra a [base de dados D&B](https://www.dnb.com/) digitando apenas alguns caracteres. O nome e endereço legais são automaticamente preenchidos com base na escolha.|

## <a name="moving-from-psc-to-pc---faq"></a>Passar de PSC para PC - FAQ

As seguintes secções respondem a perguntas frequentes sobre a migração.

### <a name="1---what-should-i-do-if-i-dont-have-access-to-partner-center"></a>1 - O que devo fazer se não tiver acesso ao Partner Center?

Pode contactar os seus administradores listados na página "Não ter acesso" para obter as funções atribuídas. Você precisará da [função de administração de encaminhamento](permissions-overview.md#manage-referrals) para ler e escrever permissão sob a secção de referências. Se está a gerir apenas perfis de negócio, então vai precisar do perfil de negócios no Partner Center.

:::image type="content" source="images/pscmigration/noaccess.png" alt-text="Imagem mostrando a experiência de não acesso no Partner Center.":::

### <a name="2---who-can-grant-me-access-to-the-referrals-section-in-partner-center"></a>2 - Quem pode conceder-me acesso à secção de Referências no Centro de Parceiros?

A sua [administração](permissions-overview.md#manage-mpn-membership-and-your-company) de conta pode dar-lhe acesso ao separador Referências. Para encontrar a sua administração de conta, selecione **as definições** de Conta do ícone de engrenagem no topo-direito do [painel](https://partner.microsoft.com/dashboard)Partner Center . Em seguida, selecione **a gestão** do utilizador a partir da barra de navegação deixada no segundo nível. No topo da lista de utilizadores, selecione o menu de entrega do **filtro** e altere a opção de **administração de conta.** A página apresentará todos os administradores da conta com os respetivos endereços de e-mail. Peça a um deles que atribua o papel de administrador de encaminhamento para a sua conta de trabalho.

### <a name="3---the-new-deal-button-is-greyed-out-for-our-account-what-should-i-do-to-start-creating-deals"></a>3 - O botão +novo acordo está acinzentado para a nossa conta. O que devo fazer para começar a criar acordos?

Isto só acontece se o ID MPN associado à sua conta não estiver habilitado para a criação de negócios IOT. Contacte a equipa de negócios da IOT sobre o e-mail fornecido durante as sessões de formação ou crie um bilhete de apoio para obter o seu ID MPN habilitado para ofertas de IOT."

### <a name="4---can-i-assign-deals-to-a-specific-person-from-our-organization-like-psc"></a>4 - Posso atribuir ofertas a uma pessoa específica da nossa organização como o PSC?

Pode atribuir membros da equipa a um acordo específico. Não impede outros administradores de visualização ou atuação nesses negócios.

### <a name="5---is-there-a-view-of-all-the-deals-assigned-to-me"></a>5 - Existe uma visão de todos os negócios que me foram atribuídos?

Pode utilizar a funcionalidade favorito, que é um separador ao nível do utilizador. Pode marcar todas as ofertas que lhe são atribuídas como favoritas para ter um acesso rápido às ofertas.

### <a name="6---is-there-a-read-only-view-for-the-deals"></a>6 - Existe uma visão apenas de leitura para os negócios?

Não, não há uma visão apenas de leitura dos negócios na secção de referências.

### <a name="7---is-adding-a-customer-organization-mandatory"></a>7 - A adição de uma organização de clientes é obrigatória?

Sim, adicionar uma [organização de clientes](./manage-co-sell-opportunities.md#select-your-customer) é obrigatório no Partner Center. Comece por procurar o local onde o cliente está. Com base nos detalhes que tem; você pode adicionar detalhes específicos, incluindo o nome exato do edifício ou apenas dar detalhes da cidade. A pesquisa da organização irá buscar todas as entidades legais que correspondem ao nome que você insere para que você não tenha que inserir quaisquer detalhes de endereço. Todos os detalhes são preenchidos automaticamente com base na organização selecionada.

### <a name="8---are-customer-contact-details-mandatory"></a>8 - Os dados de contacto do cliente são obrigatórios?

Sim, os dados de contacto do cliente são obrigatórios para a criação de ofertas IOT.

### <a name="9---how-many-solutions-can-i-add-to-a-deal"></a>9 - Quantas soluções posso acrescentar a um acordo?

Pode adicionar até 50 soluções (análogas aos 'produtos' em PSC) a um acordo. Tanto a quantidade como a data de fecho estimada para as soluções são obrigatórias e a data de fecho estimada das soluções deve ser mais cedo do que a data de fecho estimada na secção detalhes do negócio.

### <a name="10---where-can-i-find-the-opportunity-id"></a>10 - Onde posso encontrar a oportunidade de imposição?

O ID de oportunidade no PSC é o mesmo que o ID de encaminhamento no Partner Center. Pode encontrar a identificação de referência ao lado do nome do negócio quando abrir qualquer negócio.
