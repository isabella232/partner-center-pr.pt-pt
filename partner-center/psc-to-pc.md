---
title: Migrar do Partner Sales Connect (PSC)
description: Saiba como os parceiros da Microsoft podem migrar do Partner Sales Connect (PSC) para Partner Center e criar ou gerir ofertas enviadas pelos vendedores da Microsoft.
ms.topic: article
author: vikramb
ms.author: vikramb
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 11/06/2020
ms.openlocfilehash: 34a18e4a4bf4d5c29265fdf76fae05b4ba16a3bc
ms.sourcegitcommit: 445c7b70943f71cc4b2cb48a327b9dcc1814974d
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/17/2020
ms.locfileid: "94670172"
---
# <a name="guide-to-co-selling-in-partner-center-pc-for-partners-migrating-from-partner-sales-connect-psc"></a>Guia para co-venda no Partner Center (PC) para parceiros que migram do Partner Sales Connect (PSC)

**Aplica-se a**

- Partner Center

**Funções adequadas**

- Administrador de conta
- Administração de referências
- Vendedor de Vendas de Parceiros (PSC)
- Administrador de Vendas de Parceiros (PSC)
- Gestor de negócios Partner Sales Connect (PSC)

Como sabem, a sua empresa perderá acesso ao PSC pós-31 de março de 2021. No entanto, encontrará tudo o que pretende fazer para criar ofertas de co-venda, gerir as suas ofertas e agir sobre ofertas enviadas pelos vendedores da Microsoft no Partner Center. Haverá diferenças no entanto, e as seguintes orientações ajudarão a tornar a sua transição para o Partner Center mais suave e diretamente para a frente.

>[!Important]
> Se está aqui porque viu um estandarte no PSC sobre a migração, está no lugar certo. Este guia não é aplicável aos parceiros de Avaliação de Soluções (SA) e OEM IOT que gerem as suas ofertas em PSC.

## <a name="before-you-move-things-you-need-to-know"></a>Antes de te mexeres, as coisas que precisas de saber

### <a name="if-you-are-psc-admin"></a>Se você é administrador do PSC

- Precisa de um e-mail de trabalho para iniciar sessão no [Partner Center.](https://partner.microsoft.com/)
- Crie a sua conta com a ajuda da [administração](permissions-overview.md)da conta Partner Center .
- Saiba como co-vender no Partner Center lendo este documento.
- Configurar contas de utilizador no Partner Center para todos os seus utilizadores de PSC (funções de Administrador, Gestor de Acordos e Vendedor) e atribuir-lhes [funções de administração de encaminhamento](permissions-overview.md).

>[!Important]
> Certifique-se de que o ID MPN mostrado no banner do PSC está disponível na lista de localizações mpn no Partner Center. Pode verificar isso no Partner Center indo para "Definições de Conta" e "[Localizações](manage-locations.md)" sob isso para encontrar a lista de todos os MPNs associados à conta partner Center.

:::image type="content" source="images/pscmigration/mpnidcheck.png" alt-text="Imagem mostrando o banner do PSC onde os parceiros podem encontrar o ID MPN.":::

### <a name="if-you-are-psc-deal-manager-or-seller"></a>Se você é gestor de negócios psc ou vendedor

- Precisa de um e-mail de trabalho para iniciar sinscê-lo no [Partner Center.](https://partner.microsoft.com/)
- Se estiver a utilizar uma conta não-trabalho no PSC ou o seu email de trabalho for para uma empresa diferente da empresa parceira, contacte o administrador do PSC para obter ajuda de configuração de conta.
- Consulte o seu administrador do PSC se a configuração da sua conta Partner Center está completa independentemente da conta que utiliza para iniciar sessão no PSC.
- Verifique se tem acesso ao Partner Center e à secção de Referências.
- Leia este documento para compreender os fluxos de trabalho e as alterações no Centro de Parceiros.

## <a name="as-an-admin-in-psc-these-are-your-next-steps"></a>Como administrador no PSC, estes são os seus próximos passos

Se não vir o separador Referências:

- O administrador [global](permissions-overview.md) da sua empresa pode dar-lhe acesso ao separador Referências. Para encontrar o seu administrador global, vá para as definições de Parceiro a partir do ícone de engrenagem no topo direito do Partner Center. Selecione a página de gestão do Utilizador no segundo nível da barra de navegação esquerda. Clique no drop-down que mostra "Todos os utilizadores" no topo direito da página e mude para "Global Admins". A página irá então exibir todos os administradores globais com os respetivos IDs de e-mail. Contacte-os para obter acesso "Administrativo de Encaminhamento" para a sua conta de trabalho.

  >[!Important]
  > Se o seu papel é apenas gerir utilizadores em PSC, você pode obter você é o papel [de administrador de conta](permissions-overview.md#manage-mpn-membership-and-your-company) no Partner Center. Se o seu papel também inclui gerir oportunidades de co-venda, você deve obter o papel [de administrador de referências.](permissions-overview.md#manage-referrals) Além disso, nomeie um líder de gestão de mudança entre os administradores do PSC para trabalhar com a administração da conta Partner Center em vez de todos os administradores do PSC que chegam individualmente aos administradores da conta no PC.

  :::image type="content" source="images/pscmigration/accountadmin.png" alt-text="Imagem mostrando os administradores de conta na página de gestão de utilizadores de definições de parceiros.":::

- Vá ao separador Referências no painel de navegação à esquerda e verifique se pode aceder às páginas.

  >[!Note]
  > Poderá ter de assinar fora do Centro parceiro e voltar a inscrever-se para refrescar as suas credenciais de acesso às páginas de Referências.

## <a name="user-migration"></a>Migração de utilizadores

Depois de configurar a sua conta no Partner Center, utilize o assistente de migração do utilizador na página de oportunidades de co-venda para atribuir automaticamente funções do Partner Center aos colaboradores da sua empresa.

>[!Note]
> A migração de utilizadores só pode ser realizada por administradores de [conta](permissions-overview.md#manage-mpn-membership-and-your-company) da sua empresa. Se não tiver a função de administrador de conta, encontre um administrador de conta que possa ajudar a configurar as contas do utilizador com a ajuda do assistente de migração do utilizador. A funcionalidade de migração dos utilizadores estará disponível a partir de 18 de novembro de 2020.

:::image type="content" source="images/pscmigration/psc-user-migration.png" alt-text="Imagem mostrando o assistente de migração do utilizador.":::

Os administradores de conta receberão um link de assistente de migração de utilizadores de PSC na página de oportunidades de co-venda ao lado do guia de referências. Podem iniciar a migração do utilizador clicando no link. Esta ação pode ser realizada várias vezes até que todos os utilizadores que a empresa quer migrar sejam atribuídos papéis adequados no Partner Center.

A tabela de migração do utilizador tem os seguintes detalhes

- Conta de utilizador - ID de e-mail do funcionário
- Conta parceira do PSC - A conta a que o trabalhador está associado no PSC
- Função de utilizador do PSC - Uma das três funções atribuídas no PSC.
- Localização PC MPN - Local para o qual o utilizador receberá funções relevantes para PC. A conta parceira do PSC MPN é usada para encontrar a localização MPN equivalente no Partner Center para atribuir permissões. Toda a organização denota o vOrg MPN ID.
- Função de utilizador do PC - Os colaboradores são atribuídos funções com base nas suas funções de utilizador do PSC. A administração no PSC será atribuída a funções de administração de referências no PC. Será atribuído ao vendedor a função de utilizador de referências no PC. Saiba mais sobre os papéis do PC e o que os utilizadores com estas funções podem fazer no centro parceiro [aqui](permissions-overview.md#manage-referrals)
- PC AAD Tenant - o inquilino a que os utilizadores estão designados no Partner Center
- Estado - Existem três Estados possíveis para o estado da migração
    - Não migrado - O utilizador não tem qualquer função de referência para PC atribuída
    - Migrado - O utilizador foi migrado com sucesso com papel relevante atribuído como mostrado na tabela
    - Erro - Incapaz de completar a migração devido a algum erro

A migração pode falhar e resultar em erros em algumas condições para as quais as soluções são fornecidas abaixo

1. Os utilizadores de CPS podem estar a utilizar uma conta não-trabalho.

2. Os utilizadores de PSC podem estar a utilizar uma conta de um domínio diferente daquele que está a usar no Partner Center.

   - Para resolver erros relacionados com os cenários 1 e 2, todos esses utilizadores precisam de se inscrever no Partner Center utilizando a sua conta de trabalho anexada ao seu inquilino AZure AD. O teu [administrador global](permissions-overview.md#manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles) pode ajudar nisto. Para encontrar o seu administrador global, vá para as definições de Parceiro a partir do ícone de engrenagem no topo direito do Partner Center. Clique na página de gestão do Utilizador no segundo nível da barra de navegação esquerda. Clique no drop-down que mostra "Todos os utilizadores" no topo direito da página e mude para "Global Admins". O administrador Global pode criar uma nova conta de utilizador no seu inquilino AZure AD ou atribuir acesso de utilizador a outros utilizadores de conta de domínio. Uma vez que as contas são configuradas para todos os gestores e utilizadores de negócios do PSC, eles precisam de iniciar sação no Partner Center, ir ao separador De referência na navegação à esquerda, e verificar se eles podem ver a página de Referências.

3. O utilizador já tem uma função de encaminhamento atribuída no Partner Center.
    - Pode verificar o papel existente do utilizador a partir da página de gestão do Utilizador nas definições da conta e modificar o mesmo que necessário.

Depois de concluída a migração dos utilizadores, utilize as seguintes orientações para decidir a estratégia de migração: 

Se a sua empresa tiver um PDM - Quando a sua conta Partner Center estiver configurada e os seus utilizadores tiverem movimentos e permissões, pode mover as suas atividades de Co-venda para Partner Center. Informe o PDM para fazer a troca em vez de esperar até que a sua migração complete o prazo, o que permitirá que todas as suas novas ofertas fluam para o Partner Center.

>[!Note]
>Uma vez feita esta troca, só poderá atuar sobre as ofertas ativas existentes no PSC. Não pode criar novas ofertas nem receber quaisquer ofertas de vendedores da Microsoft no PSC.

Se a sua empresa não tiver um PDM - Certifique-se de que todas as contas de utilizador são configuradas e verificadas por todos os utilizadores. Será notificado através de um e-mail e de um banner no PSC sobre a data exata em que pode começar a Co-vender no Partner Center. Lembre-se que ainda terá de gerir os negócios ativos existentes no PSC.

>[!Important]
>As ofertas ativas não serão migradas para PC. Tem até 31 de dezembro de 2020 para fechar e registar as transações.

## <a name="next-steps-for-psc-admins-psc-deal-managers-and-psc-sellers"></a>Próximos passos para administradores de PSC, gestores de acordos de PSC e vendedores de PSC

Saiba como co-vender no Partner Center.
Este é um passo importante, que o ajudará a estar preparado para a Co-venda no Partner Center. Compreenda os fluxos de trabalho e as mudanças no Partner Center para que possa efetivamente Co-vender desde o primeiro dia. Comece por ler completamente este documento. Um bom conjunto de recursos também está disponível na [galeria de experiências Co-sell.](https://aka.ms/cosellexperience)

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

## <a name="psc-and-partner-center-field-mapping"></a>Mapeamento de campo do Centro de PSC e Parceiro

Esta secção apresenta o mapeamento exato de atributos entre o PSC e o Partner Center. Cada ecrã em PSC é comparado com a vista relevante na secção de oportunidades de co-venda do Partner Center. 

>[!Note]
>Siga os números nas bolhas amarelas em imagens de PSC para encontrar o atributo equivalente no Partner Center. As bolhas vermelhas indicam que o arquivado não está disponível no Partner Center.

**Página inicial do PSC e vista padrão das oportunidades de Co-venda no Partner Center**

 :::image type="content" source="images/pscmigration/homepage.png" alt-text="Imagem mostrando os mapeamentos de campo entre a página inicial do Partner Sales Connect e a visão padrão de Oportunidades de Co-venda no Partner Center.":::

**Vista da grelha do PSC e a vista de negócio do Centro Parceiro**

- Não há nenhuma vista de lista no Partner Center como a do PSC.  Todas as ofertas são listadas com base na data mais recente recebida ou criada com a informação do cliente e o tipo de negócio. O primeiro negócio na vista é selecionado por padrão. A maioria dos valores que são apresentados no formato de tabela do PSC estão disponíveis na visão detalhada do negócio no PC.
- O papel do negócio não é um campo obrigatório no PC. Não é exibido nem capturado em nenhum dos fluxos de trabalho. É derivado automaticamente do lado do vendedor da Microsoft com base nas soluções adicionadas ao negócio.
- A última data modificada não é apresentada na página de detalhes de encaminhamento no PC. Os parceiros podem usar a funcionalidade de tipo para classificar as ofertas com base na última data atualizada.

:::image type="content" source="images/pscmigration/gridview.png" alt-text="Imagem mostrando os mapeamentos de campo entre a vista da grelha de vendas de parceiros (PSC) e a vista de negócio do Partner Center.":::

**Vista de detalhes do negócio no PSC e Partner Center**

- Os parceiros podem editar um negócio clicando no botão de edição na vista de detalhes do negócio do parceiro (6). Uma vez que o botão de edição é clicado em todos os campos tornar-se-ão editáveis com a opção de guardar ou cancelar as edições feitas para o negócio.
- Não há opção para fechar o negócio como duplicado no Partner Center.
- O Resultado do Cliente não está disponível no centro de parceiros. Todos os detalhes relacionados com as interações do cliente podem ser atualizados na secção Notas no PC.
- A data de fecho estimada da solução só está disponível nas ofertas do OEM IOT no Partner Center. Não é exibido para outros tipos de negócio.
- O programa de licenciamento não é necessário no PC. É deduzido automaticamente com base nas soluções selecionadas no negócio.

>[!Note]
>Qualquer negócio marcado como ganho ou perdido não pode ser editado post que. Tenha cuidado ao mudar um negócio para um destes estados terminais.

:::image type="content" source="images/pscmigration/dealdetails.png" alt-text="Imagem mostrando os mapeamentos de campo entre a visão de detalhes de negócio do Partner Sales Connect (PSC) e a visão de detalhes do negócio do Partner Center.":::

**Visão de "Adicionar Produtos" do PSC e a visão do Centro Parceiro 'Adicionar soluções'**

:::image type="content" source="images/pscmigration/products.png" alt-text="Imagem mostrando os mapeamentos de campo entre o Partner Sales Connect (PSC) adicionar a vista de produtos e o Centro de Parceiros adicionar visão de soluções.":::

**Gestão de utilizadores em PSC e Partner Center**

 :::image type="content" source="images/pscmigration/usermanagement.png" alt-text="Imagem mostrando os mapeamentos de campo entre a casa de gestão do utilizador Partner Sales Connect (PSC) e a gestão do utilizador do Partner Center na visualização das definições de conta.":::

**Atribuição de função de utilizador no PSC e Partner Center**

- O papel equivalente para a administração do PSC é o papel de administrador de conta no Partner Center.
- Há apenas um papel no Partner Center para a gestão de negócios de co-venda que é o papel de administração de referência.

:::image type="content" source="images/pscmigration/roles.png" alt-text="Imagem mostrando os mapeamentos de campo entre a visão de atribuição de funções Partner Sales Connect (PSC) e a vista de atribuição de funções do Partner Center.":::

**Notificações no PSC e centro de parceiros**

:::image type="content" source="images/pscmigration/notifications.png" alt-text="Imagem mostrando o mapeamento entre as notificações Partner Sales Connect (PSC) e a visualização de notificações do Partner Center.":::

## <a name="moving-from-psc-to-partner-center---frequently-asked-questions"></a>Passar de PSC para Partner Center - Perguntas frequentes

**Q1. O que devo fazer se não tiver acesso ao Partner Center?**

Pode contactar os seus administradores listados na página "Não ter acesso" para obter as funções atribuídas. Você precisará de um papel de "[administração](permissions-overview.md#manage-referrals)de referência " para ler e escrever permissão sob a secção de referências. Se estiver a gerir apenas perfis de negócio, então precisará do papel de administrador de perfil de negócios no centro de parceiros.

:::image type="content" source="images/pscmigration/noaccess.png" alt-text="Imagem mostrando a experiência de não acesso no Partner Center.":::

**Q2. Quem me pode dar acesso à secção de referências no Centro de Parceiros?**

O administrador da sua [conta](permissions-overview.md#manage-mpn-membership-and-your-company) pode dar-lhe acesso ao separador Referências. Para encontrar o administrador da sua conta, vá para as definições de Parceiro a partir do ícone de engrenagem no topo direito do Partner Center. Clique na página de gestão do Utilizador no segundo nível da barra de navegação esquerda. Clique no drop-down que mostra "Todos os utilizadores" no topo direito da página e altere para "Administradores de Conta". A página irá então exibir todos os administradores da Conta com os respetivos IDs de e-mail. Contacte-os para obter acesso "Administrativo de Encaminhamento" para a sua conta de trabalho.

**Q3. O botão +new deal está acinzentado para a nossa conta. O que devo fazer para começar a criar acordos?**

Isto só acontece se não houver soluções prontas de Co-venda anexadas à organização MPN que está a utilizar no Partner Center. Contacte o seu PDM para obter o ID MPN das suas soluções corrigido ou crie um bilhete de apoio que mencione o problema "Novo botão de negócio acinzentado após a migração do PSC."

**Q4. Posso atribuir ofertas a uma pessoa específica da nossa organização como o PSC?**

Pode atribuir membros da equipa a um acordo específico. Não impede outros administradores de visualização ou atuação nesses negócios. 

**Q5. Há alguma visão de todos os acordos que me foram atribuídos?**

Pode utilizar a funcionalidade favorito, que é um separador de nível de utilizador. Pode marcar todas as ofertas que lhe são atribuídas como favoritas para ter um acesso rápido às ofertas.

**Q6. Há uma visão só de leitura para os negócios?**

Não, não há uma visão apenas de leitura dos negócios na secção de referências. Todos os administradores de referência terão leitura completa e escreverão acesso a todos os negócios.

**Q7. Como posso registar um acordo depois de o ter feito como ganho?**

Se o negócio cumprir os critérios abaixo, mostraremos um pop-up para iniciar o [registo do negócio.](./register-deals.md)

- Há uma solução elegível de incentivo anexa ao negócio.
- O vendedor da Microsoft é convidado a participar no negócio, ou convidaram-no para o negócio.
- O cartão Microsoft está no estado Aceite ou Ganho no Partner Center.

**Q8. Recebo uma mensagem de erro quando clico no botão "+New deal registration" na secção De Registo de Negócios. Como posso registar os meus acordos?**

O "+Registo de negócio novo" deve ser utilizado apenas pelos parceiros que estão registados no programa de ligação ISV para registar um acordo sem oportunidade de co-venda correspondente no Partner Center. Para registar negócios com uma oportunidade de co-venda, um pop-up será exibido quando o negócio for marcado como ganho e se cumprir os critérios de registo do negócio.

**Q9. Adicionar uma organização de clientes é obrigatório?**

Sim, adicionar uma [organização de clientes](./manage-co-sell-opportunities.md#select-your-customer) é obrigatório no Partner Center. Comece por procurar o local onde o cliente está. Com base nos detalhes que tem; você pode ser específico, incluindo o nome exato do edifício ou apenas dar detalhes da cidade. A pesquisa da organização irá buscar todas as entidades legais que correspondem ao nome que inseriu para que não tenha de inserir nenhum endereço. Todos os detalhes são preenchidos automaticamente com base na organização selecionada.

**Q10. Os dados de contacto do cliente são obrigatórios?**

Depende do [tipo de acordo](./manage-co-sell-opportunities.md#types-of-co-sell-opportunities) que está a criar. Se estiver apenas a partilhar o seu oleoduto e não necessitar de ajuda da organização de vendas da Microsoft, pode optar por não dar detalhes de contacto com o cliente. Se estiver a co-vender onde está ativamente à procura de ajuda do vendedor da Microsoft, terá de fornecer os dados de contacto do cliente. Deve obter o consentimento explícito do cliente antes de criar um pedido de co-venda no centro de parceiros.

**Q11. Quantas soluções posso acrescentar a um acordo?**

Pode adicionar até 50 soluções (análogas aos 'produtos' do PSC) a um acordo. Ao contrário do PSC, pode misturar soluções a partir de suas próprias soluções elegíveis co-venda, SKUs de primeira parte da Microsoft e outras soluções elegíveis de terceiros. Não há nenhuma função de negócio que deve ser selecionado ou disponível no centro parceiro. Para o Microsoft SKUs, pode opcionalmente adicionar quantidade e preço para cada SKU que é adicionado ao negócio.

**Q12. Quando vou conhecer os detalhes do vendedor da Microsoft depois de criar um acordo?**

Os vendedores da Microsoft são atribuídos apenas depois de corresponderem ao requisito de ajuda exato indicado enquanto criam o negócio com a personalidade do vendedor relevante no lado da Microsoft. Mesmo após a atribuição, os vendedores da Microsoft terão a opção de aceitar ou rejeitar o convite de co-venda. Só se um convite de co-venda for aceite por um vendedor, o negócio será atualizado com os dados de contacto do vendedor da Microsoft. O SLA para os vendedores da Microsoft agirem no negócio é de 14 dias. É o mesmo SLA que os sócios têm de agir sobre o negócio antes de entrar em estado caducado.

**Q13. Onde posso encontrar a oportunidade de encontrar a oportunidade de encontrar a oportunidade de id?**

O ID de oportunidade no PSC é o mesmo que o ID do negócio no PC. Pode encontrar a identificação do negócio ao lado do nome do negócio quando abrir qualquer negócio.

**Q14. Como é que o meu PDM pode ter acesso ao PC?**

O Partner Center não pode ser acedido pelos seus PDMs diretamente ao contrário do PSC. Existem múltiplas opções para ativar essa capacidade, que são mencionadas abaixo.

- OCP Insights - Se os PDMs estiverem apenas a ver as ofertas & progressos relacionados com eles, podem usar o portal OCP Insights para obter a sua visão da organização. Esta é uma ferramenta interna e disponível apenas para PDMs. Note que os insights OCP não estão disponíveis para os utilizadores da sua empresa.
- Utilizador convidado no Partner Center - Pode adicionar a sua conta PDM @microsoft.com como utilizador convidado no centro de parceiros e atribuir-lhes funções de administração de encaminhamento para que possam visualizar e agir em referências.
- Criar um [novo utilizador](./create-user-accounts-and-set-permissions.md#add-a-new-user) no seu inquilino - Pode criar um novo utilizador no seu próprio inquilino e partilhar esses detalhes com o PDM para que possam ver e agir em referências semelhantes a outros utilizadores de referência na sua conta.

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

## <a name="next-steps"></a>Próximos passos

Siga estes recursos adicionais:

- [Partner Sales Connect to Partner Center workbook](https://partner.microsoft.com/resources/detail/partner-sales-connect-to-partner-center-transition-workbook-pptx) - livro para alinhar os processos e funções de vendas dos parceiros com novos processos de vendas via Partner Center vs. Partner Sales Connect.
- [Partner Center co-sell operating guide](https://partner.microsoft.com/resources/detail/co-sell-operating-model-guide-pptx) - orientação para identificar um modelo operativo via Partner Center para gerir leads ou co-vender oportunidades e registar ofertas.
- [Deck de gestão](https://partner.microsoft.com/resources/detail/referral-management-in-partner-center-pptx) de encaminhamento - instrução passo a passo visualizada para gerir leads e co-vender oportunidades através do Partner Center.
- [Publicar e gerir no mercado comercial](https://partner.microsoft.com/resources/detail/publishing-and-managing-co-sell-offers-in-commercial-marketplace-pptx) - instrução visualizada passo a passo para criar, gerir e publicar ofertas através do Partner Center no mercado comercial.
