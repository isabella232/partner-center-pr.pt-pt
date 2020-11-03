---
title: Como ler o seu ficheiro de & de reconhecimento
ms.topic: article
ms.date: 06/05/2020
description: Conheça a sua fatura & ficheiros de reconciliação. A sua conta mostra as tarifas do Partner Center em todo o programa, produtos e clientes para esse período mensal.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: edb2d25b49bd5c40dfd30e9f21d2d8537a5669c4
ms.sourcegitcommit: e1c8bea4aaf807aebe99c125cb1fb6dc8fdfa210
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/30/2020
ms.locfileid: "92529379"
---
# <a name="understand-your-bill-and-reconciliation-file---learn-how-to-find-them-in-partner-center"></a>Understand your bill and reconciliation file - saiba como encontrá-los no Partner Center

**Aplica-se a**

- Partner Center
- Centro de Parceiros para Microsoft Cloud para governo dos EUA

**Funções adequadas**

- Administrador global
- Administrador de faturação
- Agente administrativo


A sua **fatura** é um **resumo de todas as tarifas do Partner Center** (em todo o programa, todos os produtos e todos os clientes). 

## <a name="invoice-types"></a>Tipos de fatura

A Microsoft emitirá uma fatura para quaisquer encargos baseados em licenças (como o Office 365) e encargos baseados na utilização (como o Azure) e uma fatura separada para encargos pontuais (como o plano Azure RI, Marketplace ou Azure).

Por exemplo,  

**Cenário 1 [Moeda Única]** : Parceiro tem compras para oferta de 145P e licenças O365,  

- O parceiro receberá uma fatura PDF e 2 ficheiros de reconciliação que cobrem as taxas tanto para o O365 como para o Azure (145p).  

**Cenário 2 [Moeda Única]** : O parceiro tem compras para o plano Azure RI, Marketplace e/ou Azure, juntamente com compras de 145p.

- O parceiro receberá um PDF de fatura e um ficheiro de reconciliação que cobre as taxas para a Azure (145p). 

- O parceiro receberá outro PDF de fatura e um ficheiro de reconciliação que cobre as suas taxas para o plano Azure RI, Marketplace, Azure. 

**Cenário 3 [Multi-Moeda]** : O parceiro tem compras para a Azure RI em plano DKK e Azure em EUROS, juntamente com compras de 145p em EUROS.

- O parceiro receberá uma fatura PDF e um ficheiro de reconciliação que cobre as taxas de Azure RI em DKK. 

- O parceiro receberá uma fatura PDF e um ficheiro de reconciliação que cobre os encargos do plano Azure em EUROS. 

- O parceiro receberá outro PDF de fatura e um ficheiro de reconciliação que cobre os seus encargos por uma oferta de 145p em EUROS (ou moeda de faturação de parceiros). 

## <a name="find-your-bill"></a>Encontre a sua conta 

Pode encontrar a sua fatura na página de Faturação do painel de instrumentos no Partner Center. Também pode encontrar o seu histórico de faturação, tendências de gastos e ficheiros de reconciliação nesta página. 

1. Inscreva-se no painel do Centro [de Parceiros.](https://partner.microsoft.com/dashboard/home) 

2. No menu da esquerda, selecione **Billing** . 

3. Na página 'Faturar', selecione a fatura que pretende transferir. 

Pode encontrar um link para a sua última fatura no topo da página no saldo da Conta a partir da data da última fatura. 

Pode encontrar faturas anteriores na secção história da Faturação. Escolha o ano apropriado e, em seguida, selecione a seta de queda ao lado do período de faturação apropriado. Selecione o link ao lado de Faturas (.pdf) para fazer o download da fatura desse período. 

## <a name="understanding-invoice-pdf"></a>Compreensão da fatura PDF 

**Faturas de Utilização e taxas baseadas em licenças** : As faturas para os encargos de serviços como o Office 365 e a Azure estarão disponíveis no prazo de dois (2) dias a contar da data de faturação selecionada [UTC].  

**Faturas para taxas únicas e recorrentes** : Faturas de encargos para serviços como Azure RI, plano Azure, Marketplace estarão disponíveis o mais tardar 8 de cada mês.  

Abaixo estão alguns dos campos-chave no documento PDF da fatura –

**Número da fatura** : Identificador único para o documento de fatura gerado para o respetivo período de faturação. 

**Período de faturação** : Este é o período durante o qual tem utilizações e serviços baseados em licenças. 

**Data da fatura** : A data de faturação ou data de aniversário em que a sua fatura é gerada todos os meses. 

**Data de vencimento** do pagamento : A data em que o seu pagamento deve ser recebido. 

**Encargos** : O valor devido na sua moeda de faturação para o respetivo período de faturação. 

**Créditos** : Créditos (como SLA) ou ajustamentos para alterações efetuadas a subscrições (por exemplo, aumentos ou diminuições de licenças). 

**Instruções de pagamento** : Descrição de como pagar a sua fatura, com base na sua região. Certifique-se sempre de que inclui o número da sua fatura ao efetuar um pagamento. 

Para obter uma descrição detalhada de todos os campos do seu ficheiro de fatura (incluindo campos para encargos pontuais), consulte [os campos de ficheiros de fatura](invoice-file.md). 

## <a name="understand-reconciliation-files"></a>Compreender ficheiros de reconciliação

 Os ficheiros de reconciliação, que fornecem um berbequim/detalhes itemizados das suas despesas, estão disponíveis para descarregar juntamente com o PDF da Fatura. Os ficheiros de reconciliação incluem identificadores de clientes e identificadores de subscrição que pode usar para criar faturas de clientes. Por favor, consulte  [como usar os ficheiros de reconciliação](use-the-reconciliation-files.md) para obter mais detalhes sobre os ficheiros de reconhecimento. 
