---
title: Diretor de serviço AZure AD
ms.topic: how-to
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Descubra como adicionar um diretor de serviço ao seu inquilino AZure AD. Fazê-lo significa adicionar uma aplicação AD Azure (principal serviço) no Partner Center.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 21ef2aaa46359570bbf13c12c5fb6c1f5eab080a
ms.sourcegitcommit: 37b0b2a7141907c8d21839de3128fb8a98575886
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2020
ms.locfileid: "92529491"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a><span data-ttu-id="6a061-104">Adicione uma aplicação AD AZure (principal serviço) no Partner Center</span><span class="sxs-lookup"><span data-stu-id="6a061-104">Add an Azure AD application (service principal) in Partner Center</span></span>

<span data-ttu-id="6a061-105">**Aplica-se a**</span><span class="sxs-lookup"><span data-stu-id="6a061-105">**Applies to**</span></span>

- <span data-ttu-id="6a061-106">Partner Center</span><span class="sxs-lookup"><span data-stu-id="6a061-106">Partner Center</span></span>

<span data-ttu-id="6a061-107">**Funções adequadas**</span><span class="sxs-lookup"><span data-stu-id="6a061-107">**Appropriate roles**</span></span>

- <span data-ttu-id="6a061-108">Administrador global</span><span class="sxs-lookup"><span data-stu-id="6a061-108">Global admin</span></span>

<span data-ttu-id="6a061-109">No programa Mercado Comercial no Partner Center, pode agora adicionar uma aplicação AD AD (principal serviço) como utilizador na sua conta Partner Center.</span><span class="sxs-lookup"><span data-stu-id="6a061-109">In the Commercial Marketplace program in Partner Center, you are now able to add an Azure AD application (service principal) as a user in your Partner Center account.</span></span> <span data-ttu-id="6a061-110">(Conseguiu fazê-lo anteriormente no seu Portal de Parceiros cloud, ou CPP.</span><span class="sxs-lookup"><span data-stu-id="6a061-110">(You were able to do so previously in your Cloud Partner Portal, or CPP, account.</span></span> <span data-ttu-id="6a061-111">Agora que emigrou para o Partner Center, a conta do CPP é apenas de leitura.)</span><span class="sxs-lookup"><span data-stu-id="6a061-111">Now that you have migrated to Partner Center, the CPP account is read-only.)</span></span>
 
>[!Note] 
><span data-ttu-id="6a061-112">O diretor de serviço é sinónimo de aplicação Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6a061-112">Service principal is synonymous with Azure AD application.</span></span>

## <a name="add-an-azure-ad-application-service-principal"></a><span data-ttu-id="6a061-113">Adicione uma aplicação AD AZure (principal serviço)</span><span class="sxs-lookup"><span data-stu-id="6a061-113">Add an Azure AD application (service principal)</span></span>

1. <span data-ttu-id="6a061-114">A partir do painel 'Partner Center', selecione **Definições** e, em seguida, selecione **as definições do Programador** .</span><span class="sxs-lookup"><span data-stu-id="6a061-114">From the Partner Center dashboard, select **Settings** and then select **Developer settings** .</span></span>

2. <span data-ttu-id="6a061-115">Selecione **Utilizadores** e, em seguida, **selecione Adicionar Aplicações AD Azure** .</span><span class="sxs-lookup"><span data-stu-id="6a061-115">Select **Users** and then select **Add Azure AD Applications** .</span></span>

3. <span data-ttu-id="6a061-116">Selecione uma aplicação AD Azure existente ou crie uma nova.</span><span class="sxs-lookup"><span data-stu-id="6a061-116">Select an existing Azure AD application or create a new one.</span></span>

4. <span data-ttu-id="6a061-117">Se criar uma nova aplicação AD Azure, inclua as seguintes informações:</span><span class="sxs-lookup"><span data-stu-id="6a061-117">If you create a new Azure AD Application, include the following information:</span></span>  

   - <span data-ttu-id="6a061-118">**URL de resposta** : O URL onde os utilizadores podem iniciar sação para utilizar a sua aplicação AD Azure.</span><span class="sxs-lookup"><span data-stu-id="6a061-118">**Reply URL** : The URL where users can sign in to use your Azure AD application.</span></span>

   - <span data-ttu-id="6a061-119">**App ID URI** : Um identificador lógico para a aplicação Azure AD que é apresentado quando envia um único pedido de inscrição para Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6a061-119">**App ID URI** : A logical identifier for the Azure AD application that is presented when it sends a single sign-on request to Azure AD.</span></span>

   - <span data-ttu-id="6a061-120">**Funções de segurança** : O **Gestor** de Funções (o mesmo que o papel de 'Proprietário' no CPP) e o **Desenvolvedor** (o mesmo papel de 'Contribuinte' no CPP) aplicam-se ao programa de Marketplace Comercial no Partner Center, podendo ser associados a esta Aplicação AD Azure.</span><span class="sxs-lookup"><span data-stu-id="6a061-120">**Security roles** : The roles **Manager** (the same as  ‘Owner’ role in CPP) and **Developer** (the same as ‘Contributor’ role in CPP) apply to the Commercial Marketplace program in Partner Center, and they can be associated with this Azure AD Application.</span></span>  

## <a name="next-steps"></a><span data-ttu-id="6a061-121">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="6a061-121">Next steps</span></span>

- [<span data-ttu-id="6a061-122">Visão geral do mercado comercial no Partner Center</span><span class="sxs-lookup"><span data-stu-id="6a061-122">Overview of the commercial marketplace in Partner Center</span></span>](csp-commercial-marketplace-overview.md)