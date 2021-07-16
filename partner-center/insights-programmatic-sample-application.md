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
# <a name="sample-application"></a>Aplicação da amostra

As aplicações da amostra são criadas em línguas C# e JAVA e estão disponíveis em [GitHub](https://github.com/partneranalytics)

- [C# Aplicação da amostra](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN)
- [Aplicação da amostra JAVA](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java)

Pode optar por inspirar-se na aplicação da amostra e construir a sua própria aplicação em qualquer idioma.

A aplicação da amostra alcança os seguintes objetivos:

- Gera um token de Azure Ative Directory (Azure AD).
- Obtém conjuntos de dados disponíveis.
- Cria consultas definidas pelo utilizador.
- Obtém consultas definidas pelo utilizador e sistema.
- Marca um relatório.

A aplicação da amostra não cobre o método de chamar APIs para outras funcionalidades. No entanto, o processo de chamar outras APIs permanece o mesmo que acima descrito.

## <a name="how-to-run-the-application"></a>Como executar a aplicação

- Clone o repositório para um sistema local usando este comando:

```cli
git clone https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN.git
```

> [!Note]
> Para obter mais instruções, consulte o ficheiro ProgrammaticExportSampleAppMPN/README.md no [repositório](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java)GitHub .

- Para executar rapidamente a aplicação, atualize o id do cliente e o segredo do cliente no **appsettings.Development.jsem**

:::image type="content" source="images/insights/prog-acc-appsetting-development.png" alt-text="Ilustrando o json de desenvolvimento de appsetting":::

A execução da aplicação iniciará um servidor web local e uma página será aberta ( `https://localhost:44365/ProgrammaticExportSampleApp/sample` ).
  
:::image type="content" source="images/insights/prog-acc-sample-application.png" alt-text="Ilustração da UI da aplicação da amostra":::

Esta página fará chamadas de API para o webserver que está a funcionar na máquina local, o que por sua vez fará as chamadas de acesso programático real API.

## <a name="code-snippets"></a>Fragmentos de Código

A estrutura básica do código C# para fazer as chamadas de API de acesso programático é a seguinte:
 
:::image type="content" source="images/insights/prog-acc-code-snippet.png" alt-text="Corte de código ilustrando":::

## <a name="next-steps"></a>Passos seguintes

[APIs para aceder a dados de análise de insights de parceiros](insights-programmatic-analytics-available-api.md)
