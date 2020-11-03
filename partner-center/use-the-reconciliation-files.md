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
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="6257d-103">Saiba como ler os itens de linha nos ficheiros de reconciliação do Partner Center</span><span class="sxs-lookup"><span data-stu-id="6257d-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="6257d-104">Aplica-se a:</span><span class="sxs-lookup"><span data-stu-id="6257d-104">Applies to:</span></span>

- <span data-ttu-id="6257d-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="6257d-105">Partner Center</span></span>
- <span data-ttu-id="6257d-106">Centro de Parceiros para Microsoft Cloud para governo dos EUA</span><span class="sxs-lookup"><span data-stu-id="6257d-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="6257d-107">Pode descarregar os seus ficheiros de reconciliação do Partner Center para uma visão detalhada e de item de linha de cada carga num ciclo de faturação.</span><span class="sxs-lookup"><span data-stu-id="6257d-107">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="6257d-108">Os detalhes do item da linha incluem taxas para as subscrições de cada cliente, e eventos detalhados (como uma adição intercalar de licenças a uma subscrição).</span><span class="sxs-lookup"><span data-stu-id="6257d-108">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="6257d-109">Funções adequadas:</span><span class="sxs-lookup"><span data-stu-id="6257d-109">Appropriate roles:</span></span>

- <span data-ttu-id="6257d-110">Administrador de faturação</span><span class="sxs-lookup"><span data-stu-id="6257d-110">Billing admin</span></span>
- <span data-ttu-id="6257d-111">Administrador global</span><span class="sxs-lookup"><span data-stu-id="6257d-111">Global admin</span></span>

<span data-ttu-id="6257d-112">Para obter informações sobre como ler a sua **fatura,** consulte [a sua conta](read-your-bill.md).</span><span class="sxs-lookup"><span data-stu-id="6257d-112">For information on how to read your **invoice** , see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="6257d-113">Compreender os campos de arquivos de reconciliação</span><span class="sxs-lookup"><span data-stu-id="6257d-113">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="6257d-114">Campos de ficheiros de reconciliação baseados em licença</span><span class="sxs-lookup"><span data-stu-id="6257d-114">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="6257d-115">Campos de ficheiros de reconciliação baseados em uso</span><span class="sxs-lookup"><span data-stu-id="6257d-115">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="6257d-116">Campos de ficheiros de reconciliação de utilização avaliados diariamente</span><span class="sxs-lookup"><span data-stu-id="6257d-116">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="6257d-117">Compreender tipos de carga em ficheiros de reconciliação</span><span class="sxs-lookup"><span data-stu-id="6257d-117">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="6257d-118">Para compreender os tipos de encargos nos ficheiros de reconciliação (a coluna **ChargeType),** consulte os tipos de [carga de ficheiros de reconciliação](recon-file-charge-types.md).</span><span class="sxs-lookup"><span data-stu-id="6257d-118">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="6257d-119">Corrigir problemas de formatação</span><span class="sxs-lookup"><span data-stu-id="6257d-119">Fix formatting issues</span></span>

<span data-ttu-id="6257d-120">Ocasionalmente, um ficheiro de reconciliação pode conter problemas de formatação.</span><span class="sxs-lookup"><span data-stu-id="6257d-120">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="6257d-121">Por exemplo, esta questão pode ocorrer se o local en-US não for utilizado.</span><span class="sxs-lookup"><span data-stu-id="6257d-121">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="6257d-122">Siga estes passos para corrigir quaisquer problemas de formatação nos seus ficheiros de reconciliação:</span><span class="sxs-lookup"><span data-stu-id="6257d-122">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="6257d-123">Abra o ficheiro de reconciliação (em formato .csv) no Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="6257d-123">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="6257d-124">Selecione a primeira coluna do ficheiro.</span><span class="sxs-lookup"><span data-stu-id="6257d-124">Select the first column in the file.</span></span>
3. <span data-ttu-id="6257d-125">Abra o **texto de conversão para o assistente de colunas** .</span><span class="sxs-lookup"><span data-stu-id="6257d-125">Open the **Convert Text to Columns Wizard** .</span></span> <span data-ttu-id="6257d-126">Na fita, selecione **Dados** e, em seguida, selecione **Texto para Colunas** .</span><span class="sxs-lookup"><span data-stu-id="6257d-126">On the ribbon, select **Data** , then select **Text to Columns** .</span></span>
4. <span data-ttu-id="6257d-127">No assistente, selecione **O tipo de ficheiro delimitado** .</span><span class="sxs-lookup"><span data-stu-id="6257d-127">In the wizard, select **Delimited file type** .</span></span> <span data-ttu-id="6257d-128">Em seguida, selecione **Seguinte** .</span><span class="sxs-lookup"><span data-stu-id="6257d-128">Then, select **Next** .</span></span>
5. <span data-ttu-id="6257d-129">No campo **Delimiters,** **selecione Comma** .</span><span class="sxs-lookup"><span data-stu-id="6257d-129">In the **Delimiters** field, select **Comma** .</span></span> <span data-ttu-id="6257d-130">(Se **o Separador** já estiver selecionado, pode deixar esta opção selecionada.) Em seguida, selecione **Seguinte** .</span><span class="sxs-lookup"><span data-stu-id="6257d-130">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next** .</span></span>
6. <span data-ttu-id="6257d-131">No campo do **formato de dados da Coluna,** selecione **Data:MDY** .</span><span class="sxs-lookup"><span data-stu-id="6257d-131">In the **Column data format** field, select **Date:MDY** .</span></span> <span data-ttu-id="6257d-132">Em seguida, selecione **Seguinte** .</span><span class="sxs-lookup"><span data-stu-id="6257d-132">Then, select **Next** .</span></span>
7. <span data-ttu-id="6257d-133">No campo de **formato de dados da Coluna,** selecione **Texto** para todas as colunas de valor.</span><span class="sxs-lookup"><span data-stu-id="6257d-133">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="6257d-134">Em seguida, selecione **Finish** (Concluir).</span><span class="sxs-lookup"><span data-stu-id="6257d-134">Then, select **Finish** .</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="6257d-135">Descarregue os ficheiros de reconciliação programáticamente</span><span class="sxs-lookup"><span data-stu-id="6257d-135">Download reconciliation files programmatically</span></span>

<span data-ttu-id="6257d-136">Os ficheiros de reconciliação podem ser muito grandes e por vezes são difíceis de descarregar.</span><span class="sxs-lookup"><span data-stu-id="6257d-136">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="6257d-137">Para descarregar ficheiros de reconciliação programáticamente, consulte [obter itens de linha de fatura](/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="6257d-137">To download reconciliation files programmatically, see [Get invoice line items](/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="6257d-138">Taxas de mapa ou IVA</span><span class="sxs-lookup"><span data-stu-id="6257d-138">Map taxes or VAT</span></span>

<span data-ttu-id="6257d-139">Para mapear impostos ou imposto sobre o valor acrescentado (IVA) na sua fatura:</span><span class="sxs-lookup"><span data-stu-id="6257d-139">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="6257d-140">Soma a coluna **Fiscal** do ficheiro baseado na licença.</span><span class="sxs-lookup"><span data-stu-id="6257d-140">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="6257d-141">Soma a coluna **TaxAmount** a partir do ficheiro baseado na utilização.</span><span class="sxs-lookup"><span data-stu-id="6257d-141">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="6257d-142">Itemize ficheiros de reconciliação por parceiro</span><span class="sxs-lookup"><span data-stu-id="6257d-142">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="6257d-143">Os parceiros no **modelo indireto** podem utilizar estes campos adicionais em ficheiros de reconciliação baseados em licenças e uso para itemizar os ficheiros por revendedor.</span><span class="sxs-lookup"><span data-stu-id="6257d-143">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="6257d-144">ID do MPN</span><span class="sxs-lookup"><span data-stu-id="6257d-144">MPN ID</span></span> | <span data-ttu-id="6257d-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="6257d-145">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="6257d-146">ID do MPN</span><span class="sxs-lookup"><span data-stu-id="6257d-146">MPN ID</span></span> | <span data-ttu-id="6257d-147">O identificador da Microsoft Partner Network (MPN) do parceiro Cloud Solution Provider (CSP) (direto ou indireto).</span><span class="sxs-lookup"><span data-stu-id="6257d-147">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="6257d-148">Revendedor MPN ID</span><span class="sxs-lookup"><span data-stu-id="6257d-148">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="6257d-149">O [identificador MPN do revendedor de registos para a subscrição](#reseller-mpn-id).</span><span class="sxs-lookup"><span data-stu-id="6257d-149">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="6257d-150">Este campo corresponde ao ID revendedor listado para a subscrição específica no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="6257d-150">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="6257d-151">Só aparece em ficheiros de reconciliação para parceiros no modelo indireto.</span><span class="sxs-lookup"><span data-stu-id="6257d-151">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="6257d-152">Revendedor MPN ID</span><span class="sxs-lookup"><span data-stu-id="6257d-152">Reseller MPN ID</span></span>

<span data-ttu-id="6257d-153">Se um parceiro da CSP vendeu a subscrição diretamente ao cliente, o seu **ID MPN** está listado duas vezes, tanto como o **ID MPN** e o **ID do Revendedor MPN** .</span><span class="sxs-lookup"><span data-stu-id="6257d-153">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID** .</span></span>

<span data-ttu-id="6257d-154">Se um parceiro CSP tiver um revendedor sem **ID MPN,** este valor é definido para o **ID MPN** do parceiro.</span><span class="sxs-lookup"><span data-stu-id="6257d-154">If a CSP partner has a reseller with no **MPN ID** , this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="6257d-155">Se o parceiro CSP remover um **ID MPN revendedor,** este valor será definido para *-1* .</span><span class="sxs-lookup"><span data-stu-id="6257d-155">If the CSP partner removes a **Reseller MPN ID** , this value will be set to *-1* .</span></span>

<span data-ttu-id="6257d-156">Para visualizar ou atualizar o **ID MPN do Revendedor:**</span><span class="sxs-lookup"><span data-stu-id="6257d-156">To view or update the **Reseller MPN ID** :</span></span>

1. <span data-ttu-id="6257d-157">Inicie sessão no Centro de Parceiros.</span><span class="sxs-lookup"><span data-stu-id="6257d-157">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="6257d-158">No menu Partner Center, selecione **Clientes.**</span><span class="sxs-lookup"><span data-stu-id="6257d-158">In the Partner Center menu, select **Customers** .</span></span>
3. <span data-ttu-id="6257d-159">Escolha o cliente na lista.</span><span class="sxs-lookup"><span data-stu-id="6257d-159">Choose the customer from the list.</span></span>
4. <span data-ttu-id="6257d-160">No menu do cliente, **selecione Subscrições.**</span><span class="sxs-lookup"><span data-stu-id="6257d-160">In the customer menu, select **Subscriptions** .</span></span>
5. <span data-ttu-id="6257d-161">Escolha a subscrição da lista.</span><span class="sxs-lookup"><span data-stu-id="6257d-161">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="6257d-162">Selecione **atualização** para alterar o **Revendedor (MPN ID)** .</span><span class="sxs-lookup"><span data-stu-id="6257d-162">Select **update** to change the **Reseller (MPN ID)** .</span></span>