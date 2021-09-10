---
title: Encontre a contagem do ambiente de trabalho e o nível de taxa
ms.topic: how-to
ms.date: 02/18/2021
description: Saiba como usar a plataforma Channel Incentives (CHIP) para encontrar a contagem de desktop e informações de nível de taxas para um acordo.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 288e4ebb224d3ff1b0d4050691b733e678ec29a3
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/09/2021
ms.locfileid: "123961259"
---
# <a name="locate-the-desktop-count-and-fee-level-for-an-agreement"></a>Localizar a contagem de computadores e o nível de honorários de um contrato

**Funções apropriadas**: Contacto primário ou administrador de programas

Pode iniciar sessão na [explore.ms](https://www.explore.ms/) para rever o contrato ou descarregar um ficheiro que forneça detalhes do acordo para a contagem de desktop e nível de taxas.

## <a name="to-locate-the-information"></a>Para localizar a informação

### <a name="method-1--explorems"></a>Método 1 - Explore.ms

1. Abra [explore.ms](https://www.explore.ms/) no Internet Explorer. 

>[!Note]
>Não é possível desempenhar esta função no Google Chrome ou Microsoft Edge.

2. Faça login na sua conta Work/School ou iD ao vivo.  

3. No campo **Relatórios,** selecione **Acordos**.

4. Na página resultante, introduza o número do contrato no campo **Procurar** e, em seguida, selecione **Select/Order Columns**.

5. Na janela pop-up, selecione **'Contagem de ambiente de trabalho'** da lista de colunas disponíveis e, em seguida, selecione a seta direita para adicionar a coluna. Selecione **OK**.

6. Selecione **Pesquisar.**

7. No ecrã resultante, percorra os resultados para encontrar a coluna **Contagem de Ambiente de Trabalho do Acordo.** 

8. Utilize a contagem de ambiente de trabalho para determinar o nível de taxa com base na tabela de tarifas abaixo.  

| Nível de taxa | Contagem de ambientes de trabalho |
| ------ | :-----------: |
|  A | 0 – 2,399    |
|  B | 2,400 – 5,999    |
|  C | 6,000 – 14,999    |
|  D | 15,000+   |

>[!NOTE]
>Os níveis de Incentivo empresarial baseiam-se no ambiente de trabalho ou na contagem de utilizadores (o que for mais elevado) nas matrículas do Sector Comercial e Público (PS). Para inscrições sem ambiente de trabalho ou contagem de utilizadores associados naturais, a Microsoft aplica uma contagem de ambiente de trabalho com base na contagem de desktop ou contagem de utilizadores da EA que o acompanha. <br><br>Se não houver EA acompanhante, o Nível de Taxa baseia-se no nível de preços da inscrição. O nível de preços do negócio também pode ser visto em [www.explore.ms](https://www.explore.ms/). <br><br>Se existirem vários níveis de pool e/ou preços no EA/EAS existente, a Microsoft pagará incentivos ao nível mais elevado de preços/piscinas atribuídos, sendo o nível A o mais baixo e o nível D o mais elevado.

#### <a name="pool-and-pricing-levels"></a>Níveis de Piscina e Preços

Depois de procurar o número do contrato em explore.ms utilizando os passos acima descritos, selecione o número do contrato. Isto irá levá-lo à página de detalhes do contrato, que mostrará o Resumo do **Acordo** e **Ofertas.** A secção de ofertas contém os níveis de preços.

## <a name="method-2---chip"></a>Método 2 - CHIP

1. Inscreva-se no CHIP e selecione Incentivos LSP.

2. Na página Resumo do Pagamento do **Parceiro,** selecione o mês de reporte que pretende visualizar e, em seguida, selecione **Detalhes** de Cálculo da queda em **Exportação para Excel**:

:::image type="content" source="images/chip/chiplocate.png" alt-text="Localize os detalhes do programa.":::

3. A exportação começará e poderá abrir o ficheiro ou guardar/guardar quanto a um destino.

4. Quando o relatório estiver aberto, navegue para o **separador DetailsReport-FlatFile** no fundo da esquerda:

:::image type="content" source="images/chip/flatfile.png" alt-text="Download de ficheiros planos.":::

Agora pode pesquisar o número do contrato que procura na coluna J. e encontrará a contagem de ambiente de trabalho atribuída na coluna R, marcada Agreement_DesktopCount. Também pode confirmar o Nível de Taxa para este acordo na coluna 'AI' etiquetada Tier.

## <a name="next-steps"></a>Passos seguintes

- [Problemas de acesso ao CHIP de resolução de problemas](chip-access-trouble.md)
