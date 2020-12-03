---
title: Mover clientes das ofertas atuais da Azure para o plano Azure
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como os parceiros da CSP podem usar o Partner Center para transferir os clientes das ofertas csp azure existentes para os serviços Azure ao abrigo do plano Azure.
author: mowree
ms.author: mowrim
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 06/16/2020
ms.openlocfilehash: 4e22386dc8bddd9662a0d80020a5c90c464e9d39
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534816"
---
# <a name="transition-customers-to-azure-plan-from-existing-csp-azure-offers"></a>Transição de clientes para plano Azure a partir de ofertas CSP Azure existentes

**Funções adequadas**

- Agente administrativo
- Administrador de faturação
- Administrador global
- Agente helpdesk
- Agente comercial
- Administração de gestão de utilizadores

Este artigo explica como os parceiros da CSP podem usar o Partner Center para transferir os clientes das ofertas csp azure existentes para os serviços da Azure ao abrigo do plano Azure. Os fornecedores indiretos e os parceiros de conta direto podem transitar para a nova experiência de comércio disponível no Microsoft Cloud Service Provider Program (CSP) para o Azure. (Os revendedores indiretos terão de trabalhar através dos seus fornecedores indiretos.) Os clientes terão uma forma simplificada de comprar serviços na nuvem, seja comprando de parceiros, de vendedores da Microsoft, ou diretamente na web.

A capacidade de transição destina-se apenas aos clientes que transitam para a nova experiência de comércio para o Azure e que assinaram o Acordo de Cliente da Microsoft. Não é para outras ofertas em CSP como o Office 365 ou Dynamics 365.

## <a name="transition-existing-csp-offers-to-an-azure-plan"></a>Transição cSP existente oferece a um plano Azure

Pode transitar um cliente das suas ofertas CSP Azure existentes para os serviços Azure ao abrigo do plano Azure na nova experiência de comércio no programa CSP a partir do Centro de Parceiros. Para isso, o parceiro e o cliente devem ter uma relação de revendedor estabelecida através do Partner Center, e o cliente deve ter assinado o Acordo de Cliente da Microsoft.

### <a name="select-transition-to-azure-plan"></a>Selecione a transição para o plano Azure

1. Selecione plano Azure para o seu cliente.

2. Selecione **faturação de transição para o plano Azure**.

   :::image type="content" source="images/azure/transition1.png" alt-text="Screenshot mostrando subscrições baseadas em uso reportam informações com uma opção selecionável chamada: Faturação de subscrição transitiona azure para o plano Azure.":::

3. Selecione **Continuar**

   :::image type="content" source="images/azure/transition2.png" alt-text="Caixa de diálogo intitulada Transição para plano Azure com implicações para ler sobre a transição e duas opções para selecionar, Continuar ou Cancelar.":::

   O seu cliente será transitado para o plano Azure.

   **O fluxo de trabalho de transição automatiza as etapas pré-necessárias:**

   - Compra de planos Azure
   - Um plano por cliente em cenários CSP diretos  
   - Um plano por revendedor  

   Por exemplo, um parceiro comprou duas ofertas da Microsoft Azure e incluiu dois POR distintos na compra. Neste caso, o fluxo de trabalho de transição comprará dois planos Azure (um por revendedor) e mapeará automaticamente as respetivas assinaturas Azure ao abrigo dos planos Azure.  

   **Mapeamento Azure subscrição do plano Azure**

   Após a sua compra do plano(s) Azure, o nosso sistema irá mapear as subscrições Azure existentes para os planos Azure. O progresso pode ser visto no portal Azure, bem como no Centro Parceiro.

4. Volte à página de **Subscrições** do Centro de Parceiros do seu cliente para atualizar o seu limite de orçamento utilizando a moeda local.

   :::image type="content" source="images/azure/transition3.png" alt-text="Vista parcial da página de subscrições do Partner Center com limites orçamentais definidos em moeda local por um período de faturação.":::

   >[!NOTE]
   >O orçamento que definiu no Partner Center não passa para o portal Azure. Também deverá definir o orçamento e alertar no portal Azure.

   Quando se muda para o plano Azure, já não pode comprar subscrições Azure para este cliente. Cria as subscrições ao abrigo do plano Azure no portal Azure.

   >[!NOTE]
   > Todas as subscrições da Azure adquiridas através do RBAC ao abrigo do plano Azure serão avaliadas e faturadas em moeda local. As tarifas FX não serão utilizadas.

### <a name="track-your-transition-details"></a>Acompanhe os seus dados de transição

Acompanhe o progresso da transição no portal Azure, bem como no Partner Center.

:::image type="content" source="images/azure/details1.png" alt-text="Screenshot mostrando tabela com lista de detalhes de transição por subscrição - inclui subscrição I D, data de transição e estado de transição.":::

### <a name="billing-impact-to-partners"></a>Impacto da faturação para os parceiros

Se transitar um cliente de uma oferta CSP Azure existente, terá os seguintes impactos de faturação:

- Você será cobrado na sua fatura CSP existente para todo o uso até ao ponto de sair da subscrição original do CSP Azure.

- Se tiver direitos de acesso administrativo à subscrição CSP existente, continuará a ter acesso quando essa subscrição for migrada.

Para transitar os Acordos Empresariais diretos para as inscrições de CSP e Server e Cloud para os serviços Azure, leia [Obter a propriedade de faturação de subscrições da Azure para o Microsoft Partner Agreement](/azure/billing/mpa-request-ownership)

### <a name="audit-log"></a>Registo de auditoria

Para conciliar a faturação, veja o seu histórico de subscrições "Microsoft Azure" (0145P) na página **de Subscrições.**

A subscrição "Microsoft Azure" (0145P) é composta por duas partes:

1. Assinatura de comércio
2. Assinatura Azure (direito)

Quando a transição estiver concluída, a subscrição do Azure é movida ao abrigo do novo plano Azure e a subscrição do comércio é suspensa de modo a que não seja reportada mais nenhuma utilização.  

>[!NOTE]
>Quando a subscrição do Microsoft Azure (0145P) é adquirida em CSP, tanto a subscrição de comércio como a subscrição Azure (direito) têm o mesmo valor. Só no caso de faturação de alterações de propriedade ou transferências os valores diferem.

### <a name="transition-issues"></a>Questões de transição

Não prevemos problemas durante as transições. Se ocorrer, iremos atualizá-lo no próprio fluxo de trabalho de transição. Não haverá distúrbios no uso do Azure.  

## <a name="next-steps"></a>Passos seguintes

- [Manage subscriptions and resources under the Azure plan](azure-plan-manage.md) (Gerir subscrições e recursos ao abrigo do plano do Azure)

- [Parceiro ganhou crédito - visão geral](partner-earned-credit.md)