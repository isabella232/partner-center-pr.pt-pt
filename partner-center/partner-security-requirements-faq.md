---
title: Requisitos de segurança do parceiro FAQ
ms.topic: article
ms.date: 05/26/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Muitas vezes, perguntas sobre os requisitos de segurança dos parceiros - o que são, como os parceiros devem implementá-los, e como você sabe se os conheceu.
author: isaiahwilliams
ms.author: iswillia
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 9f60b6e2624bd4f9020181a936842bdb46db8aa9
ms.sourcegitcommit: 98f5eebe7d08ba214ed5a078f1ac770439e41eb7
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/31/2020
ms.locfileid: "93133053"
---
# <a name="common-questions-about-partner-security-requirements"></a>Questões comuns sobre requisitos de segurança dos parceiros

**Aplica-se a**

- Partner Center

**Utilizadores apropriados**

- Todos os utilizadores habilitados, incluindo utilizadores convidados


Este artigo responde a algumas perguntas comuns sobre os requisitos de segurança dos [parceiros.](partner-security-requirements.md)

### <a name="what-are-the-partner-security-requirements-and-why-should-partners-implement-them"></a>Quais são os requisitos de segurança dos parceiros e por que razão os parceiros devem implementá-los?

Maiores e contínuas salvaguardas de segurança e privacidade estão entre as nossas principais prioridades e continuamos a ajudar os parceiros a proteger os seus clientes e inquilinos. Continuamos a assistir a um número cada vez maior de ataques de segurança, principalmente relacionados com incidentes de compromisso de identidade. Como os controlos preventivos desempenham um papel fundamental numa estratégia global de defesa para impedir os ataques de segurança, introduzimos [requisitos obrigatórios de segurança](partner-security-requirements.md) em 2019. Todos os parceiros que participam no programa Cloud Solution Provider (CSP), Fornecedores de Painéis de Controlo e Assessores devem implementar os requisitos para se manterem em conformidade.

### <a name="what-are-the-key-timelines-and-milestones"></a>Quais são os principais prazos e marcos?

Os termos associados a estes requisitos de segurança, incluindo os prazos e os marcos, estão incluídos no [Acordo de Parceiros](microsoft-partner-agreement.md)da Microsoft. Terá de implementar estes requisitos de segurança o mais rapidamente possível para se manter em conformidade com a sua participação no programa CSP.

### <a name="what-will-happen-if-i-dont-implement-these-partner-security-requirements"></a>O que acontecerá se eu não implementar estes requisitos de segurança dos parceiros?

O Microsoft Partner Agreement exige que imponha a autenticação de vários fatores para as contas dos utilizadores e adote o modelo de aplicação seguro para interagir com a API do Partner Center. 

Os parceiros que não cumpram estas práticas de segurança podem perder a sua capacidade de transacionar no programa CSP ou gerir os inquilinos de clientes usando direitos de administração delegado.

### <a name="do-the-security-requirements-apply-to-all-geographies"></a>Os requisitos de segurança aplicam-se a todas as geografias?

Sim, os requisitos de segurança aplicam-se a todas as geografias. Recomendamos vivamente que todos os parceiros que transacionem através de uma nuvem soberana (Governo dos EUA e Alemanha) atuem e adotem imediatamente estes novos requisitos de segurança. No entanto, estes parceiros não são atualmente obrigados a cumprir os requisitos de segurança. A Microsoft fornecerá detalhes adicionais sobre a aplicação destes requisitos de segurança para nuvens soberanas no futuro.

### <a name="is-it-possible-to-get-an-exclusion-for-an-account"></a>É possível obter uma exclusão para uma conta?

Não, não é possível excluir qualquer conta de utilizador da exigência de ter a autenticação multi-factor (MFA) aplicada. Dada a natureza altamente privilegiada de ser um parceiro, o Microsoft Partner Agreement exige que a autenticação multi-factor seja aplicada para cada conta de utilizador no seu inquilino parceiro.

### <a name="how-do-i-know-if-i-have-met-the-partner-security-requirements"></a>Como sei se cumpri os requisitos de segurança do parceiro?

Tem de completar os seguintes passos:

- Tem de cumprir todos os requisitos descritos nos requisitos de segurança do [parceiro.](partner-security-requirements.md)
- Tem de garantir que todas as contas de utilizador do seu inquilino parceiro têm a autenticação de vários fatores aplicada.

Para ajudar a identificar as áreas-chave onde pode tomar ações, estamos fornecendo o relatório de estado dos [requisitos de segurança](https://partner.microsoft.com/commerce/security/compliance) que está disponível através do Partner Center.

Consulte [o estado dos requisitos de segurança dos parceiros](partner-security-compliance.md) para obter mais informações sobre o relatório de estado.

## <a name="required-actions"></a>Ações Necessárias

### <a name="what-are-the-key-actions-i-need-to-take-to-meet-the-requirements"></a>Quais são as acções-chave que preciso de tomar para satisfazer os requisitos?

Todos os parceiros do programa CSP (conta direta, fornecedor indireto e revendedor indireto), Assessores e Fornecedores de Painéis de Controlo devem satisfazer os requisitos.

1. **Impor MFA a todos os utilizadores**

    Todos os parceiros do programa CSP, Assessores e Fornecedores de Painéis de Controlo são obrigados a impor MFA a todos os utilizadores do seu inquilino parceiro.

    Considerações adicionais:

    - Os fornecedores indiretos precisam de trabalhar com revendedores indiretos a bordo do Partner Center se ainda não o fizerem e incentivar os seus revendedores a satisfazerem os requisitos.
    - O Azure MFA está a ser disponibilizado a todos os utilizadores do inquilino parceiro sem custos através de incumprimentos de segurança Azure AD com o único método de verificação de uma aplicação autenticadora que suporta senhas de tempo únicas (TOTP) baseadas no tempo.
    - Métodos de verificação adicionais estão disponíveis através do [Azure Ative Directory Premium](/azure/active-directory/fundamentals/active-directory-get-started-premium) SKUs, se forem necessários outros métodos, como uma chamada telefónica ou uma mensagem de texto.
    - Os parceiros também podem alavancar uma solução de MFA de terceiros para cada conta ao aceder aos serviços de cloud comercial da Microsoft.

2. **Adotar o quadro do Modelo de Aplicação Segura**

    Todos os parceiros que tenham desenvolvido a integração personalizada utilizando quaisquer APIs (como Azure Resource Manager, Microsoft Graph, Partner Center API, etc.) ou a automação personalizada implementada usando ferramentas como a PowerShell, terão de adotar o [quadro do Modelo de Aplicação Segura](/partner-center/develop/enable-secure-app-model) para se integrarem com os serviços na nuvem da Microsoft. Se não o fizer, pode resultar numa perturbação devido à implantação de MFA. Os seguintes recursos fornecem uma visão geral e orientação sobre como adotar o modelo.

    - [Visão geral do modelo de aplicação segura](/partner-center/develop/enable-secure-app-model)
    - [Centro de Parceiros: Guia de modelo de aplicação segura](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)
    - [Parceiros no programa CSP: .NET código de amostra para permitir o Modelo de Aplicação Segura](/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
    - [Parceiros no programa CSP: Código de amostra de Java para permitir o Modelo de Aplicação Segura](/samples/microsoft/partner-center-java-samples/secure-app-model/)
    - [Documento de autenticação do Centro parceiro](/partner-center/develop/partner-center-authentication)
    - [Documento de autenticação multi-factor do Centro Parceiro PowerShell (MFA)](/powershell/partnercenter/multi-factor-auth)

    Consulte o fornecedor se estiver a utilizar um painel de controlo sobre a adoção da estrutura do Modelo de Aplicação Segura.

    Os fornecedores de painéis de controlo são obrigados a [embarcar no](enroll-as-cpv.md) Partner Center como fornecedor de painéis de controlo e a começar a implementar este requisito imediatamente. Consulte o [Centro de Parceiros: Quadro de modelo de aplicação segura](https://assetsprod.microsoft.com/secure-application-model-guide.pdf). Os fornecedores de painéis de controlo devem aceitar e gerir o consentimento dos parceiros da CSP em vez de credenciais e expurgar todas as credenciais dos parceiros CSP existentes.

## <a name="multi-factor-authentication"></a>Autenticação multifator

### <a name="what-is-multi-factor-authentication-mfa"></a>O que é a autenticação multi-factor (MFA)?

O MFA é um mecanismo de segurança que os indivíduos são autenticados através de mais do que um procedimento de segurança e validação necessário. Funciona requerendo dois ou mais dos seguintes métodos de autenticação:

- Algo que você sabe (tipicamente uma palavra-passe)
- Algo que você tem (um dispositivo de confiança que não é facilmente duplicado, como um telefone)
- Algo que és (biometria)

### <a name="what-is-the-cost-of-enabling-mfa"></a>Qual é o custo de permitir o MFA?

A Microsoft fornece MFA sem custos através da implementação de padrão de segurança Azure AD. A única opção de verificação disponível através desta versão de MFA é uma aplicação autenticadora. Se for necessária uma chamada telefónica ou uma mensagem SMS, terá de ser adquirida uma licença [Azure Ative Directory Premium.](/azure/active-directory/fundamentals/active-directory-get-started-premium) Em alternativa, pode utilizar uma solução de terceiros para fornecer MFA para cada utilizador no seu inquilino parceiro - neste caso, é da sua responsabilidade garantir que a sua solução de MFA está a ser aplicada e que está em conformidade.

### <a name="what-actions-do-i-need-to-take-if-i-already-have-an-mfa-solution"></a>Que ações tenho de tomar se já tenho uma solução de MFA?

Através destes requisitos de segurança, os utilizadores de um inquilino parceiro serão obrigados a autenticar usando MFA ao aceder aos serviços de cloud comercial da Microsoft. Soluções de terceiros podem ser utilizadas para satisfazer estes requisitos. A Microsoft já não fornece testes de validação a fornecedores independentes de identidade para compatibilidade com o Azure Ative Directory. Para testar o seu produto para interoperabilidade, consulte estas [diretrizes](https://www.microsoft.com/download/details.aspx?id=56843).

> [!IMPORTANT]
> Quando se utiliza uma solução de terceiros, é importante verificar se a solução está a emitir a alegação do método de autenticação (AMR) que inclui o valor MFA. Consulte [os Requisitos de Segurança do Parceiro](/powershell/partnercenter/test-partner-security-requirements) para obter detalhes sobre como validar a sua solução de terceiros está a emitir a reclamação esperada.

### <a name="i-use-multiple-partner-tenants-to-transact-do-i-need-to-implement-mfa-on-them-all"></a>Uso vários inquilinos parceiros para negociar. Preciso de implementar a MFA em todos eles?

Sim, você precisará impor MFA para cada inquilino do Azure Ative Directory associado ao programa CSP ou ao programa Advisor. Para adquirir uma licença Azure Ative Directory Premium, tem de adquirir uma licença Azure Ative Directory para os utilizadores de cada inquilino do Azure Ative Directory. 

### <a name="does-each-user-account-in-my-partner-tenant-need-to-have-mfa-enforced"></a>Cada conta de utilizador no meu inquilino parceiro precisa de ter MFA aplicada?

Sim, cada utilizador terá de ser aplicado pela MFA. No entanto, se estiver a utilizar os incumprimentos de segurança Azure AD, então não é necessária nenhuma ação adicional porque essa funcionalidade aplica MFA para todas as contas de utilizador. Permitir incumprimentos de segurança é uma forma livre e fácil de garantir que as suas contas de utilizador são compatíveis com MFA e não são impactadas quando o MFA é aplicado.

### <a name="i-am-a-direct-bill-partner-with-microsoft-what-do-i-need-to-do"></a>Sou sócio de contas diretas com a Microsoft. O que preciso fazer?

Os parceiros do Cloud Solution Provider devem impor MFA a cada utilizador no seu inquilino parceiro.

### <a name="i-am-an-indirect-reseller-and-only-transact-though-a-distributor-do-i-still-have-to-do-enable-mfa"></a>Sou um revendedor indireto e só transacionei um distribuidor. Ainda tenho de fazer o que permitir o MFA?

Todos os revendedores indiretos são obrigados a impor MFA a cada utilizador no seu inquilino parceiro. O revendedor indireto deve ativar o MFA.

### <a name="i-dont-use-the-partner-center-api-do-i-still-need-to-implement-mfa"></a>Não uso a API do Centro De Parceiros. Ainda preciso implementar o MFA?

Sim, este requisito de segurança é para todos os utilizadores, incluindo utilizadores administrativos parceiros e utilizadores finais num inquilino parceiro.

### <a name="which-third-party-vendors-provide-mfa-solutions-compatible-with-azure-active-directory"></a>Que fornecedores de terceiros fornecem soluções MFA compatíveis com o Azure Ative Directory?

Ao rever os fornecedores e soluções MFA, os parceiros devem garantir que a solução que escolherem é compatível com o Azure Ative Directory.

A Microsoft já não fornece testes de validação a fornecedores independentes de identidade para compatibilidade com o Azure Ative Directory. Se pretender testar o seu produto para interoperabilidade, consulte estas [diretrizes](https://www.microsoft.com/download/details.aspx?id=56843).

Para mais informações, consulte a lista de [compatibilidade da federação AZure AD.](/azure/active-directory/hybrid/how-to-connect-fed-compatibility)

### <a name="how-can-i-test-mfa-in-our-integration-sandbox"></a>Como posso testar mFA na nossa caixa de areia de integração?

A funcionalidade de padrão de segurança Azure AD deve ser ativada ou, em alternativa, pode alavancar a solução de terceiros que utiliza a federação.

### <a name="will-enabling-mfa-affect-how-i-interact-with-my-customers-tenant"></a>Permitir que o MFA afete a forma como interajo com o inquilino do meu cliente?

N.º O cumprimento destes requisitos de segurança não terá impacto na forma como gere os seus clientes. A sua capacidade para realizar operações administrativas delegadas não será interrompida.

### <a name="are-my-customers-subject-to-the-partner-security-requirements"></a>Os meus clientes estão sujeitos aos requisitos de segurança do parceiro?

Não, não é obrigatório que imponha MFA para cada utilizador nos inquilinos AD Azure do seu cliente. No entanto, recomenda-se que trabalhe com cada cliente para determinar a melhor forma de proteger os seus utilizadores.

### <a name="can-any-user-be-excluded-from-the-mfa-requirement"></a>Qualquer utilizador pode ser excluído do requisito de MFA?

Não, cada utilizador, incluindo contas de serviço, no seu inquilino parceiro será obrigado a autenticar usando MFA.

### <a name="do-the-partner-security-requirements-apply-to-the-integration-sandbox"></a>Os requisitos de segurança do parceiro aplicam-se à caixa de areia de integração?

Sim, os requisitos de segurança do parceiro aplicam-se à caixa de areia de integração. Isto significa que você precisará implementar a solução MFA apropriada para os utilizadores no inquilino de caixa de areia integração. Recomenda-se que implemente os incumprimentos de segurança Azure AD para fornecer MFA.

### <a name="how-do-i-configure-an-emergency-access-break-glass-account"></a>Como posso configurar uma conta de acesso de emergência (break glass) ?

É considerada uma das melhores práticas criar uma ou duas contas de acesso de emergência para evitar que seja inadvertidamente trancada fora do seu inquilino Azure AD. No que diz respeito aos requisitos de segurança do parceiro, é necessário que cada utilizador autentica usando MFA. Este requisito significa que terá de modificar a definição de uma conta de acesso de emergência. Pode ser uma conta que está a alavancar uma solução de terceiros para a MFA.

### <a name="is-active-directory-federation-service-adfs-required-if-i-am-using-a-third-party-solution"></a>O Serviço de Federação de Diretório Ativo (ADFS) é necessário se eu estiver a utilizar uma solução de terceiros?

Não, não é necessário ter o Serviço de Federação de Diretório Ativo (ADFS) se estiver a utilizar uma solução de terceiros. Recomenda-se que trabalhe com o fornecedor da solução para determinar quais são os requisitos para a sua solução.

### <a name="is-it-a-requirement-to-enable-azure-ad-security-defaults"></a>É um requisito para permitir incumprimentos de segurança Azure AD?

Não, não é necessário que ative os incumprimentos de segurança Azure AD.

### <a name="can-conditional-access-be-used-to-meet-the-mfa-requirement"></a>O acesso condicional pode ser utilizado para satisfazer os requisitos do MFA?

Sim, você pode usar acesso condicional para impor MFA para cada utilizador, incluindo contas de serviço, no seu inquilino parceiro. No entanto, dada a natureza altamente privilegiada de ser um parceiro, precisamos de garantir que cada utilizador tem um desafio MFA para cada autenticação. Isto significa que não poderá aproveitar a característica de acesso condicional que contorna o requisito de MFA.

### <a name="will-the-service-account-used-by-azure-ad-connect-be-impacted-by-the-partner-security-requirements"></a>A conta de serviço utilizada pelo Azure AD Connect será impactada pelos requisitos de segurança do parceiro?

Não, a conta de serviço utilizada pelo Azure AD Connect não será afetada pelos requisitos de segurança do parceiro. Se tiver um problema com o Azure AD Connect como resultado da aplicação do MFA, então abra um pedido de suporte técnico com o suporte da Microsoft.

## <a name="secure-application-model"></a>Modelo de aplicação segura

### <a name="who-should-adopt-the-secure-application-model-to-meet-the-requirements"></a>Quem deve adotar o modelo de aplicação seguro para satisfazer os requisitos?

A Microsoft está a introduzir um quadro seguro e escalável para autenticar parceiros do Cloud Solution Provider (CSP) e fornecedores de painéis de controlo (CPV) que alavanca a autenticação multi-factor. Consulte o [guia do Modelo de Aplicação Segura](https://assetsprod.microsoft.com/secure-application-model-guide.pdf) para obter mais informações. Todos os parceiros que tenham desenvolvido a integração personalizada utilizando quaisquer APIs (como Azure Resource Manager, Microsoft Graph, Partner Center API, etc.) ou a automação personalizada implementada usando ferramentas como a PowerShell, terão de adotar o [quadro do Modelo de Aplicação Segura](/partner-center/develop/enable-secure-app-model) para se integrarem com os serviços na nuvem da Microsoft.

### <a name="what-is-the-secure-application-model"></a>O que é o Modelo de Aplicação Segura?

A Microsoft está a introduzir um quadro seguro e escalável para autenticar parceiros do Cloud Solution Provider (CSP) e fornecedores de painéis de controlo (CPV) que alavanca a autenticação multi-factor. Consulte o [guia do Modelo de Aplicação Segura](https://assetsprod.microsoft.com/secure-application-model-guide.pdf) para obter mais informações.  

### <a name="how-do-i-implement-the-secure-application-model"></a>Como implemento o Modelo de Aplicação Segura?

Todos os parceiros que tenham desenvolvido a integração personalizada utilizando quaisquer APIs (como Azure Resource Manager, Microsoft Graph, Partner Center API, etc.) ou a automação personalizada implementada usando ferramentas como a PowerShell, terão de adotar o [quadro do Modelo de Aplicação Segura](/partner-center/develop/enable-secure-app-model) para se integrarem com os serviços na nuvem da Microsoft. Se não o fizer, pode resultar numa perturbação devido à implantação de MFA. Os seguintes recursos fornecem uma visão geral e orientação sobre como adotar o modelo.

- [Visão geral do modelo de aplicação segura](/partner-center/develop/enable-secure-app-model)
- [Centro de Parceiros: Guia de modelo de aplicação segura](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [Parceiros no programa CSP: .NET código de amostra para permitir o Modelo de Aplicação Segura](/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
- [Parceiros no programa CSP: Código de amostra de Java para permitir o Modelo de Aplicação Segura](/samples/microsoft/partner-center-java-samples/secure-app-model/)
- [Documento de autenticação do Centro parceiro](/partner-center/develop/partner-center-authentication)
- [Documento de autenticação multi-factor do Centro Parceiro PowerShell (MFA)](/powershell/partnercenter/multi-factor-auth)

Se estiver a utilizar um painel de controlo, terá de consultar o fornecedor sobre a adoção da estrutura do Modelo de Aplicação Segura.

Os fornecedores de painéis de controlo são obrigados a [embarcar no](enroll-as-cpv.md) Partner Center como fornecedor de painéis de controlo e a começar a implementar este requisito imediatamente. Consulte o [Centro de Parceiros: Quadro de modelo de aplicação segura](https://assetsprod.microsoft.com/secure-application-model-guide.pdf). Os fornecedores de painéis de controlo devem aceitar e gerir o consentimento dos parceiros da CSP em vez de credenciais e expurgar todas as credenciais dos parceiros CSP existentes.

### <a name="does-the-secure-application-model-need-to-be-implemented-for-the-partner-center-apisdk-only"></a>O Modelo de Aplicação Segura precisa de ser implementado apenas para o Centro Parceiro API/SDK?

Ao impor a autenticação de vários fatores para todas as contas do utilizador, qualquer automatização ou integração que se destine a funcionar de forma não interativa será impactada. Embora os requisitos de segurança do parceiro exijam que você permita o modelo de aplicação segura para a API do Centro Parceiro, ele pode ser alavancado para responder à necessidade de um segundo fator de autenticação com automatização e integração.

>[!Note] 
>Os recursos que estão a ser acedidos terão de suportar o acesso à autenticação baseada em símbolos.

### <a name="i-am-using-automation-tools-such-as-powershell-how-do-i-implement-the-secure-application-model"></a>Estou a usar ferramentas de automação como a PowerShell. Como implemento o Modelo de Aplicação Segura?

Terá de implementar o Modelo de Aplicação Segura se a sua automatização se destinar a ser executada de forma não interativa e se basear em credenciais de utilizador para autenticação. Ver [Modelo de Aplicação Segura / Partner Center PowerShell](/powershell/partnercenter/multi-factor-auth) para orientação sobre como implementar este quadro.  

>[!Note] 
>Nem todas as ferramentas de automatização fornecem a capacidade de autenticar usando fichas de acesso. Publique uma mensagem no grupo de [Orientação de Segurança do Centro de Parceiros](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) se precisar de ajuda para entender que alterações devem ser feitas. 

### <a name="what-user-credentials-should-the-application-administrator-provide-when-performing-the-consent-process"></a>Que credenciais de utilizador deve o administrador de aplicação fornecer ao realizar o processo de consentimento?

Recomenda-se que utilize uma conta de serviço que tenha sido atribuída às permissões menos privilegiadas. No que diz respeito à API do Centro De Parceiros, deverá utilizar uma conta que tenha sido atribuída ao papel de Agente Comercial ou Dedmin.

### <a name="why-should-the-application-administrator-not-provide-global-admin-user-credentials-when-performing-the-consent-process"></a>Por que razão o administrador de aplicação não deve fornecer credenciais globais de utilizador de administração ao realizar o processo de consentimento?

É uma boa prática usar a identidade menos privilegiada.  Isto reduzirá o risco. Não é recomendado usar uma conta que tenha privilégios de administração global porque isso seria fornecer mais permissões do que o necessário.

### <a name="i-am-a-csp-partner-how-do-i-know-if-my-control-panel-vendor-cpv-is-working-on-implementing-the-solution-or-not"></a>Sou sócio da CSP. Como é que eu sei se o meu Fornecedor de Painéis de Controlo (CPV) está a trabalhar na implementação da solução ou não?

Para os parceiros que utilizam uma solução de Fornecedor de Painéis de Controlo (CPV) para transacionar no programa Cloud Solution Provider (CSP), é da sua responsabilidade consultar o seu CPV.

### <a name="who-is-a-control-panel-vendor-cpv"></a>Quem é um Fornecedor de Painéis de Controlo (CPV)?

Um fornecedor de Painéis de Controlo é um fornecedor de software independente que desenvolve aplicações para uso pela CSP Partners para integrar com APIs do Partner Center. Um fornecedor de Painel de Controlo não é um Parceiro CSP com acesso direto ao painel de instrumentos do Centro de Parceiros ou APIs. Uma descrição detalhada está disponível dentro do [Centro de Parceiros: Guia modelo de aplicações seguras](https://assetsprod.microsoft.com/secure-application-model-guide.pdf).

### <a name="i-am-a-cpv-how-do-i-enroll"></a>Sou um cpV. Como me matriculo?

Para se inscrever como vendedor de painéis de controlo (CPV), siga as orientações [aqui fornecidas.](enroll-as-cpv.md)

Os CPVs devem contactar [CPVHelp@microsoft.com](mailto:CPVHelp@microsoft.com) para receber o link de inscrição e fornecer um patrocinador de funcionários da Microsoft que tenha uma relação comercial com o CPV ou conheça o seu negócio. Por exemplo, um Gestor de Desenvolvimento de Parceiros (PDM).

Assim que se inscrever no Partner Center e registar as suas candidaturas, terá acesso às APIs do Partner Center. Receberá a sua informação de sandbox através de uma notificação do Partner Center se for um novo CPV. Uma vez concluída a inscrição como CPV da Microsoft e aceitando o acordo CPV, pode:

1. Gerir a aplicação multi-inquilino (adicionar aplicações ao portal Azure, registar e não registar aplicações no Partner Center).

   >[!Note]
   >Os CPVs devem registar as suas candidaturas no Partner Center para ser autorizados para APIs do Partner Center. A adição de aplicações ao portal Azure por si só não autoriza aplicações de CPV para APIs do Partner Center.

1. Veja e gere o seu perfil de CPV.

1. Ver e gerir os seus utilizadores que precisam de acesso às capacidades de CPV. Um CPV só pode ter o papel global administrador.

### <a name="i-am-using-the-partner-center-sdk-will-sdk-automatically-adopt-the-secure-application-model"></a>Estou a usar o Centro De Parceiros SDK. A SDK adotará automaticamente o Modelo de Aplicação Segura?

Não, terá de seguir as diretrizes fornecidas no [guia do Modelo de Aplicação Segura.](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)

### <a name="can-i-generate-a-refresh-token-for-the-secure-application-model-with-accounts-that-dont-have-mfa-enabled"></a>Posso gerar um token de atualização para o modelo de aplicação seguro com contas que não têm MFA ativado?

Sim, um token de atualização pode ser gerado usando uma conta que não tem MFA aplicada. No entanto, isto deve ser evitado. Qualquer ficha gerada através de uma conta que não tenha MFA ativada não será capaz de aceder aos recursos devido à exigência de MFA.

### <a name="how-should-my-application-obtain-an-access-token-if-we-enable-mfa"></a>Como deve a minha aplicação obter um token de acesso se ativarmos o MFA?

Terá de seguir o [guia do Modelo de Aplicação Segura](https://assetsprod.microsoft.com/secure-application-model-guide.pdf) que fornece detalhes sobre como fazê-lo, cumprindo os novos requisitos de segurança. Pode encontrar [aqui](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model) o código de amostra .NET e o [código](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model)de amostra de Java.

### <a name="as-a-cpv-do-i-create-an-azure-ad-application-in-our-cpv-tenant-or-the-tenant-of-the-csp-partner"></a>Como CPV, crio um pedido de AD Azure no nosso inquilino CPV ou inquilino do sócio da CSP?

O CPV terá de criar o pedido de Diretório Ativo Azure no arrendatário associado à sua inscrição como CPV.

### <a name="i-am-a-csp-that-is-using-app-only-authentication-do-i-need-to-make-any-changes"></a>Sou um CSP que está a usar apenas a autenticação de aplicações. Preciso de fazer alguma alteração?

A autenticação apenas da app não é impactada, uma vez que as credenciais dos utilizadores não estão a ser usadas para solicitar um token de acesso. Se as credenciais do utilizador estiverem a ser partilhadas, os fornecedores de painéis de controlo (CPVs) devem adotar a [estrutura do Modelo de Aplicação Segura](https://assetsprod.microsoft.com/secure-application-model-guide.pdf) e expurgar quaisquer credenciais de parceiro existentes que tenham.

### <a name="as-a-cpv-can-i-leverage-the-app-only-authentication-style-to-get-access-tokens"></a>Como CPV posso aproveitar o estilo de autenticação apenas da app para ter acesso a fichas?

Não, os parceiros do Control Panel Vendor não podem utilizar o estilo de autenticação apenas para solicitar o acesso a fichas em nome do parceiro. Devem implementar o modelo de aplicação seguro, que utiliza o estilo de autenticação app + utilizador.

## <a name="technical-enforcement"></a>Execução Técnica

### <a name="what-is-the-activation-of-security-safeguards"></a>Qual é a ativação das salvaguardas de segurança?

Todos os parceiros que participam no programa Cloud Solution Provider (CSP), Fornecedores de Painéis de Controlo (CPVs) e Conselheiros devem implementar os requisitos de segurança obrigatórios para se manterem em conformidade.

Para fornecer proteção adicional, a Microsoft iniciou a ativação de salvaguardas de segurança que ajudam os parceiros a proteger os seus inquilinos e seus clientes, obrigando à verificação de autenticação multi-factor (MFA) para impedir o acesso não autorizado.  

Completamos com sucesso a ativação para capacidades de administração em nome de (AOBO) para todos os inquilinos parceiros. Para ajudar ainda mais a proteger parceiros e clientes, direcionados para o Q2 CY2020, iniciaremos a ativação para transações do Partner Center na CSP, ajudando os parceiros a proteger os seus negócios e clientes de incidentes relacionados com roubo de identidade.

Para mais informações, visite [a Autenticação De Vários Fatores (MFA) para a](partner-security-requirements-mandating-mfa.md) página do seu parceiro de inquilino.

### <a name="i-am-using-a-third-party-mfa-solution-and-i-am-being-blocked-what-should-i-do"></a>Estou a usar uma solução de MFA de terceiros e estou a ser bloqueado, o que devo fazer?

Para validar que os recursos de acesso à conta foram contestados para a autenticação de vários fatores, vamos verificar o pedido de referência do [método de autenticação](https://tools.ietf.org/html/rfc8176) para ver se o MFA está listado. Algumas soluções de terceiros não emitem esta alegação ou não incluem o valor MFA. Se a reclamação faltar ou o valor MFA não estiver listado, então não há forma de determinar se a conta autenticada foi contestada para a autenticação de vários fatores. Terá de trabalhar com o fornecedor para obter a sua solução de terceiros para determinar que ações devem ser tomadas para que a solução emita a reclamação de referência do método de autenticação.

Consulte [os Requisitos de Segurança do Parceiro](/powershell/partnercenter/test-partner-security-requirements) se não tiver a certeza se a sua solução de terceiros está a emitir ou não a reclamação esperada.

### <a name="mfa-is-blocking-me-from-supporting-my-customer-using-aobo-what-should-i-do"></a>A MFA está a impedir-me de apoiar o meu cliente usando o AOBO, o que devo fazer?

A aplicação técnica dos requisitos de segurança do parceiro será verificada se a conta autenticada foi contestada para a autenticação de vários fatores. Se a conta não tiver sido, então será redirecionado para o sinal na página e solicitado a autenticar novamente. Leia experiência e orientação adicionais nesta [Obrigação de Autenticação Multi-factor (MFA) para a](partner-security-requirements-mandating-mfa.md#partner-delegated-administration) documentação do seu inquilino parceiro. No cenário em que o seu domínio não é federado, depois de autenticar com sucesso, será solicitado que se ingiu para configurar a autenticação multi-factor. Uma vez concluído, poderá gerir os seus clientes usando o AOBO. No cenário em que o seu domínio é federado, então terá de garantir que a conta está a ser desafiada para a autenticação de vários fatores.

## <a name="security-defaults-transition"></a>Transição de incumprimentos de segurança

### <a name="how-can-i-transition-from-baseline-policies-to-security-defaults-or-other-mfa-solutions"></a>Como posso transitar das políticas de base para incumprimentos de segurança ou outras soluções MFA?

As políticas de "linha de base" do Azure Ative Directory (Azure AD) [estão a ser removidas e substituídas por](/azure/active-directory/fundamentals/whats-new#replacement-of-baseline-policies-with-security-defaults) "incumprimentos de segurança", um conjunto mais abrangente de políticas de proteção para si e para os seus clientes. [Os incumprimentos de segurança](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) podem ajudar a proteger a sua organização de ataques de segurança relacionados com roubo de identidade.

A sua implementação de autenticação multi-factor (MFA) será removida devido à reforma das políticas de base se não tiver transitado das políticas de base para a política de incumprimentos de segurança ou [outras opções de implementação do MFA.](partner-security-requirements.md#implementing-multi-factor-authentication) Qualquer utilizadores no seu parceiro inquilinos que realizem operações protegidas de MFA serão solicitados para completar a verificação de MFA. Reveja aqui orientações mais [detalhadas.](partner-security-requirements-mandating-mfa.md)
Para se manter em conformidade e minimizar as perturbações, tome uma das seguintes ações:

- Transição para incumprimentos de segurança
    - A política de incumprimentos de segurança é uma das opções que os parceiros podem escolher para implementar MFA. Oferece um nível básico de segurança, sem custos adicionais.
    - Saiba como ativar o MFA para a sua organização com a Azure AD e reveja as [considerações fundamentais de segurança.](partner-security-requirements.md#security-defaults)
    - Ativar a política de incumprimentos de segurança se satisfaça as necessidades do seu negócio.
- Transição para Acesso Condicional
    - Se a política de incumprimentos de segurança não servir as suas necessidades, ative o Acesso Condicional. Para mais informações, reveja a documentação de Acesso Condicionado Azure AD.

## <a name="key-resources"></a>Recursos-chave

### <a name="how-to-get-started"></a>Como começar

- [Requisitos de segurança do parceiro: guia passo a passo](partner-security-requirements.md).
- Direcione as suas perguntas e feedback para este [Grupo de Orientação de Segurança do Centro de Parceiros.](https://aka.ms/MPCSecurityGuidance)
- Assista ao próximo horário de escritório dos parceiros e webinars. Consulte aqui o [horário e os recursos detalhados.](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)

### <a name="resources-for-adopting-secure-application-model"></a>Recursos para a adoção de modelo de aplicação segura

- [Visão geral do modelo de aplicação segura](/partner-center/develop/enable-secure-app-model)
- [Centro de Parceiros: Guia de modelo de aplicação segura](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [Parceiros no programa CSP: .NET código de amostra para permitir o Modelo de Aplicação Segura](/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
- [Parceiros no programa CSP: Código de amostra de Java para permitir o Modelo de Aplicação Segura](/samples/microsoft/partner-center-java-samples/secure-app-model/)
- [Documento de autenticação do Centro parceiro](/partner-center/develop/partner-center-authentication)
- [Documento de autenticação multi-factor do Centro Parceiro PowerShell (MFA)](/powershell/partnercenter/multi-factor-auth)

## <a name="support"></a>Suporte

### <a name="where-can-i-get-support"></a>Onde posso conseguir apoio?

Para que os recursos de apoio satisfaçam os requisitos de segurança, se tiver Apoio Avançado para Parceiros (ASfP) contacte o seu Gestor de Conta de Serviço; para o acordo premier Support for Partners (PSfP), contacte o seu Gestor de Conta de Serviço e Gestor de Conta Técnica.

### <a name="how-do-i-get-technical-information-and-support-to-help-me-adopt-secure-application-model-framework"></a>Como obter informações técnicas e apoio para me ajudar a adotar um quadro de modelo de aplicação segura?

As opções técnicas de suporte ao produto para o Azure Ative Directory estão disponíveis através dos seus benefícios MPN. Os parceiros com acesso a uma subscrição ativa de ASfP ou PSfP podem trabalhar com o seu gestor de conta associado (SAM/TAM) para melhor entender as opções de que dispõem.

### <a name="how-do-i-contact-support-if-ive-lost-access-to-partner-center"></a>Como posso contactar o suporte se perdi acesso ao Partner Center?

Se perder o acesso devido a um problema de MFA, contacte o administrador global para o seu inquilino. O seu departamento de TI interno poderá dizer-lhe quem é o seu administrador global. 

Se esqueceu a sua palavra-passe, leia [Não pode entrar para](unable-to-sign-in.md) pedir ajuda.

### <a name="where-can-i-find-more-information-about-common-technical-issues"></a>Onde posso encontrar mais informações sobre questões técnicas comuns?

As informações relativas às questões técnicas comuns podem ser encontradas nos [requisitos de segurança dos parceiros que utilizam o Partner Center ou as APIs do Partner Center](partner-security-requirements.md)