---
title: Pré-requisitos para aceder programaticamente a dados de análise
description: Pré-requisitos para aceder programaticamente a dados de análise
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: d4c39025aa3804435dd4d2359b93cd4a2e13ccc4
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376951"
---
# <a name="prerequisites-to-programmatically-access-analytics-data"></a>Pré-requisitos para aceder programaticamente a dados de análise

**Funções adequadas:** Administração global | Administrador da MPN

Antes de poder aceder programáticamente aos dados de análise de insights de parceiros, tem de cumprir os seguintes requisitos.

## <a name="mpn-program-enrollment"></a>Inscrição no Programa MPN

Para aceder a informações de análise de parceiros programáticamente, precisa de estar inscrito no programa MPN e ter uma conta Partner Center. Para saber como, consulte [Criar uma conta MPN no Partner Center](mpn-create-a-partner-center-account.md)

## <a name="create-azure-active-directory-aad-application"></a>Criar Azure Ative Directory (aplicação AAD)

As credenciais regulares do utilizador não podem ser utilizadas para o acesso programático de dados partner Informações Analytics. Uma aplicação Azure Ative Directory (AAD) precisa de ser criada juntamente com uma aplicação secreta (aplicação + acesso ao utilizador) para aceder às APIs de acesso programático. Para aprender a criar uma aplicação AAD e segredo, consulte [Quickstart: Registe uma aplicação com o plataforma de identidades da Microsoft.](/azure/active-directory/develop/quickstart-register-app)   A permissão é necessária para aceder à Microsoft Partner API. Para aprender a adicionar permissão, consulte a [autenticação da API do Parceiro - Partner](/partner/develop/api-authentication#application-and-user-access)

## <a name="assign-executive-report-viewer-erv-role-to-the-user"></a>Atribuir papel de Visualizador de Relatório Executivo (ERV) ao utilizador

Para aceder a insights de parceiros analíticos dados programáticamente, você deve ter O Espectador de Relatório Executivo (ERV). Para aprender a atribuir o papel ERV ao utilizador, consulte [o Partner Center Informações acesso baseado em funções - Partner Center](insights-roles.md)

## <a name="generate-an-aad-token"></a>Gerar um token AAD

Precisa gerar um token AAD utilizando o ID da Aplicação (cliente), segredo do cliente, iD do utilizador e senha.   [Consulte aqui](insights-programmatic-first-api-call.md#token-generation) os passos para gerar o token AAD.

> [!Note]
> O sinal é válido por uma hora.

## <a name="next-steps"></a>Passos seguintes
[Paradigma de acesso programático](insights-programmatic-access-paradigm.md)