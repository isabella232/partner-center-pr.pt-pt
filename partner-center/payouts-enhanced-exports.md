---
title: Página de dados de exportação de pagamentos
description: Explica como usar a página de dados de exportação melhorada para gerar relatórios de histórico de transações personalizados
author: Satinder37
ms.author: sabajaj
ms.topic: how-to
ms.date: 10/04/2021
ms.custom: template-how-to
ms.openlocfilehash: 9ac19a8ea42020b4ec2543d9f4ef197eb95e3a61
ms.sourcegitcommit: cf8c78e0c8831371432007d5ab05f934f15a77b5
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/05/2021
ms.locfileid: "129528672"
---
# <a name="payouts-export-data-page"></a>Página de dados de exportação de pagamentos
**Funções adequadas**: Incentivos administrativos | Utilizador de incentivos

Este artigo discute melhorias na experiência de exportação de dados para **pagamentos** no Partner Center. Esta experiência guiada fornece novos modelos padrão para exportar os seus relatórios de histórico de transações. Também tem a capacidade dinâmica de permitir criar os seus próprios modelos personalizados para os seus relatórios de histórico de transações.

## <a name="access-the-export-data-page"></a>Aceda à página de dados de exportação
1.  Inicie sessão no [dashboard do Centro de Parceiros](https://partner.microsoft.com/dashboard/home).
2.  Selecione **Pagamentos,** em seguida, selecione o histórico de exportação de **incentivos** ou **transações** a partir do menu.

> [!Note] 
> Você terá acesso a esta página se você é um [administrador de incentivo ou utilizador de incentivos](/payout-statement#roles-and-permissionsData). O que vê dependerá de que programa e combinações da Microsoft Partner Network (MPN) tem acesso (semelhante ao **histórico de Transações** e Páginas **de Pagamento).**

## <a name="export-your-data"></a>Exportar os seus dados
1.   Selecione o tipo de dados que pretende exportar. 
      - Para um relatório de histórico de transações, selecione **Resultados, transações, dados do estado do pagamento**.  Note que **Os dados de Resultados, transações, dados do estado de pagamento (alavancas de crescimento)** não se aplicam aos mercados comerciais. 
      - Para um relatório de pagamento, selecione **Detalhes de pagamento**.
   :::image type="content" source="images/payouts/type-of-data.png" lightbox="images/payouts/type-of-data.png" alt-text="Screenshot mostrando tipo de seleções de dados.":::

2.   Selecione um tipo de modelo de relatório.

      :::image type="content" source="images/payouts/report-template-type.png" lightbox="images/payouts/report-template-type.png" alt-text="Screenshot mostrando seleções do tipo de modelo de relatório.":::

      A sua escolha para o passo 1 determinará as opções do modelo para o passo 2. Por exemplo, se selecionar **Resultados, transações, dados de estado de pagamento** no passo 1, verá quatro opções de modelo diferentes:
      - **Histórico de transações padrão**: Este relatório mostra todos os atributos possíveis disponíveis no relatório em todos os programas (incentivos, mercados comerciais e de consumo). Este era o modelo de descarregamento que estava disponível antes de outubro de 2021.
      - **Lugar de mercado padrão**: Este relatório mostra todos os atributos necessários para os membros mpn matriculados em programas de marketplace comercial, como o Azure Marketplace. 
      - **Loja predefinida**: Este relatório mostra todos os atributos necessários para os membros MPN inscritos nos programas de loja de consumidores, tais como Microsoft Store, Minecraft e MS Flight Simulator. 
      - **Histórico de transações personalizadas**: Este relatório permite-lhe personalizar o seu relatório de histórico de transações.

      Se selecionar **Resultados, transações, dados do estado** de pagamento no passo 1, poderá selecionar o modelo **de resumo de Transação** no passo 2. Se selecionar **detalhes de pagamento** no passo 1, verá um modelo de "Pagamentos" no passo 2. Se selecionar detalhes de **receitas da AGI** no passo 1, poderá escolher entre a receita do **Programa** ou os modelos **de adicionações do Cliente** no passo 2.

3. Selecione um formato de ficheiro de relatório.
   
      :::image type="content" source="images/payouts/report-file-format.png" lightbox="images/payouts/report-file-format.png" alt-text="Screenshot mostrando seleções de formato de ficheiro de relatório.":::

4.   Escolha o seu período de tempo e aplique quaisquer outros filtros e, em seguida, selecione **Baixar os dados**.
   
      :::image type="content" source="images/payouts/time-period-filters.png" lightbox="images/payouts/time-period-filters.png" alt-text="Screenshot mostrando a seleção do período de tempo do relatório e a opção de filtro.":::

> [!Note] 
> Pode exportar dados e gerir pedidos a partir da tabela **de pedidos de descarregamento.**

## <a name="create-your-customized-transaction-history-report"></a>Crie o seu relatório de histórico de transações personalizado

Personalize o seu relatório de reconciliação do histórico de transações para se adaptar às suas necessidades. Pode criar e gerir até cinco modelos de relatório. 

1.  Selecione **+ histórico de transações personalizadas** para configurar um novo modelo de reconciliação. 
   
      :::image type="content" source="images/payouts/custom-trans-history.png" lightbox="images/payouts/custom-trans-history.png" alt-text="Screenshot mostrando configuração do histórico de transações personalizadas.":::


2.   Introduza um nome de modelo e uma breve descrição e, em seguida, selecione **Seguinte**.
   
      :::image type="content" source="images/payouts/template-name.png" lightbox="images/payouts/template-name.png" alt-text="Screenshot mostrando novos campos de modelo de reconciliação personalizada.":::


3.  Selecione as colunas de dados que gostaria de incluir e reveja as colunas predefinitivas já listadas no relatório. Selecione **Seguinte**.
   
     :::image type="content" source="images/payouts/data-selection.png" lightbox="images/payouts/data-selection.png" alt-text="Screenshot mostrando novas opções de seleção de dados do modelo de reconciliação personalizada.":::

4.  Reveja os detalhes do seu modelo e as seleções de dados, faça edições se necessário e, em seguida, **selecione Criar modelo personalizado.**
   
      :::image type="content" source="images/payouts/new-custom-template.png" lightbox="images/payouts/new-custom-template.png" alt-text="Screenshot mostrando o ecrã de confirmação para novo modelo de reconciliação personalizada.":::

5.  Selecione **Baixar** a partir do ecrã seguinte para exportar os seus dados. Também pode adicionar, editar, transferir ou eliminar outros modelos deste ecrã.
   
      :::image type="content" source="images/payouts/download-manage-templates.png" lightbox="images/payouts/download-manage-templates.png" alt-text="Screenshot mostrando modelos de gestão e opções de dados de descarregamento.":::

## <a name="next-steps"></a>Passos seguintes
- [Visão geral dos pagamentos](non-payment-fraud-misuse.md)
- [Resumo das receitas](revenue-summary.md)
- [Declaração de dividendos](payout-statement.md)
- [Questões comuns sobre pagamentos e impostos](payout-faq.yml)
