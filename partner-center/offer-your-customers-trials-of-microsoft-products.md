---
title: Oferecer aos clientes testes de produtos da Microsoft
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Deixe os clientes experimentarem os produtos de subscrição da Microsoft durante 30 dias. Inscreva-se para estes testes gratuitos no catálogo, tal como muitos outros serviços online.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 393bd70096ba3cd7d1c9889d5b521cc94a389d90
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/29/2021
ms.locfileid: "114845980"
---
# <a name="give-customers-30-day-free-trials-of-microsoft-products"></a>Dar aos clientes 30 dias de testes gratuitos de produtos microsoft

**Funções adequadas**: Administração global | Administração de administração de utilizadores | Agente comercial

Uma boa forma de apresentar clientes aos novos produtos da Microsoft é oferecer testes gratuitos de 30 dias. Você pode se inscrever para os testes no catálogo, assim como muitos outros serviços on-line. Todos os parceiros podem participar.

## <a name="available-trial-offers"></a>Ofertas de teste disponíveis

Pode encontrar todas as suas ofertas de teste pendentes na página **do Cliente.** Esta página lista todas as subscrições, incluindo testes gratuitos e subscrições pagas. (Esta funcionalidade não está atualmente disponível na China.)

Cada cliente tem direito a um teste gratuito por cada oferta disponível. Por exemplo, podem obter um julgamento gratuito por Microsoft 365 Empresas e um julgamento gratuito para Office 365 E3. No entanto, se o cliente já é dono da oferta, não pode usar um teste gratuito para essa oferta.

### <a name="available-products"></a>Produtos disponíveis

Estão disponíveis testes gratuitos para as ofertas mais abrangentes e populares baseadas em licesen. As novas ofertas experimentais podem ser introduzidas mensalmente.

Os parceiros podem encontrar testes na lista de preços mensais na página **de preços e ofertas** no Partner Center. As ofertas de ensaio terão "TRIAL" listadas na coluna De **Tipo de Licença Secundária** da lista de preços.

Atualmente, não há **testes gratuitos** para ofertas governamentais, ofertas de educação ou ofertas adicionais.

## <a name="licenses-for-free-trial-offers"></a>Licenças para ofertas de teste gratuitos

Todos os testes gratuitos fornecem 25 licenças. Não podes mudar este número durante o julgamento. Não pode adicionar ou remover licenças no julgamento gratuito. Após o ensaio ser convertido para uma subscrição paga, pode adicionar mais licenças à subscrição.

As licenças de ensaio devem ser atribuídas aos utilizadores da mesma forma que a licença de serviços pagos é atribuída.

## <a name="sign-customers-up-for-trials"></a>Inscreva clientes para testes

Obtenha um teste para o seu cliente no Partner Center:

1. A partir da **Venda** no Centro de Parceiros, vá ao **Catálogo.** 
2. No catálogo, a partir da **frequência Billing,** selecione **Trial offer**. Isto permite apenas a aparecerem testes gratuitos e desativa outras ofertas que não são gratuitas. Os testes aparecerão no **separador Trials** no catálogo.
3. Selecione o teste gratuito que pretende oferecer e, em seguida, **selecione submeter**. Todos os julgamentos são por 30 dias durante os quais não será cobrado. Também pode convertê-lo numa subscrição paga a qualquer momento durante o julgamento.

## <a name="converting-trials-to-paid-subscriptions"></a>Conversão de ensaios para assinaturas pagas

Um teste gratuito não é automaticamente convertido para uma subscrição paga. Após 30 dias, um ensaio gratuito deve ser convertido para uma subscrição paga ou [expirará](#expiring-offers). Os julgamentos gratuitos não podem ser prolongados.

Terá de converter o julgamento numa subscrição paga. Pode [fazê-lo utilizando o Centro de Parceiros](#convert-trials-using-partner-center) ou [através das APIs do Partner Center](#convert-trials-using-apis).

> [!NOTE]
> Os ensaios gratuitos para o programa Fornecedor de Soluções em Nuvem (CSP) não podem ser convertidos para outro inquilino do programa (como EA, Open ou MOSP).

### <a name="convert-trials-using-partner-center"></a>Converter ensaios usando Partner Center

Pode converter ensaios em subscrições pagas utilizando o Partner Center:

1. Vá à página de subscrição do cliente e selecione o teste gratuito.
2. Selecione **Converter o ensaio para a subscrição paga.**
3. Introduza a quantidade de licença desejada e a frequência de faturação e selecione **Apply**.
4. A faturação da subscrição paga começa na data de conversão e a subscrição renova automaticamente 12 meses a partir da data de conversão. 

### <a name="convert-trials-using-apis"></a>Converter ensaios usando APIs

Poderá ser necessário alterar as suas APIs para acomodar a conversão de um teste gratuito para uma subscrição paga. Para mais informações, consulte a seguinte documentação do programador:

- [Converter uma subscrição de avaliação em paga](/partner-center/develop/convert-a-trial-subscription-to-paid)
- [Obter uma lista de ofertas de conversão de avaliação](/partner-center/develop/get-a-list-of-trial-conversion-offers)

### <a name="trials-without-conversions"></a>Ensaios sem conversões

Nem todos os ensaios podem ser convertidos em subscrições pagas. Os parceiros podem usar um ensaio que não tenha conversões até à data de validade. Os parceiros podem adquirir ofertas compatíveis que suportam os mesmos serviços que a oferta experimental.  Isto deve ser feito antes do termo do julgamento para garantir que os serviços de ofertas recém-adquiridos se alinham com os serviços do ensaio. 

|**Avaliação**   |**Ofertas compatíveis de Pequenas Empresas**   |**Ofertas empresariais compatíveis**   |
|----------------------------|:---------------------------------|:------------------------------------------|
|Microsoft Teams Ensaio de Nuvem Comercial (Iniciado pelo Utilizador)   |Microsoft 365 Empresas Basic, Microsoft 365 Empresas, Microsoft 365 Empresas Premium   | F3 (anteriormente F1), Office 365 para a Enterprise (E1, E3 e E5), Microsoft 365 F1/F3, Microsoft 365 Enterprise (E3)   |

>[!NOTE]
>As ofertas acima têm planos de serviço semelhantes com funcionalidades semelhantes, no entanto pode haver algumas diferenças entre as ofertas.

### <a name="expiring-offers"></a>Ofertas caducadas

Não será notificado das ofertas caducadas. Pode rastrear as próximas datas de validade utilizando a vista do cliente no Partner Center ou consultando a API. É uma boa ideia monitorizar estas datas com frequência para que possa tomar as ações de acompanhamento apropriadas com os clientes à medida que se aproximam de um ponto de decisão.

Depois de expirado o julgamento, um cliente que tentar entrar nesse julgamento verá uma mensagem de caducidade. No entanto, os dados são armazenados de acordo com as normas de retenção de dados. Depois de adquirir uma nova subscrição com os mesmos planos de serviço, as informações do seu cliente podem ser novamente acedidas a partir da subscrição recém-ativada.

## <a name="billing"></a>Faturação

A faturação anual e os testes gratuitos são os mesmos nas nuvens soberanas e na nuvem pública. A única diferença é o teste SKUs disponível no momento do lançamento.

## <a name="billing-for-free-trials"></a>Faturação para julgamentos gratuitos

Os ensaios gratuitos podem ser utilizados tanto para subscrições mensais como anuais. Pode selecionar a frequência de faturação quando converter o ensaio numa subscrição paga.

A data de início da subscrição baseia-se na data de conversão. Se o teste gratuito for convertido para uma oferta paga com faturação anual, a data de renovação da subscrição será de 12 meses a contar da data de conversão. Se o teste gratuito for convertido para uma oferta paga com faturação mensal, a data de renovação da subscrição será de doze meses a contar da data de faturação seguinte à data de conversão.

### <a name="invoices"></a>Faturas

Não verá testes gratuitos listados na sua fatura ou ficheiro de reconciliação baseado em licença. Os testes gratuitos só aparecerão na sua fatura e ficheiro de reconciliação baseado na licença depois de converter um teste gratuito numa subscrição paga. A subscrição convertida aparecerá da mesma forma que qualquer nova subscrição.

### <a name="incentives"></a>Incentivos

Os ensaios gratuitos não têm impacto nos incentivos.

## <a name="support"></a>Suporte

Para apoio em testes gratuitos, envie um pedido de serviço através do Partner Center.