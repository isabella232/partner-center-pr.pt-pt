---
title: Use os seus ficheiros de reconciliação
ms.topic: article
ms.date: 06/08/2020
description: Conheça os ficheiros de reconciliação no Partner Center e como interpretar as vistas detalhadas e de item de linha das taxas para um determinado ciclo de faturação.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 98bfd9a9ce6f03ad62a830f05ba82f9b90268326
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/22/2020
ms.locfileid: "92529855"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a>Saiba como ler os itens de linha nos ficheiros de reconciliação do Partner Center

Aplica-se a:

- Partner Center
- Centro de Parceiros para Microsoft Cloud para governo dos EUA

Pode descarregar os seus ficheiros de reconciliação do Partner Center para uma visão detalhada e de item de linha de cada carga num ciclo de faturação. Os detalhes do item da linha incluem taxas para as subscrições de cada cliente, e eventos detalhados (como uma adição intercalar de licenças a uma subscrição).

Funções adequadas:

- Administrador de faturação
- Administrador global

Para obter informações sobre como ler a sua **fatura,** consulte [a sua conta](read-your-bill.md).

## <a name="understand-reconciliation-file-fields"></a>Compreender os campos de arquivos de reconciliação

- [Campos de ficheiros de reconciliação baseados em licença](license-based-recon-files.md)
- [Campos de ficheiros de reconciliação baseados em uso](usage-based-recon-files.md)
- [Campos de ficheiros de reconciliação de utilização avaliados diariamente](daily-rated-usage-recon-files.md)

## <a name="understand-charge-types-in-reconciliation-files"></a>Compreender tipos de carga em ficheiros de reconciliação

Para compreender os tipos de encargos nos ficheiros de reconciliação (a coluna **ChargeType),** consulte os tipos de [carga de ficheiros de reconciliação](recon-file-charge-types.md).

## <a name="fix-formatting-issues"></a>Corrigir problemas de formatação

Ocasionalmente, um ficheiro de reconciliação pode conter problemas de formatação. Por exemplo, esta questão pode ocorrer se o local en-US não for utilizado.

Siga estes passos para corrigir quaisquer problemas de formatação nos seus ficheiros de reconciliação:

1. Abra o ficheiro de reconciliação (em formato .csv) no Microsoft Excel.
2. Selecione a primeira coluna do ficheiro.
3. Abra o **texto de conversão para o assistente de colunas** . Na fita, selecione **Dados** e, em seguida, selecione **Texto para Colunas** .
4. No assistente, selecione **O tipo de ficheiro delimitado** . Em seguida, selecione **Seguinte** .
5. No campo **Delimiters,** **selecione Comma** . (Se **o Separador** já estiver selecionado, pode deixar esta opção selecionada.) Em seguida, selecione **Seguinte** .
6. No campo do **formato de dados da Coluna,** selecione **Data:MDY** . Em seguida, selecione **Seguinte** .
7. No campo de **formato de dados da Coluna,** selecione **Texto** para todas as colunas de valor. Em seguida, selecione **Finish** (Concluir).

## <a name="download-reconciliation-files-programmatically"></a>Descarregue os ficheiros de reconciliação programáticamente

Os ficheiros de reconciliação podem ser muito grandes e por vezes são difíceis de descarregar. Para descarregar ficheiros de reconciliação programáticamente, consulte [obter itens de linha de fatura](/partner-center/develop/get-invoiceline-items).

## <a name="map-taxes-or-vat"></a>Taxas de mapa ou IVA

Para mapear impostos ou imposto sobre o valor acrescentado (IVA) na sua fatura:

- Soma a coluna **Fiscal** do ficheiro baseado na licença.
- Soma a coluna **TaxAmount** a partir do ficheiro baseado na utilização.

## <a name="itemize-reconciliation-files-by-partner"></a>Itemize ficheiros de reconciliação por parceiro

Os parceiros no **modelo indireto** podem utilizar estes campos adicionais em ficheiros de reconciliação baseados em licenças e uso para itemizar os ficheiros por revendedor.

| ID do MPN | Descrição |
| ------ | ----------- |
| ID do MPN | O identificador da Microsoft Partner Network (MPN) do parceiro Cloud Solution Provider (CSP) (direto ou indireto). |
| [Revendedor MPN ID](#reseller-mpn-id) | O [identificador MPN do revendedor de registos para a subscrição](#reseller-mpn-id). Este campo corresponde ao ID revendedor listado para a subscrição específica no Partner Center. Só aparece em ficheiros de reconciliação para parceiros no modelo indireto. |

### <a name="reseller-mpn-id"></a>Revendedor MPN ID

Se um parceiro da CSP vendeu a subscrição diretamente ao cliente, o seu **ID MPN** está listado duas vezes, tanto como o **ID MPN** e o **ID do Revendedor MPN** .

Se um parceiro CSP tiver um revendedor sem **ID MPN,** este valor é definido para o **ID MPN** do parceiro.

Se o parceiro CSP remover um **ID MPN revendedor,** este valor será definido para *-1* .

Para visualizar ou atualizar o **ID MPN do Revendedor:**

1. Inicie sessão no Centro de Parceiros.
2. No menu Partner Center, selecione **Clientes.**
3. Escolha o cliente na lista.
4. No menu do cliente, **selecione Subscrições.**
5. Escolha a subscrição da lista.
6. Selecione **atualização** para alterar o **Revendedor (MPN ID)** .