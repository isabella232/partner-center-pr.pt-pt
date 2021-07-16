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
# <a name="prerequisites-to-programmatically-access-analytics-data"></a><span data-ttu-id="83beb-103">Pré-requisitos para aceder programaticamente a dados de análise</span><span class="sxs-lookup"><span data-stu-id="83beb-103">Prerequisites to programmatically access analytics data</span></span>

<span data-ttu-id="83beb-104">**Funções adequadas:** Administração global | Administrador da MPN</span><span class="sxs-lookup"><span data-stu-id="83beb-104">**Appropriate roles:** Global admin | MPN admin</span></span>

<span data-ttu-id="83beb-105">Antes de poder aceder programáticamente aos dados de análise de insights de parceiros, tem de cumprir os seguintes requisitos.</span><span class="sxs-lookup"><span data-stu-id="83beb-105">Before you can programmatically access partner insights analytics data, you need to meet the following requirements.</span></span>

## <a name="mpn-program-enrollment"></a><span data-ttu-id="83beb-106">Inscrição no Programa MPN</span><span class="sxs-lookup"><span data-stu-id="83beb-106">MPN Program enrollment</span></span>

<span data-ttu-id="83beb-107">Para aceder a informações de análise de parceiros programáticamente, precisa de estar inscrito no programa MPN e ter uma conta Partner Center.</span><span class="sxs-lookup"><span data-stu-id="83beb-107">To access partner insights analytics data programmatically, you need to be enrolled in the MPN program and have a Partner Center account.</span></span> <span data-ttu-id="83beb-108">Para saber como, consulte [Criar uma conta MPN no Partner Center](mpn-create-a-partner-center-account.md)</span><span class="sxs-lookup"><span data-stu-id="83beb-108">To learn how, see [Create an MPN account in Partner Center](mpn-create-a-partner-center-account.md)</span></span>

## <a name="create-azure-active-directory-aad-application"></a><span data-ttu-id="83beb-109">Criar Azure Ative Directory (aplicação AAD)</span><span class="sxs-lookup"><span data-stu-id="83beb-109">Create Azure Active Directory (AAD) application</span></span>

<span data-ttu-id="83beb-110">As credenciais regulares do utilizador não podem ser utilizadas para o acesso programático de dados partner Informações Analytics.</span><span class="sxs-lookup"><span data-stu-id="83beb-110">Regular user credentials cannot be used for programmatic access of Partner Insights Analytics data.</span></span> <span data-ttu-id="83beb-111">Uma aplicação Azure Ative Directory (AAD) precisa de ser criada juntamente com uma aplicação secreta (aplicação + acesso ao utilizador) para aceder às APIs de acesso programático.</span><span class="sxs-lookup"><span data-stu-id="83beb-111">An Azure Active Directory (AAD) application needs to be created along with a secret (application + user access) to access the programmatic access APIs.</span></span> <span data-ttu-id="83beb-112">Para aprender a criar uma aplicação AAD e segredo, consulte [Quickstart: Registe uma aplicação com o plataforma de identidades da Microsoft.](/azure/active-directory/develop/quickstart-register-app)   A permissão é necessária para aceder à Microsoft Partner API.</span><span class="sxs-lookup"><span data-stu-id="83beb-112">To learn how to create an AAD application and secret, see [Quickstart: Register an application with the Microsoft identity platform.](/azure/active-directory/develop/quickstart-register-app) Permission is required to access Microsoft Partner API.</span></span> <span data-ttu-id="83beb-113">Para aprender a adicionar permissão, consulte a [autenticação da API do Parceiro - Partner](/partner/develop/api-authentication#application-and-user-access)</span><span class="sxs-lookup"><span data-stu-id="83beb-113">To learn how to add permission, see [Partner API authentication - Partner](/partner/develop/api-authentication#application-and-user-access)</span></span>

## <a name="assign-executive-report-viewer-erv-role-to-the-user"></a><span data-ttu-id="83beb-114">Atribuir papel de Visualizador de Relatório Executivo (ERV) ao utilizador</span><span class="sxs-lookup"><span data-stu-id="83beb-114">Assign Executive Report Viewer (ERV) role to the user</span></span>

<span data-ttu-id="83beb-115">Para aceder a insights de parceiros analíticos dados programáticamente, você deve ter O Espectador de Relatório Executivo (ERV).</span><span class="sxs-lookup"><span data-stu-id="83beb-115">To access partner insights analytics data programmatically, you should have Executive Report Viewer (ERV).</span></span> <span data-ttu-id="83beb-116">Para aprender a atribuir o papel ERV ao utilizador, consulte [o Partner Center Informações acesso baseado em funções - Partner Center](insights-roles.md)</span><span class="sxs-lookup"><span data-stu-id="83beb-116">To learn how to assign ERV role to the user, see [Partner Center Insights role-based access - Partner Center](insights-roles.md)</span></span>

## <a name="generate-an-aad-token"></a><span data-ttu-id="83beb-117">Gerar um token AAD</span><span class="sxs-lookup"><span data-stu-id="83beb-117">Generate an AAD token</span></span>

<span data-ttu-id="83beb-118">Precisa gerar um token AAD utilizando o ID da Aplicação (cliente), segredo do cliente, iD do utilizador e senha.   [Consulte aqui](insights-programmatic-first-api-call.md#token-generation) os passos para gerar o token AAD.</span><span class="sxs-lookup"><span data-stu-id="83beb-118">You need to Generate an AAD token using the Application (client) ID, client secret, your user ID and password.  [Check here](insights-programmatic-first-api-call.md#token-generation) for steps to generate AAD token.</span></span>

> [!Note]
> <span data-ttu-id="83beb-119">O sinal é válido por uma hora.</span><span class="sxs-lookup"><span data-stu-id="83beb-119">The token is valid for one hour.</span></span>

## <a name="next-steps"></a><span data-ttu-id="83beb-120">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="83beb-120">Next steps</span></span>
[<span data-ttu-id="83beb-121">Paradigma de acesso programático</span><span class="sxs-lookup"><span data-stu-id="83beb-121">Programmatic access paradigm</span></span>](insights-programmatic-access-paradigm.md)