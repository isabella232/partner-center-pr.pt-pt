---
title: Taxas e taxas regionais do PSTN
description: Como parceiro Office 365 que transaciona produtos Microsoft 365 Voice, poderá estar sujeito a impostos regionais, taxas ou requisitos regulamentares para os serviços PSTN.
ms.topic: article
ms.date: 09/10/2020
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 228534aff70db5c60116d408550361477da7302b784c78ea746cd2ae017c70a0
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/06/2021
ms.locfileid: "115691672"
---
# <a name="regional-taxes-regulations-for-public-switched-telephone-network-ptsn-services"></a>Impostos regionais, regulamentos para serviços de Rede Telefónica Comutado Público (PTSN)

**Funções adequadas**: Administração global | Administração de utilizadores | Agente administrativo

Os serviços da Rede Telefónica Comutado Público (PSTN) em algumas jurisdições podem estar sujeitos a requisitos fiscais e regulamentares especiais que possam afetar a ordem e faturação dos parceiros. Nos Estados Unidos, incluindo Porto Rico, os serviços PSTN, que incluem Audio Conferencing, Call Plans e Créditos de Comunicação, estão sujeitos a requisitos fiscais e regulamentares especiais. Nos Estados Unidos e porto Rico, a Microsoft avalia os serviços PSTN como impostos inclusivos.  Os impostos e regulamentos exclusivos da PSTN afetarão Office 365 parceiros que transfiram produtos Microsoft 365 Voice.  Se um parceiro marcar o preço de um Serviço PSTN da Microsoft, poderá ser responsável pelo cálculo e remissão de impostos e taxas PSTN.

## <a name="partner-recommendations"></a>Recomendações de parceiros

Envolva o seu conselho fiscal e jurídico para compreender a responsabilidade da sua organização em relação à regulação, impostos e taxas dos serviços pstn, bem como outras responsabilidades potenciais.

## <a name="invoice-presentation-and-partner-reconciliation-file"></a>Arquivo de apresentação de fatura e reconciliação de parceiros

Fornecedor de Soluções em Nuvem faturas (CSP) e ficheiros de reconciliação CSP nos Estados Unidos, Porto Rico e Canadá, que incluem Skype para Empresas serviços PSTN e Microsoft 365 Voice, fornecerão itens de linha separados para os componentes PSTN e não PSTN.

Além disso, as faturas CSP apresentarão a seguinte nota de rodapé:

* O preço apresentado é um custo para serviços de Audio Conferencing e Call Plan Services.  Os impostos transacionais aplicáveis são cobrados exclusivamente do montante indicado, com exceção das vendas efetuadas nos Estados Unidos.  Nos EUA, o preço apresentado é tax inclusive, uma vez que inclui uma taxa para o Plano de Chamada e Serviços de Conferência sonora e um custo pelos impostos e taxas que somos obrigados a cobrar.  Os Serviços de Conferência sonora e De Chamada são servidos pela Microsoft Affiliate autorizada a fornecê-los.  Veja o [Licenciamento em Volume da Microsoft](https://go.microsoft.com/fwlink/?LinkId=690247) para obter detalhes.

## <a name="reconciliation-file-example"></a>Exemplo de arquivo de reconciliação

Office 365 Enterprise A E5 apresenta no ficheiro de reconciliação dois itens de linha com nomes idênticos e IDs idênticos, mas cada item de linha tem um preço unitário único (exemplo: $28,40 e $2,00). Isto separa a componente de conferência Skype para Empresas PSTN da oferta de Office 365, para que possa aplicar corretamente os impostos.

**Exemplo de reconciliação de parceiros #1 (selecionar colunas):**

|**Durable_offer_ID**|**Offer_Name**|**Subscription_Start_Date**|**Subscription_End_Date**|**Charge_Start_Date**|**Charge_End_Date**|**Charge_Type**|**Unit_Price**|
|:----:|:----:|:----:|:----:|:----:|:----:|:----:|:----:|
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 Enterprise E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00|9/10/2019 0:00   |Taxa de ciclo   |28,40   |
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 Enterprise E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00   |9/10/2019 0:00   |Taxa de ciclo   |2.00   |

**Exemplo de reconciliação de parceiros #2**

Microsoft 365 Voz Para Empresas disponível no Canadá tem componentes tributáveis PSTN adicionais que são consolidados na Fatura CSP (semelhante a Office 365 E5, são apresentados dois itens de linha, um para componentes PSTN e outro para componentes não PSTN).  O ficheiro de reconciliação da CSP para Microsoft 365 Voz Para Empresas apresentará individualmente todos os componentes tributáveis pstn (componentes PSTN individuais não serão consolidados em .CSV ou API).  A soma dos dados da encomenda e dos montantes cobrados para os clientes encontrados no ficheiro de reconciliação corresponderá à Fatura CSP.

## <a name="additional-resources"></a>Recursos Adicionais
Para mais detalhes, visite o [site Microsoft 365 para Parceiros.](https://www.microsoft.com/microsoft-365/partners/)

