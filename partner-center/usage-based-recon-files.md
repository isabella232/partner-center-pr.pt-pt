---
title: Ficheiros de reconciliação baseados em uso
ms.topic: article
ms.date: 06/08/2020
description: Saiba mais sobre todos os itens do seu ficheiro de reconciliação baseado no uso no Partner Center. Inclui alguns exemplos.
author: sodeb
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 6c486d4866b0a2a912801d2648a1822418687078
ms.sourcegitcommit: bce54ddb9fff7332a03d6aa228ba9414a87d76b7
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/22/2021
ms.locfileid: "112431703"
---
# <a name="understand-usage-based-reconciliation-files-and-their-specific-fields-in-partner-center"></a>Compreenda os ficheiros de reconciliação baseados no uso e os seus campos específicos no Partner Center

**Funções adequadas**: Administração de contas | Administrador de faturação

Para conciliar os seus encargos com a utilização de um cliente, compare o **ResellerID,** **o ResellerName** e o **ResellerBillableAccount** do ficheiro de reconciliação com o **nome do Cliente** e **iD** de assinatura do Partner Center.

## <a name="fields-in-usage-based-reconciliation-files"></a>Campos em ficheiros de reconciliação baseados na utilização

Os seguintes campos explicam quais os serviços utilizados e a taxa.

| Coluna | Descrição | Valor da amostra |
| ------ | ----------- | ------------ |
| PartnerId | Identificador de parceiro, em formato GUID. | *DA41BC5F-C52D-4464-8A8D-8C8DCC43503B* |
| PartnerName | Nome do parceiro. | *Contoso, Ltd.* |
| PartnerBillableAccountId | Identificador de conta de parceiro. | *1010578050* |
| Nome da Empresa de Clientes | Nome da organização do cliente, conforme relatado no Partner Center. *Isto é muito importante para conciliar a fatura com a informação do seu sistema.* | *Cliente de teste* |
| MpnId | Identificador da Microsoft Partner Network (MPN) do parceiro Cloud Solution Provider (CSP). | *4390934* |
| RevendedorMpnId | Identificador MPN do revendedor de registo para a subscrição.  |
| FaturaNumber | Número de fatura onde aparece a transação especificada. | *D020001IVK* |
| ChargeStartDate | Data de início do ciclo de faturação, exceto quando apresentar datas de dados de utilização latente previamente não cobrados (do ciclo de fatura anterior). A hora é sempre o início do dia, 00:00. | *2/1/2019 0:00* |
| ChargeEndDate | Data de fim do ciclo de faturação, exceto quando apresentar datas de dados de utilização latente previamente não cobrados (do ciclo de fatura anterior). A hora é sempre o fim do dia, 23:59. | *2/28/2019 23:59* |
| SubscriptionId | Identificador exclusivo para uma subscrição na plataforma de faturação da Microsoft. Pode ser útil identificar a subscrição ao contactar o suporte. Não é usado para a reconciliação. *Isto não é o mesmo que o **ID de subscrição** na Consola de Administração do Parceiro.* | *usCBMgAAAAAAAIAIA* |
| SubscriptionName | Apelido para a oferta de serviço. | *Microsoft Azure* |
| AssinaturaDescrição | Linha de negócios da oferta de serviços. | *Microsoft Azure* |
| OrderID | Identificador único para uma encomenda na plataforma de faturação da Microsoft. Pode ser útil identificar a subscrição ao contactar o suporte. Não é usado para a reconciliação. | *566890604832738111* |
| ServiceName | O nome do serviço Azure em questão. | *MÁQUINAS VIRTUAIS* |
| ServiceType | O tipo específico de serviço Azure. | *Service Bus – Individual or Pack*, BASE de *dados SQL Azure – Business or Web Edition* |
| ResourceGuid | Identificador exclusivo específico para todos os dados de serviço e estrutura de preços. | *DA41BC5F-C52D-4464-8A8D-8C8DCC43503B* |
| ResourceName | O nome do recurso Azure. | *Transferência de dados em (GB)*, *Transferência de Dados (GB)* |
| Region | A região à qual se aplica o uso. Principalmente usado para atribuir taxas a transferências de dados, porque as taxas variam por região. | *Ásia Pacífico*, *Europa*, *América Latina,* *América do Norte* |
| Sku | Identificador exclusivo da Microsoft para uma oferta. | *7UD-00001* |
| DetalheLineItemId | Um identificador e quantidade para itemizar diferentes tarifas para um serviço ou recurso num determinado período de faturação. Para o preço hierárquico Azure, pode haver uma taxa para até uma certa quantidade de unidades faturadas, em seguida, uma taxa diferente após essa quantidade. | *1* |
| ConsumedQuantity | A quantidade de serviço consumida (por exemplo, horas ou GB) durante o período de reporte. Também inclui qualquer utilização não mediada de períodos de reporte anteriores. | *11* |
| IncludedQuantity | Unidades incluídas como parte da oferta. Normalmente não está presente na CSP. | *0* |
| Excesso de sobreaquidadeQuantidade | Unidades não incluídas como parte da oferta. Estes devem ser pagos pelo parceiro. Igual **aQuantidade Consumida** menos **IncluaQuantidade**. | *11* |
| ListPrice | Preço de oferta em vigor na data de início da subscrição. | *$0.0808* |
| Pré-impostos | Igual a **ListPrist** multiplicado por **OverageQuantity,** arredondado para o cent mais próximo. | *$0,085* |
| TaxAmount | Valor dos impostos cobrado. Com base nas regras fiscais do seu mercado e circunstâncias específicas. | *$0,08* |
| PostTaxTotal | Total após impostos, quando o imposto é aplicável. | *$0,93* |
| Moeda | Tipo de moeda. Cada entidade de faturação tem apenas uma moeda. Verifique se corresponde à sua primeira fatura e depois após quaisquer atualizações importantes da plataforma de faturação. | *EUR* |
| Imposto Pré-Impostor | Preço pré-imposto por unidade. Igual a **PretaxCharges** dividido por **OverageQuantity,** arredondado para o cent mais próximo. | *$0,08* |
| Pós-Comoramento Ineficaz | Preço do imposto postal por unidade. Igual a **PostTaxTotal** dividido por **OverageQuantity,** arredondado para o centés mais próximo. Ou, igual a **PretaxEffectiveRate** mais a taxa de imposto por valor unitário, arredondada para o centésta mais próximo. | *$0,08* |
| ChargeType | O [tipo de carga](recon-file-charge-types.md) ou ajuste. | Consulte [os tipos de carga.](recon-file-charge-types.md) |
| CustomerId | Identificador exclusivo da Microsoft para o cliente, em formato GUID. | *ORDDC52E52FDEF405786F0642D0108BE4* |
| DomainName | Nome de domínio do cliente. Este campo pode parecer em branco até ao segundo ciclo de faturação. | *example.onmicrosoft.com* |
| BillingCycleType | Frequência de faturação de tempo.| **Mensalmente**  |
| Unidade | A unidade do **nome** de recurso . | *GB* ou *HORAS* |
| Contabillável do Cliente | Identificador de conta único na plataforma de faturação da Microsoft. | *1280018095* |
| UsageDate | Data de implantação de serviço. | *2/1/2019 0:00* |
| Região Medido | Identifica a localização de um centro de dados na região (para serviços onde este valor é aplicável e povoado). | *Leste asiático*, *Sudeste Asiático*, *Norte da Europa*, Europa *Ocidental*, Norte *Central EUA*, Centro Sul *dos EUA* |
| Serviço Medido | Identifica o uso do serviço Azure individual quando não está especificamente identificado na coluna **ServiceName.** Por exemplo, as transferências de dados são reportadas como *Microsoft Azure - Todos os Serviços* na coluna **ServiceName.** | *AccessControl*, *CDN*, *Compute,* *Database*, *ServiceBus,* *Storage* |
| MedidoServiceType | Subposição para o campo **MeteredService** que fornece esclarecimentos adicionais sobre a utilização do serviço Azure. | *EXTERNA* |
| Project | Nome definido pelo cliente para a sua instância de serviço. | *ORDDC52E52FDEF405786F0642D0108BE4* |
| ServiceInfo | O número de ligações Azure Service Bus que foram a provisionadas e utilizadas num determinado dia. | *1.000000 Ligações / 30 dias* (se tivesse uma ligação individualmente a provisionada durante um mês de 30 dias), *25 Ligações / 30 Dias – Usado: 1.000000* (se tivesse um pacote de 25 ligações de Service Bus provisidas e utilizasse 1 durante esse dia) |

## <a name="next-steps"></a>Passos seguintes

- [Compreenda os campos em ficheiros de reconciliação baseados em licenças do Partner Center](license-based-recon-files.md)