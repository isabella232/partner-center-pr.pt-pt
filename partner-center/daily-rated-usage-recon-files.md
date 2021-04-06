---
title: Ficheiros de reconciliação de utilização diária
ms.topic: article
ms.date: 06/12/2020
description: Saiba como ler ficheiros de reconciliação de utilização diários no Partner Center. Inclui descrições para campos específicos no ficheiro de reconhecimento.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 89080cb580d9b451454d108c6ef0ce0a08c1bf0c
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441902"
---
# <a name="learn-how-to-read-daily-rated-usage-reconciliation-files-in-partner-center"></a>Saiba como ler ficheiros de reconciliação de utilização diária no Partner Center

**Aplica-se a**

- Centro de Parceiros do Microsoft Cloud for US Government

**Funções adequadas**

- Agente administrativo
- Administrador de faturação
- Agente comercial
- Agente helpdesk

Este artigo explica como ler ficheiros de reconciliação de utilização diária.

>[!NOTE]
>O uso diário normalmente demora 24 horas a aparecer no Partner Center ou a ser acedido através da API.

## <a name="fields-in-daily-rated-usage-reconciliation-files"></a>Campos em ficheiros de reconciliação de utilização cotados diariamente

| Coluna | Descrição |
| ------ | ----------- |
| PartnerId | Identificador de parceiros no formato GUID. |
| PartnerName | Nome do parceiro. |
| CustomerId | Identificador exclusivo da Microsoft para o cliente em formato GUID. |
| CustomerName | Nome da organização do cliente, conforme relatado no Partner Center. *Esta coluna é importante para conciliar a fatura com a informação do seu sistema.* |
| Nome do Nome do Cliente | O nome de domínio do cliente. |
| CustomerCountry | O país em que o cliente está localizado. |
| MpnId | Identificador mpn do parceiro da CSP. |
| Tier2MpnId | Identificador MPN do revendedor de registo para a subscrição. |
| FaturaNumber | Número de fatura onde aparece a transação especificada. |
| ProductId | O identificador do produto. |
| SkuId | O identificador de um SKU em particular. |
| DisponibilidadeyId | O identificador para a disponibilidade de um SKU em particular. Esta coluna mostra se o SKU está disponível para compra no país dado, moeda, segmento da indústria, etc. |
| SkuName | O título de um SKU em particular. |
| NomeDoProduto | O nome do produto. |
| Nome do Editor | O nome da editora. |
| PublisherId | O identificador da editora em formato GUID. |
| AssinaturaDescrição | O nome da oferta de serviço adquirida pelo cliente, conforme definido na tabela de preços. (Esta coluna é um campo idêntico ao **Nome Offer).** |
| SubscriptionId | Identificador exclusivo para uma subscrição na plataforma de faturação da Microsoft. Não é usado para a reconciliação. *Este identificador não é o mesmo que o **ID de subscrição** na consola de administração do parceiro.* |
| ChargeStartDate | Data de início do ciclo de faturação (exceto quando apresentar datas de dados de utilização latente previamente não cobrados do ciclo de faturação anterior). A hora é sempre o início do dia, 00:00. |
| ChargeEndDate | Data de fim do ciclo de faturação (exceto quando apresentar datas de dados de utilização latente previamente não cobrados do ciclo de faturação anterior). A hora é sempre o fim do dia, 23:59. |
| UsageDate | Data de utilização do serviço. |
| Medidor deTipo | O tipo de medidor. |
| MeterCategory | O serviço de nível superior para a utilização. |
| MeterId | O identificador do medidor que está a ser usado. |
| MeterSubCategory | O tipo de serviço Azure, que pode afetar a taxa. |
| MeterName | A unidade de medida para o contador que está a ser consumido. |
| MeterRegion | Esta coluna identifica a localização de um centro de dados na região para serviços onde a MeterRegion é aplicável e povoada. |
| Unidade | A unidade do **nome** de recurso . |
| ResourceLocation | O centro de dados onde o contador está a funcionar. |
| ConsumedService | O serviço de plataforma Azure que usou. |
| ResourceGroup | Representa um contentor que detém recursos relacionados para uma solução Azure. |
| RecursoURI | O URI do recurso que está a ser utilizado. |
| ChargeType | O tipo de custo ou ajuste.  |
| UnitPrice | Preço por licença, conforme publicado na tabela de preços no momento da compra. Certifique-se de que este preço corresponde às informações armazenadas no seu sistema de faturação durante a reconciliação. |
| Quantidade | Número de licenças. Certifique-se de que este preço corresponde às informações armazenadas no seu sistema de faturação durante a reconciliação. |
| UnitType | O tipo de unidade em que o contador é carregado.  |
| BillingPreTaxTotal | Valor total da faturação antes de impostos.<br/> _**BillingPreTaxTotal** = FLOOR([ [ @EffectiveUnitPrice *@Quantity* @PCToBCExchangeRate [], 2)_ |
| BillingCurrency | A moeda na região geográfica do cliente. |
| PreçosPreTaxTotal | O preço, antes de serem adicionados impostos. |
| PricingCurrency | A moeda na lista de preços. |
| ServiceInfo1 | O número de ligações de Service Bus que foram a provisionadas e utilizadas num determinado dia. |
| ServiceInfo2 | Um campo legado que captura metadados opcionais específicos do serviço. |
| Etiquetas | Representa uma organização lógica de recursos Azure definida pelo utilizador. |
| AdditionalInfo | Qualquer informação adicional não abrangida noutras colunas. |
| EffectiveUnitPrice | O valor real cobrado por unidade, incluindo quaisquer descontos, ganhou crédito, e assim por diante. |
| PCToBCExchangeRate | Taxa de câmbio aplicada para a moeda de fixação de moeda à moeda de faturação. |
| PCToBCExchangeRateDate | A data em que é determinada a moeda de fixação da moeda de faturação. |
| Direitodid | Representa o ID de subscrição Azure. |
| DireitosDescrição | Representa o nome do ID de assinatura Azure. |
| PartnerEarnedCreditPercentage | Apresenta o PartnerEarnedCredit para o item da linha. O crédito adquirido será de 0 ou 15 por cento |
| CreditPercentage | Exibe o Crédito de Consumo Azure. O crédito ganho será de 0 ou 100 por cento. |
| CréditoType | Tipo de crédito. Por exemplo, **a Azure Credit Applied.** |
>[!NOTE]
>O uso diário normalmente leva 24 horas para aparecer no Partner Center ou para ser acedido através da API.


