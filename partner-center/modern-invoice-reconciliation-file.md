---
title: Recon campos de arquivo para compras únicas da CSP
ms.topic: conceptual
ms.date: 01/29/2021
description: Saiba mais sobre todos os itens do seu ficheiro de reconciliação de compra única no Partner Center, incluindo valores de amostra.
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.openlocfilehash: d5d404519c107a3e1f0e926451eef4935c993fbd
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/09/2021
ms.locfileid: "123961039"
---
# <a name="csp-one-time-purchase-reconciliation-file-fields"></a>CSP uma vez comprar campos de arquivos de reconciliação

**Funções adequadas**: Administração de contas | Agente de faturação

## <a name="using-the-recon-file"></a>Usando o ficheiro de reconhecimento
O quadro abaixo apresenta descrições e valores de amostra para os campos no ficheiro de reconciliação para compras únicas da CSP.

Para obter mais informações sobre ficheiros de reconciliação, consulte [utilizar os ficheiros de reconciliação](use-the-reconciliation-files.md).

| Coluna | Descrição | Valor da amostra |
| ------ | ----------- | ------------ |
| PartnerId | Identificador único no formato GUID para uma entidade de faturação específica. Não é necessário para a reconciliação. O mesmo em todas as filas. | *0e195b37-4574-4539-bc42-0e539b9684c0* |
| CustomerId | Identificador exclusivo da Microsoft para o cliente em formato GUID. | *196e2273-9651-43a3-ba7e-7cbcd918fc40* |
| CustomerName | Nome da organização do cliente, conforme relatado no Partner Center. Esta coluna é importante para conciliar a fatura com a informação do seu sistema. | *Johnny Modern Cust DE2* |
| Nome do Nome do Cliente | Nome de domínio do cliente. | *testcustomerdomain.onmicrosoft.com* |
| CustomerCountry | O país onde está localizado o seu cliente. Veja a lista completa [dos países](./regional-authorization-overview.md) para a sua região.  | *DE* |
| FaturaNumber | O número da fatura associado ao ficheiro de reconciliação.  | *G002297372* |
| MpnId | Identificador mpn do parceiro da CSP. Para mais informações, consulte [como itemar por parceiro.](./use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner) | *6034453* |
| RevendedorMpnId | Identificador MPN do revendedor de registo para a subscrição. | *6048879* |
| OrderId | Identificador único para uma encomenda na plataforma de faturação da Microsoft. Pode ser útil identificar a ordem ao contactar o suporte. Não é usado para a reconciliação. | *0ET2qaZvJGfF9wgSKnWzR5JLmhp10lOc1* |
| OrderDate | Data na UTC a encomenda foi feita. | *10/3/2020* |
| ProductId | O identificador único do produto. | *DZH318Z0BNZ5* |
| SkuId | O identificador único da SKU. | *006G* |
| DisponibilidadeyId | O identificador único de disponibilidade. | *DZH318Z08B80* |
| SkuName | O nome SKU. | *Tabelas - LRS* |
| NomeDoProduto | O nome do produto. | *Tabelas* |
| ChargeType | O [tipo de carga](./recon-file-charge-types.md) ou ajuste. | *Novo* |
| UnitPrice | Preço por licença, conforme publicado na tabela de preços no momento da compra. Certifique-se de que isto corresponde às informações armazenadas no seu sistema de faturação durante a reconciliação. | *0.045* |
| Quantidade | O número de licenças. Certifique-se de que isto corresponde às informações armazenadas no seu sistema de faturação durante a reconciliação. | *1* |
| Subtotal | Total antes de impostos. O subtotal deve ser igual à quantidade faturada multiplicada pelo preço unitário efetivo. | *0* |
| ImpostoTotal | Carga de imposto. Com base nas regras fiscais do seu mercado e circunstâncias específicas. | *0* |
| Total | O montante total é igual ao subtotal mais o valor do imposto. | *0* |
| Moeda | A sua conta é gerada no contexto da moeda do cliente. Isto significa que se você é um parceiro que transaciona com clientes de diferentes moedas faturantes, você receberá uma fatura para cada tipo de moeda de cliente.  | *EUR* |
| PreçoDjustmentDescription | As razões dos ajustamentos no preço unitário. Estas são as principais razões, mas não se limitam a determinar o preço unitário efetivo. | *["15,0% Parceiro ganhou crédito pelos serviços geridos"]* |
| Nome do Editor | Publisher do produto.  | *Microsoft* |
| PublisherId | Um identificador único que o Partner Center utiliza para identificar a editora. | *ND* |
| AssinaturaDescrição | O nome da oferta de serviço adquirida pelo cliente, conforme definido na tabela de preços. Esta coluna é um campo idêntico ao OfferName. | *Plano do Azure* |
| SubscriptionId | Identificador exclusivo para uma subscrição na plataforma de faturação da Microsoft. Não é usado para a reconciliação. Note que este identificador não é o mesmo que o ID de subscrição na consola de administração do parceiro. | *307628f1-d9d2-f09c-ea1f-4183f0cae308* |
| ChargeStartDate | A data em que o período de faturação de uma subscrição começa. | *9/1/2020* |
| ChargeEndDate | A data de fim do período de faturação de uma subscrição. | *30/9/2020* |
| TermAndBillingCycle | O compromisso de duração para continuar a subscrição no momento da compra. | *Dados Armazenados (GB/Mês)* |
| EffectiveUnitPrice | O preço unitário proscedido para calcular o custo do ciclo de faturação. Descontos, ajustes nos dias de faturação e outros fatores determinam o preço unitário efetivo. Para obter mais informações, consulte [o Cálculo Efetivo do Preço Unitário](./effective-unit-price-calculation.md).  | *0.03825* |
| UnitType | O tipo de unidade em que o contador é carregado. | *1 GB/Mês* |
| AlternateId | A identificação alternativa do item da linha de encomenda referenciada. | *6dc5c039750a* |
| BillableQuantity | A quantidade total a ser cobrada.  | *0.005001* |
| BillingFrequency | O plano de faturação selecionado no momento da compra. | *ND*  |
| PricingCurrency | A moeda na lista de preços. | *USD* |
| PCToBCExchangeRate | A taxa de câmbio aplicava-se à moeda de fixação de preços à moeda de faturação. | *0.846202666* |
| PCToBCExchangeRateDate | A data em que é determinada a moeda de fixação da moeda de faturação. | *30/9/2020* |
| Descrição do Medidor | Descrição do medidor.  | *Tabelas - Dados LRS Armazenados (GB/Mês)* |
| ReservationOrderId | O ID da Ordem de Reserva. | *E21A6344E398FFC1C4D7...* |
| Código CreditReason | A descrição do crédito. | *Crédito de consumo Azure* |
| SubscriçãoStartDate | A data em que uma subscrição é comprada. | *5/1/2021* |
| SubscriçãoEndDate | A data em que uma subscrição expira. | *4/30/2022* |
| ReferenceID | A ligação a todas as transações que ocorrem durante as atualizações. | *025d68a6-1bd6-42ab-9636-15e8d76a30e* |
| ProdutosQualificadores | O identificador para saber compras de Add-on ou Trial. | *["Add-on"]* |
| PromoçãoID | O identificador usa para recolher a informação da promoção. | *78bcf906-b945-4210-8818-cfb93caf12a1* |

>[!NOTE]
>Pode conciliar o seu consumo de Azure no seu ficheiro de reconhecimento de compra única. Para isso, vá ao seu arquivo de reconhecimento de utilização diária e procure a sua SubscriçãoID. Isto mostrará todos os custos associados ao seu ID do plano Azure. O seu Azure SubscriptionID é apresentado como o EntitlementID.
>

## <a name="how-to-connect-the-base-subscription-with-the-upgraded-subscription"></a>Como ligar a subscrição base com a subscrição atualizada?

Deve utilizar o ID de subscrição do produto base para encontrar os IDs de referência correspondentes e usá-los para obter todas as transações associadas. Combinado com o ID de subscrição e iD de referência, pode ligar todas as atualizações que ocorreram num único evento.

## <a name="next-steps"></a>Passos seguintes

- [Faturação e impostos](billing.md)
