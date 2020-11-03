---
title: Azure Cost Management by Cloudyn para CSPs
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como registar a aplicação web Cloudyn e use uma chave secreta para ela no Partner Center para que possa usar a app para rastrear o uso e os custos do cliente Azure.
author: aparnagkrishnan
ms.author: aparnag
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4ea156ef0932fe1af20f3e3c4b9be1a5f931cdde
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/17/2020
ms.locfileid: "92529268"
---
# <a name="track-customer-azure-usage-and-costs-with-the-azure-cost-management-app-for-csp-partners"></a><span data-ttu-id="a9e16-103">Acompanhe o uso do cliente Azure e os custos com a app de gestão de custos Azure para parceiros CSP</span><span class="sxs-lookup"><span data-stu-id="a9e16-103">Track customer Azure usage and costs with the Azure cost management app for CSP partners</span></span>  

<span data-ttu-id="a9e16-104">**Aplica-se a**</span><span class="sxs-lookup"><span data-stu-id="a9e16-104">**Applies to**</span></span>

- <span data-ttu-id="a9e16-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="a9e16-105">Partner Center</span></span>
- <span data-ttu-id="a9e16-106">Parceiros de programas cloud Solution Provider</span><span class="sxs-lookup"><span data-stu-id="a9e16-106">Cloud Solution Provider program partners</span></span>

<span data-ttu-id="a9e16-107">**Funções adequadas**</span><span class="sxs-lookup"><span data-stu-id="a9e16-107">**Appropriate roles**</span></span>

- <span data-ttu-id="a9e16-108">Administrador global</span><span class="sxs-lookup"><span data-stu-id="a9e16-108">Global admin</span></span>
- <span data-ttu-id="a9e16-109">Agente administrativo</span><span class="sxs-lookup"><span data-stu-id="a9e16-109">Admin agent</span></span>

[<span data-ttu-id="a9e16-110">Obtenha mais informações sobre a Azure Cost Management</span><span class="sxs-lookup"><span data-stu-id="a9e16-110">Get More information about Azure Cost Management</span></span>](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a><span data-ttu-id="a9e16-111">Antes de começar</span><span class="sxs-lookup"><span data-stu-id="a9e16-111">Before you begin</span></span>
<span data-ttu-id="a9e16-112">Antes de poder utilizar a Azure Cost Management, certifique-se de que cumpre os seguintes requisitos:</span><span class="sxs-lookup"><span data-stu-id="a9e16-112">Before you can use Azure Cost Management, be sure you meet the following requirements:</span></span>

- <span data-ttu-id="a9e16-113">É um parceiro no programa Cloud Solution Provider.</span><span class="sxs-lookup"><span data-stu-id="a9e16-113">You are a partner in the Cloud Solution Provider program.</span></span>
- <span data-ttu-id="a9e16-114">Você tem a capacidade de criar uma aplicação web Partner Center API.</span><span class="sxs-lookup"><span data-stu-id="a9e16-114">You have the ability to create a Partner Center API web app.</span></span>

## <a name="overview"></a><span data-ttu-id="a9e16-115">Descrição geral</span><span class="sxs-lookup"><span data-stu-id="a9e16-115">Overview</span></span>

<span data-ttu-id="a9e16-116">A Cloudyn é uma aplicação web que permite rastrear e gerir o quanto os seus clientes estão a usar o Azure e os custos dessa utilização.</span><span class="sxs-lookup"><span data-stu-id="a9e16-116">Cloudyn is a web app that allows you to track and manage how much your customers are using Azure and the costs of that usage.</span></span> <span data-ttu-id="a9e16-117">Usa-o através da API do Centro Parceiro.</span><span class="sxs-lookup"><span data-stu-id="a9e16-117">You use it through the Partner Center API.</span></span>

## <a name="register-your-web-app-in-the-partner-center"></a><span data-ttu-id="a9e16-118">Registe a sua aplicação web no Centro de Parceiros</span><span class="sxs-lookup"><span data-stu-id="a9e16-118">Register your web app in the Partner Center</span></span>
<span data-ttu-id="a9e16-119">Quando regista uma aplicação web Azure Ative Directory no Partner Center, permite o acesso à API do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="a9e16-119">When you register an Azure Active Directory web app in Partner Center you enable access to the Partner Center API.</span></span> 
1.  <span data-ttu-id="a9e16-120">Inscreva-se [no Partner Center](https://partnercenter.microsoft.com/pcv/dashboard/overview) utilizando uma conta global de administrador ou agente [administrativo.](create-user-accounts-and-set-permissions.md)</span><span class="sxs-lookup"><span data-stu-id="a9e16-120">Sign into [the Partner Center](https://partnercenter.microsoft.com/pcv/dashboard/overview) using a [global admin or admin agent account](create-user-accounts-and-set-permissions.md).</span></span>
2.  <span data-ttu-id="a9e16-121">A partir do **Centro de Parceiros,** selecione Gestão de **aplicações de contas.** &gt; **[App management](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)**</span><span class="sxs-lookup"><span data-stu-id="a9e16-121">From the **Partner Center** , select **Account settings** &gt; **[App management](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)** .</span></span>
3.  <span data-ttu-id="a9e16-122">Na secção **Aplicação Web,** clique em **Adicionar nova aplicação web.**</span><span class="sxs-lookup"><span data-stu-id="a9e16-122">In the **Web App** section, click **Add new web app** .</span></span>
<br> <span data-ttu-id="a9e16-123">**Nota:** Se já criou uma aplicação web, pode saltar o passo 3.</span><span class="sxs-lookup"><span data-stu-id="a9e16-123">**Note** : If you have previously created a web app, you can skip step 3.</span></span>
4.  <span data-ttu-id="a9e16-124">Copie e guarde o **Commerce ID** GUID e o **App ID** GUID para a sua aplicação web.</span><span class="sxs-lookup"><span data-stu-id="a9e16-124">Copy and save the **Commerce ID** GUID and the **App ID** GUID for your web app.</span></span> <span data-ttu-id="a9e16-125">Você precisará de ambos os IDs para usar o teste gratuito de 30 dias da app de gestão de custos Azure.</span><span class="sxs-lookup"><span data-stu-id="a9e16-125">You will need both IDs to use the 30-day free trial of the Azure cost management app.</span></span>

## <a name="add-a-secret-key-to-your-app"></a><span data-ttu-id="a9e16-126">Adicione uma chave secreta à sua aplicação</span><span class="sxs-lookup"><span data-stu-id="a9e16-126">Add a secret key to your app</span></span>
1. <span data-ttu-id="a9e16-127">Na descida ao lado do botão **Adicionar,** selecione uma duração de 1 ou 2 anos.</span><span class="sxs-lookup"><span data-stu-id="a9e16-127">In the drop down next to the **Add key** button, select a duration of 1 or 2 years.</span></span>
2. <span data-ttu-id="a9e16-128">Clique **na tecla Adicionar** .</span><span class="sxs-lookup"><span data-stu-id="a9e16-128">Click **Add key** .</span></span> 
3. <span data-ttu-id="a9e16-129">Copie e guarde o valor da chave secreta.</span><span class="sxs-lookup"><span data-stu-id="a9e16-129">Copy and save the secret key value.</span></span> <span data-ttu-id="a9e16-130">Vai precisar disto para o julgamento gratuito de 30 dias.</span><span class="sxs-lookup"><span data-stu-id="a9e16-130">You will need this for the 30-day free trial.</span></span><br>
   > [!NOTE]  
   > <span data-ttu-id="a9e16-131">As chaves secretas da aplicação são como senhas com datas de validade mais longas.</span><span class="sxs-lookup"><span data-stu-id="a9e16-131">The application secret keys are like passwords with longer expiration dates.</span></span> <span data-ttu-id="a9e16-132">Guarde o valor da chave num local seguro para utilização futura.</span><span class="sxs-lookup"><span data-stu-id="a9e16-132">Please save the key value in a secure location for future use.</span></span>

## <a name="next-steps"></a><span data-ttu-id="a9e16-133">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="a9e16-133">Next steps</span></span>
<span data-ttu-id="a9e16-134">Inicie um [julgamento gratuito de 30 dias.](https://go.microsoft.com/fwlink/?linkid=857895)</span><span class="sxs-lookup"><span data-stu-id="a9e16-134">Start a [30-day free trial](https://go.microsoft.com/fwlink/?linkid=857895).</span></span>
<span data-ttu-id="a9e16-135">Precisa dos seguintes detalhes para iniciar o julgamento:</span><span class="sxs-lookup"><span data-stu-id="a9e16-135">You need the following details to start the trial:</span></span>
- <span data-ttu-id="a9e16-136">Signo do Centro parceiro em credenciais</span><span class="sxs-lookup"><span data-stu-id="a9e16-136">Partner Center sign in credentials</span></span>
- <span data-ttu-id="a9e16-137">Commerce ID GUID</span><span class="sxs-lookup"><span data-stu-id="a9e16-137">Commerce ID GUID</span></span>
- <span data-ttu-id="a9e16-138">App ID GUID</span><span class="sxs-lookup"><span data-stu-id="a9e16-138">App ID GUID</span></span>
- <span data-ttu-id="a9e16-139">Valor chave segredo da aplicação</span><span class="sxs-lookup"><span data-stu-id="a9e16-139">Application secret key value</span></span>
