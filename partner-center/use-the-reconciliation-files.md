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
ms.openlocfilehash: 1a7d5f3169c4b338a07475a7e246e87841b8dcfb
ms.sourcegitcommit: bce54ddb9fff7332a03d6aa228ba9414a87d76b7
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/22/2021
ms.locfileid: "112431560"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="48b09-103">Saiba como ler os itens de linha nos ficheiros de reconciliação do Partner Center</span><span class="sxs-lookup"><span data-stu-id="48b09-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="48b09-104">**Funções apropriadas**: Administrador de Faturação | Administração global</span><span class="sxs-lookup"><span data-stu-id="48b09-104">**Appropriate roles**: Billing admin | Global admin</span></span>

<span data-ttu-id="48b09-105">Pode descarregar os seus ficheiros de reconciliação do Partner Center para uma visão detalhada e de item de linha de cada carga num ciclo de faturação.</span><span class="sxs-lookup"><span data-stu-id="48b09-105">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="48b09-106">Os detalhes do item da linha incluem taxas para as subscrições de cada cliente, e eventos detalhados (como uma adição intercalar de licenças a uma subscrição).</span><span class="sxs-lookup"><span data-stu-id="48b09-106">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="48b09-107">Para obter informações sobre como ler a sua **fatura,** consulte [a sua conta](read-your-bill.md).</span><span class="sxs-lookup"><span data-stu-id="48b09-107">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="48b09-108">Compreender os campos de arquivos de reconciliação</span><span class="sxs-lookup"><span data-stu-id="48b09-108">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="48b09-109">Campos do ficheiro de reconciliação baseado em licenças</span><span class="sxs-lookup"><span data-stu-id="48b09-109">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="48b09-110">Campos do ficheiro de reconciliação baseado na utilização</span><span class="sxs-lookup"><span data-stu-id="48b09-110">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="48b09-111">Campos do ficheiro de reconciliação da utilização diária</span><span class="sxs-lookup"><span data-stu-id="48b09-111">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)
- [<span data-ttu-id="48b09-112">Compra única campos de ficheiros de reconciliação CSP</span><span class="sxs-lookup"><span data-stu-id="48b09-112">One-time purchase CSP reconciliation file fields</span></span>](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="48b09-113">Compreender tipos de carga em ficheiros de reconciliação</span><span class="sxs-lookup"><span data-stu-id="48b09-113">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="48b09-114">Para compreender os tipos de encargos nos ficheiros de reconciliação (a coluna **ChargeType),** consulte os tipos de [carga de ficheiros de reconciliação](recon-file-charge-types.md).</span><span class="sxs-lookup"><span data-stu-id="48b09-114">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="48b09-115">Corrigir problemas de formatação</span><span class="sxs-lookup"><span data-stu-id="48b09-115">Fix formatting issues</span></span>

<span data-ttu-id="48b09-116">Ocasionalmente, um ficheiro de reconciliação pode conter problemas de formatação.</span><span class="sxs-lookup"><span data-stu-id="48b09-116">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="48b09-117">Por exemplo, esta questão pode ocorrer se o local en-US não for utilizado.</span><span class="sxs-lookup"><span data-stu-id="48b09-117">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="48b09-118">Siga estes passos para corrigir quaisquer problemas de formatação nos seus ficheiros de reconciliação:</span><span class="sxs-lookup"><span data-stu-id="48b09-118">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="48b09-119">Abra o ficheiro de reconciliação (em formato .csv) no Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="48b09-119">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="48b09-120">Selecione a primeira coluna do ficheiro.</span><span class="sxs-lookup"><span data-stu-id="48b09-120">Select the first column in the file.</span></span>
3. <span data-ttu-id="48b09-121">Abra o **texto de conversão para o assistente de colunas**.</span><span class="sxs-lookup"><span data-stu-id="48b09-121">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="48b09-122">Na fita, selecione **Dados** e, em seguida, selecione **Texto para Colunas**.</span><span class="sxs-lookup"><span data-stu-id="48b09-122">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="48b09-123">No assistente, selecione **O tipo de ficheiro delimitado**.</span><span class="sxs-lookup"><span data-stu-id="48b09-123">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="48b09-124">Em seguida, selecione **Seguinte**.</span><span class="sxs-lookup"><span data-stu-id="48b09-124">Then, select **Next**.</span></span>
5. <span data-ttu-id="48b09-125">No campo **Delimiters,** **selecione Comma**.</span><span class="sxs-lookup"><span data-stu-id="48b09-125">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="48b09-126">(Se **o Separador** já estiver selecionado, pode deixar esta opção selecionada.) Em seguida, selecione **Seguinte**.</span><span class="sxs-lookup"><span data-stu-id="48b09-126">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="48b09-127">No campo do **formato de dados da Coluna,** selecione **Data:MDY**.</span><span class="sxs-lookup"><span data-stu-id="48b09-127">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="48b09-128">Em seguida, selecione **Seguinte**.</span><span class="sxs-lookup"><span data-stu-id="48b09-128">Then, select **Next**.</span></span>
7. <span data-ttu-id="48b09-129">No campo de **formato de dados da Coluna,** selecione **Texto** para todas as colunas de valor.</span><span class="sxs-lookup"><span data-stu-id="48b09-129">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="48b09-130">Em seguida, selecione **Finish** (Concluir).</span><span class="sxs-lookup"><span data-stu-id="48b09-130">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="48b09-131">Descarregue os ficheiros de reconciliação programáticamente</span><span class="sxs-lookup"><span data-stu-id="48b09-131">Download reconciliation files programmatically</span></span>

<span data-ttu-id="48b09-132">Os ficheiros de reconciliação podem ser muito grandes e por vezes são difíceis de descarregar.</span><span class="sxs-lookup"><span data-stu-id="48b09-132">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="48b09-133">Para descarregar ficheiros de reconciliação programáticamente, consulte [obter itens de linha de fatura](/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="48b09-133">To download reconciliation files programmatically, see [Get invoice line items](/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="if-your-file-exceeds-the-row-limit-in-excel"></a><span data-ttu-id="48b09-134">Se o seu ficheiro exceder o limite de linha no Excel</span><span class="sxs-lookup"><span data-stu-id="48b09-134">If your file exceeds the row limit in Excel</span></span>

<span data-ttu-id="48b09-135">Se conseguir descarregar um ficheiro de reconciliação mas não o abrir no Microsoft Excel, provavelmente significa que o ficheiro contém mais linhas do que o Excel permitirá.</span><span class="sxs-lookup"><span data-stu-id="48b09-135">If you’re able to download a reconciliation file but not open it in Microsoft Excel, it probably means the file contains more rows than Excel will allow.</span></span> <span data-ttu-id="48b09-136">Se isso acontecer, pode utilizar qualquer um dos procedimentos abaixo para abrir o ficheiro.</span><span class="sxs-lookup"><span data-stu-id="48b09-136">If this happens, you can use either of the procedures below to open the file.</span></span>

### <a name="open-a-recon-file-in-power-bi"></a><span data-ttu-id="48b09-137">Abra um ficheiro de reconhecimento no Power BI</span><span class="sxs-lookup"><span data-stu-id="48b09-137">Open a recon file in Power BI</span></span>

1. <span data-ttu-id="48b09-138">Descarregue o ficheiro de reconciliação como normalmente faria.</span><span class="sxs-lookup"><span data-stu-id="48b09-138">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="48b09-139">Faça o download, instale e abra uma instância do Microsoft Power BI.</span><span class="sxs-lookup"><span data-stu-id="48b09-139">Download, install, and open an instance of Microsoft Power BI.</span></span>
3. <span data-ttu-id="48b09-140">No separador Power BI **Home,** **selecione Obter dados**.</span><span class="sxs-lookup"><span data-stu-id="48b09-140">On the Power BI **Home** tab, select **Get data**.</span></span>
4. <span data-ttu-id="48b09-141">Na lista de fontes de **dados comuns,** selecione **Texto/CSV**.</span><span class="sxs-lookup"><span data-stu-id="48b09-141">In the list of **Common data sources**, select **Text/CSV**.</span></span>
5. <span data-ttu-id="48b09-142">Quando solicitado, abra o seu ficheiro de reconhecimento.</span><span class="sxs-lookup"><span data-stu-id="48b09-142">When prompted, open your recon file.</span></span>

### <a name="open-a-recon-file-in-an-excel-pivot-table"></a><span data-ttu-id="48b09-143">Abra um ficheiro de reconhecimento numa mesa de pivô do Excel</span><span class="sxs-lookup"><span data-stu-id="48b09-143">Open a recon file in an Excel pivot table</span></span>

1. <span data-ttu-id="48b09-144">Descarregue o ficheiro de reconciliação como normalmente faria.</span><span class="sxs-lookup"><span data-stu-id="48b09-144">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="48b09-145">Abra um novo ficheiro no Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="48b09-145">Open a new file in Microsoft Excel.</span></span>
3. <span data-ttu-id="48b09-146">No separador **Dados,** **selecione Obter dados**, selecione **'Ficheiro'** e, em seguida, selecione **Texto/CSV**.</span><span class="sxs-lookup"><span data-stu-id="48b09-146">On the **Data** tab, select **Get data**, select **From file**, and then select **Text/CSV**.</span></span>
4. <span data-ttu-id="48b09-147">Quando solicitado, abra o seu ficheiro de reconhecimento.</span><span class="sxs-lookup"><span data-stu-id="48b09-147">When prompted, open your recon file.</span></span> <span data-ttu-id="48b09-148">Os seus dados aparecerão.</span><span class="sxs-lookup"><span data-stu-id="48b09-148">Your data will appear.</span></span>
5. <span data-ttu-id="48b09-149">No menu de entrega de **carga,** selecione **Carregar para**, e, em seguida, selecione **OK**.</span><span class="sxs-lookup"><span data-stu-id="48b09-149">In the **Load** dropdown menu, select **Load to**, and then select **OK**.</span></span>
6. <span data-ttu-id="48b09-150">Na caixa de diálogo **de dados de importação,** selecione **O Relatório De Mesa Para** abrir o seu ficheiro.</span><span class="sxs-lookup"><span data-stu-id="48b09-150">In the **Import Data** dialog box, select **PivotTable Report** to open your file.</span></span>

## <a name="negative-amount-displayed"></a><span data-ttu-id="48b09-151">Quantidade negativa exibida</span><span class="sxs-lookup"><span data-stu-id="48b09-151">Negative amount displayed</span></span>

<span data-ttu-id="48b09-152">Pode ver uma quantia negativa no seu ficheiro de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="48b09-152">You may see a negative amount in your reconciliation file.</span></span> <span data-ttu-id="48b09-153">Este problema, provavelmente, é causado por uma das razões seguintes:</span><span class="sxs-lookup"><span data-stu-id="48b09-153">This is probably caused by one of the following things:</span></span>

- <span data-ttu-id="48b09-154">Cancelou recentemente ou reduziu o seu número de licenças</span><span class="sxs-lookup"><span data-stu-id="48b09-154">You recently canceled or reduced your number of licenses</span></span>
- <span data-ttu-id="48b09-155">Recebeu crédito por um contrato de licença de serviço (SLA) ou para consumo Azure</span><span class="sxs-lookup"><span data-stu-id="48b09-155">You received credit for either a service license agreement (SLA) or for Azure consumption</span></span>

<span data-ttu-id="48b09-156">Para obter mais informações sobre esta transação, veja o atributo de tipo de custo no ficheiro de reconciliação.</span><span class="sxs-lookup"><span data-stu-id="48b09-156">To get more information about this transaction, review its charge type attribute in your reconciliation file.</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="48b09-157">Taxas de mapa ou IVA</span><span class="sxs-lookup"><span data-stu-id="48b09-157">Map taxes or VAT</span></span>

<span data-ttu-id="48b09-158">Para mapear impostos ou imposto sobre o valor acrescentado (IVA) na sua fatura:</span><span class="sxs-lookup"><span data-stu-id="48b09-158">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="48b09-159">Soma a coluna **Fiscal** do ficheiro baseado na licença.</span><span class="sxs-lookup"><span data-stu-id="48b09-159">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="48b09-160">Soma a coluna **TaxAmount** a partir do ficheiro baseado na utilização.</span><span class="sxs-lookup"><span data-stu-id="48b09-160">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="48b09-161">Itemize ficheiros de reconciliação por parceiro</span><span class="sxs-lookup"><span data-stu-id="48b09-161">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="48b09-162">Os parceiros no **modelo indireto** podem utilizar estes campos adicionais em ficheiros de reconciliação baseados em licenças e uso para itemizar os ficheiros por revendedor.</span><span class="sxs-lookup"><span data-stu-id="48b09-162">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="48b09-163">ID do MPN</span><span class="sxs-lookup"><span data-stu-id="48b09-163">MPN ID</span></span> | <span data-ttu-id="48b09-164">Description</span><span class="sxs-lookup"><span data-stu-id="48b09-164">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="48b09-165">ID do MPN</span><span class="sxs-lookup"><span data-stu-id="48b09-165">MPN ID</span></span> | <span data-ttu-id="48b09-166">O identificador da Microsoft Partner Network (MPN) do parceiro Cloud Solution Provider (CSP) (direto ou indireto).</span><span class="sxs-lookup"><span data-stu-id="48b09-166">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="48b09-167">Revendedor MPN ID</span><span class="sxs-lookup"><span data-stu-id="48b09-167">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="48b09-168">O [identificador MPN do revendedor de registos para a subscrição](#reseller-mpn-id).</span><span class="sxs-lookup"><span data-stu-id="48b09-168">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="48b09-169">Este campo corresponde ao ID revendedor listado para a subscrição específica no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="48b09-169">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="48b09-170">Só aparece em ficheiros de reconciliação para parceiros no modelo indireto.</span><span class="sxs-lookup"><span data-stu-id="48b09-170">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="48b09-171">Revendedor MPN ID</span><span class="sxs-lookup"><span data-stu-id="48b09-171">Reseller MPN ID</span></span>

<span data-ttu-id="48b09-172">Se um parceiro da CSP vendeu a subscrição diretamente ao cliente, o seu **ID MPN** está listado duas vezes, tanto como o **ID MPN** e o **ID do Revendedor MPN**.</span><span class="sxs-lookup"><span data-stu-id="48b09-172">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="48b09-173">Se um parceiro CSP tiver um revendedor sem **ID MPN,** este valor é definido para o **ID MPN** do parceiro.</span><span class="sxs-lookup"><span data-stu-id="48b09-173">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="48b09-174">Se o parceiro CSP remover um **ID MPN revendedor,** este valor será definido para *-1*.</span><span class="sxs-lookup"><span data-stu-id="48b09-174">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="48b09-175">Para visualizar ou atualizar o **ID MPN do Revendedor:**</span><span class="sxs-lookup"><span data-stu-id="48b09-175">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="48b09-176">Inicie sessão no Centro de Parceiros.</span><span class="sxs-lookup"><span data-stu-id="48b09-176">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="48b09-177">No menu Partner Center, selecione **Clientes.**</span><span class="sxs-lookup"><span data-stu-id="48b09-177">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="48b09-178">Escolha o cliente na lista.</span><span class="sxs-lookup"><span data-stu-id="48b09-178">Choose the customer from the list.</span></span>
4. <span data-ttu-id="48b09-179">No menu do cliente, **selecione Subscrições.**</span><span class="sxs-lookup"><span data-stu-id="48b09-179">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="48b09-180">Escolha a subscrição da lista.</span><span class="sxs-lookup"><span data-stu-id="48b09-180">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="48b09-181">Selecione **atualização** para alterar o **Revendedor (MPN ID)**.</span><span class="sxs-lookup"><span data-stu-id="48b09-181">Select **update** to change the **Reseller (MPN ID)**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="48b09-182">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="48b09-182">Next steps</span></span>

- [<span data-ttu-id="48b09-183">Como ler o seu ficheiro de & de reconhecimento</span><span class="sxs-lookup"><span data-stu-id="48b09-183">How to read your bill & recon file</span></span>](read-your-bill.md) 