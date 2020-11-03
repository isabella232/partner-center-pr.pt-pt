---
title: Requisitos de segurança dos parceiros
ms.topic: article
ms.date: 10/26/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Introduz os requisitos do parceiro para permitir a autenticação multi-factor (MFA) e adotar o quadro do Modelo de Aplicação Segura.
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: c92e8c9a9a08582d89ef478a4600f737a548b787
ms.sourcegitcommit: 2847efac28d3bff24ed37cdfaa88ff4be06705c8
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/27/2020
ms.locfileid: "92680388"
---
# <a name="partner-security-requirements-for-partners-using-partner-center-or-partner-center-apis"></a>Requisitos de segurança do parceiro para parceiros que utilizem APIs do Partner Center ou do Partner Center

**Aplica-se a**

- Todos os parceiros no programa Cloud Solution Provider
  - Conta direta
  - Fornecedor indireto
  - Revendedor indireto
- Todos os fornecedores de painéis de controlo
- Todos os Conselheiros

**Utilizadores apropriados**

- Todos os utilizadores habilitados, incluindo utilizadores convidados

Uma maior salvaguarda de privacidade e segurança estão entre as nossas principais prioridades. Sabemos que a melhor defesa é a prevenção e que somos tão fortes quanto o nosso elo mais fraco. É por isso que precisamos que todos os nossos ecossistemas atuem e garantam a proteção de segurança adequadas. Para ajudar a salvaguardar parceiros e clientes, estamos a introduzir um conjunto de requisitos de segurança obrigatórios para assessores, fornecedores de painéis de controlo e parceiros que participam no programa Cloud Solution Provider.

## <a name="overview"></a>Descrição geral

Os parceiros são obrigados a impor a autenticação de vários fatores para todas as contas de utilizador no seu inquilino parceiro. Os termos associados aos requisitos de segurança do parceiro foram adicionados ao Acordo de Parceiros da Microsoft. No que diz respeito aos Consultores, os mesmos requisitos contratuais estarão em vigor.

Os parceiros que não implementarem os requisitos de segurança obrigatórios não poderão negociar no programa Cloud Solution Provider ou gerir os inquilinos dos clientes aproveitando os direitos de administração delegados, uma vez que estes requisitos são aplicados. Além disso, os parceiros que não implementem os requisitos de segurança podem colocar a sua participação em programas em risco.  

Para protegê-lo e aos seus clientes, exigimos que os parceiros tomem as seguintes ações imediatamente:  

1. **Ativar a Autenticação Multi-Factor (MFA) para todas as contas do utilizador no seu inquilino parceiro.** Todas as contas de utilizador no seu(s) inquilino(s) parceiro devem ser desafiadas por autenticação multi-factor (MFA) quando assinarem nos serviços de nuvem comercial da Microsoft ou quando transacionam no programa Cloud Solution Provider através do Partner Center ou via APIs.

2. **Adotar o quadro do Modelo de Aplicação Segura** . Adotar o quadro do Modelo de Aplicação Segura. Todos os parceiros que se integram com a API do Partner Center devem adotar o quadro do Modelo de Aplicação Segura para qualquer aplicação + aplicações de modelos de utilizador.

    > [!IMPORTANT]
    > Recomendamos vivamente que os parceiros implementem o Modelo de Aplicação Segura para integração com uma API da Microsoft, como o Azure Resource Manager, o Microsoft Graph, ou a automatização de alavancagem, como o PowerShell, utilizando credenciais de utilizador, para evitar qualquer perturbação quando o MFA é aplicado.

Ativar a Autenticação Multi-Factor (MFA) e a adoção do quadro do Modelo de Aplicação Segura ajudarão a proteger a sua infraestrutura e a proteger os dados do seu cliente de potenciais riscos de segurança, tais como identificar roubos ou outros incidentes de fraude.  

## <a name="actions-that-you-need-to-take"></a>Ações que precisa de tomar

Para cumprir os requisitos de segurança do parceiro, deve impor a autenticação de vários fatores para cada conta de utilizador no seu inquilino parceiro. Pode fazer isto de uma das seguintes formas:

- Implementação de [falhas de segurança Azure AD](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults).

- Compra do Azure Ative Directory Premium para cada conta de utilizador. Para obter mais informações, consulte [Planejando uma implementação de autenticação multi-factor Azure baseada na nuvem](/azure/active-directory/authentication/howto-mfa-getstarted).

- Utilizar uma solução de terceiros para impor a autenticação de vários fatores para cada conta de utilizador no seu inquilino parceiro. Para garantir que a solução fornecerá a solução esperada, veja [como os requisitos de segurança serão cumpridos.](#how-the-requirements-are-enforced)

> [!NOTE]
> Embora a autenticação multi-factor não seja contratualmente necessária para uma nuvem soberana (21Vianet, Governo dos EUA e Alemanha) é altamente recomendado que adote estes requisitos de segurança.

## <a name="security-defaults"></a>Predefinições de segurança

A política de incumprimentos de segurança é uma das [opções](#actions-that-you-need-to-take) que os parceiros podem optar por implementar MFA para os requisitos de segurança, dependendo das suas necessidades de negócio. Oferece um nível básico de segurança, sem custos adicionais. Reveja como ativar o MFA para a sua organização com Azure AD e as principais considerações abaixo antes de permitir os incumprimentos de segurança.

- As políticas de base permanecerão durante os próximos meses e serão alvos precotados no final de fevereiro de 2020.

- Os parceiros que já adotaram políticas de base precisam de tomar medidas para a transição para incumprimentos de segurança.

- Os incumprimentos de segurança são a substituição geral da disponibilidade das políticas de base de pré-visualização. Uma vez que um parceiro permita os incumprimentos de segurança, eles deixarão de ser capazes de ativar políticas de base.

- Com os incumprimentos de segurança, todas as políticas serão ativadas de uma só vez.

- Para os parceiros que utilizam [acesso condicional,](/azure/active-directory/conditional-access/concept-conditional-access-policy-common) [não estarão disponíveis padrão de segurança](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults#disabling-security-defaults).

- O bloqueio da autenticação do legado não será aplicado aos parceiros neste momento. No entanto, como a maioria dos eventos relacionados com identidades comprometidas provém de tentativas de inscrição usando a autenticação antiga, os parceiros são encorajados a afastar-se destes protocolos mais antigos.

- A conta de sincronização Azure AD Connect está excluída de incumprimentos de segurança.

- Para obter informações detalhadas, leia [Ativar a autenticação multi-factor para a sua organização](/azure/active-directory/authentication/concept-mfa-get-started) e as falhas de segurança do [Azure Ative Directory](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults).

> [!NOTE]
> O incumprimento de segurança Azure AD é a evolução das políticas de proteção de base simplificadas. Se já ativou as políticas de proteção de base, é altamente recomendável que ative os incumprimentos de segurança.

Para a transição das políticas de base para os incumprimentos de segurança, leia [O que são os incumprimentos de segurança?](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)

### <a name="consideration"></a>Consideração

Uma vez que estes requisitos se aplicam a todas as contas de utilizador no seu inquilino parceiro, é necessário considerar várias coisas para garantir uma implementação suave, incluindo identificar contas de utilizadores no Azure Ative Directory que não podem realizar a autenticação de vários fatores, bem como aplicações e dispositivos utilizados pela sua organização que não suportam a autenticação moderna.

Antes de realizar qualquer ação, recomendamos que complete as seguintes validações: 

#### <a name="do-you-have-an-application-or-device-that-does-not-support-the-use-of-modern-authentication"></a>Possui uma aplicação ou dispositivo que não suporte ao uso da autenticação moderna?

Quando aplicar a autenticação de vários fatores, os protocolos de autenticação de legados como IMAP, POP3, SMTP, etc. serão bloqueados porque não suportam a autenticação de vários fatores. Para resolver esta limitação, uma funcionalidade conhecida como [palavras-passe da aplicação](/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords) pode ser utilizada para garantir que a aplicação ou dispositivo continuará a autenticar. Deve rever as considerações de utilização de palavras-passe de aplicações documentadas [aqui](/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords) para determinar se podem ser usadas no seu ambiente.

#### <a name="do-you-have-users-using-office-365-provided-by-licenses-associated-with-your-partner-tenant"></a>Tem utilizadores que utilizem o Office 365 fornecidos por licenças associadas ao seu inquilino parceiro?

Antes de implementar qualquer solução, recomendamos que determine qual a versão do Microsoft Office que está a ser usada pelos utilizadores no seu inquilino parceiro. Existe a possibilidade de os seus utilizadores experimentarem problemas de conectividade com aplicações como o Outlook. Antes de impor a autenticação multi-factor, é importante garantir que o Outlook 2013 SP1, ou mais tarde, está a ser utilizado e que a sua organização tem a autenticação moderna ativada. Para mais informações, consulte [Ative a autenticação moderna em Exchange Online.](/exchange/clients-and-mobile-in-exchange-online/enable-or-disable-modern-authentication-in-exchange-online) 

Para ativar a autenticação moderna para qualquer dispositivo que esteja a executar o Windows, que tenha o Microsoft Office 2013 instalado, terá de criar duas chaves de registo. Consulte [a autenticação moderna do Office 2013 em dispositivos Windows](/office365/admin/security-and-compliance/enable-modern-authentication).

#### <a name="is-there-a-policy-preventing-any-of-your-users-from-using-their-mobile-devices-while-working"></a>Existe uma política que impeça qualquer um dos seus utilizadores de utilizar os seus dispositivos móveis durante o trabalho?

É importante identificar qualquer política corporativa que impeça os colaboradores de usar dispositivos móveis durante o trabalho, pois irá influenciar a solução de autenticação multi-factor que implementa. Existem soluções, como a fornecida através da implementação de falhas de [segurança Azure AD,](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)que apenas permitem a utilização de uma aplicação autenticadora para verificação. Se a sua organização tiver uma política que impeça a utilização de dispositivos móveis, considere uma das seguintes opções:

- Implementar uma aplicação de senha de base única (TOTP) baseada no tempo que pode ser executada no sistema seguro

- Implementar uma solução de terceiros que aplique a autenticação de vários fatores para cada conta de utilizador no inquilino parceiro que fornece a opção de verificação mais adequada

- Comprar licenças [Azure Ative Directory Premium](https://azure.microsoft.com/pricing/details/active-directory/) para os utilizadores com impacto

#### <a name="what-automation-or-integration-do-you-have-to-leverage-user-credentials-for-authentication"></a>Que automatização ou integração tem para alavancar as credenciais do utilizador para a autenticação?

Uma vez que o requisito é fazer cumprir o MFA para cada utilizador, incluindo contas de serviço, no seu diretório de parceiros qualquer automatização ou integração que alavancar as credenciais de utilizadores para a autenticação será impactada. Por isso, é importante que identifique quais as contas que estão a ser utilizadas nestas situações. Consulte a seguinte lista de pedidos ou serviços de amostra a considerar:

- Painel de controlo utilizado para a prestação de recursos em nome dos seus clientes

- Integração com qualquer plataforma que seja usada para faturar (no que diz respeito ao programa CSP) e apoiar os seus clientes

- Scripts PowerShell que utilizam os módulos Az, AzureRM, Azure AD, MS Online, etc.

A lista acima não é abrangente. Por isso, é importante que realize uma avaliação completa de qualquer aplicação ou serviço no seu ambiente que aproveite as credenciais do utilizador para a autenticação. Para fazer face à exigência de autenticação de vários fatores, deve implementar sempre que possível a orientação no [quadro do Modelo de Aplicação Segura.](/partner-center/develop/enable-secure-app-model)

## <a name="accessing-your-environment"></a>Acedendo ao seu ambiente

Para melhor entender o que ou quem autentica sem ser desafiado para a autenticação de vários fatores, recomendamos que reveja a atividade de inscrição. Através do Azure Ative Directory Premium, pode aproveitar o relatório de inscrição. Para obter mais informações sobre este tópico, consulte os [relatórios de atividade de inscrição no portal Azure Ative Directory](/azure/active-directory/reports-monitoring/concept-sign-ins). Se não tiver o Azure Ative Directory Premium, ou estiver à procura de uma forma de obter esta atividade de entrada através do PowerShell, então terá de aproveitar o cmdlet [Get-PartnerUserSignActivity](/powershell/module/partnercenter/get-partnerusersigninactivity) do módulo [Partner Center PowerShell.](https://www.powershellgallery.com/packages/PartnerCenter/)

## <a name="how-the-requirements-are-enforced"></a>Como os requisitos são aplicados

Os requisitos de segurança dos parceiros são aplicados pela Azure Ative Directory e, por sua vez, pelo Partner Center, verificando a presença da alegação do MFA para identificar que a verificação de autenticação de vários fatores ocorreu. Iniciada a 18 de novembro de 2019, a Microsoft ativou salvaguardas de segurança adicionais (anteriormente conhecidas como "aplicação técnica") aos inquilinos parceiros.

Após a ativação, os utilizadores do inquilino parceiro serão solicitados a completar a verificação de autenticação multi-fator (MFA) quando efetuam qualquer administração em nome de operações (AOBO), acedendo ao portal partner Center ou chamando a API do Partner Center. Para obter mais informações detalhadas, consulte [a Autenticação De Vários Fatores (MFA) para o seu inquilino parceiro.](partner-security-requirements-mandating-mfa.md) 

Os parceiros que não cumpriram os requisitos devem aplicar estas medidas o mais rapidamente possível para evitar quaisquer perturbações nas empresas. 

Se estiver a utilizar a autenticação multi-factor Azure ou as falhas de segurança Azure AD, não existem ações adicionais que necessite de tomar.

se estiver a utilizar uma solução de autenticação multi-factor de terceiros, existe a possibilidade de a alegação de MFA não ser emitida. Se esta reclamação faltar, o Azure Ative Directory não poderá determinar se o pedido de autenticação foi contestado pela autenticação multi-factor. Para obter informações sobre como verificar a sua solução está a emitir a reclamação esperada, leia [testando os Requisitos de Segurança do Parceiro](/powershell/partnercenter/test-partner-security-requirements). 

> [!IMPORTANT]
> Se a sua solução de terceiros não emitir a reclamação esperada, então terá de trabalhar com o fornecedor que desenvolveu a solução para determinar que ações devem ser tomadas.

## <a name="resources-and-support"></a>Recursos e suporte

Consulte os seguintes recursos para suporte e código de amostra:

- [Comunidade do Grupo de Orientação de Segurança do Centro de Parceiros](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance): A comunidade do Grupo de Orientação de Segurança do Centro de Parceiros é uma comunidade online onde pode aprender sobre os próximos eventos e fazer quaisquer perguntas que possa ter.
- [Amostras do Centro Parceiro .NET](https://github.com/microsoft/partner-center-dotnet-samples): Este repositório GitHub contém amostras, desenvolvidas através do .NET, que demonstrarão como pode implementar a estrutura do Modelo de Aplicação Segura.
- [Amostras de Java do Centro Parceiro](https://github.com/microsoft/partner-center-java-samples): Este repositório GitHub contém amostras, desenvolvidas com recurso a Java, que demonstrarão como pode implementar a estrutura do Modelo de Aplicação Segura.
- [Partner Center PowerShell - Autenticação multi-factor](/powershell/partnercenter/multi-factor-auth): Este artigo de autenticação multi-factor fornece detalhes sobre como implementar a estrutura do Modelo de Aplicação Segura utilizando o PowerShell.