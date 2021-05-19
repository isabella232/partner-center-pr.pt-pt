---
title: Requisitos de segurança dos parceiros
ms.topic: article
ms.date: 10/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Introduz requisitos de segurança dos parceiros para permitir a autenticação multi-factor (MFA) e adotar o quadro do Modelo de Aplicação Segura.
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 201ea34d30814974936da032805f1ee7dfa590be
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110145852"
---
# <a name="security-requirements-for-using-partner-center-or-partner-center-apis"></a>Requisitos de segurança para a utilização de APIs do Partner Center ou do Partner Center

**Funções apropriadas**: Todos os utilizadores do Partner Center

Este artigo explica os requisitos de segurança obrigatórios para assessores, fornecedores de painéis de controlo e parceiros que participam no programa Cloud Solution Provider, bem como opções de autenticação e outras considerações de segurança. As salvaguardas de privacidade e a segurança estão entre as nossas principais prioridades. Sabemos que a melhor defesa é a prevenção e que somos tão fortes quanto o nosso elo mais fraco. É por isso que precisamos que todos os nossos ecossistemas atuem e garantam a proteção de segurança adequadas.

## <a name="mandatory-security-requirements"></a>Requisitos de segurança obrigatórios

Os parceiros que não implementarem os requisitos de segurança obrigatórios não poderão negociar no programa Cloud Solution Provider ou gerir os inquilinos dos clientes utilizando direitos de administração delegados. Além disso, os parceiros que não implementem os requisitos de segurança podem colocar a sua participação em programas em risco. Os termos associados aos requisitos de segurança do parceiro foram adicionados ao Acordo de Parceiros da Microsoft. No que diz respeito aos Consultores, os mesmos requisitos contratuais estarão em vigor.

Para protegê-lo e aos seus clientes, exigimos que os parceiros tomem as seguintes ações imediatamente:  

1. **Ativar a autenticação de vários fatores (MFA) para todas as contas do utilizador no seu inquilino parceiro.** Deve impor MFA em todas as contas de utilizador no seu(s) inquilino(s) parceiro. Os utilizadores devem ser desafiados pelo MFA quando iniciarem sação nos serviços de nuvem comercial da Microsoft ou quando transacionam no programa Cloud Solution Provider através do Partner Center ou através de APIs.

2. **Adotar o quadro do Modelo de Aplicação Segura**. Todos os parceiros que se integram com as APIs do Partner Center devem adotar o [quadro do Modelo de Aplicação Segura](/partner-center/develop/enable-secure-app-model) para qualquer aplicação e aplicações de modelos de utilizador.

    > [!IMPORTANT]
    > Recomendamos vivamente que os parceiros implementem o Modelo de Aplicação Segura para integração com uma API da Microsoft, como o Azure Resource Manager ou o Microsoft Graph, ou quando alavancam a automatização, como o PowerShell, utilizando credenciais de utilizador, para evitar qualquer perturbação quando o MFA é aplicado.

Estes requisitos de segurança ajudarão a proteger a sua infraestrutura e a proteger os dados dos seus clientes de potenciais riscos de segurança, tais como identificar roubos ou outros incidentes de fraude.  

## <a name="implementing-multi-factor-authentication"></a>Implementação da autenticação de vários fatores

Para cumprir os requisitos de segurança do parceiro, deve implementar e aplicar MFA para cada conta de utilizador no seu inquilino parceiro. Pode fazer isto de uma das seguintes formas:

- Implementar [o Azure Ative Directory (Azure AD) por defeitos de segurança](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults). Veja mais na [secção Local.](#security-defaults)

- Comprar Azure Ative Directory Premium para cada conta de utilizador. Para obter mais informações, consulte [Plan a Azure AD Multi-Factor Authentication deployment](/azure/active-directory/authentication/howto-mfa-getstarted).

- Utilize uma solução de terceiros para impor o MFA para cada conta de utilizador no seu inquilino parceiro. Para garantir que a solução fornecerá a solução esperada, veja [como os requisitos de segurança serão cumpridos.](#how-the-requirements-are-enforced)

> [!NOTE]
> Embora a autenticação multi-factor não seja contratualmente necessária para uma nuvem soberana (Governo dos EUA e Alemanha), é altamente recomendado que adote estes requisitos de segurança.

### <a name="security-defaults"></a>Predefinições de segurança

Uma das opções que os parceiros podem escolher para implementar os requisitos de MFA é permitir incumprimentos de segurança no Azure AD. Os incumprimentos de segurança oferecem um nível básico de segurança sem custos adicionais. Reveja como ativar o MFA para a sua organização com Azure AD e as principais considerações abaixo antes de permitir incumprimentos de segurança.

- Os parceiros que já adotaram políticas de base precisam de tomar medidas para a transição para incumprimentos de segurança.

- Os incumprimentos de segurança são a substituição geral da disponibilidade das políticas de base de pré-visualização. Uma vez que um parceiro permita os incumprimentos de segurança, eles deixarão de ser capazes de ativar políticas de base.

- Com os incumprimentos de segurança, todas as políticas serão ativadas de uma só vez.

- Para os parceiros que utilizam [acesso condicional,](/azure/active-directory/conditional-access/concept-conditional-access-policy-common) [não estarão disponíveis padrão de segurança](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults#disabling-security-defaults).

- Não bloqueamos a autenticação do legado neste momento. No entanto, como a maioria dos eventos relacionados com identidades comprometidas provém da tentativa de entrada em adoção, os parceiros são encorajados a afastarem-se destes protocolos mais antigos.

- A conta de sincronização Azure AD Connect está excluída de incumprimentos de segurança.

Para obter informações [detalhadas, leia a visão geral da Autenticação Multi-Factor AD Azure para a sua organização](/azure/active-directory/authentication/concept-mfa-get-started) e quais são os [padrão de segurança?](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)

> [!NOTE]
> O incumprimento de segurança Azure AD é a evolução das políticas de proteção de base simplificadas. Se já ativou as políticas de proteção de base, é altamente recomendável que ative [as falhas de segurança](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults).

## <a name="implementation-considerations"></a>Considerações de implementação

Como estes requisitos se aplicam a todas as contas de utilizador no seu inquilino parceiro, você precisa considerar várias coisas para garantir uma implementação suave. Por exemplo, identifique as contas de utilizadores em Azure AD que não podem realizar MFA, e aplicações e dispositivos na sua organização que não suportam a autenticação moderna.

Antes de realizar qualquer ação, recomendamos que preencha as seguintes validações. 

#### <a name="do-you-have-an-application-or-device-that-does-not-support-the-use-of-modern-authentication"></a>Possui uma aplicação ou dispositivo que não suporte ao uso da autenticação moderna?

Quando executa o MFA, a autenticação legacy usa protocolos como IMAP, POP3, SMTP e outros serão bloqueados porque não suportam MFA. Para resolver esta limitação, utilize a funcionalidade [de palavras-passe](/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords) da aplicação para garantir que a aplicação ou dispositivo continuará a autenticar. Reveja as [considerações para usar as palavras-passe da aplicação](/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords) para determinar se podem ser usadas no seu ambiente.

#### <a name="do-you-have-office-365-users-with-licenses-associated-with-your-partner-tenant"></a>Tem utilizadores do Office 365 com licenças associadas ao seu inquilino parceiro?

Antes de implementar qualquer solução, recomendamos que determine quais versões dos utilizadores do Microsoft Office no seu inquilino parceiro estão a usar. Existe a possibilidade de os seus utilizadores experimentarem problemas de conectividade com aplicações como o Outlook. Antes de impor o MFA, é importante garantir que está a utilizar o Outlook 2013 SP1, ou mais tarde, e que a sua organização tem a autenticação moderna ativada. Para mais informações, consulte [Ative a autenticação moderna em Exchange Online.](/exchange/clients-and-mobile-in-exchange-online/enable-or-disable-modern-authentication-in-exchange-online) 

Para permitir a autenticação moderna para dispositivos que executam o Windows que tenham o Microsoft Office 2013 instalado, terá de criar duas chaves de registo. Consulte [a autenticação moderna do Office 2013 em dispositivos Windows](/office365/admin/security-and-compliance/enable-modern-authentication).

#### <a name="is-there-a-policy-preventing-any-of-your-users-from-using-their-mobile-devices-while-working"></a>Existe uma política que impeça qualquer um dos seus utilizadores de utilizar os seus dispositivos móveis durante o trabalho?

É importante identificar qualquer política corporativa que impeça os colaboradores de usar dispositivos móveis durante o trabalho porque irá influenciar a solução MFA que implementa. Existem soluções, como a fornecida através da implementação de falhas de [segurança Azure AD,](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)que apenas permitem a utilização de uma aplicação autenticadora para verificação. Se a sua organização tiver uma política que impeça a utilização de dispositivos móveis, considere uma das seguintes opções:

- Implemente uma aplicação de senha de base única (TOTP) baseada no tempo que pode ser executada no sistema seguro.

- Implementar uma solução de terceiros que aplique MFA para cada conta de utilizador no inquilino parceiro que fornece a opção de verificação mais adequada.

- Compre licenças [Azure Ative Directory Premium](https://azure.microsoft.com/pricing/details/active-directory/) para os utilizadores afetados.

#### <a name="what-automation-or-integration-do-you-have-to-leverage-user-credentials-for-authentication"></a>Que automatização ou integração tem para alavancar as credenciais do utilizador para a autenticação?

Como aplicamos o MFA a cada utilizador, incluindo contas de serviço, no seu diretório de parceiros, isso afetará qualquer automatização ou integração que utilize credenciais de utilizador para autenticação. Por isso, é importante que identifique quais as contas que estão a ser utilizadas nestas situações. Consulte a seguinte lista de pedidos ou serviços de amostra a considerar:

- Painel de controlo utilizado para a prestação de recursos em nome dos seus clientes

- Integração com qualquer plataforma que seja usada para faturar (no que diz respeito ao programa CSP) e apoiar os seus clientes

- Scripts PowerShell que usam os módulos Az, AzureRM, Azure AD, MS Online e outros módulos

A lista acima não é abrangente. Por isso, é importante que efetue uma avaliação completa de qualquer aplicação ou serviço no seu ambiente que utilize credenciais de utilizador para autenticação. Para fazer face à exigência de MFA, deve implementar sempre que possível a orientação no [quadro do Modelo de Aplicação Segura.](/partner-center/develop/enable-secure-app-model)

## <a name="accessing-your-environment"></a>Acedendo ao seu ambiente

Para melhor entender o que ou quem autentica sem ser desafiado para MFA, recomendamos que reveja a atividade de inscrição. Através do Azure Ative Directory Premium, pode utilizar o relatório de inscrição. Para obter mais informações sobre este assunto, consulte [relatórios de atividades de inscrição no portal Azure Ative Directory](/azure/active-directory/reports-monitoring/concept-sign-ins). Se não tiver o Azure Ative Directory Premium, ou se estiver à procura de uma forma de obter esta atividade de entrada através do PowerShell, então terá de utilizar o cmdlet [Get-PartnerUserSignActivity](/powershell/module/partnercenter/get-partnerusersigninactivity) do módulo [Partner Center PowerShell.](https://www.powershellgallery.com/packages/PartnerCenter/)

## <a name="how-the-requirements-are-enforced"></a>Como os requisitos são aplicados

Os requisitos de segurança dos parceiros são aplicados pela Azure AD e, por sua vez, o Partner Center, verificando a presença da alegação do MFA para identificar que a verificação do MFA foi realizada. A partir de 18 de novembro de 2019, a Microsoft ativou salvaguardas de segurança adicionais (anteriormente conhecidas como "execução técnica") aos inquilinos parceiros.

Após a ativação, os utilizadores do inquilino parceiro são solicitados a completar a verificação do MFA ao realizar qualquer administração em nome das operações (AOBO), acedendo ao portal Partner Center ou chamando APIs do Partner Center. Para obter mais informações, consulte [a Autenticação De Vários Fatores (MFA) para o seu inquilino parceiro.](partner-security-requirements-mandating-mfa.md) 

Os parceiros que não cumpriram os requisitos devem aplicar estas medidas o mais rapidamente possível para evitar quaisquer perturbações nas empresas. Se estiver a utilizar o Azure Ative Directory Multi-Factor Authentication ou os padrãos de segurança Azure AD, não existem ações adicionais que necessite de tomar.

Se estiver a utilizar uma solução de MFA de terceiros, existe a possibilidade de a reclamação do MFA não ser emitida. Se esta reclamação faltar, a Azure AD não poderá determinar se o pedido de autenticação foi contestado pela MFA. Para obter informações sobre como verificar a sua solução está a emitir a reclamação esperada, leia [testando os Requisitos de Segurança do Parceiro](/powershell/partnercenter/test-partner-security-requirements). 

> [!IMPORTANT]
> Se a sua solução de terceiros não emitir a reclamação esperada, então terá de trabalhar com o fornecedor que desenvolveu a solução para determinar que ações devem ser tomadas.

## <a name="resources-and-samples"></a>Recursos e amostras

Consulte os seguintes recursos para suporte e código de amostra:

- [Comunidade do Grupo de Orientação de Segurança do Centro de Parceiros](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance): A comunidade do Grupo de Orientação de Segurança do Centro de Parceiros é uma comunidade online onde pode aprender sobre os próximos eventos e fazer quaisquer perguntas que possa ter.
- [Amostras do Centro Parceiro .NET](https://github.com/microsoft/partner-center-dotnet-samples): Este repositório GitHub contém amostras, desenvolvidas através do .NET, que demonstrarão como pode implementar a estrutura do Modelo de Aplicação Segura.
- [Amostras de Java do Centro Parceiro](https://github.com/microsoft/partner-center-java-samples): Este repositório GitHub contém amostras, desenvolvidas com recurso a Java, que demonstrarão como pode implementar a estrutura do Modelo de Aplicação Segura.
- [Partner Center PowerShell - Autenticação multi-factor](/powershell/partnercenter/multi-factor-auth): Este artigo de autenticação multi-factor fornece detalhes sobre como implementar a estrutura do Modelo de Aplicação Segura utilizando o PowerShell.

## <a name="next-steps"></a>Passos seguintes

- [Mandatar autenticação multi-factor (MFA) para o seu inquilino parceiro](partner-security-requirements-mandating-mfa.md)