---
title: Movendo-se do Centro de Adesão de Parceiros
ms.topic: article
ms.date: 06/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Reveja as informações úteis e as perguntas frequentes antes de mudar o seu negócio do Partner Membership Center para Partner Center.
author: parthpandyamsft
ms.author: parthp
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: b267f89ec1c7b27e87eaaf3d7b594ebbd0fd6942
ms.sourcegitcommit: a691d4cbe144a8fd71e344fd293cc658ac11d6f3
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/27/2021
ms.locfileid: "105633884"
---
# <a name="prepare-for-your-move-from-partner-membership-center-pmc-to-partner-center"></a>Prepare-se para a sua mudança do Centro de Adesão de Parceiros (PMC) para o Partner Center

**Funções adequadas**

- Administrador global
- Administração de gestão de utilizadores
- Agente comercial
- Agente administrativo

Estamos a mudar a gestão de membros do Partner Membership Center (PMC) para o Partner Center - o destino único para gerir a sua relação comercial com a Microsoft. Queremos que a sua mudança para o Partner Center seja o mais eficiente e fácil possível. Identificamos algumas áreas onde o Centro de Parceiros difere do PMC, e achamos que vai querer entender e preparar-se para elas antes de avançar.

## <a name="account-and-identity-setup"></a>Configuração de conta e identidade

Consulte abaixo as respostas a perguntas comuns sobre a configuração de conta e identidade.

### <a name="what-is-an-azure-active-directory-azure-ad-work-account"></a>O que é uma conta de trabalho do Azure Ative Directory (Azure AD) ?

Uma conta de trabalho Azure é uma representação virtual dedicada e isolada da sua empresa na nuvem pública Azure, criada para si quando subscreve um serviço de cloud da Microsoft como Azure, Microsoft Intune ou Office 365.

A sua conta de trabalho acolhe os seus utilizadores AD Azure e as informações sobre eles - o seu email, palavras-passe, dados de perfil, permissões, e assim por diante. A conta de trabalho contém também grupos, aplicações e outras informações relativas a uma empresa e à sua segurança. 

O seu email de trabalho faz parte do seu inquilino de diretório ativo Azure. Para ter uma conta no Partner Center, precisa de ter um inquilino da AAD. Para obter mais informações sobre o Azure Ative Directory, leia [Criar o seu diretório em Azure AD](/azure/active-directory/fundamentals/add-custom-domain#create-your-directory-in-azure-ad).

No Partner Center, utilizará o seu email de trabalho para iniciar scontabilidade e não para o seu email pessoal.

- A sua conta de trabalho: john@contoso.com
- A sua conta pessoal: John@outlook.com

### <a name="what-account-should-you-sign-into-partner-center-with-if-you-have-an-aad-tenant-with-microsoft-for-office-365-for-example-and-you-also-have-a-tenant-for-your-csp-business"></a>Com que conta deve assinar no Partner Center se tiver um inquilino da AAD com a Microsoft (para o Office 365, por exemplo) e também tiver um inquilino para o seu negócio de CSP?

Pode inscrever-se no Partner Center com a conta CSP ou com a sua conta de e-mail de trabalho MPN. Se optar por iniciar sposição utilizando o seu email de trabalho CSP, a navegação à esquerda no seu painel de instrumentos apresentará as informações do programa MPN e CSP. Se iniciar sedições com o seu e-mail de trabalho do seu inquilino MPN Azure AD, verá apenas a informação do seu programa MPN. 

### <a name="if-you-dont-want-to-use-your-existing-office-365-azure-ad-tenant-for-partner-center-you-can-create-a-new-tenant-prior-to-migrating-from-pmc"></a>Se você não quiser usar o seu inquilino AD Azure 365 existente para o Partner Center, você pode criar um novo inquilino antes de migrar do PMC.

Pode haver muitas razões para não querer usar um inquilino AZure AD existente para criar a sua conta Partner Center. Antes de começar a migrar para o Partner Center, vá ao [portal Azure](https://ms.portal.azure.com/#home) para criar um novo inquilino AZure AD. Siga as orientações em [Criar um novo inquilino no Azure Ative Directory](/azure/active-directory/develop/quickstart-create-new-tenant). Use o novo inquilino da AAD para criar a sua conta Partner Center. Deve ser um administrador global para criar o inquilino. 

### <a name="user-roles-including-guest-user-roles-in-partner-center"></a>Funções de utilizador, incluindo funções de utilizador convidado no Partner Center

O Partner Center tem diferentes tipos de funções dependendo dos tipos de trabalho necessários para ser feito. Há papéis como a administração global que são papéis de AD Azure. Algumas das funções são específicas de programas como o programa cloud service provider ou incentivos, e há papéis específicos da MPN. Para saber quais são todas as funções do Partner Center, leia [atribuir as funções e permissões dos utilizadores](permissions-overview.md).

### <a name="what-happens-to-my-users-roles-when-they-move-from-pmc-to-partner-center"></a>O que acontece com as funções dos meus utilizadores quando se mudam de PMC para Partner Center?

Com exceção do contacto global de administração ou programa primário da MPN que conduz a migração, todos os utilizadores em PMC perderão as suas funções de administrador. O indivíduo que completar a migração terá de atribuir funções no Partner Center. As funções no Partner Center diferem das funções no PMC. Leia [Atribuir as funções e permissões dos utilizadores](permissões-overview.md e [mover-se de PMC para Partner Center](move-pmc-pc-map.md#user-roles) para obter mais sobre as funções dos utilizadores no Partner Center.

### <a name="whats-the-difference-between-my-company-profile-and-my-business-profile"></a>Qual é a diferença entre o meu perfil de empresa e o meu perfil de negócios?

O perfil da sua empresa é a informação sobre a sua empresa que inclui endereços, localizações, contacto primário, banco e detalhes fiscais.

O seu perfil de negócio é a forma como se apresenta aos clientes e é uma página de marketing que exibe o seu logótipo, detalhes sobre o seu foco de negócio, a sua experiência, etc.

### <a name="what-does-account-consolidation-mean-for-my-account"></a>O que significa consolidação de contas para a minha conta?

Se utilizar o mesmo inquilino AZure AD para migrar várias contas MPN para o Partner Center, o sistema reconhecerá automaticamente isso e pedir-lhe-á para consolidar as suas contas. Isto é verdade mesmo que você tenha vários domínios associados ao mesmo inquilino AD Azure. 

Você ainda pode decidir migrar para o Partner Center usando inquilinos separados da AAD, mas note isso resulta em avaliação isolada das suas competências e custos de compra extra. Para obter mais informações sobre a consolidação de contas, leia [Consolidar as contas da sua empresa](consolidate-accounts.md)

### <a name="if-i-have-multiple-aad-tenants-and-a-single-mpn-account-is-it-possible-to-link-them-in-partner-center"></a>Se eu tiver vários inquilinos da AAD e uma única conta MPN, é possível ligá-los no Partner Center?

Sim, no Partner Center pode ligar vários inquilinos da Azure AD a uma única conta do Partner Center.
Para obter mais informações sobre a consolidação de contas, leia [Consolidar as contas da sua empresa](consolidate-accounts.md)

### <a name="are-there-restrictions-to-adding-multiple-azure-ad-tenants-to-a-single-partner-center-account"></a>Existem restrições para adicionar vários inquilinos da AD Azure a uma única conta partner Center?

Se o inquilino AZURE AD já estiver associado a uma conta existente do Partner Center, não pode ser associado a novas contas do Partner Center utilizando a funcionalidade multi-arrendamento. Outra forma de pensar é que um inquilino AZure AD só pode ser associado a uma conta do Partner Center, mas uma conta partner Center pode ter vários inquilinos associados a ela.

## <a name="microsoft-partner-network-mpn-membership-migration"></a>Migração de membros da Microsoft Partner Network (MPN) 

Consulte as seguintes respostas a perguntas comuns sobre a migração de membros da MPN.

### <a name="who-can-perform-the-move-from-pmc-to-partner-center"></a>Quem pode realizar a mudança de PMC para Partner Center?

A administração global da sua empresa MPN ou o contacto do programa primário (estas duas funções são muitas vezes detidas pela mesma pessoa) podem iniciar e executar o movimento.

### <a name="will-the-person-completing-the-migration-become-the-primary-contact-on-the-company-legal-profile-in-partner-center"></a>A pessoa que completa a migração tornar-se-á o principal contacto sobre o perfil jurídico da empresa no Partner Center?

No entanto, não necessariamente, o contacto primário tem de ser alguém que tenha autorização para assinar acordos.

### <a name="can-microsoft-migrate-my-mpn-membership-for-me"></a>A Microsoft pode migrar a minha filiação mpn para mim?

N.º A Microsoft não pode ajudá-lo a mover a sua conta de membro para o centro de parceiros. Terá de mover a sua conta ao inscrever-se no PMC com a sua conta de trabalho (assinar em credenciais) para iniciar o processo de migração. Depois de ter concluído os passos para mover a sua conta, pode começar a gerir a sua adesão e atribuir funções e permissões de utilizador à sua equipa para que possam aceder aos benefícios e ajudar a gerir a adesão. 

A Microsoft migrará automaticamente as competências, benefícios, informações de localização, informação bancária/fiscal para incentivos e associações MCP, incluindo o acesso à Universidade Parceira.

### <a name="how-will-the-renewal-policy-change"></a>Como é que a política de renovação vai mudar?

No Partner Center, a janela de renovação é da data do seu aniversário até os 30 dias seguintes.

### <a name="will-our-competencies-remain-unchanged-after-we-move-to-partner-center"></a>As nossas competências permanecerão inalteradas depois de nos mudarmos para o Partner Center?

Sim, as competências não serão afetadas pela mudança para o Centro de Parceiros. Se notar discrepâncias, contacte [o Suporte](https://partner.microsoft.com/support).

### <a name="will-my-benefits-including-cloud-benefits-technical-support-software-benefits-visual-studio-change-after-we-move"></a>Os meus benefícios (incluindo benefícios na nuvem, suporte técnico, benefícios de software, Visual Studio) mudarão depois de nos mudarmos?

Os seus benefícios elegíveis não mudarão. Se notar discrepâncias, contacte [o Suporte](https://partner.microsoft.com/support).

### <a name="will-our-microsoft-accounts-that-have-visual-studio-benefits-allocations-be-honored"></a>As nossas contas da Microsoft que têm alocações de benefícios do Visual Studio serão honradas?

Sim. Os benefícios do Estúdio Visual atribuídos aos MSAs serão honrados e retidos. Também serão preservados após a renovação no Partner Center. No entanto, se remover uma alocação de MSA uma vez migrada no Partner Center, não pode ser adicionada de volta ao Partner Center.

No Partner Center, um parceiro pode adicionar contas de trabalho e contas de utilizador convidado, que são MSA do mesmo inquilino onde o parceiro é administrador MPN no inquilino AZure AD. Se o parceiro é um administrador global em vários inquilinos da AD Azure e todos estes inquilinos estão associados à mesma conta Partner Center, então o parceiro é autorizado a adicionar utilizadores em todos estes inquilinos para os benefícios do Estúdio Visual e alolocações baseadas em uso Azure.

Embora os utilizadores convidados possam ser atribuídos subscrições baseadas no uso do Visual Studio pelo administrador MPN ou administração global, os utilizadores convidados não podem entrar no Partner Center usando o seu MSA. Os utilizadores convidados podem, no entanto, iniciar sessão no Azure e no Visual Studio para validar e utilizar os seus benefícios atribuídos.

### <a name="how-should-we-manage-our-mcp-associations-and-our-partner-university-access"></a>Como devemos gerir as nossas associações MCP e o nosso acesso à Universidade Parceira?

Não há alterações nas associações MCP que se movem do PMC. No entanto, quaisquer novos colaboradores depois de se mudarem para o Partner Center terão de ser associados no Partner Center. Todas as permissões da Universidade Parceira para os utilizadores existentes permanecerão, mas quaisquer novos funcionários devem ir ao [centro de formação](https://partner.microsoft.com/training) para obter informações sobre como ter acesso à Partner University.

### <a name="how-do-i-view-mcp-information-once-i-move-to-partner-center"></a>Como vejo a informação do MCP assim que me mudo para o Partner Center?

Selecione **Competências** da navegação esquerda no painel de instrumentos. Na página **De Competências,** você é capaz de baixar o relatório de competências. O relatório de competências irá listar os seus utilizadores que adquiriram competências relevantes para as competências e programas no Partner Center. Se os seus utilizadores tiverem adquirido competências, mas essas competências não forem relevantes para as competências para as quais está a trabalhar, não serão listadas no relatório.

### <a name="are-customer-references-used-in-partner-center"></a>As referências ao cliente são utilizadas no Partner Center?

Não, não precisa de referências de clientes para satisfazer os requisitos de competência no Partner Center.

### <a name="will-partner-of-record-associations-move-to-partner-center"></a>A Partner of Record associações vai mudar-se para o Partner Center?

Sim, não há nenhuma alteração para o Parceiro da Record. Saiba mais sobre [a ligação da identificação do seu parceiro aos seus clientes.](/azure/billing/billing-partner-admin-link-started)

### <a name="is-there-an-impact-to-incentives-because-of-the-move-to-partner-center"></a>Existe um impacto nos incentivos por causa da mudança para o Partner Center?

Não, não há impacto em incentivos se tiver mudado a sua conta sem consolidar localizações. Se o seu negócio tiver várias contas em PMC e, quando se muda para o Partner Center, decide consolidar-se numa conta global, não haverá perdas para incentivos, mas pode haver um atraso no pagamento de incentivos. 

Se não mover todas as suas contas pmc que estiveram envolvidas em programas de incentivos, pode parar de ganhar incentivos que estão ligados a essas contas.

### <a name="what-are-the-incentive-roles-in-partner-center"></a>Quais são as funções de incentivo no Partner Center?

As funções de incentivo no Partner Center são baseadas na localização e incluem incentivos administrados e incentivos ao utilizador. Para obter mais informações sobre o que essas funções podem fazer, consulte [atribuir as funções e permissões dos utilizadores](permissions-overview.md).

### <a name="can-incentives-admins-be-assigned-at-the-global-and-location-level"></a>Os administradores de incentivos podem ser atribuídos ao nível global e localização?

Sim. Você pode atribuir um administrador de incentivos para ser o administrador de incentivos para todos os locais ou cada local pode ter os seus próprios incentivos administrados.

### <a name="can-incentives-be-paid-at-the-global-or-location-level"></a>Os incentivos podem ser pagos ao nível global ou localização?

Os incentivos são pagos apenas ao nível da localização.

### <a name="regarding-referrals-how-many-business-profiles-can-we-create"></a>No que diz respeito a referências, quantos perfis de negócio podemos criar?

A sua empresa pode criar tantos perfis de negócio que precisar para representar plenamente os interesses da sua empresa. Em cada perfil de negócio, pode listar até cinco locais, um local por país. Cada um dos perfis de negócio pode receber referências para cada uma das suas localizações.

### <a name="how-will-referrals-be-assigned-what-changes-can-i-expect-for-example-if-i-have-a-global-company-in-one-market-and-locations-in-other-markets-how-will-referrals-be-assigned"></a>Como serão atribuídas referências, que alterações posso esperar? Por exemplo, se eu tiver uma empresa global num mercado e em locais noutros mercados, como serão atribuídas referências?

As referências são atribuídas com base nos parâmetros de pesquisa que o cliente define. Independentemente de ter uma localização ou muitas, se o cliente especificar uma localização desejada e tiver um negócio lá que satisfaça os outros parâmetros, então a referência iria para esse local.

### <a name="i-am-migrating-to-partner-center-from-within-russia-i-get-an-error-message-about-web-direct-how-do-i-continue-with-the-migration"></a>Estou a migrar para o Centro de Parceiros de dentro da Rússia. Recebo uma mensagem de erro sobre a Web Direct. Como continuo com a migração?

Se receber uma mensagem de erro por estar a participar no programa Web Direct, deve fazer o seguinte:

1. Inscreva-se no portal. Azure.com, e criar um novo inquilino AZure AD. Para mais informações leia [Criar um novo inquilino AZure AD.](/azure/active-directory/fundamentals/active-directory-access-create-new-tenant)

2. Uma vez criado o novo inquilino AZure AD, use-o para migrar do Centro de Membros de Parceiros para o Partner Center ou para se inscrever como um novo net no Partner Center.