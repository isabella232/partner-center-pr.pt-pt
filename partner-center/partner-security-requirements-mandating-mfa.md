---
title: Obrigando à autenticação de vários fatores (MFA) para o seu inquilino parceiro
ms.topic: article
ms.date: 10/29/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-account
description: Saiba como mandatar o MFA para os inquilinos do seu parceiro ajudará a garantir o seu acesso aos recursos dos clientes. Inclui cenários de amostra.
author: isaiahwilliams
ms.author: iswillia
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: c29e59118f4b50cd25fbe0f1560519bb178768e2
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/09/2021
ms.locfileid: "123961100"
---
# <a name="mandating-multi-factor-authentication-mfa-for-your-partner-tenant"></a>Obrigando à autenticação de vários fatores (MFA) para o seu inquilino parceiro

**Funções adequadas**: Agente administrador | Agente comercial | Agente helpdesk | Administrador de faturação | Administração global

Este artigo dá exemplos e orientações detalhadas para a obrigatoriedade da autenticação de vários fatores (MFA) no Partner Center. A intenção desta funcionalidade é ajudar os parceiros a garantir o seu acesso aos recursos dos clientes contra o compromisso de credenciais. Os parceiros são obrigados a impor MFA para todas as contas de utilizador no seu inquilino parceiro, incluindo utilizadores convidados. Os utilizadores serão mandatados para completar a verificação do MFA para as seguintes áreas:

- [Painel de instrumentos do Centro de Parceiros](#partner-center-dashboard)
- [API do Centro de Parceiros](#partner-center-api)
- [Administração Delegada de Parceiros](#partner-delegated-administration)

Maiores e contínuas salvaguardas de segurança e privacidade estão entre as nossas principais prioridades e continuamos a ajudar os parceiros a proteger os seus clientes e inquilinos. Todos os parceiros que participam no programa Fornecedor de Soluções em Nuvem (CSP), Fornecedores de Painéis de Controlo (CPVs) e Assessores devem implementar os [Requisitos de Segurança](partner-security-requirements.md) do Parceiro para se manterem em conformidade.

Para ajudar os parceiros a proteger os seus negócios e clientes de roubo de identidade e acesso não autorizado, ativamos salvaguardas de segurança adicionais para os inquilinos parceiros que mandatam e verificam o MFA. 

## <a name="partner-center-dashboard"></a>Painel de instrumentos do Centro parceiro

Algumas páginas no painel do Partner Center serão protegidas por MFA, incluindo:

- Todas as páginas no separador **Clientes,** por exemplo, todas as páginas que podem ser acedidas através do seguinte URL: https://partner.microsoft.com/commerce/*
- Todas as páginas no **separador De apoio > pedidos do Cliente,** por exemplo, a página acedida em https://partner.microsoft.com/dashboard/support/csp/customers/*
- Página Faturação

A tabela que se segue mostra quais os tipos de utilizadores autorizados a aceder a estas páginas protegidas por MFA (e, portanto, são afetados por esta funcionalidade).


| Página protegida pelo MFA       | Agentes administrativos      |  Agentes de vendas     |   Agentes helpdesk     | Administrador global      |  Administrador de faturação     | 
|---    |---    |---    |---    |---    |---    |
| Todas as páginas no separador Clientes      |   x    |    x   |  x     |       |       |
| Todas as páginas no separador de pedidos de cliente > de suporte     | x      |       |    x   |       |       |
| Página Faturação     |   x    |       |       |    x   |   x    |

Se tentar aceder a alguma destas páginas e ainda não tiver concluído a verificação de MFA mais cedo, será obrigado a fazê-lo. Outras páginas no Partner Center, como a página De visão geral, a página de verificação do Estado de Saúde do Serviço não requerem MFA.

## <a name="verification-examples"></a>Exemplos de verificação

Para ilustrar como funciona a verificação no painel do Partner Center, considere os seguintes exemplos.

### <a name="example-1-partner-has-implemented-azure-ad-mfa"></a>Exemplo 1: Parceiro implementou Azure AD MFA

1. Jane trabalha para a CSP Contoso. A Contoso implementou o MFA para todos os seus utilizadores sob o abrigo do inquilino parceiro da Contoso utilizando Azure Ative Directory (Azure AD) MFA.

2. Jane inicia uma nova sessão de navegador e navega para a página geral do painel do Partner Center (que não está protegida pelo MFA). Partner Center redireciona Jane para Azure AD para iniciar sação.

3. Devido à configuração de MFA Azure AD existente por Contoso, a Jane é obrigada a completar a verificação de MFA. Após a verificação de s-in e MFA com sucesso, a Jane é redirecionada de volta para a página geral do painel do Partner Center.

4. Jane tenta aceder a uma das páginas protegidas pela MFA no Partner Center. Uma vez que a Jane já concluiu a verificação do MFA durante a sindução anterior, a Jane pode aceder à página protegida pelo MFA sem ser obrigada a passar novamente pela verificação do MFA.

### <a name="example-2-partner-has-implemented-third-party-mfa-using-identity-federation"></a>Exemplo 2: Parceiro implementou MFA de terceiros usando a federação de identidade

1. Trent trabalha para a CSP Wingtip. Wingtip implementou MFA para todos os seus utilizadores sob o inquilino parceiro Wingtip usando MFA de terceiros, que é integrado com Azure AD via federação de identidade.

2. Trent inicia uma nova sessão de navegador e navega para a página geral do painel do Partner Center (que não está protegida pelo MFA). Partner Center redireciona Trent para Azure AD para iniciar sação.

3. Uma vez que wingtip tem federação de identidade de configuração, Azure AD redireciona Trent para o fornecedor de identidade federado para completar a verificação de inscrição e MFA. Após a verificação de súmis e MFA com sucesso, Trent é redirecionado de volta para Azure AD e, em seguida, para a página geral do painel do Partner Center.

4. Trent tenta aceder a uma das páginas protegidas pelo MFA no Partner Center. Uma vez que o Trent já concluiu a verificação do MFA durante a entrada anterior, o Trent pode aceder à página protegida do MFA sem ser obrigado a passar novamente pela verificação do MFA.

### <a name="example-3-partner-hasnt-implemented-mfa"></a>Exemplo 3: Parceiro não implementou MFA

1. John trabalha para a CSP Fabrikam. A Fabrikam não implementou o MFA para nenhum utilizador sob o abrigo do parceiro Fabrikam.

2. John inicia uma nova sessão de navegador e navega para a página geral do painel do Partner Center (que não está protegida pelo MFA). Partner Center redireciona John para Azure AD para iniciar sação.

3. Como o Fabrikam não implementou o MFA, o John não é obrigado a completar a verificação da MFA. Após o sucesso do s-in, John é redirecionado de volta para a página geral do painel do Partner Center.

4. John tenta aceder a uma das páginas protegidas pelo MFA no Centro de Parceiros. Uma vez que o John não concluiu a verificação do MFA, o Partner Center redireciona o John para a Azure AD para completar a verificação do MFA. Uma vez que esta é a primeira vez que João é obrigado a concluir o MFA, João também é solicitado a [inscrever-se para MFA](#mfa-registration-experience). Após o registo bem sucedido do MFA e a verificação do MFA, John pode agora aceder à página protegida pelo MFA.

5. Mais um dia antes de Fabrikam implementar MFA para qualquer utilizador, John inicia uma nova sessão de navegador e navega para a página geral do painel do Partner Center (que não está protegida pelo MFA). Partner Center redireciona John para Azure AD para iniciar sação sem pedido de MFA. 

6. John tenta aceder a uma das páginas protegidas pelo MFA no Centro de Parceiros. Uma vez que o John não concluiu a verificação do MFA, o Partner Center redireciona o John para a Azure AD para completar a verificação do MFA. Uma vez que o John registou o MFA, desta vez só lhe é pedido que complete a verificação do MFA.

> [!NOTE]
>Ação: Os administradores da empresa têm [três opções](partner-security-requirements.md#implementing-multi-factor-authentication) para implementar o MFA.

## <a name="partner-center-api"></a>API do Centro de Parceiros

A API do Partner Center suporta a autenticação apenas de App e a autenticação app+User. 

Quando a autenticação app+user for utilizada, o Partner Center exigirá a verificação de MFA. Mais especificamente, quando uma aplicação de parceiro quer enviar um pedido de API para o Centro de Parceiros, deve incluir um token de acesso no cabeçalho de Autorização do pedido. 

> [!NOTE]
>O [quadro do Modelo de Aplicação Segura](/partner-center/develop/enable-secure-app-model) é um quadro escalável para autenticar parceiros e CPVs de CSP através da arquitetura Microsoft Azure MFA ao chamar APIs do Partner Center. Você precisa implementar este quadro antes de ativar mFA no seu inquilino. 

Quando o Partner Center recebe um pedido de API com um token de acesso obtido através da autenticação App+User, a API do Centro Parceiro verificará a presença do valor *MFA* na reivindicação do Método de *Autenticação (AMR).* Pode utilizar um descodificador JWT para validar se um token de acesso contém ou não o valor previsto do método de autenticação (AMR):

``` csharp
{
  "aud": "https://api.partnercenter.microsoft.com",
  "iss": "https://sts.windows.net/df845f1a-7b35-40a2-ba78-6481de91f8ae/",
  "iat": 1549088552,
  "nbf": 1549088552,
  "exp": 1549092452,
  "acr": "1",
  "amr": [
    "pwd",
    "mfa"
  ],
  "appid": "23ec45a3-5127-4185-9eff-c8887839e6ab",
  "appidacr": "0",
  "family_name": "Adminagent",
  "given_name": "CSP",
  "ipaddr": "127.0.0.1",
  "name": "Adminagent CSP",
  "oid": "4988e250-5aee-482a-9136-6d269cb755c0",
  "scp": "user_impersonation",
  "tenant_region_scope": "NA",
  "tid": "df845f1a-7b35-40a2-ba78-6481de91f8ae",
  "unique_name": "Adminagent.csp@testtestpartner.onmicrosoft.com",
  "upn": "Adminagent.csp@testtestpartner.onmicrosoft.com",
  "ver": "1.0"
}
```

Se o valor estiver presente, o Partner Center conclui que a verificação do MFA foi concluída e processa o pedido da API. Se o valor não estiver presente, a API do Partner Center rejeitará o pedido com a seguinte resposta:

``` csharp
HTTP/1.1 401 Unauthorized - MFA required
Transfer-Encoding: chunked
Request-Context: appId=cid-v1:03ce8ca8-8373-4021-8f25-d5dd45c7b12f
WWW-Authenticate: Bearer error="invalid_token"
Date: Thu, 14 Feb 2019 21:54:58 GMT
```

Quando App-Only autenticação for utilizada, as APIs que suportam App-Only autenticação funcionarão continuamente sem necessitar de MFA.

## <a name="partner-delegated-administration"></a>Administração Delegada de Parceiros

As contas de parceiros, incluindo Agentes Admin e Agentes Helpdesk, podem utilizar os seus Privilégios de Administração Delegados de Parceiros para gerir os recursos dos clientes através dos Portais de Serviços Online da Microsoft, interface de linha de comando (CLI) e APIs (utilizando a autenticação app+user).

### <a name="using-service-portals"></a>Usando portais de serviço

Ao aceder aos Portais de Serviços Online da Microsoft utilizando os Privilégios Admin Delegados (Admin-On-Behalf-Of) para gerir os recursos do cliente, muitos destes portais exigem que a conta do parceiro autente interativamente, com o cliente Azure AD a definir como o contexto de autenticação - a conta do parceiro é obrigada a assinar no cliente inquilino.

Quando a Azure AD receber tais pedidos de autenticação, exigirá que a conta do parceiro complete a verificação do MFA. Existem duas experiências possíveis de utilizador, dependendo se a conta do parceiro é uma identidade gerida ou federada:

- Se a conta do parceiro for uma identidade **gerida,** a Azure AD irá diretamente solicitar ao utilizador que complete a verificação de MFA. Se a conta parceira não tiver registado para MFA com Azure AD antes, o utilizador será solicitado a completar primeiro o [registo de MFA.](#mfa-registration-experience)

- Se a conta do parceiro for uma identidade **federada,** a experiência depende da forma como o administrador parceiro configura a federação em Azure AD. Ao criar uma federação em Azure AD, o administrador do parceiro pode indicar à Azure AD se o fornecedor de identidade federado apoia ou não o MFA. Em caso afirmativo, o Azure AD irá redirecionar o utilizador para o fornecedor de identidade federado para completar a verificação do MFA. Caso contrário, o Azure AD irá diretamente levar o utilizador a completar a verificação de MFA. Se a conta parceira não tiver registado para MFA com Azure AD antes, o utilizador será solicitado a completar primeiro o [registo de MFA.](#mfa-registration-experience)

A experiência global é semelhante ao cenário em que um inquilino de cliente final implementou mFA para os seus administradores. Por exemplo, o inquilino do cliente permitiu [incumprimentos de segurança Azure AD,](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)que requer todas as contas com direitos administrativos para assinar no cliente inquilino com verificação de MFA, incluindo Agentes Admin e Agentes helpdesk. Para efeitos de teste, os parceiros podem ativar os [incumprimentos de segurança Azure AD](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) no inquilino do cliente e, em seguida, tentar usar privilégios de administração delegado de parceiro para aceder ao cliente inquilino.

> [!NOTE]
> Nem todos os Portais de Serviço Online da Microsoft exigem que as contas dos parceiros assinem o cliente ao aceder aos recursos do cliente utilizando privilégios de administração delegados de parceiros. Em vez disso, apenas exigem que as contas do parceiro assinem o inquilino do parceiro. Um exemplo é o Exchange Centro de Administração. Com o tempo, esperamos que estes portais exijam contas de parceiros para assinar no inquilino do cliente quando utilizar privilégios de administração delegados de parceiro.

### <a name="using-service-apis"></a>Utilização de APIs de serviço

Alguns APIs de Serviços Online da Microsoft (tais como Azure Resource Manager, Azure AD Graph, Microsoft Graph, etc.) parceiros de suporte usando parceiros delegados de Admin Privileges para gerir programáticamente os recursos do cliente. Para utilizar os Privilégios de Administração Delegados de Parceiros com estas APIs, a aplicação do parceiro deve incluir um token de acesso no cabeçalho de autorização de pedido da API, onde o token de acesso é obtido por ter uma conta de utilizador parceira para autenticar com Azure AD, com o cliente Azure AD definido como o contexto de autenticação. A aplicação do parceiro é necessária para ter um sinal de conta de utilizador parceiro no inquilino do cliente.

Quando a Azure AD receber, tal como o pedido de autenticação, o Azure AD exigirá que a conta de utilizador do parceiro complete a verificação do MFA. Se a conta de utilizador do parceiro não tiver registado anteriormente para MFA, a conta de utilizador será solicitada para completar primeiro o registo de MFA.

Todas as aplicações de parceiros que são integradas com estas APIs utilizando privilégios de administração delegados de parceiros são afetadas por esta funcionalidade. Para garantir que as aplicações dos parceiros podem continuar a trabalhar com estas APIs sem interrupção:

- O parceiro deve evitar a utilização de métodos de autenticação não interativos com Azure AD para obter o token de acesso. Ao utilizar métodos de autenticação não interativos de utilizador, como [o Password Flow,](https://github.com/AzureAD/azure-activedirectory-library-for-dotnet/wiki/Acquiring-tokens-with-username-and-password)a Azure AD não poderá solicitar ao utilizador que complete a verificação do MFA. O parceiro deve mudar para o método de autenticação interativa do utilizador, como [o fluxo de Ligação OpenID.](/azure/active-directory/develop/v1-protocols-openid-connect-code)

- Durante o método de autenticação interativa do utilizador, o parceiro deve utilizar uma conta de utilizador parceira que já esteja ativada para MFA. Em alternativa, quando solicitado pela Azure AD, o parceiro pode completar o registo de MFA e a verificação de MFA durante a entrada.

- Isto é semelhante ao cenário em que um inquilino de cliente final implementou mFA para os seus administradores. Por exemplo, o inquilino do cliente permitiu [incumprimentos de segurança Azure AD,](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)que requer todas as contas de utilizador com direitos administrativos para assinar no cliente inquilino com verificação de MFA, incluindo Agentes Admin e Agentes helpdesk. Para efeitos de teste, os parceiros podem ativar os [incumprimentos de segurança Azure AD](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) no inquilino do cliente e, em seguida, tentar usar privilégios de administração delegado de parceiro para aceder programáticamente ao inquilino do cliente.

### <a name="mfa-registration-experience"></a>Experiência de registo de MFA

Durante a verificação do MFA, se a conta parceira não tiver registado para MFA antes, a Azure AD solicitará ao utilizador que complete primeiro o registo de MFA:

:::image type="content" source="images/MfaRegistration1.png" alt-text="Passo de registo do MFA 1.":::

Depois de clicar em **Seguinte,** o utilizador será convidado a escolher entre uma lista de métodos de verificação.

:::image type="content" source="images/MfaRegistration2.png" alt-text="Passo de registo do MFA 2.":::

Após o registo bem sucedido, o utilizador é então obrigado a completar a verificação de MFA com base na verificação escolhida pelo utilizador.
 
## <a name="list-of-common-issues"></a>Lista de questões comuns

Antes de solicitar [a exceção técnica](#how-to-submit-a-request-for-technical-exception) ao requisito do MFA, reveja a lista de questões comuns comunicadas por outros parceiros para entender se o seu pedido é válido.

#### <a name="issue-1-partner-needs-more-time-to-implement-mfa-for-their-partner-agents"></a>Edição 1: O parceiro precisa de mais tempo para implementar o MFA para os seus agentes parceiros
Um parceiro ainda não iniciou ou ainda está em processo de implementação de MFA para os seus agentes parceiros que exigem acesso aos Portais de Serviços Online da Microsoft usando privilégios de administração delegados de parceiros para gerir os recursos dos clientes. O parceiro precisa de mais tempo para concluir a implementação do MFA. Esta questão é uma razão válida para exceção técnica?

**Resposta:** Não. O parceiro precisa de fazer planos de implementação de MFA para os seus utilizadores para evitar perturbações.

> [!NOTE]
> Apesar de o parceiro não ter implementado o MFA para os seus agentes parceiros, os agentes parceiros ainda podem aceder aos Portais de Serviços Online da Microsoft utilizando privilégios de administração delegados de parceiros, desde que possam completar o registo de MFA e a verificação do MFA quando solicitados durante o início de sedução ao cliente. O preenchimento do registo MFA não permite automaticamente o utilizador de MFA.

##### <a name="issue-2-partner-has-not-implemented-mfa-for-user-accounts-not-using-delegated-admin-privileges"></a>Edição 2: Parceiro não implementou MFA para contas de utilizador que não utilizem privilégios de administração delegados
Um parceiro tem alguns utilizadores nos seus inquilinos parceiros que não necessitam de acesso aos Portais de Serviços Online da Microsoft para gerir os recursos dos clientes usando privilégios de administração delegados de parceiros. O parceiro está em processo de implementação de MFA para estes utilizadores e precisa de mais tempo para completar. Esta questão é uma razão válida para exceção técnica?

**Resposta:** Não. Uma vez que estas contas de utilizador não estão a utilizar privilégios de administração delegados de parceiros para gerir os recursos do cliente, não serão obrigados a inscrever-se no cliente. Não serão afetados pela Azure AD que exija a verificação do MFA durante a entrada no cliente.

##### <a name="issue-3-partner-has-not-implemented-mfa-for-user-service-accounts"></a>Edição 3: Parceiro não implementou MFA para contas de serviço de utilizador
Um parceiro tem algumas contas de utilizador nos seus inquilinos parceiros, que estão a ser usadas por dispositivos como contas de serviço. Estas são contas privilegiadas baixas que não requerem acesso ao Partner Center nem portais de serviços online da Microsoft para gerir os recursos do cliente usando privilégios de administração delegados de parceiros. Esta questão é uma razão válida para exceção técnica?

**Resposta:** Não. Uma vez que estas contas de utilizador não estão a utilizar privilégios de administração delegados de parceiros para gerir os recursos do cliente, não serão obrigados a inscrever-se no cliente. Não serão afetados pela Azure AD que exija a verificação do MFA durante a entrada no cliente.

##### <a name="issue-4-partner-cannot-implement-mfa-using-ms-authenticator-app"></a>Edição 4: O parceiro não pode implementar o MFA utilizando a App MS Authenticator
Um parceiro tem uma política de "mesa limpa", que não permite que os colaboradores tragam os seus dispositivos móveis pessoais para a sua área de trabalho. Sem acesso aos seus dispositivos móveis pessoais, os colaboradores não podem instalar a App MS Authenticator, que é a única verificação MFA suportada por padrão de segurança Azure AD. Esta questão é uma razão válida para exceção técnica?

**Resposta**: Não, esta não é uma razão válida para exceção técnica. O parceiro deve considerar as seguintes alternativas, para que os seus colaboradores ainda possam completar a verificação de MFA ao aceder ao Partner Center:
- O parceiro também pode inscrever-se para soluções de MFA de Azure AD Premium ou de terceiros (compatíveis com Azure AD) que podem fornecer métodos de verificação adicionais.

##### <a name="issue-5-partner-cannot-implement-mfa-due-to-the-use-of-legacy-authentication-protocols"></a>Edição 5: O parceiro não pode implementar MFA devido à utilização de protocolos de autenticação de legados
Um parceiro tem alguns agentes parceiros que ainda usam protocolos de autenticação legado, que não são compatíveis com MFA. Por exemplo, os utilizadores ainda estão a utilizar Outlook 2010, que se baseia em protocolos de autenticação antigas. Permitir que o MFA para estes agentes parceiros irá perturbar a utilização de protocolos de autenticação legado.

**Resposta**: Não, esta não é uma razão válida para exceção técnica. Os parceiros são fortemente encorajados a afastarem-se da utilização de protocolos de autenticação legado devido a potenciais implicações de segurança, uma vez que estes protocolos não podem ser protegidos com a verificação do MFA e são muito mais suscetíveis a compromissos credenciais. Se afastarem-se da utilização de protocolos de autenticação legado não for uma opção, os parceiros devem considerar inscrever-se para Azure AD Premium, que suporta a utilização de Passwords de Aplicação. As palavras-passe de aplicação são senhas geradas pelo sistema uma única vez, e são geralmente mais fortes do que as palavras-passe geradas pelo homem. Ao utilizarem as Passwords de Aplicação, os parceiros podem implementar MFA para os seus utilizadores, ao mesmo tempo que recorrem a Passwords de Aplicação apenas para protocolos de autenticação legado.

Leia a publicação sobre o [Basic Auth e o Exchange Online](https://techcommunity.microsoft.com/t5/exchange-team-blog/basic-auth-and-exchange-online-february-2020-update/ba-p/1191282) para compreender o mais recente plano de apoio à autenticação de legados para Outlook, e siga o blog da equipa [Exchange](https://techcommunity.microsoft.com/t5/exchange-team-blog/bg-p/Exchange) para obter as próximas novidades. 

> [!NOTE]
> Apesar de o parceiro não ter implementado o MFA para os seus agentes parceiros, os agentes parceiros ainda podem aceder aos Portais de Serviços Online da Microsoft utilizando privilégios de administração delegados de parceiros, desde que possam completar o registo de MFA e a verificação do MFA quando solicitados durante o início de sedução ao cliente. O preenchimento do registo MFA não permite automaticamente o utilizador de MFA.

##### <a name="issue-6-partner-has-implemented-third-party-mfa-that-isnt-recognized-by-azure-ad"></a>Edição 6: Parceiro implementou MFA de terceiros que não é reconhecido pela Azure AD
Um parceiro implementou mFA para os seus utilizadores usando uma solução de MFA de terceiros. No entanto, o parceiro não consegue configurar corretamente a solução MFA de terceiros para transmitir à Azure AD que a verificação do MFA foi concluída durante a autenticação do utilizador. É uma razão válida para exceção técnica?

**Resposta**: Sim, esta questão pode ser considerada como uma razão válida para exceção técnica. Antes de apresentar um pedido de exceção técnica, confirme com o fornecedor de soluções MFA de terceiros que a solução MFA não pode ser configurada para fluir a *reivindicação de autenticação de métodos* (com valor *múltiplo)* para Azure AD para indicar que a verificação do MFA foi concluída durante a autenticação do utilizador. Ao apresentar um pedido de exceção técnica, deve fornecer detalhes sobre a solução de MFA de terceiros utilizada, e indicar o método de integração (por exemplo, através da federação de identidade ou utilização do Controlo Personalizado Azure AD), e fornecer as seguintes informações no pedido de exceção técnica como os documentos comprovativos:

- As configurações de MFA de terceiros.

- O resultado do [Teste dos Requisitos de Segurança do Parceiro](/powershell/partnercenter/test-partner-security-requirements) que são geridos pela conta ativada por MFA de terceiros.

- A ordem de compra da solução MFA de terceiros que está a usar ou planeia utilizar.

## <a name="how-to-submit-a-request-for-technical-exception"></a>Como apresentar um pedido de exceção técnica

Os parceiros podem solicitar uma exceção técnica para suprimir a verificação do MFA se estiverem a encontrar problemas técnicos com os Serviços Online da Microsoft e não houver solução ou solução viável. Antes de o fazer, reveja a [lista de questões comuns](#list-of-common-issues) na secção anterior.

Para apresentar um pedido de exceção técnica:

1. Inscreva-se no Partner Center como Global Admin ou Agente Administrador.

2. Crie um novo pedido de serviço de parceiro navegando para apoiar pedidos de apoio ao Parceiro de **Apoio** e  >   selecionando **novo pedido.**

3. Pesquisa de **MFA - Pedido de exceção** na caixa de pesquisa; ou selecione **CSP** a partir da categoria, em **seguida, selecione Contas, Onboarding, Acesso** a partir de Tópico, em seguida, selecione **MFA - Pedido** de exceção a partir do subtópico, em seguida, selecione o **próximo passo**.

4. Forneça os detalhes solicitados para apresentar um pedido de serviço de exceção técnica e **selecione Enviar por isso.**

A Microsoft pode demorar até três dias úteis para dar uma resposta a um pedido de exceção técnica.

## <a name="next-steps"></a>Passos seguintes

 - [Estado dos requisitos de segurança dos parceiros](partner-security-compliance.md)