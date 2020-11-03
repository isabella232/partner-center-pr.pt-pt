---
title: Estado dos requisitos de segurança dos parceiros
ms.date: 05/26/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Conheça os novos requisitos obrigatórios aumentando a segurança para assessores, fornecedores de painéis de controlo e parceiros no programa Cloud Solution Provider.
author: isaiahwilliams
ms.author: iswillia
ms.localizationpriority: high
ms.topic: conceptual
ms.custom: SEOMAY.20
ms.openlocfilehash: 1b6c2d56a0747ddf2bd1a821886e371ed698a4a1
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/22/2020
ms.locfileid: "92529864"
---
# <a name="partner-security-requirements-status---get-answers-and-check-reports-about-current-status"></a>Estatuto dos requisitos de segurança do parceiro - obtenha respostas e verifique relatórios sobre o estado atual

**Aplica-se a**

- Todos os parceiros no programa Cloud Solution Provider
  - Conta direta
  - Fornecedor indireto
  - Revendedor indireto
- Todos os fornecedores de painéis de controlo
- Todos os Conselheiros

**Utilizadores apropriados**
- Todos os utilizadores habilitados, incluindo utilizadores convidados

Uma maior salvaguarda de privacidade e segurança estão entre as nossas principais prioridades. Sabemos que a melhor defesa é a prevenção e que somos tão fortes quanto o nosso elo mais fraco. É por isso que precisamos que todos os nossos ecossistemas atuem e garantam que dispõem de proteções de segurança adequadas. Para ajudar a salvaguardar parceiros e clientes, estamos a introduzir um conjunto de requisitos de segurança obrigatórios para assessores, fornecedores de painéis de controlo e parceiros que participam no programa Cloud Solution Provider.

A partir de 1 de agosto de 2019, todos os parceiros são obrigados a impor a autenticação de vários fatores para todos os utilizadores, incluindo contas de serviço, no seu inquilino parceiro. Para obter informações mais detalhadas sobre as novas políticas de segurança, leia [os Requisitos de Segurança dos Parceiros.](partner-security-requirements.md)

Queremos garantir que cada utilizador tem um desafio MFA para cada autenticação. Esta experiência pode ser realizada através de uma das seguintes formas:

- Implementação do Azure AD Premium para garantir que o MFA é aplicado a cada utilizador
- Implementação dos [incumprimentos de segurança Azure AD](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)
- Implementação de uma solução de terceiros para garantir que o MFA é aplicado a cada utilizador

## <a name="partner-security-requirements-status"></a>Estado dos requisitos de segurança dos parceiros

Este relatório pode ajudá-lo a verificar o estado dos requisitos de segurança, fornecendo uma forma de ver onde pode estar a ficar aquém. O rastreio é regularmente atualizado.

>[!NOTE]
>O relatório de estado dos requisitos de segurança do Parceiro é suportado apenas no Partner Center. Não está disponível na Microsoft Cloud para o Governo dos EUA ou microsoft Cloud Germany. Recomendamos vivamente que todos os parceiros que transacionem através de uma nuvem soberana (21Vianet, Governo dos EUA e Alemanha) adotem imediatamente estes novos requisitos de segurança. No entanto, estes parceiros não são obrigados a cumprir os novos requisitos de segurança a partir de 1 de agosto de 2019. A Microsoft fornecerá detalhes adicionais sobre a aplicação destes requisitos de segurança para nuvens soberanas no futuro.

## <a name="multi-factor-authentication-mfa-report"></a>Relatório de autenticação de vários fatores ("MFA")

O relatório do MFA do Partner Center oferece insights sobre a implementação do MFA parceiro, fornecendo dois tipos de métricas com base na configuração de MFA e atividades do Centro de Parceiros do inquilino CSP: 

### <a name="mfa-configuration-on-a-csp-tenant"></a>Configuração de MFA em um inquilino CSP

Esta métrica está relacionada com a configuração do MFA num inquilino da CSP que capturou e reportou diariamente. Mede a percentagem de contas de utilizador ativadas com MFA aplicadas utilizando qualquer uma dessas [opções de MFA](/azure/active-directory/fundamentals/concept-fundamentals-mfa-get-started). Por exemplo:

- A Contoso é parceira da CSP com 110 contas de utilizador no arrendatário, 10 dessas contas de utilizador estão desativadas. 
- Das restantes 100 contas de utilizador, 90 são aplicadas com recurso às [opções de MFA fornecidas.](/azure/active-directory/fundamentals/concept-fundamentals-mfa-get-started) Assim, a métrica mostra 90%. 

### <a name="partner-center-activities-with-mfa"></a>Atividades do Centro de Parceiros com MFA

Sempre que os seus colaboradores se inscrevem no Partner Center para trabalhar ou, através de APIs, obter ou enviar dados através do Partner Center, o seu estado de segurança é contestado e rastreado. Também estão incluídas no rastreio do estado de segurança, estão as suas aplicações e quaisquer aplicações de fornecedor de painéis de controlo. O estado apresentado é para os sete dias anteriores.

#### <a name="mfa-verification-completed-by-users"></a>Verificação do MFA concluída pelos utilizadores

Esta métrica está relacionada com atividades dentro do painel do Centro de Parceiros. Mede a percentagem de operações efetuadas por utilizadores que tenham concluído a verificação do MFA. Por exemplo:

- Contoso é sócio da CSP com dois agentes administrativos, Jane e John.
- No primeiro dia, a Jane entrou no painel do Partner Center sem verificação de MFA e fez três operações.
- No segundo dia, John entrou no dashboard do Partner Center sem verificação de MFA e fez cinco operações.
- No terceiro dia, a Jane entrou no painel do Partner Center com verificação de MFA e fez duas operações.
- Não houve operações feitas por nenhum dos agentes nos restantes quatro dias.
- Das 10 operações e realizadas na janela de 7 dias, duas foram feitas pelo utilizador com verificação de MFA. Assim, a métrica mostra 20%.

Utilize os pedidos do Portal do Ficheiro **sem MFA** para perceber qual o utilizador que iniciou sessão no painel de instrumentos do Partner Center sem ter verificação de MFA e hora da última visita durante a janela de reporte.

#### <a name="appuser-authentication"></a>App+Autenticação do utilizador

Esta métrica está relacionada com a utilização de pedidos de API do Partner Center espetam-se através da autenticação app+User. Mede a percentagem de pedidos de API feitos com recurso a um token de acesso com pedido de MFA. Por exemplo:

- A Fabrikam é parceira da CSP e tem uma aplicação CSP que utiliza uma mistura de métodos de autenticação app+user e apenas para aplicações.
- No primeiro dia, a aplicação equindo três pedidos de API, que foram apoiados por um token de acesso obtido através do método de autenticação App+User sem verificação de MFA.
- No segundo dia, a aplicação e fez cinco pedidos de API, que foram apoiados por um token de acesso obtido com a autenticação apenas da App.
- No terceiro dia, a aplicação e fez dois pedidos de API, que foram apoiados por um token de acesso obtido utilizando o método de autenticação App+User com verificação de MFA.
- Não houve operações feitas por nenhum dos agentes nos restantes quatro dias.
- Os cinco pedidos da API no segundo dia, que foram apoiados por um token de acesso obtido através da autenticação apenas da App, são omitidos da métrica, uma vez que não recorre às credenciais dos utilizadores. Das restantes cinco operações, duas foram apoiadas por um sinal de acesso obtido com verificação de MFA. Assim, a métrica mostra 40%.

Se quiser entender quais as atividades app+utilizador que resultam na não 100% nesta métrica, utilize ficheiros:

- **A API solicita um resumo** para compreender o estado global do MFA por aplicação.
- **Todos os pedidos** da API para compreender o detalhe de cada pedido de API feito pelos utilizadores do seu inquilino, o resultado está limitado a um máximo de 10.000 pedidos mais recentes para uma melhor experiência de descarregamento.

## <a name="what-should-i-do-if-the-metrics-under-mfa-report-arent-100"></a>O que devo fazer se as métricas do relatório da MFA não forem 100%

É possível que as métricas no relatório MFA do Partner Center não sejam 100% para os parceiros que implementaram o MFA. Para entender o porquê, aqui estão alguns fatores a considerar.

> [!NOTE]
> Você precisará trabalhar com alguém da sua organização que esteja familiarizado com a gestão de identidade e implementação de MFA para o seu inquilino parceiro.

### <a name="have-you-implemented-mfa-for-your-partner-tenant"></a>Implementou o MFA para o seu inquilino parceiro?

Caso contrário, primeiro tem de implementar o MFA para o seu inquilino parceiro. Para obter mais informações sobre como implementar o MFA, consulte o artigo [Requisito de Segurança do Parceiro](partner-security-requirements.md).

### <a name="have-you-only-recently-completed-mfa-implementation"></a>Só recentemente concluiu a implementação do MFA?

As métricas são calculadas diariamente e têm em conta as operações realizadas nos últimos sete dias. Se só recentemente concluiu a implementação do MFA para o seu inquilino parceiro, as métricas podem não ser 100%.

### <a name="have-some-user-accounts-been-excluded-from-mfa-implementation"></a>Algumas contas de utilizador foram excluídas da implementação do MFA?

Compreenda se a sua atual implementação de MFA cobre todas as contas de utilizador ou apenas algumas. Algumas soluções MFA são baseadas em políticas e suportam a exclusão do utilizador, enquanto outras podem exigir que você ative explicitamente mFA por utilizador. Verifique se não excluiu nenhum utilizador da sua implementação atual do MFA. Qualquer conta de utilizador que esteja excluída e faça login no Partner Center para realizar qualquer atividade relacionada com csp pode fazer com que as métricas não sejam 100%.

### <a name="is-mfa-only-required-when-certain-conditions-are-met"></a>A MFA só é necessária quando determinadas condições são satisfeitas?

Compreenda se a sua implementação atual apenas aplica MFA apenas em condições específicas. Algumas soluções MFA proporcionam flexibilidade para apenas impor mFA quando determinadas condições são satisfeitas. Por exemplo, o utilizador está a aceder a partir de um dispositivo desconhecido ou de uma localização desconhecida. Um utilizador, que está habilitado para MFA mas não é obrigado a completar a verificação de MFA ao aceder ao Partner Center, pode fazer com que as métricas não sejam 100%.

>[!NOTE]
>Para os parceiros que implementaram o MFA utilizando os incumprimentos de segurança Azure AD, é importante notar que para as contas de utilizador não administradas a autenticação multi-factor será aplicada com base no risco. Os utilizadores serão solicitados para MFA apenas durante tentativas de entrada de risco (por exemplo, o utilizador está a iniciar sessão a partir de um local diferente). Além disso, os utilizadores terão até 14 dias para se inscreverem no MFA. Os utilizadores que não tenham preenchido o registo de MFA não serão contestados para verificação de MFA durante o período de 14 dias. Por isso, espera-se que as métricas não sejam 100% para os parceiros que implementaram o MFA utilizando os incumprimentos de segurança Azure AD.

### <a name="are-you-using-third-party-mfa-solution"></a>Está a utilizar a solução de MFA de terceiros?

Se estiver a utilizar uma solução de MFA de terceiros, identifique como a está a integrar com a Azure AD. Em geral, existem dois métodos, incluindo a federação e os controlos personalizados:

* **Federação de Identidade** - Quando a Azure AD recebe um pedido de autenticação, a Azure AD irá redirecionar o utilizador para o fornecedor de identidade federado para a autenticação. Após a autenticação bem sucedida, o fornecedor de identidade federado irá redirecionar o utilizador de volta para Azure AD juntamente com um token SAML. Para que a Azure AD reconheça que o utilizador concluiu a verificação do MFA ao autenticar o fornecedor de identidade federado, o token SAML deve incluir a *reivindicação de referências de métodos de autenticação* (com valor *multipleauthn).* Verifique se o prestador de identidade federado apoia a emissão de tal reclamação. Em caso afirmativo, verifique se o fornecedor de identidade federado foi configurado para o fazer. Se a reclamação faltar, a Azure AD (e, portanto, o Partner Center) não saberá que o utilizador concluiu a verificação do MFA e que faltar a reclamação pode fazer com que a métrica não seja a 100%.

* **Controlo Personalizado** - O Controlo Personalizado Azure AD não pode ser utilizado para identificar se um utilizador completou a verificação de MFA através de uma solução de MFA de terceiros. Como resultado, qualquer utilizador que tenha concluído a verificação de MFA através de um controlo personalizado aparecerá sempre a Azure AD (e, por sua vez, partner Center) como não tendo concluído a verificação de MFA. Sempre que possível, recomenda-se que mude a utilizar a Federação de Identidade em oposição ao Controlo Personalizado ao integrar-se com a Azure AD.

### <a name="identify-which-users-have-logged-into-partner-center-without-mfa"></a>Identifique quais os utilizadores que iniciaram sessão no Partner Center sem MFA

Pode ser útil identificar quais os utilizadores que estão a iniciar sessão no Partner Center sem verificação de MFA e verifico-los contra a sua implementação atual de MFA. Pode utilizar [o relatório de inscrição do Azure AD](/azure/active-directory/reports-monitoring/concept-sign-ins) para saber se um utilizador completou ou não a verificação de MFA. A azure AD relatório de login está atualmente disponível apenas para parceiros que tenham subscrito a Azure AD Premium ou qualquer SKU O365, que inclui Azure AD Premium (por exemplo, EMS).

## <a name="next-steps"></a>Passos seguintes

- [Comunidade de grupo de orientação de segurança do Centro parceiro](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)
- [Requisitos de segurança do Centro parceiro](partner-security-requirements.md)
- [Requisitos de segurança do Partner Center FAQ](partner-security-requirements-faq.md)