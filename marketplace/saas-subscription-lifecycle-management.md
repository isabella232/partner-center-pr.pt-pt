---
title: Software como gestão do ciclo de vida de subscrição de serviço (SaaS)
description: Software como gestão de ciclo de vida por subscrição de serviço (SaaS) no Azure Marketplace.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: conceptual
ms.date: 08/20/2021
ms.author: yonits
author: yonits
ms.openlocfilehash: c5f06fb88a29def9df8d8cc2936f9eea91d8b2b4
ms.sourcegitcommit: fceaca54b0ec695cf214209c09b4516e1b40866a
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/23/2021
ms.locfileid: "128322055"
---
# <a name="saas-subscription-lifecycle-management"></a>Gestão do ciclo de vida por subscrição do SaaS

Este artigo abrange como descobrir um recurso SaaS, as diferenças entre o SaaS e o SaaS Classic, e a gestão de recursos saaS no portal Azure.

## <a name="find-a-saas-resource"></a>Encontre um recurso SaaS

Ao adquirir uma oferta SaaS do Azure Marketplace, cria um software como subscrição de serviço (SaaS) no portal Azure (para mais informações, consulte [Comprar uma oferta SaaS no portal Azure).](purchase-saas-offer-in-azure-portal.md) Para encontrar um recurso SaaS no portal:

- **Janela de pesquisa global** (em cima) – Procure a sua subscrição SaaS pelo nome.
- **SaaS** – Lista todas as suas subscrições SaaS. Existem dois tipos de listas de SaaS; ver a seguinte secção.
- **Assinaturas** – Lista todas as subscrições do Azure a que tem acesso como parte do seu inquilino. Para encontrar uma subscrição específica, utilize o filtro ou a janela de pesquisa.
- **Todos os recursos** – Lista todos os recursos criados em todas as subscrições a que tem acesso. Para encontrar uma subscrição específica, utilize o filtro (Tipo > SaaS) ou procure na lista.

## <a name="differences-between-saas-and-saas-classic-lists-of-resources-in-the-azure-portal"></a>Diferenças entre SaaS e SaaS Classic listas de recursos no portal Azure

A diferença entre estes dois tipos é que o SaaS Classic permite encontrar as subscrições SaaS que foram criadas sob o seu inquilino e não sob um grupo de recursos.
Se adquiriu uma subscrição saaS no portal Azure antes de fevereiro de 2021, foi criada sob o seu inquilino e pode encontrá-la sob o SaaS Classic. Todas as compras efetuadas no Microsoft AppSource estão nesta lista.

Se adquiriu uma subscrição saaS no portal Azure antes de fevereiro de 2021 e quer transferi-la de baixo do Inquilino para um grupo de Recursos (recomendado), vá à subscrição saaS na secção **SaaS Classic** e selecione **Move to Resource Group**. Só é possível mover subscrições no estado **pendente** ou **ativo.** Uma vez movido, a subscrição do SaaS aparece agora na vista **SaaS,** não **no SaaS Classic.** Não é possível mover uma subscrição SaaS para um grupo de recursos se for comprada no AppSource.

Este movimento oferece os seguintes benefícios:

- Melhor acesso e controlo do seu recurso SaaS com políticas herdadas e permissões dos grupos de subscrição e recursos do Azure (controlo total do RBAC)
- O ciclo de vida do SaaS está ligado ao ciclo de vida da assinatura Azure para ações como transferências e supressões
- Mais fácil descoberta, com recursos SaaS encontrados usando pesquisa global
- Utilização da Azure Cost Management – Monitorizar os gastos com recursos da SaaS
- Os recursos de nível de subscrição têm eventos de recursos no log de atividade

## <a name="manage-your-saas-service"></a>Gerir o seu serviço SaaS

Existem várias formas de gerir as suas subscrições SaaS

* Para as assinaturas SaaS adquiridas no portal Azure, gerencie-as lá.
* Para as subscrições SaaS adquiridas no AppSource, gerencie-as no portal Azure e no [Centro Administração Microsoft 365;](https://admin.microsoft.com/Adminportal/Home?#/subscriptions) para obter detalhes sobre a utilização do Administração Microsoft 365 Center, consulte [Gerir subscrições de aplicações de terceiros para a sua organização.](/microsoft-365/commerce/manage-saas-apps?view=o365-worldwide&preserve-view=true)
* Algumas editoras permitem-lhe gerir as subscrições do SaaS diretamente na sua plataforma. Visite o site da editora utilizando um link na página de subscrição do SaaS no portal Azure.

Há várias ações que pode tomar após a sua compra; alguns exigirão permissões do Proprietário ou do Contribuinte:

### <a name="change-plans"></a>Mudar planos

As alterações que fizer a um plano a que está subscrito entrarão em vigor entrarão em vigor imediatamente. A faturação será proscê-lo de acordo com o prazo de faturação do plano atual. A alteração de planos requer permissões **de Proprietário** ou **Contribuinte.**

> [!NOTE]
> O editor poderá recusar-se a aprovar a alteração se as alterações selecionadas não forem viáveis dentro do seu serviço. Neste caso, a mudança falhará.

Há alguns casos em que o **plano de mudança** pode não funcionar:

- Se a sua subscrição estiver ao nível do Inquilino com permissões **de Leitura,** não pode alterar o plano. Neste caso, solicite permissões à pessoa que tem a função **de Proprietário** na subscrição.
- Se não houver nenhum Instrumento de Pagamento (PI) associado à Subscrição Azure, não poderá alterar o seu plano gratuito para um plano pago. No entanto, pode selecionar uma subscrição Azure diferente e, em seguida, escolher um plano pago, ou adicionar um PI à Subscrição Azure selecionada.
- Se o plano selecionado tiver uma limitação mínima/máxima de utilizadores que não inclua o número atual de utilizadores, selecione um plano diferente com o mesmo número de utilizadores incluídos no plano original que adquiriu ou contacte a editora.
- Se o editor não conseguir cumprir o pedido, contacte-os diretamente.

### <a name="change-number-of-users"></a>Alterar número de utilizadores

Para planos baseados em assentos, pode adicionar ou reduzir o número de utilizadores que definiu durante o processo de compra. A alteração do número de utilizadores a que está subscrito entrará em vigor de imediato e a faturação será proscrito de acordo com o prazo de faturação do plano atual. As alterações nos lugares só são possíveis dentro da gama mínima e máxima de lugares, tal como definido pela editora. Em alguns casos, você será obrigado a mudar um plano antes de mudar de lugar, e vice-versa.

- Se a sua subscrição estiver ao nível do Inquilino com permissões de Leitura, não pode alterar o número de utilizadores. Em vez disso, Solicite permissões ao Contribuinte da pessoa que tem a função de Proprietário na subscrição.
- Se o editor não conseguir cumprir o pedido, contacte-os diretamente.

> [!NOTE]
> O editor pode recusar-se a aprovar a alteração se não for viável dentro do seu serviço. Neste caso, a mudança falhará.

### <a name="edit-recurring-billing"></a>Editar faturação recorrente

A faturação recorrente permite-lhe gerir a renovação da sua subscrição SaaS. Quando a faturação recorrente estiver desligada, a subscrição e o serviço saaS terminarão na data de renovação. Só pode alterar a opção de renovação enquanto a subscrição estiver ativa. Uma subscrição SaaS encerrada e/ou cancelada não pode ser reativada; uma nova subscrição saaS precisa de ser criada no seu lugar.

### <a name="view-billing"></a>Ver faturação

Ver faturas para a sua subscrição Azure e produtos Azure Marketplace adquiridos com esta subscrição. Para o SaaS adquirido no portal, consulte a página de faturação na página de subscrição do SaaS na secção **Billing,** que o redirecionará para **a Gestão de Custos.**

A Gestão de Custos ajuda-o a compreender a quebra da fatura, a gerir a sua conta de faturação e subscrições, a monitorizar/controlar os gastos do Azure e a otimizar o uso de recursos. Permite analisar custos, criar e gerir orçamentos, e muito mais. Por exemplo, permite-lhe acompanhar o uso personalizado do medidor (para as subscrições SaaS criadas após fevereiro de 2021, ou transferidas para um grupo de recursos). Saiba mais sobre gestão de custos na [Azure Cost Management + documentação de faturação.](/azure/cost-management-billing/)

Se a sua compra foi feita através do Microsoft AppSource, pode ver as suas faturas no Microsoft Admin Center ao abrigo **de pagamentos & Contas.**

### <a name="cancel-subscription"></a>Cancelar subscrição

O cancelamento remove o seu acesso ao software que adquiriu como parte desta subscrição do SaaS. As restituições são processadas de acordo com a política de reembolsos; para mais detalhes, consulte [as políticas de reembolso para o Microsoft AppSource e para o Azure Marketplace.](refund-policies.md)

Se a sua subscrição estiver ao nível do Inquilino com permissões **de Leitura,** não pode cancelar uma subscrição. Em vez disso, contacte a pessoa com permissões **do Proprietário.**

Se tiver uma subscrição mensal do SaaS por mais de 24 horas ou uma subscrição anual ou plucária por mais de 14 dias, não será utilizado qualquer reembolso para o termo atual da subscrição (ver política de cancelamento). A faturação com base no consumo depois de configurada uma conta SaaS também não é elegível para reembolso.

### <a name="delete-subscription"></a>Eliminar subscrição

Esta ação é como cancelar, com a adição de remover o recurso SaaS da sua lista de subscrições saaS. Depois de eliminar uma subscrição, não poderá aceder-lhe a partir do portal Azure.

Se a sua subscrição estiver ao nível do Inquilino com permissões **de Leitura,** não pode excluir uma subscrição. Em vez disso, contacte a pessoa com permissões **do Proprietário.**

### <a name="change-azure-subscription-andor-resource-group"></a>Alterar subscrição e/ou grupo de recursos do Change Azure

Para alterar um grupo de subscrição/recursos associado a uma oferta que foi adquirida no portal Azure:

1. Vá à secção **SaaS.**
2. Selecione a subscrição para alterar.
3. Em **Billing**, selecione **Alterar subscrição faturada**.
4. Selecione o grupo de subscrição/recursos pretendido ou crie um novo grupo de recursos para mover o recurso SaaS para..
5. Selecione **Alterar** na parte inferior para concluir o processo.

Há alguns casos em que a mudança pode não funcionar:

- Se a sua Subscrição SaaS não estiver no estado de Subscrição, consulte o seu estado de subscrição na secção SaaS ou na sua página de subscrição **SaaS.**
- Se a assinatura SaaS for um recurso de nível de inquilino:
    - Deverá ter permissões *de Proprietário/Contribuinte* na subscrição target Azure.
- Se a subscrição do SaaS for um recurso de nível de subscrição:
    - Precisa de permissões *de Leitura* ou *Proprietário/Colaborador* para a Assinatura Azure alvo.
    - Precisa de permissões *de Proprietário/Contribuinte* para o grupo de recursos-alvo.
    - Se já existe uma subscrição SaaS com o mesmo nome no grupo de recursos-alvo, selecione um grupo de recursos-alvo diferente.
- A subscrição e subscrição de recursos target Azure será submetida a todos os controlos realizados durante a compra. Para saber mais sobre os cheques de compra, consulte a secção [de Subscrição e configuração saaS](purchase-saas-offer-in-azure-portal.md#saas-subscription-and-configuration) na **Compra de uma oferta SaaS no portal Azure**.

## <a name="next-steps"></a>Passos seguintes

- Se já comprou uma oferta no mercado, vá a [Billing e Faturação](billing-invoicing.md)
- Saiba mais sobre as opções [do plano privado](./private-plans.md)