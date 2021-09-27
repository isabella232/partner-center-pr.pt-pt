---
title: Pré-requisitos para aceder programaticamente a dados de análise
description: Pré-requisitos para aceder programaticamente a dados de análise
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: 9359cb25fee113ee166c7ce407ed70f319f3e6b6
ms.sourcegitcommit: d731813da1d31519dc2dc583d17899e5cf4ec1b2
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/27/2021
ms.locfileid: "129071090"
---
# <a name="prerequisites-to-programmatically-access-analytics-data"></a>Pré-requisitos para aceder programaticamente a dados de análise

**Funções adequadas:** | de administração global Administrador da MPN

Antes de poder aceder programáticamente aos dados de análise de insights de parceiros, tem de cumprir os seguintes requisitos.

## <a name="mpn-program-enrollment"></a>Inscrição no Programa MPN

Para aceder a informações de análise de parceiros programáticamente, precisa de estar inscrito no programa MPN e ter uma conta Partner Center. Para saber como, consulte [Criar uma conta MPN no Partner Center](mpn-create-a-partner-center-account.md)

## <a name="create-azure-active-directory-aad-application"></a>Criar Azure Ative Directory (aplicação AAD)

As credenciais regulares do utilizador não podem ser utilizadas para o acesso programático de dados partner Informações Analytics. Uma aplicação Azure Ative Directory (AAD) precisa de ser criada juntamente com um segredo (aplicação + acesso ao utilizador) para aceder às APIs de acesso programático. Para aprender a criar uma aplicação AAD e segredo, consulte [Quickstart: Registe uma aplicação com o plataforma de identidades da Microsoft.](/azure/active-directory/develop/quickstart-register-app)   A permissão é necessária para aceder à Microsoft Partner API. Para aprender a adicionar permissão, consulte a [autenticação da API do Parceiro - Partner](/partner/develop/api-authentication#application-and-user-access)

## <a name="assign-executive-report-viewer-erv-role-to-the-user"></a>Atribuir papel de Visualizador de Relatório Executivo (ERV) ao utilizador

Para aceder a informações de análise de parceiros programáticamente, deverá ter o Visualizador de Relatório Executivo (ERV). Para aprender a atribuir a função ERV ao utilizador, consulte [o Partner Center Informações acesso baseado em funções - Partner Center](insights-roles.md)

## <a name="generate-an-aad-token"></a>Gerar um token AAD

Precisa gerar um token AAD utilizando o ID da Aplicação (cliente), segredo do cliente, iD do utilizador e senha.   [Consulte aqui](insights-programmatic-first-api-call.md#token-generation) os passos para gerar token AAD.

> [!Note]
> O sinal é válido por uma hora.

## <a name="next-steps"></a>Passos seguintes
[Paradigma de acesso programático](insights-programmatic-access-paradigm.md)