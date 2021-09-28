---
title: Compreenda o seu projeto de lei e arquivo de reconciliação
ms.topic: article
ms.date: 09/27/2021
description: Saiba mais sobre a sua fatura & ficheiros de reconciliação. A sua conta mostra as tarifas do Partner Center em todo o programa, produtos e clientes para esse período mensal.
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: df1e7f4aa34c44f0fcb030cda3df1d6f9cb241f9
ms.sourcegitcommit: e1da62b36420d78bf44e3962358d0af65ebc3402
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/27/2021
ms.locfileid: "129089526"
---
# <a name="understand-your-bill-and-reconciliation-file---learn-how-to-find-them-in-partner-center"></a>Understand your bill and reconciliation file - saiba como encontrá-los no Partner Center

**Funções adequadas**: Administração global | Administrador de faturação | Agente administrativo

A sua fatura é um resumo de todas as tarifas do Seu Centro de Parceiros em todo o programa, todos os produtos e todos os clientes.

## <a name="find-your-bill-and-reconciliation-file"></a>Encontre o seu projeto de lei e arquivo de reconciliação

Pode encontrar a sua fatura na página de Faturação do painel de instrumentos no Partner Center. Também pode encontrar o seu histórico de faturação, tendências de gastos e ficheiros de reconciliação nesta página.

> [!NOTE]
> Para saber mais sobre a interface de espaços de trabalho, consulte [o Centro de Parceiros.](get-around-partner-center.md#turn-workspaces-on-and-off)

#### <a name="workspaces-view"></a>[Vista de espaços de trabalho](#tab/workspaces-view)

1. Inicie sessão no [dashboard do Centro de Parceiros](https://partner.microsoft.com/dashboard/home).

2. Selecione o **azulejo de Faturação.**

3. Selecione uma fatura ou ficheiro de reconciliação para visualizar informações mais detalhadas.

Pode encontrar um link para a sua última fatura no topo da página no saldo da Conta a partir da data da última fatura.

Pode encontrar faturas anteriores na secção história da Faturação. Escolha o ano apropriado e, em seguida, selecione a seta de queda ao lado do período de faturação apropriado. Selecione o link ao lado das Faturas (.pdf) para fazer o download da fatura desse período.

#### <a name="current-view"></a>[Vista atual](#tab/current-view)

1. Inicie sessão no [dashboard do Centro de Parceiros](https://partner.microsoft.com/dashboard/home).

2. No menu da esquerda, selecione **Billing**.

3. Na página de estado de faturação, selecione uma fatura ou um ficheiro de reconciliação para ver informações mais detalhadas.

Pode encontrar um link para a sua última fatura no topo da página no saldo da Conta a partir da data da última fatura.

Pode encontrar faturas anteriores na secção história da Faturação. Escolha o ano apropriado e, em seguida, selecione a seta de queda ao lado do período de faturação apropriado. Selecione o link ao lado das Faturas (.pdf) para fazer o download da fatura desse período.

* * *

## <a name="invoice-types"></a>Tipos de fatura

A Microsoft emitirá uma fatura para quaisquer encargos baseados em licenças (como Office 365) e encargos baseados em uso (como Azure) e uma fatura separada para taxas pontuais (como Azure RI, Marketplace ou Plano Azure).

Por exemplo,  

**Cenário 1 [Moeda Única]**: O parceiro tem compras para oferta de 145P e licenças de Office 365,  

- O parceiro receberá um PDF de fatura e dois ficheiros de reconciliação que cobrem as acusações tanto para Office 365 como para a Azure (145p).  

**Cenário 2 [Moeda Única]**: O parceiro tem compras para o plano Azure RI, Marketplace e/ou Azure juntamente com compras de 145p.

- O parceiro receberá uma fatura PDF e um ficheiro de reconciliação que cobre as acusações de Azure (145p). 

- O parceiro receberá outro PDF de fatura e um ficheiro de reconciliação que cobre os seus encargos para a instância reservada do Azure (RI), Marketplace, plano Azure. 

**Cenário 3 [Multi-Moeda]**: O parceiro tem compras para a Azure RI em plano DKK e Azure em EUROS, juntamente com compras de 145p em EUROS.

- O parceiro receberá uma fatura PDF e um ficheiro de reconciliação que cobre as taxas da Azure RI em DKK. 

- O parceiro receberá uma fatura PDF e um ficheiro de reconciliação que cobre os encargos do plano Azure em EUROS. 

- O parceiro receberá outro PDF de fatura e um ficheiro de reconciliação que cobre os seus encargos por uma oferta de 145p em EUROS (ou moeda de faturação de parceiros). 

## <a name="understanding-invoice-pdf"></a>Compreensão da fatura PDF 

**Faturas de Utilização e taxas baseadas em licenças**: As faturas para os encargos de serviços como Office 365 e Azure estarão disponíveis no prazo de dois (2) dias a contar da data de faturação selecionada [UTC].  

**Faturas para taxas únicas e recorrentes**: Faturas para taxas para serviços como Azure RI, plano Azure, Marketplace estarão disponíveis o mais tardar no oitavo de cada mês.  

Abaixo estão alguns dos campos-chave no documento PDF da fatura –

**Número da fatura**: Identificador único para o documento de fatura gerado para o respetivo período de faturação. 

**Período de faturação**: Este é o período durante o qual tem utilizações e serviços baseados em licenças. 

**Data da faturação**: A data de faturação ou data de aniversário em que a sua fatura é gerada todos os meses. 

**Data de vencimento** do pagamento : A data em que o seu pagamento deve ser recebido. 

**Encargos**: O valor devido na sua moeda de faturação para o respetivo período de faturação. 

**Créditos**: Créditos (como contrato de nível de serviço (SLA)) ou ajustamentos para alterações efetuadas a subscrições (por exemplo, aumentos ou diminuições de licenças). 

**Instruções de pagamento**: Descrição de como pagar a sua fatura, com base na sua região. Certifique-se sempre de que inclui o número da sua fatura ao efetuar um pagamento. 

Para obter uma descrição detalhada de todos os campos do seu ficheiro de fatura (incluindo campos para encargos pontuais), consulte [os campos de ficheiros de fatura](invoice-file.md). 

## <a name="understand-reconciliation-files"></a>Compreender ficheiros de reconciliação

 Os ficheiros de reconciliação, que fornecem um berbequim/detalhes itemizados das suas despesas, estão disponíveis para descarregar juntamente com o PDF da Fatura. Os ficheiros de reconciliação incluem identificadores de clientes e identificadores de subscrição que pode usar para criar faturas de clientes. Para obter mais informações sobre ficheiros de reconciliação, consulte [Como utilizar os ficheiros de reconciliação](use-the-reconciliation-files.md). 

## <a name="next-steps"></a>Passos seguintes

- [Como usar os ficheiros de reconciliação](use-the-reconciliation-files.md)