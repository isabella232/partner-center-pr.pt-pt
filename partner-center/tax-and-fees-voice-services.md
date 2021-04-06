---
title: Taxas e taxas regionais do PSTN
description: Como parceiro do Office 365 que transaciona produtos microsoft 365 Voice, pode estar sujeito a impostos regionais, taxas ou requisitos regulamentares para serviços PSTN.
ms.topic: article
ms.date: 09/10/2020
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 411932923e6bd35732e64521abe567f40f7499e9
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441494"
---
# <a name="regional-taxes-regulations-for-public-switched-telephone-network-ptsn-services"></a>Impostos regionais, regulamentos para serviços de Rede Telefónica Comutado Público (PTSN)

**Funções adequadas**

- Administrador global
- Administrador de utilizadores
- Agente administrativo

Os serviços da Rede Telefónica Comutado Público (PSTN) em algumas jurisdições podem estar sujeitos a requisitos fiscais e regulamentares especiais que possam afetar a ordem e faturação dos parceiros. Nos Estados Unidos, incluindo Porto Rico, os serviços PSTN, que incluem Audio Conferencing, Call Plans e Créditos de Comunicação, estão sujeitos a requisitos fiscais e regulamentares especiais. Nos Estados Unidos e porto Rico, a Microsoft avalia os serviços PSTN como impostos inclusivos.  Os impostos e regulamentos exclusivos da PSTN afetarão os parceiros do Office 365 que transacionam produtos Microsoft 365 Voice.  Se um parceiro marcar o preço de um Serviço PSTN da Microsoft, poderá ser responsável pelo cálculo e remissão de impostos e taxas PSTN.

## <a name="partner-recommendations"></a>Recomendações de Parceiros

Envolva o seu conselho fiscal e jurídico para compreender a responsabilidade da sua organização em relação à regulação, impostos e taxas dos serviços pstn, bem como outras responsabilidades potenciais.

## <a name="invoice-presentation-and-partner-reconciliation-file"></a>Arquivo de apresentação de fatura e reconciliação de parceiros

As faturas de CSP e os ficheiros de reconciliação da CSP nos Estados Unidos, Porto Rico e Canadá, que incluem o Skype para os serviços de pstn empresarial e microsoft 365 Voice, fornecerão itens de linha separados para os componentes PSTN e não PSTN.

Além disso, as faturas CSP apresentarão a seguinte nota de rodapé:

* O preço apresentado é um custo para serviços de Audio Conferencing e Call Plan Services.  Os impostos transacionais aplicáveis são cobrados exclusivamente do montante indicado, com exceção das vendas efetuadas nos Estados Unidos.  Nos EUA, o preço apresentado é tax inclusive, uma vez que inclui uma taxa para o Plano de Chamada e Serviços de Conferência sonora e um custo pelos impostos e taxas que somos obrigados a cobrar.  Os Serviços de Conferência sonora e De Chamada são servidos pela Microsoft Affiliate autorizada a fornecê-los.  Veja o [Licenciamento em Volume da Microsoft](https://go.microsoft.com/fwlink/?LinkId=690247) para obter detalhes.

## <a name="reconciliation-file-example"></a>Exemplo de arquivo de reconciliação

O Office 365 Enterprise E5 apresenta no ficheiro de reconciliação dois itens de linha com nomes idênticos e IDs idênticos, mas cada item de linha tem um preço unitário único (exemplo: $28,40 e $2,00). Isto separa o Componente de Conferências do Skype para negócios PSTN conferenciação da oferta do Office 365, para que possa aplicar corretamente os impostos.

**Exemplo de reconciliação de parceiros #1 (selecionar colunas):**

|**Durable_offer_ID**|**Offer_Name**|**Subscription_Start_Date**|**Subscription_End_Date**|**Charge_Start_Date**|**Charge_End_Date**|**Charge_Type**|**Unit_Price**|
|:----:|:----:|:----:|:----:|:----:|:----:|:----:|:----:|
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 Enterprise E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00|9/10/2019 0:00   |Taxa de ciclo   |28,40   |
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 Enterprise E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00   |9/10/2019 0:00   |Taxa de ciclo   |2.00   |

**Exemplo de reconciliação de parceiros #2**

O Microsoft 365 Business Voice disponível no Canadá tem componentes tributáveis PSTN adicionais que são consolidados na Fatura CSP (semelhante ao Office 365 E5, são apresentados dois itens de linha, um para componentes PSTN e outro para componentes não PSTN).  O ficheiro de reconciliação CSP para o Microsoft 365 Business Voice apresentará individualmente todos os componentes tributáveis pstn (os componentes PSTN individuais não serão consolidados em . Ferramenta CSV ou API).  A soma dos dados da encomenda e dos montantes cobrados para os clientes encontrados no ficheiro de reconciliação corresponderá à Fatura CSP.

## <a name="additional-resources"></a>Recursos Adicionais
Para mais detalhes, visite o site [da Microsoft 365 para Parceiros.](https://www.microsoft.com/microsoft-365/partners/)

