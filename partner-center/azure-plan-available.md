---
title: Available Azure services in Azure CSP (Serviços do Azure disponíveis no Azure CSP)
description: Este artigo discute os serviços Azure que estão e não estão disponíveis no programa Azure Fornecedor de Soluções em Nuvem (CSP).
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
author: amitravat
ms.author: amrava
ms.localizationpriority: high
ms.date: 05/13/2020
ms.custom: SEOMAY.20
ms.openlocfilehash: 6037044a72bd9bd71131ddbc66fec0555bbd5f86
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/09/2021
ms.locfileid: "123961219"
---
# <a name="azure-services-available-in-the-azure-cloud-solution-provider-csp-program"></a>Serviços Azure disponíveis no programa Azure Fornecedor de Soluções em Nuvem (CSP)

**Funções adequadas**: Agente administrador | Administrador de faturação | Administração global | Agente helpdesk | Agente comercial | Administração de gestão de utilizadores

## <a name="available-azure-services-in-azure-csp"></a>Available Azure services in Azure CSP (Serviços do Azure disponíveis no Azure CSP)

Este artigo lista os serviços Azure que estão e não estão disponíveis no programa Azure Fornecedor de Soluções em Nuvem (CSP). Aborda também a disponibilidade de serviços nas nuvens nacionais [Microsoft Azure a Alemanha](https://azure.microsoft.com/overview/clouds/germany/) e Microsoft Azure [Governo.](https://azure.microsoft.com/overview/clouds/government/)

>[!Note]
> [A Azure China](https://www.azure.cn/) não está disponível no programa Azure CSP.

## <a name="global-cloud"></a>Nuvem Global

Todos os serviços baseados no modelo Azure Resource Manager estão disponíveis no Programa CSP.  Os serviços de Gestor de Recursos Não-Azure, como os serviços de modelos de implantação clássicos, não estão disponíveis no programa CSP.  

## <a name="csp-specific-service-configurations"></a>Configurações de serviço CSP-Specific

Os seguintes serviços requerem configurações especiais em CSP:

- [StorSimple](/azure/storsimple/storsimple-partner-csp-overview)

- [Azure Active Directory Domain Services](/azure/active-directory-domain-services/active-directory-ds-csp)

- [Cofre de Chaves](https://azurecsp.blob.core.windows.net/files/key-vault-in-csp.docx)

- [Azure Time Series Informações](https://azure.microsoft.com/services/time-series-insights/) Apenas os utilizadores do inquilino do cliente podem aceder aos dados no seu ambiente de Informações Séries Tempotárias. Os parceiros podem gerir o ambiente de Informações time series dos seus clientes por padrão, mas se precisarem de acesso aos dados nele, devem ser adicionados ao cliente.

- Os certificados de gestão para autenticação de bibliotecas Azure SDK através de certificado não são suportados no modelo CSP.  Utilize a autenticação principal do serviço Azure e a biblioteca Azure.Identity.  Autenticação de referência [com o Azure SDK para .NET](/dotnet/azure/sdk/authentication)

## <a name="visual-studio-marketplace"></a>Visual Studio Marketplace

Pode agora adquirir os itens listados abaixo Visual Studio Marketplace, com exceção das extensões de terceiros.

- [Azure DevOps](https://www.visualstudio.com/team-services/)

- [Subscrições do Visual Studio](https://www.visualstudio.com/subscriptions/)

- [Formação da Universidade de Xamarin](https://marketplace.visualstudio.com/items?itemName=ms.xamarin-university)

Para ajudá-lo a começar, criámos vídeos e documentação sobre [como configurar, comprar e gerir a Azure DevOps](/vsts/billing/csp/set-up-csp-customer) em CSP.

## <a name="azure-marketplace-items-in-azure-csp"></a>Azure Marketplace items in Azure CSP (Itens do Azure Marketplace no Azure  CSP)

Nem todos os itens do Azure Marketplace estão atualmente disponíveis nas subscrições do Azure CSP.

- Serviços Azure baseados na Microsoft: Estes serviços estão disponíveis. Reveja a tabela anterior e os comentários.

- Traga a sua própria licença (BYOL) itens: Estes itens estão disponíveis. Uma lista completa de itens Azure Marketplace ativados pela BYOL está disponível na [página Azure Marketplace BYOL](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol).

- Pay-As-You-Go Itens Azure Marketplace de terceiros: Estes itens estão disponíveis se o fornecedor tiver publicado no canal CSP. Para mais informações, consulte [venda de subscrições de produtos Azure Marketplace.](csp-commercial-marketplace-overview.md)

- Citrix XenApp Essentials: Os parceiros podem adquirir o XenApp Essentials para clientes em CSP. Para mais informações, consulte o seguinte blog Citrix- [Distribuição do XenApp Essentials já disponível através do Fornecedor de Soluções em Nuvem da Microsoft Channel](https://www.citrix.com/blogs/2018/02/01/xenapp-essentials-now-available-through-microsoft-cloud-solution-provider-channel/).

## <a name="national-clouds"></a>Clouds nacionais

A tabela que se segue apresenta uma lista regularmente atualizada dos produtos, serviços e funcionalidades disponíveis da Azure de primeira parte nas nuvens nacionais.

| Produto, serviço ou recurso Azure | Governo dos Estados Unidos | Alemanha |
| ------ | :-----------: | :-----------: |
|  **Computação**  |    |    |
|  Máquinas Virtuais  |  X  |  X  |
|  Serviços Cloud  |    |    |
|  Conjuntos de dimensionamento de máquinas virtuais  |  X  |  X  |
|  Funções  |    |    |
|  Azure Container Service  |    |    |
|  **Redes**  |    |    |
|  DNS do Azure  |    |    |
|  Rede de Entrega de Conteúdos  |    |    |
|  Gestor de Tráfego  |    |    |
|  ExpressRoute  |  X  |  X  |
|  Rede Virtual  |  X  |  X  |
|  Balanceador de Carga  |  X  |  X  |
|  Gateway de VPN  |  X  |  X  |
|  Gateway de Aplicação  |  X  |  X  |
|  Observador de Rede  |  X  |  X  |
|  **Armazenamento**  |    |    |
|  Armazenamento  |  X  |  X  |
|  Backup  |  X  |  X  |
|  StorSimple  |    |  X  |
|  Recuperação de sites  |  X  |  X  |
|  Data Lake Storage  |    |    |
|  Managed Disks  |  X  |  X  |
|  **Web + Mobile**  |    |    |
|  Serviço de Aplicações  |  X  |  X  |
|  Serviço de Aplicações no Linux  |    |  X  |
|  Gestão de API  |  X  |    |
|  Rede de Entrega de Conteúdos  |    |    |
|  Serviços de Multimédia  |  X  |  X  |
|  Hubs de Notificação  |  X  |  X  |
|  Azure Search  |    |    |
|  Funcionalidade de Apps lógicas do Azure App Service  |    |    |
|  **Contentores**  |    |    |
|  Serviço de Aplicações  |  X  |  X  |
|  Serviço de Aplicações no Linux  |    |  X  |
|  Batch  |  X  |  X  |
|  Container Registry  |    |    |
|  Container Instances  |    |    |
|  Service Fabric  |  X  |  X  |
|  Serviço de Contentor  |    |    |
|  **Bases de dados**  |    |    |
|  Base de Dados SQL  |  X  |  X  |
|  Azure Cosmos DB  |  X  |  X  |
|  SQL Data Warehouse  |  X  |  X  |
|  Cache de Redis  |  X  |  X  |
|  SQL Server Stretch Database  |  X  |  X  |
|  Base de Dados do Azure para MySQL  |    |    |
|  Base de Dados do Azure para PostgreSQL  |    |    |
|  **Dados + Análise**  |    |    |
|  Databricks  |    |    |
|  HDInsight  |  X  |  X  |
|  Stream Analytics  |    |  X  |
|  Data Factory  |    |    |
|  Log Analytics  |  X  |    |
|  Catálogo de Dados  |    |    |
|  Data Lake Storage  |    |    |
|  Data Lake Analytics  |    |    |
|  Azure Analysis Services  |    |    |
|  Power BI Embedded  |    |    |
|  **AI + Serviços Cognitivos**  |    |    |
|  Machine Learning  |    |  X  |
|  Azure Bot Service  |    |    |
|  Serviços Cognitivos  |    |    |
|  IA do Azure Batch  |    |    |
|  **Internet das Coisas**  |    |    |
|  IoT Hub  |  X  |  X  |
|  IoT Central  |    |    |
|  Machine Learning  |    |  X  |
|  Stream Analytics  |    |  X  |
|  Hubs de Eventos  |  X  |  X  |
|  Serviços Location-Based  |    |    |
|  Hubs de Notificação  |  X  |  X  |
|  Time Series Insights  |    |    |
|  **Integração Empresarial**  |    |    |
|  StorSimple  |  X  |    |
|  Gestão de API  |    |    |
|  Event Grid  |    |    |
|  Data Factory  |    |    |
|  Service Bus  |  X  |  X  |
|  Catálogo de Dados  |    |    |
|  SQL Server Stretch Database  |    |  X  |
|  Funcionalidade de Apps lógicas do Azure App Service  |    |    |
|  **Segurança + Identidade**  |    |    |
|  Azure Active Directory  |  X  |  X  |
|  Azure Active Directory B2C  |    |    |
|  Multi-Factor Authentication  |    |    |
|  Azure Active Directory Domain Services  |    |    |
|  Key Vault  |  X  |  X  |
|  Centro de Segurança  |  X  |  X  |
|  **Ferramentas de Programação**  |    |    |
|  Visual Studio Team Services  |    |    |
|  Application Insights  |    |    |
|  DevTest Labs  |    |    |
|  Visual Studio App Center  |    |    |
|  Universidade de Xamarin  |    |    |
|  **Monitorização + Gestão**  |    |    |
|  Assistente  |    |    |
|  Cópia de segurança  |  X  |  X  |
|  Recuperação de sites  |  X  |  X  |
|  Scheduler  |  X  |  X  |
|  Automatização  |  X  |  X  |
|  Log Analytics  |  X  |    |
|  Azure Monitor  |    |    |
|  Aplicações Azure-Managed  |    |    |
|  Azure Migrate  |    |    |
|  Grupos de Gestão  |    |  

## <a name="next-steps"></a>Passos seguintes

- [Conheça](/azure/cloud-solution-provider/overview/partner-center-overview) as capacidades disponíveis para a Azure no Partner Center.

- [Crie](/azure/cloud-solution-provider/customer-management/create-new-customer) o seu primeiro cliente na Azure CSP e implante os serviços Azure.
