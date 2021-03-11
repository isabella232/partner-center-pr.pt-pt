---
title: Use os seus ficheiros de reconciliação
ms.topic: article
ms.date: 03/10/2021
description: Conheça os ficheiros de reconciliação no Partner Center e como interpretar as vistas detalhadas e de item de linha das taxas para um determinado ciclo de faturação.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e6b9e466402d71c988729052bd72ba2346a9d977
ms.sourcegitcommit: 868f90c54f26a037eee29749c207a7316bb4b475
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/11/2021
ms.locfileid: "103022779"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="11a0a-103">Saiba como ler os itens de linha nos ficheiros de reconciliação do Partner Center</span><span class="sxs-lookup"><span data-stu-id="11a0a-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="11a0a-104">**Funções adequadas**</span><span class="sxs-lookup"><span data-stu-id="11a0a-104">**Appropriate roles**</span></span>

- <span data-ttu-id="11a0a-105">Administrador de faturação</span><span class="sxs-lookup"><span data-stu-id="11a0a-105">Billing admin</span></span>
- <span data-ttu-id="11a0a-106">Administrador global</span><span class="sxs-lookup"><span data-stu-id="11a0a-106">Global admin</span></span>

<span data-ttu-id="11a0a-107">Pode descarregar os seus ficheiros de reconciliação do Partner Center para uma visão detalhada e de item de linha de cada carga num ciclo de faturação.</span><span class="sxs-lookup"><span data-stu-id="11a0a-107">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="11a0a-108">Os detalhes do item da linha incluem taxas para as subscrições de cada cliente, e eventos detalhados (como uma adição intercalar de licenças a uma subscrição).</span><span class="sxs-lookup"><span data-stu-id="11a0a-108">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="11a0a-109">Para obter informações sobre como ler a sua **fatura,** consulte [a sua conta](read-your-bill.md).</span><span class="sxs-lookup"><span data-stu-id="11a0a-109">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="11a0a-110">Compreender os campos de arquivos de reconciliação</span><span class="sxs-lookup"><span data-stu-id="11a0a-110">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="11a0a-111">Campos do ficheiro de reconciliação baseado em licenças</span><span class="sxs-lookup"><span data-stu-id="11a0a-111">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="11a0a-112">Campos do ficheiro de reconciliação baseado na utilização</span><span class="sxs-lookup"><span data-stu-id="11a0a-112">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="11a0a-113">Campos do ficheiro de reconciliação da utilização diária</span><span class="sxs-lookup"><span data-stu-id="11a0a-113">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)
- [<span data-ttu-id="11a0a-114">Compra única campos de ficheiros de reconciliação CSP</span><span class="sxs-lookup"><span data-stu-id="11a0a-114">One-time purchase CSP reconciliation file fields</span></span>](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="11a0a-115">Compreender tipos de carga em ficheiros de reconciliação</span><span class="sxs-lookup"><span data-stu-id="11a0a-115">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="11a0a-116">Para compreender os tipos de encargos nos ficheiros de reconciliação (a coluna **ChargeType),** consulte os tipos de [carga de ficheiros de reconciliação](recon-file-charge-types.md).</span><span class="sxs-lookup"><span data-stu-id="11a0a-116">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="11a0a-117">Corrigir problemas de formatação</span><span class="sxs-lookup"><span data-stu-id="11a0a-117">Fix formatting issues</span></span>

<span data-ttu-id="11a0a-118">Ocasionalmente, um ficheiro de reconciliação pode conter problemas de formatação.</span><span class="sxs-lookup"><span data-stu-id="11a0a-118">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="11a0a-119">Por exemplo, esta questão pode ocorrer se o local en-US não for utilizado.</span><span class="sxs-lookup"><span data-stu-id="11a0a-119">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="11a0a-120">Siga estes passos para corrigir quaisquer problemas de formatação nos seus ficheiros de reconciliação:</span><span class="sxs-lookup"><span data-stu-id="11a0a-120">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="11a0a-121">Abra o ficheiro de reconciliação (em .csv formato) no Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="11a0a-121">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="11a0a-122">Selecione a primeira coluna do ficheiro.</span><span class="sxs-lookup"><span data-stu-id="11a0a-122">Select the first column in the file.</span></span>
3. <span data-ttu-id="11a0a-123">Abra o **texto de conversão para o assistente de colunas**.</span><span class="sxs-lookup"><span data-stu-id="11a0a-123">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="11a0a-124">Na fita, selecione **Dados** e, em seguida, selecione **Texto para Colunas**.</span><span class="sxs-lookup"><span data-stu-id="11a0a-124">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="11a0a-125">No assistente, selecione **O tipo de ficheiro delimitado**.</span><span class="sxs-lookup"><span data-stu-id="11a0a-125">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="11a0a-126">Em seguida, selecione **Seguinte**.</span><span class="sxs-lookup"><span data-stu-id="11a0a-126">Then, select **Next**.</span></span>
5. <span data-ttu-id="11a0a-127">No campo **Delimiters,** **selecione Comma**.</span><span class="sxs-lookup"><span data-stu-id="11a0a-127">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="11a0a-128">(Se **o Separador** já estiver selecionado, pode deixar esta opção selecionada.) Em seguida, selecione **Seguinte**.</span><span class="sxs-lookup"><span data-stu-id="11a0a-128">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="11a0a-129">No campo do **formato de dados da Coluna,** selecione **Data:MDY**.</span><span class="sxs-lookup"><span data-stu-id="11a0a-129">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="11a0a-130">Em seguida, selecione **Seguinte**.</span><span class="sxs-lookup"><span data-stu-id="11a0a-130">Then, select **Next**.</span></span>
7. <span data-ttu-id="11a0a-131">No campo de **formato de dados da Coluna,** selecione **Texto** para todas as colunas de valor.</span><span class="sxs-lookup"><span data-stu-id="11a0a-131">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="11a0a-132">Em seguida, selecione **Finish** (Concluir).</span><span class="sxs-lookup"><span data-stu-id="11a0a-132">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="11a0a-133">Descarregue os ficheiros de reconciliação programáticamente</span><span class="sxs-lookup"><span data-stu-id="11a0a-133">Download reconciliation files programmatically</span></span>

<span data-ttu-id="11a0a-134">Os ficheiros de reconciliação podem ser muito grandes e por vezes são difíceis de descarregar.</span><span class="sxs-lookup"><span data-stu-id="11a0a-134">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="11a0a-135">Para descarregar ficheiros de reconciliação programáticamente, consulte [obter itens de linha de fatura](/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="11a0a-135">To download reconciliation files programmatically, see [Get invoice line items](/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="11a0a-136">Taxas de mapa ou IVA</span><span class="sxs-lookup"><span data-stu-id="11a0a-136">Map taxes or VAT</span></span>

<span data-ttu-id="11a0a-137">Para mapear impostos ou imposto sobre o valor acrescentado (IVA) na sua fatura:</span><span class="sxs-lookup"><span data-stu-id="11a0a-137">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="11a0a-138">Soma a coluna **Fiscal** do ficheiro baseado na licença.</span><span class="sxs-lookup"><span data-stu-id="11a0a-138">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="11a0a-139">Soma a coluna **TaxAmount** a partir do ficheiro baseado na utilização.</span><span class="sxs-lookup"><span data-stu-id="11a0a-139">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="11a0a-140">Itemize ficheiros de reconciliação por parceiro</span><span class="sxs-lookup"><span data-stu-id="11a0a-140">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="11a0a-141">Os parceiros no **modelo indireto** podem utilizar estes campos adicionais em ficheiros de reconciliação baseados em licenças e uso para itemizar os ficheiros por revendedor.</span><span class="sxs-lookup"><span data-stu-id="11a0a-141">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="11a0a-142">ID do MPN</span><span class="sxs-lookup"><span data-stu-id="11a0a-142">MPN ID</span></span> | <span data-ttu-id="11a0a-143">Description</span><span class="sxs-lookup"><span data-stu-id="11a0a-143">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="11a0a-144">ID do MPN</span><span class="sxs-lookup"><span data-stu-id="11a0a-144">MPN ID</span></span> | <span data-ttu-id="11a0a-145">O identificador da Microsoft Partner Network (MPN) do parceiro Cloud Solution Provider (CSP) (direto ou indireto).</span><span class="sxs-lookup"><span data-stu-id="11a0a-145">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="11a0a-146">Revendedor MPN ID</span><span class="sxs-lookup"><span data-stu-id="11a0a-146">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="11a0a-147">O [identificador MPN do revendedor de registos para a subscrição](#reseller-mpn-id).</span><span class="sxs-lookup"><span data-stu-id="11a0a-147">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="11a0a-148">Este campo corresponde ao ID revendedor listado para a subscrição específica no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="11a0a-148">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="11a0a-149">Só aparece em ficheiros de reconciliação para parceiros no modelo indireto.</span><span class="sxs-lookup"><span data-stu-id="11a0a-149">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="11a0a-150">Revendedor MPN ID</span><span class="sxs-lookup"><span data-stu-id="11a0a-150">Reseller MPN ID</span></span>

<span data-ttu-id="11a0a-151">Se um parceiro da CSP vendeu a subscrição diretamente ao cliente, o seu **ID MPN** está listado duas vezes, tanto como o **ID MPN** e o **ID do Revendedor MPN**.</span><span class="sxs-lookup"><span data-stu-id="11a0a-151">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="11a0a-152">Se um parceiro CSP tiver um revendedor sem **ID MPN,** este valor é definido para o **ID MPN** do parceiro.</span><span class="sxs-lookup"><span data-stu-id="11a0a-152">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="11a0a-153">Se o parceiro CSP remover um **ID MPN revendedor,** este valor será definido para *-1*.</span><span class="sxs-lookup"><span data-stu-id="11a0a-153">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="11a0a-154">Para visualizar ou atualizar o **ID MPN do Revendedor:**</span><span class="sxs-lookup"><span data-stu-id="11a0a-154">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="11a0a-155">Inicie sessão no Centro de Parceiros.</span><span class="sxs-lookup"><span data-stu-id="11a0a-155">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="11a0a-156">No menu Partner Center, selecione **Clientes.**</span><span class="sxs-lookup"><span data-stu-id="11a0a-156">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="11a0a-157">Escolha o cliente na lista.</span><span class="sxs-lookup"><span data-stu-id="11a0a-157">Choose the customer from the list.</span></span>
4. <span data-ttu-id="11a0a-158">No menu do cliente, **selecione Subscrições.**</span><span class="sxs-lookup"><span data-stu-id="11a0a-158">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="11a0a-159">Escolha a subscrição da lista.</span><span class="sxs-lookup"><span data-stu-id="11a0a-159">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="11a0a-160">Selecione **atualização** para alterar o **Revendedor (MPN ID)**.</span><span class="sxs-lookup"><span data-stu-id="11a0a-160">Select **update** to change the **Reseller (MPN ID)**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="11a0a-161">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="11a0a-161">Next steps</span></span>

- [<span data-ttu-id="11a0a-162">Como ler o seu ficheiro de & de reconhecimento</span><span class="sxs-lookup"><span data-stu-id="11a0a-162">How to read your bill & recon file</span></span>](read-your-bill.md) 