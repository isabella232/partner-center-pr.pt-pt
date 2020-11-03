---
title: Gerir a sua lista de clientes
ms.topic: how-to
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Os registos de clientes estão entre os ativos de informação mais importantes. Saiba como ver, pesquisar, atualizar, & informações de exportação na sua lista de clientes do Partner Center.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 40df034e88a1bba7829d6f73e0fb970795a2a0dd
ms.sourcegitcommit: 37b0b2a7141907c8d21839de3128fb8a98575886
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2020
ms.locfileid: "92529496"
---
# <a name="manage-your-customer-list---search-update-or-export-customers-in-partner-center"></a>Gerir a sua lista de clientes - pesquisar, atualizar ou exportar clientes no Partner Center

**Aplica-se a**

- Partner Center
- Centro de Parceiros para Microsoft Cloud para governo dos EUA

Os registos de clientes estão entre os seus ativos de informação mais importantes no Partner Center. Pode pesquisar a sua base de dados de contas de clientes, exportar toda a base de dados do cliente ou exportar um subconjunto para um formato de ficheiro de valor separado de vírgula compatível com o Excel (.csv). Também pode exportar as informações de subscrição de um cliente para um ficheiro .csv.

Os registos de atividade também fornecem dados exportáveis sobre transações e ações de gestão para os clientes. Para obter mais informações, consulte [os registos de atividade do cliente.](activity-logs.md)

## <a name="search-for-a-customer"></a>Pesquisar por um cliente

1.  A partir do menu **Partner Center,** selecione **Clientes.**
2.  Para procurar um cliente, insira o nome do cliente ou o nome de domínio na caixa de pesquisa.
3.  Selecione a **seta para baixo** no final de uma linha de clientes para ver o seu ID Microsoft, e as suas subscrições e links rápidos de serviços associados.

## <a name="update-a-customers-company-name"></a>Atualizar o nome da empresa de um cliente

A partir do menu **Partner Center,** selecione **Clientes.**
2.  Para procurar um cliente, insira o nome do cliente ou o nome de domínio na caixa de pesquisa.
3.  Selecione a **seta para baixo** no final de uma linha de clientes para ver o seu ID Microsoft, e as suas subscrições e links rápidos de serviços associados.
4.  Sob a informação do **cliente,** atualize o nome da empresa. Quando guardar o novo valor, este será refletido na lista de clientes. Isto só alterará o nome da empresa Bill-to e o valor da lista de clientes. Não será refletida em mais lado nenhum.

## <a name="export-your-customer-list"></a>Exporte a sua lista de clientes

1. A partir do menu **Partner Center,** selecione **Clientes.**
2. Selecione **clientes de exportação.**

   O Partner Center converte a sua lista completa de clientes num ficheiro .csv e envia-a para a pasta de descarregamento predefinido no seu computador. Também pode exportar subconjuntos de dados do cliente. As colunas de dados incluem:

   - **ID da Microsoft;**
   - **Nome da empresa;**
   - **Nome de domínio primário;**
   - **Relação** — a relação comercial do Parceiro com cada cliente listado.

    Por padrão, o Partner Center exporta toda a lista de clientes, independentemente do comprimento. Também pode pesquisar a lista de clientes pelo nome ou domínio da empresa e exportar esse subconjunto de dados.

3. Se for um fornecedor indireto, pode filtrar a sua lista de clientes por revendedor indireto. Selecione **Filtro por revendedor indireto** da lista e, em seguida, escolha um revendedor.


## <a name="export-customer-subscription-information"></a>Informação sobre subscrição de clientes de exportação

1. A partir do menu **Partner Center,** selecione **Clientes.**

2. Selecione o **nome da Empresa** para qualquer cliente. A página **de Subscrições** do cliente abre, mostrando a sua lista completa de subscrições de produtos.

3. Selecione **subscrições de exportação** . O Partner Center converte os dados de subscrição do cliente num ficheiro .csv e envia-os para a pasta de descarregamento predefinido no seu computador. As colunas de dados incluem:
   - **ID de assinatura;**
   - **Subscrição** — o nome do produto para a subscrição;
   - **Quantidade** — número de licenças adquiridas;
   - **Estado;**
   - **Revendedor** — o ID do revendedor que detém e gere a subscrição.

> [!NOTE]  
> Para obter mais informações sobre a gestão da subscrição, consulte [as subscrições do Cliente.](customer-subscriptions.md)
