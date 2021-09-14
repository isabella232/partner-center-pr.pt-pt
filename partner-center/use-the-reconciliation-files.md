---
title: Utilizar os ficheiros de reconciliação
ms.topic: article
ms.date: 03/26/2021
description: Conheça os ficheiros de reconciliação no Partner Center e como interpretar as vistas detalhadas e de item de linha das taxas para um determinado ciclo de faturação.
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e5fae4c9b9b40c8a71b56c46d0d1be629f832842
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/13/2021
ms.locfileid: "126246575"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a>Saiba como ler os itens de linha nos ficheiros de reconciliação do Partner Center

**Funções apropriadas**: Administrador de Faturação | Administração global

Pode descarregar os seus ficheiros de reconciliação do Partner Center para uma visão detalhada e de item de linha de cada carga num ciclo de faturação. Os detalhes do item da linha incluem taxas para as subscrições de cada cliente, e eventos detalhados (como uma adição intercalar de licenças a uma subscrição).

Para obter informações sobre como ler a sua **fatura,** consulte [a sua conta](read-your-bill.md).

## <a name="understand-reconciliation-file-fields"></a>Compreender os campos de arquivos de reconciliação

- [Campos do ficheiro de reconciliação baseado em licenças](license-based-recon-files.md)
- [Campos do ficheiro de reconciliação baseado na utilização](usage-based-recon-files.md)
- [Campos do ficheiro de reconciliação da utilização diária](daily-rated-usage-recon-files.md)
- [Compra única campos de ficheiros de reconciliação CSP](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a>Compreender tipos de carga em ficheiros de reconciliação

Para compreender os tipos de encargos nos ficheiros de reconciliação (a coluna **ChargeType),** consulte os tipos de [carga de ficheiros de reconciliação](recon-file-charge-types.md).

## <a name="fix-formatting-issues"></a>Corrigir problemas de formatação

Ocasionalmente, um ficheiro de reconciliação pode conter problemas de formatação. Por exemplo, esta questão pode ocorrer se o local en-US não for utilizado.

Siga estes passos para corrigir quaisquer problemas de formatação nos seus ficheiros de reconciliação:

1. Abra o ficheiro de reconciliação (em formato .csv) em Microsoft Excel.
2. Selecione a primeira coluna do ficheiro.
3. Abra o **texto de conversão para o assistente de colunas**. Na fita, selecione **Dados** e, em seguida, selecione **Texto para Colunas**.
4. No assistente, selecione **O tipo de ficheiro delimitado**. Em seguida, selecione **Seguinte**.
5. No campo **Delimiters,** **selecione Comma**. (Se **o Separador** já estiver selecionado, pode deixar esta opção selecionada.) Em seguida, selecione **Seguinte**.
6. No campo do **formato de dados da Coluna,** selecione **Data:MDY**. Em seguida, selecione **Seguinte**.
7. No campo de **formato de dados da Coluna,** selecione **Texto** para todas as colunas de valor. Em seguida, selecione **Finish** (Concluir).

## <a name="download-reconciliation-files-programmatically"></a>Descarregue os ficheiros de reconciliação programáticamente

Os ficheiros de reconciliação podem ser muito grandes e por vezes são difíceis de descarregar. Para descarregar ficheiros de reconciliação programáticamente, consulte [obter itens de linha de fatura](/partner-center/develop/get-invoiceline-items).

## <a name="if-your-file-exceeds-the-row-limit-in-excel"></a>Se o seu ficheiro exceder o limite de linha em Excel

Se conseguir descarregar um ficheiro de reconciliação mas não o abrir em Microsoft Excel, provavelmente significa que o ficheiro contém mais linhas do que Excel permitirá. Se isso acontecer, pode utilizar qualquer um dos procedimentos abaixo para abrir o ficheiro.

### <a name="open-a-recon-file-in-power-bi"></a>Abra um ficheiro de reconhecimento em Power BI

1. Descarregue o ficheiro de reconciliação como normalmente faria.
2. Faça o download, instale e abra uma instância do Microsoft Power BI.
3. No separador Power BI **Home,** **selecione Obter dados**.
4. Na lista de fontes de **dados comuns,** selecione **Texto/CSV**.
5. Quando solicitado, abra o seu ficheiro de reconhecimento.

### <a name="open-a-recon-file-in-an-excel-pivot-table"></a>Abra um arquivo de reconhecimento numa mesa de pivô Excel

1. Descarregue o ficheiro de reconciliação como normalmente faria.
2. Abra um novo arquivo em Microsoft Excel.
3. No separador **Dados,** **selecione Obter dados**, selecione **'Ficheiro'** e, em seguida, selecione **Texto/CSV**.
4. Quando solicitado, abra o seu ficheiro de reconhecimento. Os seus dados aparecerão.
5. No menu de entrega de **carga,** selecione **Carregar para**, e, em seguida, selecione **OK**.
6. Na caixa de diálogo **de dados de importação,** selecione **O Relatório De Mesa Para** abrir o seu ficheiro.

## <a name="negative-amount-displayed"></a>Quantidade negativa exibida

Pode ver uma quantia negativa no seu ficheiro de reconciliação. Este problema, provavelmente, é causado por uma das razões seguintes:

- Cancelou recentemente ou reduziu o seu número de licenças
- Recebeu crédito por um contrato de licença de serviço (SLA) ou para consumo Azure

Para obter mais informações sobre esta transação, veja o atributo de tipo de custo no ficheiro de reconciliação.

## <a name="map-taxes-or-vat"></a>Taxas de mapa ou IVA

Para mapear impostos ou imposto sobre o valor acrescentado (IVA) na sua fatura:

- Soma a coluna **Fiscal** do ficheiro baseado na licença.
- Soma a coluna **TaxAmount** a partir do ficheiro baseado na utilização.

## <a name="itemize-reconciliation-files-by-partner"></a>Itemize ficheiros de reconciliação por parceiro

Os parceiros no **modelo indireto** podem utilizar estes campos adicionais em ficheiros de reconciliação baseados em licenças e uso para itemizar os ficheiros por revendedor.

| ID do MPN | Description |
| ------ | ----------- |
| ID do MPN | O identificador da Microsoft Partner Network (MPN) do parceiro Fornecedor de Soluções em Nuvem (CSP) (direto ou indireto). |
| [Revendedor MPN ID](#reseller-mpn-id) | O [identificador MPN do revendedor de registos para a subscrição](#reseller-mpn-id). Este campo corresponde ao ID revendedor listado para a subscrição específica no Partner Center. Só aparece em ficheiros de reconciliação para parceiros no modelo indireto. |

### <a name="reseller-mpn-id"></a>Revendedor MPN ID

Se um parceiro da CSP vendeu a subscrição diretamente ao cliente, o seu **ID MPN** está listado duas vezes, tanto como o **ID MPN** e o **ID do Revendedor MPN**.

Se um parceiro CSP tiver um revendedor sem **ID MPN,** este valor é definido para o **ID MPN** do parceiro.

Se o parceiro CSP remover um **ID MPN revendedor,** este valor será definido para *-1*.

Para visualizar ou atualizar o **ID MPN do Revendedor:**

1. Inicie sessão no Centro de Parceiros.
2. No menu Partner Center, selecione **Clientes.**
3. Escolha o cliente na lista.
4. No menu do cliente, **selecione Subscrições.**
5. Escolha a subscrição da lista.
6. Selecione **atualização** para alterar o **Revendedor (MPN ID)**.

## <a name="next-steps"></a>Passos seguintes

- [Como ler o seu ficheiro de & de reconhecimento](read-your-bill.md) 