---
title: Compreender faturas de faturação do Partner Center
ms.topic: article
ms.date: 05/18/2020
description: Compreenda os campos no seu ficheiro de fatura para a faturação do Partner Center. Incluem-se campos e definições para todos os campos de fatura e campos de carregamento único.
author: sodeb
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5cb60c775bd8de38b8d7ca69c4dd97cf11b919fd
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110146617"
---
# <a name="understand-partner-center-billing-invoice-fields"></a>Compreenda os campos de faturação do Partner Center

**Funções adequadas**: Administração global | Administração de administração de utilizadores | Administrador de faturação | Agente helpdesk

Pode utilizar as seguintes tabelas para entender os campos nos ficheiros de fatura do Partner Center.

## <a name="invoice-file-fields"></a>Campos de arquivo de fatura

Os seguintes campos aparecem nos seus ficheiros de fatura.

| Campo | Definição |
| ----- | ---------- |
| EUA FEIN | O seu Número de Identificação do Empregador Federal (FEIN). Este é o seu número de identificador de impostos federal dos Estados Unidos. |
| Número de cliente | O seu número de cliente. |
| Faturar a | O endereço para onde enviamos a sua fatura. Pode alterar o nome e endereço da sua empresa no seu perfil de faturação do Partner Center. |
| Encargos baseados em licença | Os encargos mensais ou anuais fixos para as suas licenças de utilização adquiridas, faturadas antes do serviço. Este número é a soma de todos os encargos na coluna **Subtotal** (coluna **T)** no seu ficheiro de reconciliação baseado na licença. |
| Encargos baseados na utilização | O seu uso de Azure. Isto inclui novos serviços ou aplicações ativadas e utilizadas durante o período de faturação. Este número é a soma de todos os encargos na coluna **PretaxCharges** (coluna **Z)** no seu ficheiro de reconciliação baseado na utilização. |
| Descontos | O desconto que o cliente recebe do preço normal da subscrição. Este número é apresentado como uma *quantia plana,* não como um preço por unidade ou licença. |
| Créditos | Créditos ou ajustes para alterações efetuadas a subscrições (por exemplo, aumentos ou diminuições de licenças). |
| Subtotal | Total antes de impostos e taxas e créditos exclusivos de impostos. |
| Impostos | O imposto total para os seus encargos correntes, tal como está na secção **Detalhes** a partir da página 2 da sua fatura. Este número é a soma de todos os encargos na coluna **TaxAmount** (coluna **AA)** no seu ficheiro de reconciliação baseado em uso, e a coluna **Fiscal** (coluna **U)** no seu ficheiro de reconciliação baseado na licença. |
| Outros créditos | Créditos exclusivos de impostos. |
| Total de encargos correntes | O valor devido na sua moeda de faturação para o período de faturação. Estas despesas são devidas até à data de vencimento do pagamento. |
| Instruções de pagamento | Descrição de como pagar a sua fatura, com base na sua região. *Certifique-se sempre de que inclui o número da sua fatura ao efetuar um pagamento.* |
| Fatura não | O número da sua fatura. |
| Período de faturação | O período mensal que antecede a data da fatura. Este é o período durante o qual os serviços baseados na utilização são consumidos e os serviços baseados em licenças são reconciliados para quaisquer ajustamentos de crédito ou alterações na contagem de licenças. |
| Data da fatura | A data de faturação ou data de aniversário em que a sua fatura é gerada todos os meses. |
| Termos de pagamento | O prazo de pagamento. Para compras únicas serão sempre 60 dias. |
| Data de pagamento | A data em que o seu pagamento deve ser recebido. |
| Po do cliente | A sua ordem de compra. |
| Suporte ao cliente | O endereço do site onde pode aceder ao atendimento ao cliente. |
| Destinatário de serviço | O endereço onde o serviço está a ser utilizado. (Este é o endereço da empresa legal associado à verificação da empresa.) |

## <a name="one-time-charges-fields"></a>Campos de cargas únicas

Os seguintes campos **aplicam-se apenas** a taxas pontuais no Partner Center:

| Campo | Definição |
| ----- | ---------- |
| Date | Data de compra. |
| Description | Nome do produto. |
| Quantidade | O número de produtos (como reservas) adquiridos. |
| Preço unitário | Preço por produto (como uma reserva). |
| Descontos | Quaisquer descontos aplicáveis. |
| Valor antes de impostos | Subtotal das compras antes de impostos. |
| Imposto sobre vendas | Montante dos impostos. |
| Total | Montante total a ser pago. |
