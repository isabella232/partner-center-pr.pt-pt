---
title: Aplicação da amostra
ms.topic: article
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Utilize a aplicação da amostra para construir a sua própria aplicação para aceder programaticamente aos dados de insights dos parceiros.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.openlocfilehash: 6f334b9047c38e8b7763a4ba96d21d987c252682
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376944"
---
# <a name="sample-application"></a><span data-ttu-id="818f9-103">Aplicação da amostra</span><span class="sxs-lookup"><span data-stu-id="818f9-103">Sample Application</span></span>

<span data-ttu-id="818f9-104">As aplicações da amostra são criadas em línguas C# e JAVA e estão disponíveis em [GitHub](https://github.com/partneranalytics)</span><span class="sxs-lookup"><span data-stu-id="818f9-104">Sample applications are created in C# and JAVA languages and are available on [GitHub](https://github.com/partneranalytics)</span></span>

- [<span data-ttu-id="818f9-105">C# Aplicação da amostra</span><span class="sxs-lookup"><span data-stu-id="818f9-105">C# Sample Application</span></span>](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN)
- [<span data-ttu-id="818f9-106">Aplicação da amostra JAVA</span><span class="sxs-lookup"><span data-stu-id="818f9-106">JAVA Sample Application</span></span>](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java)

<span data-ttu-id="818f9-107">Pode optar por inspirar-se na aplicação da amostra e construir a sua própria aplicação em qualquer idioma.</span><span class="sxs-lookup"><span data-stu-id="818f9-107">You can choose to take inspiration from the sample application and build your own application in any language.</span></span>

<span data-ttu-id="818f9-108">A aplicação da amostra alcança os seguintes objetivos:</span><span class="sxs-lookup"><span data-stu-id="818f9-108">The sample application achieves the following objectives:</span></span>

- <span data-ttu-id="818f9-109">Gera um token de Azure Ative Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="818f9-109">Generates an Azure Active Directory (Azure AD) Token.</span></span>
- <span data-ttu-id="818f9-110">Obtém conjuntos de dados disponíveis.</span><span class="sxs-lookup"><span data-stu-id="818f9-110">Gets available datasets.</span></span>
- <span data-ttu-id="818f9-111">Cria consultas definidas pelo utilizador.</span><span class="sxs-lookup"><span data-stu-id="818f9-111">Creates user defined queries.</span></span>
- <span data-ttu-id="818f9-112">Obtém consultas definidas pelo utilizador e sistema.</span><span class="sxs-lookup"><span data-stu-id="818f9-112">Gets user defined and system queries.</span></span>
- <span data-ttu-id="818f9-113">Marca um relatório.</span><span class="sxs-lookup"><span data-stu-id="818f9-113">Schedules a report.</span></span>

<span data-ttu-id="818f9-114">A aplicação da amostra não cobre o método de chamar APIs para outras funcionalidades.</span><span class="sxs-lookup"><span data-stu-id="818f9-114">The sample application doesn't cover the method of calling APIs for other functionalities.</span></span> <span data-ttu-id="818f9-115">No entanto, o processo de chamar outras APIs permanece o mesmo que acima descrito.</span><span class="sxs-lookup"><span data-stu-id="818f9-115">However, the process of calling other APIs remains the same as outlined above.</span></span>

## <a name="how-to-run-the-application"></a><span data-ttu-id="818f9-116">Como executar a aplicação</span><span class="sxs-lookup"><span data-stu-id="818f9-116">How to run the application</span></span>

- <span data-ttu-id="818f9-117">Clone o repositório para um sistema local usando este comando:</span><span class="sxs-lookup"><span data-stu-id="818f9-117">Clone the repository to a local system using this command:</span></span>

```cli
git clone https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN.git
```

> [!Note]
> <span data-ttu-id="818f9-118">Para obter mais instruções, consulte o ficheiro ProgrammaticExportSampleAppMPN/README.md no [repositório](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java)GitHub .</span><span class="sxs-lookup"><span data-stu-id="818f9-118">For more instructions, refer to the ProgrammaticExportSampleAppMPN/README.md file in the GitHub [repository](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java).</span></span>

- <span data-ttu-id="818f9-119">Para executar rapidamente a aplicação, atualize o id do cliente e o segredo do cliente no **appsettings.Development.jsem**</span><span class="sxs-lookup"><span data-stu-id="818f9-119">To quickly run the app, update the client id and client secret in the **appsettings.Development.json**</span></span>

:::image type="content" source="images/insights/prog-acc-appsetting-development.png" alt-text="Ilustrando o json de desenvolvimento de appsetting":::

<span data-ttu-id="818f9-121">A execução da aplicação iniciará um servidor web local e uma página será aberta ( `https://localhost:44365/ProgrammaticExportSampleApp/sample` ).</span><span class="sxs-lookup"><span data-stu-id="818f9-121">Running the app will start a local web server and a page will open (`https://localhost:44365/ProgrammaticExportSampleApp/sample`).</span></span>
  
:::image type="content" source="images/insights/prog-acc-sample-application.png" alt-text="Ilustração da UI da aplicação da amostra":::

<span data-ttu-id="818f9-123">Esta página fará chamadas de API para o webserver que está a funcionar na máquina local, o que por sua vez fará as chamadas de acesso programático real API.</span><span class="sxs-lookup"><span data-stu-id="818f9-123">This page will make API calls to the webserver running on the local machine, which in turn will make the actual programmatic access API calls.</span></span>

## <a name="code-snippets"></a><span data-ttu-id="818f9-124">Fragmentos de Código</span><span class="sxs-lookup"><span data-stu-id="818f9-124">Code Snippets</span></span>

<span data-ttu-id="818f9-125">A estrutura básica do código C# para fazer as chamadas de API de acesso programático é a seguinte:</span><span class="sxs-lookup"><span data-stu-id="818f9-125">The basic structure of the C# code for doing the programmatic access API calls is as follows:</span></span>
 
:::image type="content" source="images/insights/prog-acc-code-snippet.png" alt-text="Corte de código ilustrando":::

## <a name="next-steps"></a><span data-ttu-id="818f9-127">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="818f9-127">Next steps</span></span>

[<span data-ttu-id="818f9-128">APIs para aceder a dados de análise de insights de parceiros</span><span class="sxs-lookup"><span data-stu-id="818f9-128">APIs for accessing partner insights analytics data</span></span>](insights-programmatic-analytics-available-api.md)
