---
title: Relatório de estado dos requisitos de segurança
ms.date: 10/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-account
description: Saiba como verificar os seus requisitos de segurança, cumprindo o relatório de estado dos requisitos de segurança e o relatório MFA do Partner Center
author: isaiahwilliams
ms.author: iswillia
ms.localizationpriority: high
ms.topic: conceptual
ms.custom: SEOMAY.20
ms.openlocfilehash: 15e2792a38f8fc90612282ff30ad57dc320fc96a
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/13/2021
ms.locfileid: "126246755"
---
# <a name="security-requirements-status-report"></a>Relatório de estado dos requisitos de segurança

**Funções adequadas**: Administração cpV | Administração global

Este artigo explica o relatório de estado dos requisitos de segurança no Partner Center. Este relatório fornece métricas sobre o cumprimento dos requisitos de segurança do parceiro para a autenticação de [vários](partner-security-requirements.md) fatores (MFA) para os utilizadores do seu inquilino parceiro.

Para aceder a este relatório no [Partner Center,](https://partner.microsoft.com/dashboard)vá a **Definições**  >  **Defina o** estado  >  **dos requisitos de segurança**. O relatório é atualizado diariamente e reflete os dados de inscrição dos últimos sete dias.

>[!NOTE]
>O relatório de estado dos requisitos de segurança é suportado apenas no Partner Center. Não está disponível no Microsoft Cloud for US Government ou Microsoft Cloud Germany. Recomendamos vivamente que todos os parceiros que transacionem através de uma nuvem soberana (Governo dos EUA e Alemanha) adotem imediatamente estes novos requisitos de segurança. No entanto, estes parceiros não são atualmente obrigados a satisfazer os novos requisitos de segurança. A Microsoft fornecerá detalhes adicionais sobre a aplicação destes requisitos de segurança para nuvens soberanas no futuro.

## <a name="security-status-metrics"></a>Métricas de estado de segurança

O relatório de estado dos requisitos de segurança oferece insights sobre a implementação do MFA parceiro, e fornece métricas sobre a configuração de MFA e atividades do Partner Center em inquilinos parceiros. As seguintes secções explicam estas métricas mais detalhadamente.

### <a name="mfa-configuration-on-a-partner-tenant"></a>Configuração de MFA em um inquilino parceiro

A percentagem métrica **de contas de utilizador ativadas com MFA aplicadas utilizando opções listadas aqui:** mostra a percentagem de contas de utilizador ativadas no seu inquilino parceiro que têm MFA aplicada. Pode utilizar uma destas [opções de MFA](/azure/active-directory/fundamentals/concept-fundamentals-mfa-get-started) para alcançar o cumprimento. Estes dados são capturados e reportados diariamente. Por exemplo:

- A Contoso é parceira da CSP com 110 contas de utilizador no arrendatário, 10 dessas contas de utilizador estão desativadas. 
- Das restantes 100 contas de utilizador, 90 são aplicadas com recurso às [opções de MFA fornecidas.](/azure/active-directory/fundamentals/concept-fundamentals-mfa-get-started) Assim, a métrica mostra 90%. 

### <a name="partner-center-requests-with-mfa"></a>Pedidos do Centro de Parceiros com OMF

Sempre que os seus colaboradores se inscrevem no Partner Center para trabalhar ou, através de APIs, obter ou enviar dados através do Partner Center, o seu estado de segurança é contestado e rastreado. Também estão incluídas no rastreio do estado de segurança as suas aplicações e quaisquer aplicações de fornecedor de painéis de controlo. Estes dados são apresentados em métricas em **percentagem de pedidos ao Partner Center com MFA,** e refletem os últimos sete dias.

#### <a name="dashboard-mfa-verification"></a>Verificação do Painel de Instrumentos MFA

A métrica **através do portal Partner Center** está relacionada com atividades dentro do painel do Centro de Parceiros. Mede a percentagem de operações efetuadas por utilizadores que tenham concluído a verificação do MFA. Por exemplo:

- Contoso é sócio da CSP com dois agentes administrativos, Jane e John.
- No primeiro dia, a Jane entrou no painel do Partner Center sem verificação de MFA e fez três operações.
- No segundo dia, John entrou no dashboard do Partner Center sem verificação de MFA e fez cinco operações.
- No terceiro dia, a Jane entrou no painel do Partner Center com verificação de MFA e fez duas operações.
- Não houve operações feitas por nenhum dos agentes nos restantes quatro dias.
- Das 10 operações e realizadas na janela de sete dias, duas foram feitas pelo utilizador com verificação de MFA. Assim, a métrica mostra 20%.

Utilize os pedidos do Portal do Ficheiro **sem MFA** para perceber qual o utilizador que iniciou sessão no painel de instrumentos do Partner Center sem ter verificação de MFA e hora da última visita durante a janela de reporte.

#### <a name="appuser-mfa-verification"></a>App+User MFA verificação

A métrica **Através da API ou da SDK** está relacionada com a autenticação app+user através de pedidos de API do Partner Center. Mede a percentagem de pedidos de API feitos com recurso a um token de acesso com pedido de MFA. Por exemplo:

- A Fabrikam é parceira da CSP e tem uma aplicação CSP que utiliza uma mistura de métodos de autenticação app+user e apenas para aplicações.
- No primeiro dia, a aplicação equindo três pedidos de API, que foram apoiados por um token de acesso obtido através do método de autenticação App+User sem verificação de MFA.
- No segundo dia, a aplicação e fez cinco pedidos de API, que foram apoiados por um token de acesso obtido com a autenticação apenas da App.
- No terceiro dia, a aplicação e fez dois pedidos de API, que foram apoiados por um token de acesso obtido utilizando o método de autenticação App+User com verificação de MFA.
- Não houve operações feitas por nenhum dos agentes nos restantes quatro dias.
- Os cinco pedidos da API no segundo dia, que foram apoiados por um token de acesso obtido através da autenticação apenas da App, são omitidos da métrica, uma vez que não recorre às credenciais dos utilizadores. Das restantes cinco operações, duas foram apoiadas por um sinal de acesso obtido com verificação de MFA. Assim, a métrica mostra 40%.

Se quiser entender quais as atividades app+utilizador que resultam na não 100% nesta métrica, utilize ficheiros:

- **A API solicita um resumo** para compreender o estado global do MFA por aplicação.
- **Todos os pedidos** da API para compreender o detalhe de cada pedido de API feito pelos utilizadores do seu inquilino, o resultado está limitado a um máximo de 10.000 pedidos mais recentes para uma melhor experiência de descarregamento.

## <a name="actions-for-mfa-status-below-100"></a>Ações para o estatuto de MFA abaixo de 100%

Alguns parceiros que implementaram o MFA podem ver métricas de relatório abaixo de 100%. Para entender o porquê, aqui estão alguns fatores a considerar.

> [!NOTE]
> Você precisará trabalhar com alguém da sua organização que esteja familiarizado com a gestão de identidade e implementação de MFA para o seu inquilino parceiro.

### <a name="implemented-mfa-for-your-partner-tenant"></a>MFA implementado para o seu inquilino parceiro

Tem de implementar o MFA para que o seu inquilino parceiro atinja o cumprimento. Para obter detalhes sobre como implementar o MFA, consulte [os requisitos de Segurança para a utilização de APIs do Partner Center ou partner Center](partner-security-requirements.md).

>[!NOTE]
> As métricas de MFA são calculadas diariamente e têm em conta as operações realizadas nos últimos sete dias. Se só recentemente concluiu a implementação do MFA para o seu inquilino parceiro, as métricas podem ainda não apresentar 100%.

### <a name="verify-mfa-on-all-user-accounts"></a>Verificar MFA em todas as contas de utilizador

Compreenda se a sua atual implementação de MFA cobre todas as contas de utilizador ou apenas algumas. Algumas soluções MFA são baseadas em políticas e suportam a exclusão do utilizador, enquanto outras podem exigir que você ative explicitamente mFA por utilizador. Verifique se não excluiu nenhum utilizador da sua implementação atual do MFA. Qualquer conta de utilizador que esteja excluída e faça login no Partner Center para realizar qualquer atividade relacionada com CSP, CPV ou Advisor pode fazer com que as métricas não sejam 100%.

### <a name="review-your-mfa-conditions"></a>Reveja as suas condições de MFA

Compreenda se a sua implementação atual apenas aplica MFA apenas em condições específicas. Algumas soluções MFA proporcionam flexibilidade para apenas impor mFA quando determinadas condições são satisfeitas. Por exemplo, o utilizador está a aceder a partir de um dispositivo desconhecido ou de uma localização desconhecida. Um utilizador, que está habilitado para MFA mas não é obrigado a completar a verificação de MFA ao aceder ao Partner Center, pode fazer com que as métricas não sejam 100%.

>[!NOTE]
>Para os parceiros que implementaram o MFA utilizando os incumprimentos de segurança Azure AD, é importante notar que para as contas de utilizador não administradas a autenticação multi-factor será aplicada com base no risco. Os utilizadores serão solicitados para MFA apenas durante tentativas de entrada de risco (por exemplo, o utilizador está a iniciar sessão a partir de um local diferente). Além disso, os utilizadores terão até 14 dias para se inscreverem no MFA. Os utilizadores que não tenham preenchido o registo de MFA não serão contestados para verificação de MFA durante o período de 14 dias. Por isso, espera-se que as métricas não sejam 100% para os parceiros que implementaram o MFA utilizando os incumprimentos de segurança Azure AD.

### <a name="review-third-party-mfa-configurations"></a>Rever configurações de MFA de terceiros

Se estiver a utilizar uma solução de MFA de terceiros, identifique como a está a integrar com a Azure AD. Em geral, existem dois métodos, incluindo a federação e os controlos personalizados:

* **Federação de Identidade** - Quando a Azure AD recebe um pedido de autenticação, a Azure AD irá redirecionar o utilizador para o fornecedor de identidade federado para a autenticação. Após a autenticação bem sucedida, o fornecedor de identidade federado irá redirecionar o utilizador de volta para Azure AD juntamente com um token SAML. Para que a Azure AD reconheça que o utilizador concluiu a verificação do MFA ao autenticar o fornecedor de identidade federado, o token SAML deve incluir a *reivindicação de referências de métodos de autenticação* (com valor *multipleauthn).* Verifique se o prestador de identidade federado apoia a emissão de tal reclamação. Em caso afirmativo, verifique se o fornecedor de identidade federado foi configurado para o fazer. Se a reclamação faltar, a Azure AD (e, portanto, o Partner Center) não saberá que o utilizador concluiu a verificação do MFA e que faltar a reclamação pode fazer com que a métrica não seja a 100%.

* **Controlo Personalizado** - O Controlo Personalizado Azure AD não pode ser utilizado para identificar se um utilizador completou a verificação de MFA através de uma solução de MFA de terceiros. Como resultado, qualquer utilizador que tenha concluído a verificação de MFA através de um controlo personalizado aparecerá sempre a Azure AD (e, por sua vez, partner Center) como não tendo concluído a verificação de MFA. Sempre que possível, recomenda-se que mude a utilizar a Federação de Identidade em oposição ao Controlo Personalizado ao integrar-se com a Azure AD.

### <a name="identify-which-users-have-signed-in-to-partner-center-without-mfa"></a>Identifique quais os utilizadores que se inscreveram no Partner Center sem MFA

Pode ser útil identificar quais os utilizadores que estão a iniciar sessão no Partner Center sem verificação de MFA e verifico-los contra a sua implementação atual de MFA. Pode utilizar [o relatório de inscrição do Azure AD](/azure/active-directory/reports-monitoring/concept-sign-ins) para saber se um utilizador completou ou não a verificação de MFA. A azure AD relatório de entrada só está disponível atualmente para parceiros que tenham subscrito Azure AD Premium ou qualquer SKU O365, que inclui Azure AD Premium (por exemplo, EMS).

## <a name="next-steps"></a>Passos seguintes

- [Comunidade de grupo de orientação de segurança do Centro parceiro](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)
- [Requisitos de segurança do Centro de Parceiros](partner-security-requirements.md)
- [Requisitos de segurança do Partner Center FAQ](partner-security-requirements-faq.yml)
