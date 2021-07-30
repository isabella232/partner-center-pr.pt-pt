---
title: Faturação de produtos de mercado comercial
ms.topic: article
ms.date: 05/12/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
description: Saiba como funciona a faturação para produtos ISV SaaS ou subscrições compradas para clientes do mercado comercial dentro do Partner Center.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 102f13530ece08cd813412a44897ece0186e7cbb
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/29/2021
ms.locfileid: "114837956"
---
# <a name="billing-for-commercial-marketplace-products-and-subscriptions-in-partner-center"></a>Faturação para produtos e subscrições de mercado comercial no Partner Center


**Funções adequadas**: Administração global | Administrador de faturação

Como parceiro no programa CSP, pode utilizar o Partner Center para comprar produtos SaaS baseados em licenças a editores da ISV no mercado comercial. Depois de o fazer, pode aceder a uma conta para este tipo de compras. O período de faturação começa no primeiro dia do mês civil e termina no último dia do mês civil. As faturas são disponibilizadas no 8º dia do mês seguinte.

Pode aceder às faturas a partir do painel partner [center](https://partner.microsoft.com/dashboard/) ou utilizando [APIs do Partner Center](/partner-center/develop/).

Os parceiros do programa CSP são faturados para soluções de mercado comercial ISV compradas para um cliente quando compram esses produtos a partir do Partner Center ou do portal Azure (utilizando o inquilino Azure comprado anteriormente pelo cliente).

>[!NOTE]
>Se os clientes utilizarem o seu próprio inquilino Azure AD (nenhum adquirido a um parceiro no programa CSP), os clientes também podem optar por adquirir a sua própria solução ISV SaaS diretamente de[(Microsoft AppSource](https://appsource.microsoft.com/) ou [Azure Marketplace).](https://azuremarketplace.microsoft.com/) Se o fizerem, receberão a sua própria conta diretamente da Microsoft. Da mesma forma, se um parceiro no programa CSP vender uma subscrição Azure ou o novo plano Azure ao cliente e conceder ao cliente (ou revendedor indireto) [acesso baseado em funções](/azure/role-based-access-control/built-in-roles) a esse inquilino (atribuindo qualquer papel ao cliente além **do Reader),** esse cliente (ou revendedor indireto) também pode comprar ofertas comerciais sem aprovação prévia ou notificação ao parceiro CSP. Nestes casos, a Microsoft não notificará diretamente os parceiros do programa CSP sobre as compras efetuadas pelos seus clientes. No entanto, a Microsoft oferece um mecanismo opcional [do Azure Monitor](/azure/azure-monitor/platform/alerts-activity-log) que pode utilizar para definir alertas ou notificações sobre a atividade numa subscrição do Azure.

## <a name="access-billing-information-for-commercial-marketplace-products"></a>Acesso à informação de faturação para produtos de mercado comercial

O administrador global ou administrador de faturação da sua empresa receberá um e-mail quando uma fatura estiver pronta para ver. Para aceder à fatura mais recente e ficheiro de reconciliação para compras de produtos de mercado comercial:

1. Inicie sessão no [dashboard](https://partner.microsoft.com/dashboard/) do Centro de Parceiros.

2. No menu Partner Center, selecione **Billing**. 

    Verá dois separadores no topo da página de Faturação: **Compras recorrentes** e **recorrentes e únicas.** Cada separador permite-lhe aceder a ficheiros de fatura e reconciliação (recon) para diferentes produtos de mercado:

    - **Separador recorrente:** Apresenta ficheiros de fatura e reconciliação para subscrições relacionadas com Office 365, Microsoft 365, Dynamics 365, Azure Ative Directory, Power BI Pro e Microsoft Azure.

    - **Separador de compras recorrentes e pontuais:** Mostra ficheiros de fatura e reconciliação para o plano Azure, reservas Azure, software e produtos de mercado comercial.
  
3. Selecione o **separador compras recorrente e único.** Se adquiriu subscrições para um cliente numa moeda diferente, verá um separador para cada moeda. Pode fazer algumas coisas a partir desta página:

    - Para ver a fatura mais recente e o ficheiro de reconciliação, selecione **Fatura** ou **Arquivo de Reconciliação**. (Se assim o quisesse, também pode aceder aos dados mais recentes da fatura e do ficheiro de reconhecimento utilizando [APIs do Partner Center](/partner-center/develop/).

    - Para ver faturas anteriores e ficheiros de reconhecimento, expanda a linha de histórico de **Billing** abaixo.

    - Para verificar o saldo ou conta estimadas a qualquer momento com base na última atividade da conta, selecione um link na rubrica **Estimativas.**  

    >[!NOTE]
    > Quando publicarmos a sua conta no 8º dia do mês, incluirá impostos e quaisquer outros encargos e créditos aplicáveis. Isto significa que o valor final devido pode diferir do que se vê durante o período de faturação.

## <a name="more-about-invoices-and-recon-files-for-commercial-marketplace-products"></a>Mais sobre faturas e ficheiros de reconhecimento para produtos de mercado comercial

Esta secção oferece mais informações sobre ficheiros de fatura e reconciliação para assinaturas SaaS de marketplace comercial compradas para clientes de editores ISV de terceiros.

Quando seleciona **compras recorrentes e pontuais** a partir da opção **De Faturação** no menu Partner Center, você tem acesso a faturas e ficheiros de reconciliação para taxas relacionadas com as compras da Microsoft (primeira parte) e ISV (terceiros). Estas compras podem estar associadas a:

- Subscrições SaaS (de editores microsoft ou ISV)

- Plano do Azure

- Reservas do Azure

- Outro software baseado em subscrições (de editores microsoft ou ISV)

Exemplos destas compras podem incluir software SUSE Linux (uma subscrição de software) ou uma subscrição de produto Azure ISV SaaS.

>[!NOTE]
> Para obter mais informações sobre como ler ficheiros de fatura e reconhecimento, consulte também [a visão geral do Billing](billing.md).

### <a name="tips-on-reading-your-invoice"></a>Sugestões na leitura da sua fatura

Ao comprar um produto SaaS baseado em licença a um editor ISV de terceiros, só verá os custos da taxa de licença na sua fatura. Isto é verdade mesmo quando o produto SaaS da ISV utiliza (ou consome) recursos de infraestrutura Azure subjacentes. Isto porque os custos de utilização da infraestrutura Azure do seu cliente para um produto SaaS da ISV são faturados diretamente para o ISV. (Os ISVs verão os encargos associados de consumo da Azure no seu próprio ficheiro de reconciliação de faturas de utilização diária.)

A sua fatura conterá várias páginas:

- **Página 1 da fatura:** Contém uma visão geral resumo dos detalhes de faturação do parceiro do programa CSP. Isto inclui um resumo dos encargos para o período de faturação, um número de faturação, condições de pagamento (Net 60 dias) e métodos de pagamento de faturação para pagar por fio ou por cheque.

- **Página 2 (e quaisquer páginas subsequentes) da fatura:** Detalhes encargos tanto para compras de primeira parte da Microsoft como para compras isv de terceiros (baseada em licenças) no mercado comercial. Pode identificar as compras baseadas em licenças ISV pela linha **Publisher** por baixo de cada nome do produto. O ficheiro de reconciliação associado oferece mais detalhes de faturação para taxas específicas de fatura.

- **Página final da fatura:** Se foi cobrado por produtos de mercado baseados em licença a partir de um ISV, esta página final apresentará mais detalhes sobre o nome e endereço da editora ISV.

### <a name="tips-on-reading-your-reconciliation-file"></a>Sugestões na leitura do seu ficheiro de reconciliação

O ficheiro de reconciliação **de compras recorrentes e únicas** contém várias colunas com detalhes adicionais que mapeiam os encargos na sua fatura. A coluna **PublisherName** mostra se a compra é da Microsoft ou de um editor ISV de terceiros.

Algumas acusações no seu ficheiro de reconciliação podem aparecer com um custo de $0. Isto pode dever-se a uma oferta de "teste gratuito" da ISV (geralmente 30 ou 60 dias) ou a uma oferta de Bring Your Own License.

No caso de ofertas isv de teste gratuito:

- O período experimental gratuito cobre o custo do produto SaaS baseado na licença da ISV durante esse período. Também não será cobrado pela utilização associada da infraestrutura Azure daquele produto SaaS.  Se estiver a utilizar uma oferta ISV baseada na utilização, no entanto, o teste gratuito não inclui o custo da utilização subjacente da infraestrutura Azure. Neste caso, os encargos de utilização da infraestrutura Azure aparecerão num ficheiro de reconciliação Azure separado.

- Ao comprar e implantar um produto livre de testes da ISV para o seu cliente, o cliente é automaticamente inscrito no teste gratuito pela editora ISV. O período experimental gratuito termina automaticamente após o período definido pela editora ISV. Após o fim do período, o cliente será cobrado. Isto significa que o ficheiro de reconciliação pode mostrar duas linhas para um produto elegível para o ensaio: um que acompanha o período experimental e outro que acompanha a oferta paga (que apresentará um custo de $0 até ao final do período experimental). Assim que o julgamento terminar, a fila que mostra a oferta paga começará a mostrar encargos. 

Para obter mais informações sobre o que cada coluna representa, consulte [utilizar os seus ficheiros de reconciliação](use-the-reconciliation-files.md). Ver também [Tipos de faturação no Centro de Parceiros](./billing-basics.md)

## <a name="next-steps"></a>Passos seguintes

- [Gerir produtos de mercado comercial para clientes](csp-commercial-marketplace-manage.md)
- [Conheça o apoio a produtos de mercado comercial](csp-commercial-marketplace-support.md)