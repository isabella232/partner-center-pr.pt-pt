---
title: Use os seus ficheiros de reconciliação
ms.topic: article
ms.date: 03/26/2021
description: Conheça os ficheiros de reconciliação no Partner Center e como interpretar as vistas detalhadas e de item de linha das taxas para um determinado ciclo de faturação.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4a6a1455304f12e364d71e666cbd548821f8be55
ms.sourcegitcommit: a691d4cbe144a8fd71e344fd293cc658ac11d6f3
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/27/2021
ms.locfileid: "105633901"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="d0b58-103">Saiba como ler os itens de linha nos ficheiros de reconciliação do Partner Center</span><span class="sxs-lookup"><span data-stu-id="d0b58-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="d0b58-104">**Funções adequadas**</span><span class="sxs-lookup"><span data-stu-id="d0b58-104">**Appropriate roles**</span></span>

- <span data-ttu-id="d0b58-105">Administrador de faturação</span><span class="sxs-lookup"><span data-stu-id="d0b58-105">Billing admin</span></span>
- <span data-ttu-id="d0b58-106">Administrador global</span><span class="sxs-lookup"><span data-stu-id="d0b58-106">Global admin</span></span>

<span data-ttu-id="d0b58-107">Pode descarregar os seus ficheiros de reconciliação do Partner Center para uma visão detalhada e de item de linha de cada carga num ciclo de faturação.</span><span class="sxs-lookup"><span data-stu-id="d0b58-107">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="d0b58-108">Os detalhes do item da linha incluem taxas para as subscrições de cada cliente, e eventos detalhados (como uma adição intercalar de licenças a uma subscrição).</span><span class="sxs-lookup"><span data-stu-id="d0b58-108">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="d0b58-109">Para obter informações sobre como ler a sua **fatura,** consulte [a sua conta](read-your-bill.md).</span><span class="sxs-lookup"><span data-stu-id="d0b58-109">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="d0b58-110">Compreender os campos de arquivos de reconciliação</span><span class="sxs-lookup"><span data-stu-id="d0b58-110">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="d0b58-111">Campos do ficheiro de reconciliação baseado em licenças</span><span class="sxs-lookup"><span data-stu-id="d0b58-111">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="d0b58-112">Campos do ficheiro de reconciliação baseado na utilização</span><span class="sxs-lookup"><span data-stu-id="d0b58-112">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="d0b58-113">Campos do ficheiro de reconciliação da utilização diária</span><span class="sxs-lookup"><span data-stu-id="d0b58-113">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)
- [<span data-ttu-id="d0b58-114">Compra única campos de ficheiros de reconciliação CSP</span><span class="sxs-lookup"><span data-stu-id="d0b58-114">One-time purchase CSP reconciliation file fields</span></span>](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="d0b58-115">Compreender tipos de carga em ficheiros de reconciliação</span><span class="sxs-lookup"><span data-stu-id="d0b58-115">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="d0b58-116">Para compreender os tipos de encargos nos ficheiros de reconciliação (a coluna **ChargeType),** consulte os tipos de [carga de ficheiros de reconciliação](recon-file-charge-types.md).</span><span class="sxs-lookup"><span data-stu-id="d0b58-116">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="d0b58-117">Corrigir problemas de formatação</span><span class="sxs-lookup"><span data-stu-id="d0b58-117">Fix formatting issues</span></span>

<span data-ttu-id="d0b58-118">Ocasionalmente, um ficheiro de reconciliação pode conter problemas de formatação.</span><span class="sxs-lookup"><span data-stu-id="d0b58-118">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="d0b58-119">Por exemplo, esta questão pode ocorrer se o local en-US não for utilizado.</span><span class="sxs-lookup"><span data-stu-id="d0b58-119">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="d0b58-120">Siga estes passos para corrigir quaisquer problemas de formatação nos seus ficheiros de reconciliação:</span><span class="sxs-lookup"><span data-stu-id="d0b58-120">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="d0b58-121">Abra o ficheiro de reconciliação (em .csv formato) no Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="d0b58-121">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="d0b58-122">Selecione a primeira coluna do ficheiro.</span><span class="sxs-lookup"><span data-stu-id="d0b58-122">Select the first column in the file.</span></span>
3. <span data-ttu-id="d0b58-123">Abra o **texto de conversão para o assistente de colunas**.</span><span class="sxs-lookup"><span data-stu-id="d0b58-123">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="d0b58-124">Na fita, selecione **Dados** e, em seguida, selecione **Texto para Colunas**.</span><span class="sxs-lookup"><span data-stu-id="d0b58-124">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="d0b58-125">No assistente, selecione **O tipo de ficheiro delimitado**.</span><span class="sxs-lookup"><span data-stu-id="d0b58-125">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="d0b58-126">Em seguida, selecione **Seguinte**.</span><span class="sxs-lookup"><span data-stu-id="d0b58-126">Then, select **Next**.</span></span>
5. <span data-ttu-id="d0b58-127">No campo **Delimiters,** **selecione Comma**.</span><span class="sxs-lookup"><span data-stu-id="d0b58-127">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="d0b58-128">(Se **o Separador** já estiver selecionado, pode deixar esta opção selecionada.) Em seguida, selecione **Seguinte**.</span><span class="sxs-lookup"><span data-stu-id="d0b58-128">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="d0b58-129">No campo do **formato de dados da Coluna,** selecione **Data:MDY**.</span><span class="sxs-lookup"><span data-stu-id="d0b58-129">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="d0b58-130">Em seguida, selecione **Seguinte**.</span><span class="sxs-lookup"><span data-stu-id="d0b58-130">Then, select **Next**.</span></span>
7. <span data-ttu-id="d0b58-131">No campo de **formato de dados da Coluna,** selecione **Texto** para todas as colunas de valor.</span><span class="sxs-lookup"><span data-stu-id="d0b58-131">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="d0b58-132">Em seguida, selecione **Finish** (Concluir).</span><span class="sxs-lookup"><span data-stu-id="d0b58-132">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="d0b58-133">Descarregue os ficheiros de reconciliação programáticamente</span><span class="sxs-lookup"><span data-stu-id="d0b58-133">Download reconciliation files programmatically</span></span>

<span data-ttu-id="d0b58-134">Os ficheiros de reconciliação podem ser muito grandes e por vezes são difíceis de descarregar.</span><span class="sxs-lookup"><span data-stu-id="d0b58-134">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="d0b58-135">Para descarregar ficheiros de reconciliação programáticamente, consulte [obter itens de linha de fatura](/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="d0b58-135">To download reconciliation files programmatically, see [Get invoice line items](/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="if-your-file-exceeds-the-row-limit-in-excel"></a><span data-ttu-id="d0b58-136">Se o seu ficheiro exceder o limite de linha no Excel</span><span class="sxs-lookup"><span data-stu-id="d0b58-136">If your file exceeds the row limit in Excel</span></span>

<span data-ttu-id="d0b58-137">Se conseguir descarregar um ficheiro de reconciliação mas não o abrir no Microsoft Excel, provavelmente significa que o ficheiro contém mais linhas do que o Excel permitirá.</span><span class="sxs-lookup"><span data-stu-id="d0b58-137">If you’re able to download a reconciliation file but not open it in Microsoft Excel, it probably means the file contains more rows than Excel will allow.</span></span> <span data-ttu-id="d0b58-138">Se isso acontecer, pode utilizar qualquer um dos procedimentos abaixo para abrir o ficheiro.</span><span class="sxs-lookup"><span data-stu-id="d0b58-138">If this happens, you can use either of the procedures below to open the file.</span></span>

### <a name="open-a-recon-file-in-power-bi"></a><span data-ttu-id="d0b58-139">Abra um ficheiro de reconhecimento no Power BI</span><span class="sxs-lookup"><span data-stu-id="d0b58-139">Open a recon file in Power BI</span></span>

1. <span data-ttu-id="d0b58-140">Descarregue o ficheiro de reconciliação como normalmente faria.</span><span class="sxs-lookup"><span data-stu-id="d0b58-140">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="d0b58-141">Faça o download, instale e abra uma instância do Power BI.</span><span class="sxs-lookup"><span data-stu-id="d0b58-141">Download, install, and open an instance of Power BI.</span></span>
3. <span data-ttu-id="d0b58-142">No separador Power BI **Home,** **selecione Obter dados**.</span><span class="sxs-lookup"><span data-stu-id="d0b58-142">On the Power BI **Home** tab, select **Get data**.</span></span>
4. <span data-ttu-id="d0b58-143">Na lista de fontes de **dados comuns,** selecione **Texto/CSV**.</span><span class="sxs-lookup"><span data-stu-id="d0b58-143">In the list of **Common data sources**, select **Text/CSV**.</span></span>
5. <span data-ttu-id="d0b58-144">Quando solicitado, abra o seu ficheiro de reconhecimento.</span><span class="sxs-lookup"><span data-stu-id="d0b58-144">When prompted, open your recon file.</span></span>

### <a name="open-a-recon-file-in-an-excel-pivot-table"></a><span data-ttu-id="d0b58-145">Abra um ficheiro de reconhecimento numa mesa de pivô do Excel</span><span class="sxs-lookup"><span data-stu-id="d0b58-145">Open a recon file in an Excel pivot table</span></span>

1. <span data-ttu-id="d0b58-146">Descarregue o ficheiro de reconciliação como normalmente faria.</span><span class="sxs-lookup"><span data-stu-id="d0b58-146">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="d0b58-147">Abra um novo ficheiro no Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="d0b58-147">Open a new file in Microsoft Excel.</span></span>
3. <span data-ttu-id="d0b58-148">No separador **Dados,** **selecione Obter dados**, selecione **'Ficheiro'** e, em seguida, selecione **Texto/CSV**.</span><span class="sxs-lookup"><span data-stu-id="d0b58-148">On the **Data** tab, select **Get data**, select **From file**, and then select **Text/CSV**.</span></span>
4. <span data-ttu-id="d0b58-149">Quando solicitado, abra o seu ficheiro de reconhecimento.</span><span class="sxs-lookup"><span data-stu-id="d0b58-149">When prompted, open your recon file.</span></span> <span data-ttu-id="d0b58-150">Os seus dados aparecerão.</span><span class="sxs-lookup"><span data-stu-id="d0b58-150">Your data will appear.</span></span>
5. <span data-ttu-id="d0b58-151">No menu de entrega de **carga,** selecione **Load to**, e, em seguida, **OK**.</span><span class="sxs-lookup"><span data-stu-id="d0b58-151">In the **Load** dropdown menu, select **Load to**, and then **OK**.</span></span>
6. <span data-ttu-id="d0b58-152">Na caixa de diálogo **de dados de importação,** selecione **O Relatório De Mesa Para** abrir o seu ficheiro.</span><span class="sxs-lookup"><span data-stu-id="d0b58-152">In the **Import Data** dialog box, select **PivotTable Report** to open your file.</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="d0b58-153">Taxas de mapa ou IVA</span><span class="sxs-lookup"><span data-stu-id="d0b58-153">Map taxes or VAT</span></span>

<span data-ttu-id="d0b58-154">Para mapear impostos ou imposto sobre o valor acrescentado (IVA) na sua fatura:</span><span class="sxs-lookup"><span data-stu-id="d0b58-154">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="d0b58-155">Soma a coluna **Fiscal** do ficheiro baseado na licença.</span><span class="sxs-lookup"><span data-stu-id="d0b58-155">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="d0b58-156">Soma a coluna **TaxAmount** a partir do ficheiro baseado na utilização.</span><span class="sxs-lookup"><span data-stu-id="d0b58-156">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="d0b58-157">Itemize ficheiros de reconciliação por parceiro</span><span class="sxs-lookup"><span data-stu-id="d0b58-157">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="d0b58-158">Os parceiros no **modelo indireto** podem utilizar estes campos adicionais em ficheiros de reconciliação baseados em licenças e uso para itemizar os ficheiros por revendedor.</span><span class="sxs-lookup"><span data-stu-id="d0b58-158">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="d0b58-159">ID do MPN</span><span class="sxs-lookup"><span data-stu-id="d0b58-159">MPN ID</span></span> | <span data-ttu-id="d0b58-160">Description</span><span class="sxs-lookup"><span data-stu-id="d0b58-160">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="d0b58-161">ID do MPN</span><span class="sxs-lookup"><span data-stu-id="d0b58-161">MPN ID</span></span> | <span data-ttu-id="d0b58-162">O identificador da Microsoft Partner Network (MPN) do parceiro Cloud Solution Provider (CSP) (direto ou indireto).</span><span class="sxs-lookup"><span data-stu-id="d0b58-162">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="d0b58-163">Revendedor MPN ID</span><span class="sxs-lookup"><span data-stu-id="d0b58-163">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="d0b58-164">O [identificador MPN do revendedor de registos para a subscrição](#reseller-mpn-id).</span><span class="sxs-lookup"><span data-stu-id="d0b58-164">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="d0b58-165">Este campo corresponde ao ID revendedor listado para a subscrição específica no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="d0b58-165">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="d0b58-166">Só aparece em ficheiros de reconciliação para parceiros no modelo indireto.</span><span class="sxs-lookup"><span data-stu-id="d0b58-166">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="d0b58-167">Revendedor MPN ID</span><span class="sxs-lookup"><span data-stu-id="d0b58-167">Reseller MPN ID</span></span>

<span data-ttu-id="d0b58-168">Se um parceiro da CSP vendeu a subscrição diretamente ao cliente, o seu **ID MPN** está listado duas vezes, tanto como o **ID MPN** e o **ID do Revendedor MPN**.</span><span class="sxs-lookup"><span data-stu-id="d0b58-168">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="d0b58-169">Se um parceiro CSP tiver um revendedor sem **ID MPN,** este valor é definido para o **ID MPN** do parceiro.</span><span class="sxs-lookup"><span data-stu-id="d0b58-169">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="d0b58-170">Se o parceiro CSP remover um **ID MPN revendedor,** este valor será definido para *-1*.</span><span class="sxs-lookup"><span data-stu-id="d0b58-170">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="d0b58-171">Para visualizar ou atualizar o **ID MPN do Revendedor:**</span><span class="sxs-lookup"><span data-stu-id="d0b58-171">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="d0b58-172">Inicie sessão no Centro de Parceiros.</span><span class="sxs-lookup"><span data-stu-id="d0b58-172">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="d0b58-173">No menu Partner Center, selecione **Clientes.**</span><span class="sxs-lookup"><span data-stu-id="d0b58-173">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="d0b58-174">Escolha o cliente na lista.</span><span class="sxs-lookup"><span data-stu-id="d0b58-174">Choose the customer from the list.</span></span>
4. <span data-ttu-id="d0b58-175">No menu do cliente, **selecione Subscrições.**</span><span class="sxs-lookup"><span data-stu-id="d0b58-175">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="d0b58-176">Escolha a subscrição da lista.</span><span class="sxs-lookup"><span data-stu-id="d0b58-176">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="d0b58-177">Selecione **atualização** para alterar o **Revendedor (MPN ID)**.</span><span class="sxs-lookup"><span data-stu-id="d0b58-177">Select **update** to change the **Reseller (MPN ID)**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="d0b58-178">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="d0b58-178">Next steps</span></span>

- [<span data-ttu-id="d0b58-179">Como ler o seu ficheiro de & de reconhecimento</span><span class="sxs-lookup"><span data-stu-id="d0b58-179">How to read your bill & recon file</span></span>](read-your-bill.md) 