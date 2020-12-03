---
title: Plano Azure - Gerir subscrições & recursos
ms.topic: article
ms.date: 05/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como os parceiros podem usar diferentes opções de controlo de acesso baseado em funções (RBAC) para obter controlo operacional e gestão dos recursos Azure de um cliente.
author: amitravat
ms.author: amrava
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 31e9c6862a5aa19407fa6da5e15333bb7e696720
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534935"
---
# <a name="manage-subscriptions-and-resources-under-the-azure-plan"></a>Manage subscriptions and resources under the Azure plan (Gerir subscrições e recursos ao abrigo do plano do Azure)

**Funções adequadas**

- Agente administrativo


Este artigo explica como os parceiros da CSP podem usar diferentes opções de controlo de acesso baseado em funções (RBAC) para obter controlo operacional e gestão dos recursos Azure de um cliente. Quando transita um cliente para o plano Azure, é-lhe atribuído direitos de administração privilegiados em Azure (direitos de proprietário de subscrição através de administração em nome de) por padrão.

 > [!NOTE]
 > Os direitos de administração da subscrição Azure podem ser removidos pelo cliente a um nível de subscrição, grupo de recursos ou carga de trabalho. 

 Os parceiros podem obter controlo operacional 24x7 e gestão dos recursos Azure de um cliente em CSP, utilizando diferentes opções fornecidas através da funcionalidade de controlo de acesso baseada em funções (RBAC). 

- **Administrador em Nome de (AOBO)** - Com [a AOBO,](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO)qualquer utilizador com o papel de Agente Administrador no inquilino parceiro terá acesso ao proprietário do RBAC às subscrições Azure que cria através do programa CSP.

- **Farol Azure**: A AOBO não permite a flexibilidade para criar grupos distintos que trabalham com diferentes clientes, ou para permitir diferentes funções para grupos ou utilizadores. Utilizando o Farol Azure, pode atribuir diferentes grupos a diferentes clientes ou funções. Uma vez que os utilizadores terão o nível de acesso adequado através da gestão de recursos delegados do Azure, pode reduzir o número de utilizadores que têm a função de Agente Administrador (e assim ter acesso total ao AOBO). Isto ajuda a melhorar a segurança limitando o acesso desnecessário aos recursos dos seus clientes. Também lhe dá mais flexibilidade para gerir vários clientes em escala. Para mais informações, leia [o Farol Azure e o programa Cloud Solution Provider](/azure/lighthouse/concepts/cloud-solution-provider).

- **Diretório ou Utilizadores convidados ou [principais de serviço :](/azure/active-directory/develop/app-objects-and-service-principals)** Pode delegar o acesso granular às subscrições do CSP adicionando utilizadores no diretório de clientes ou adicionando utilizadores convidados e atribuindo funções específicas de RBAC.

A Microsoft recomenda que os utilizadores tenham as permissões mínimas necessárias para realizar o seu trabalho como prática de segurança. Consulte os recursos de Gestão de Identidade Privilegiada do [Diretório Ativo Azure.](/azure/active-directory/privileged-identity-management/pim-configure)

## <a name="link-your-partner-id-mpn-idto-your-credentials-for-managing-customers-azure-resources"></a>Ligue o seu parceiro ID (MPN ID)às suas credenciais para gerir os recursos Azure do cliente

A tabela a seguir mostra os métodos utilizados para associar o seu ID ao seu parceiro com várias opções de acesso RBAC.

|**Categoria**   |**Cenário**   |**Associação MPN ID**|
|-----------------|:------------------------|:------------------|
|AOBO   |O parceiro direto da CSP ou fornecedor indireto cria a subscrição para o cliente que torna o parceiro direto da CSP ou o fornecedor indireto proprietário da assinatura utilizando a AOBO.; O parceiro direto da CSP ou o fornecedor indireto dão acesso indireto ao revendedor à subscrição utilizando o AOBO.|Automático (não é necessário trabalho de parceiro)|
|Azure Lighthouse|Parceiro cria uma nova [oferta de Serviços Geridos no Marketplace.](/azure/lighthouse/concepts/managed-services-offers) Esta oferta é aceite na subscrição da CSP e o parceiro tem acesso à subscrição da CSP.|Automático (não é necessário trabalho de parceiro)|
|Azure Lighthouse|Parceiro implementa [modelo ARM](/azure/lighthouse/how-to/onboard-customer) na subscrição do Azure|O parceiro precisa de associar o ID MPN ao utilizador ou ao principal de serviço no inquilino sócio. Para mais informações - [Link Partner ID](/azure/billing/billing-partner-admin-link-started).|
|Diretório ou utilizador convidado|O Parceiro cria um novo utilizador ou principal de serviço no diretório de clientes e dá acesso à subscrição CSP ao utilizador. O Parceiro cria um novo utilizador ou diretor de serviço no diretório de clientes. O parceiro adiciona o utilizador a um grupo e dá acesso à subscrição da CSP ao grupo.|O parceiro precisa de associar o ID MPN ao utilizador ou ao principal de serviço no cliente. Para mais informações - [Link Partner ID](/azure/billing/billing-partner-admin-link-started).|

## <a name="confirm-that-you-have-admin-access"></a>Confirme que tem acesso a administrador

Necessita de acesso administrativo para gerir os serviços do seu cliente e receber créditos obtidos. Leia [o Parceiro ganhou créditos](partner-earned-credit.md) por informações detalhadas sobre créditos ganhos. Tem duas maneiras de se certificar de que sabe que tem acesso administrativo.

- Reveja o ficheiro de utilização diária - Isto pode ser determinado através da revisão do preço unitário e do preço unitário efetivo dentro do ficheiro de utilização diária e confirmando se está a ser aplicado um desconto. Se está a receber o desconto, é o administrador.

- Crie um alerta de monitor Azure - Pode criar um [alerta](/azure/azure-monitor/platform/alerts-activity-log) de registo de atividade do Azure Monitor para ser notificado quando o seu acesso AO RBAC for removido da subscrição de CSP.

### <a name="create-an-azure-monitor-alert"></a>Criar um alerta de monitor Azure

1. Criar alerta.

   :::image type="content" source="images/azure/azurealert1.png" alt-text="alerta azul":::

2. Selecione o tipo de ação que deseja que o alerta tome. Por exemplo, se especificar que deseja um e-mail, receberá um e-mail notificando-o caso de ocorrer alguma eliminação de funções.

   :::image type="content" source="images/azure/azureconfigurealert2.png" alt-text="alerta de configuração":::

### <a name="aobo-removal"></a>Remoção do AOBO

Os clientes podem gerir o acesso às suas subscrições indo ao **Access Control** no portal Azure. A partir do separador **Funções,** selecionam **remover o acesso.** Se isto acontecer, pode:

- Fale com o seu cliente para ver se o acesso a administrador pode ser reintegrado.

- Utilize o acesso fornecido através [do controlo de acesso baseado em funções (RBAC)](/azure/role-based-access-control/overview).

- Utilize o acesso fornecido através do [Farol Azure.](https://azure.microsoft.com/services/azure-lighthouse/)

O acesso baseado em funções difere do acesso a administradores. Os papéis delimitam precisamente o que se pode ou não fazer. O acesso a administrador é mais amplo.

Para ver as funções elegíveis para ganhar PEC, leia [Papéis e permissões para o parceiro ganhou crédito.](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3QuW2)

## <a name="next-steps"></a>Passos seguintes

- [Revogação e reinstauração de privilégios administrativos para assinaturas CSP Azure](revoke-reinstate-csp.md)

- [Parceiro ganhou crédito - visão geral](partner-earned-credit.md)

- [Parceiro ganhou crédito por serviços geridos](partner-earned-credit-explanation.md)