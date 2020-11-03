---
title: Ficheiros de reconciliação baseados em licenças
ms.topic: article
ms.date: 05/18/2020
description: Saiba como ler ficheiros de reconciliação baseados em licenças no Partner Center. Este artigo explica o significado de cada campo no seu ficheiro de reconhecimento baseado na licença.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 86581db73f1bf2b6660af45aca4747a5db779bbe
ms.sourcegitcommit: e1c8bea4aaf807aebe99c125cb1fb6dc8fdfa210
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/30/2020
ms.locfileid: "92529376"
---
# <a name="understand-the-fields-in-partner-center-license-based-reconciliation-files"></a>Compreenda os campos em ficheiros de reconciliação baseados em licenças do Partner Center

**Aplica-se a**

- Partner Center
- Centro de Parceiros para Microsoft Cloud para governo dos EUA

**Funções adequadas**
- Administrador global
- Administrador de utilizadores
- Administrador de faturação
- Agente administrativo

Para conciliar as suas alterações com as ordens de um cliente, compare o **Syndication_Partner_Subscription_Number** do ficheiro de reconciliação com o ID de **Subscrição** do Partner Center.

## <a name="fields-in-license-based-reconciliation-files"></a>Campos em ficheiros de reconciliação baseados em licenças

| Coluna | Descrição | Valor da amostra |
| ------ | ----------- | ------------ |
| PartnerId | Identificador único no formato GUID para uma entidade de faturação específica. Não é necessário para a reconciliação. O mesmo em todas as filas. | *8ddd03642-test-test-test-test-46b58d356b4e* |
| CustomerId | Identificador exclusivo da Microsoft para o cliente em formato GUID. | *12ABCD34-001A-BCD2-987C-3210ABCD5678* |
| CustomerName | Nome da organização do cliente, conforme relatado no Partner Center. *Campo muito importante para conciliar a fatura com a informação do seu sistema.* | *Testar cliente A* |
| MpnId | Identificador mpn do parceiro da CSP. Veja [como itemizar por parceiro.](use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner) | *4390934* |
| RevendedorMpnId | Identificador MPN do revendedor de registo para a subscrição.  |
| OrderId | Identificador único para uma encomenda na plataforma de faturação da Microsoft. Pode ser útil identificar a ordem ao contactar o suporte. Não é usado para a reconciliação. | *566890604832738111* |
| SubscriptionId | Identificador exclusivo para uma subscrição na plataforma de faturação da Microsoft. Pode ser útil identificar a subscrição ao contactar o suporte. Não é usado para a reconciliação. *Este valor não é o mesmo que o **ID de subscrição** na Consola de Administração do Parceiro. Consulte **syndicationPartnerSubscriptionNumber.*** | *usCBMgAAAAAAAIAIA* |
| SindicalizaçãoPartnerSubscriptionNumber | Identificador único para assinaturas. Um cliente pode ter várias subscrições para o mesmo plano. Esta coluna é importante para a análise de ficheiros de reconciliação. Este campo mapeia para o **ID de subscrição** na Consola de Administração de Parceiros. | *fb977ab5-test-test-test-test-24c8d9591708* |
| OfferId | Identificador de oferta única. Identificador de oferta padrão, conforme definido na tabela de preços. *Este valor não corresponde **ao ID** da Oferta da tabela de preços. Consulte **DurableOfferID** em vez disso.* | *FE616D64-E9A8-40EF-843F-152E9BB3D1* |
| DurableOfferId | Identificador de oferta durável único, conforme definido na tabela de preços. *Este valor corresponde ao **ID** da Oferta da tabela de preços.* | *1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C* |
| OfferName | O nome da oferta de serviço adquirida pelo cliente, conforme definido na tabela de preços. | *Microsoft Office 365 (Plano E3)* |
| SubscriçãoStartDate | A data de início da subscrição. A hora é sempre o início do dia, 00:00. Este campo é definido para o dia seguinte à encomenda foi submetida. Utilizado em conjunto com o **SubscriptionEndDate** para determinar: se o cliente ainda se encontra no primeiro ano da subscrição, ou se a subscrição foi renovada para o ano seguinte. | *2/1/2019 0:00* |
| SubscriçãoEndDate | A data final da assinatura. A hora é sempre o início do dia, 00:00. *Ou 12 meses mais **x** dias após a data de início* para alinhar com a data de faturação do parceiro ou *12 meses a partir da data de renovação* . Na renovação, os preços são atualizados para a lista de preços em vigor. A comunicação do cliente pode ser necessária antes da renovação automatizada. | *2/1/2019 0:00* |
| ChargeStartDate | Início do dia das acusações. A hora é sempre o início do dia, 00:00. Usado para calcular os encargos diários *(custos pro rata)* quando um cliente muda os números da licença. | *2/1/2019 0:00* |
| ChargeEndDate | Fim do dia das acusações. A hora é sempre o fim do dia, 23:59. Usado para calcular os encargos diários *(custos pro rata)* quando um cliente muda os números da licença. | *2/28/2019 23:59* |
| ChargeType | O [tipo de carga](recon-file-charge-types.md) ou ajuste. | Consulte [os tipos de carga.](recon-file-charge-types.md) |
| Preço Unitário | Preço por licença, conforme publicado na tabela de preços no momento da compra. Certifique-se de que isto corresponde às informações armazenadas no seu sistema de faturação durante a reconciliação. | *6.82* |
| Quantidade | Número de licenças. Certifique-se de que isto corresponde às informações armazenadas no seu sistema de faturação durante a reconciliação. | *2* |
| Montante | Preço total para quantidade. Usado para verificar se o cálculo da quantidade corresponde à forma como calcula este valor para os seus clientes. | *13.32* |
| TotalOtherDiscount | Montante de desconto aplicado a estes encargos. As licenças de produtos incluídas com uma competência ou MAPS, ou novas subscrições elegíveis para um incentivo, também conterão um valor de desconto nesta coluna. | *2.32* |
| Subtotal | Total antes de impostos. Verifique se o seu subtotal corresponde ao total esperado, em caso de desconto. | *11* |
| Impostos | Carga de imposto. Com base nas regras fiscais do seu mercado e circunstâncias específicas. | *0* |
| TotalForCustomer | Total após impostos. Verifica se é cobrado imposto na fatura. | *11* |
| Moeda | Tipo de moeda. Cada entidade de faturação tem apenas uma moeda. Verifique se corresponde à sua primeira fatura. Verifique novamente depois de quaisquer atualizações importantes da plataforma de faturação. | *EUR* |
| DomainName | Nome de domínio do cliente. Este campo pode parecer em branco até ao segundo ciclo de faturação. *Não utilize este campo como um identificador único para o cliente. O cliente/parceiro pode atualizar o domínio de vaidade ou predefinição através do portal Office 365.* | *example.onmicrosoft.com* |
| SubscriptionName | Apelido de assinatura. Se não for especificado qualquer apelido, o Partner Center utiliza o **Nome de Oferta** . | *PROJETO ONLINE* |
| AssinaturaDescrição | O nome da oferta de serviço adquirida pelo cliente, conforme definido na tabela de preços. (Este é um campo idêntico ao **Nome Oferta** .) | *PROJETO PREMIUM ONLINE SEM CLIENTE DO PROJETO* |
| BillingCycleType | Frequência de faturação única.| *Mensalmente* |