---
title: Configurar os seus utilizadores com a autenticação multifator
ms.topic: how-to
ms.date: 12/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Saiba como configurar os seus colaboradores com o MFA
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: f42c97be88a1a505f7e0ae9b8af0d4a9167d8447
ms.sourcegitcommit: 531151a5dbc999b8b7de478d72ea115e6d579ff1
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/13/2021
ms.locfileid: "98182380"
---
# <a name="set-up-your-users-with-multi-factor-authentication"></a><span data-ttu-id="50196-103">Configurar os seus utilizadores com a autenticação multifator</span><span class="sxs-lookup"><span data-stu-id="50196-103">Set up your users with multi-factor authentication</span></span>

<span data-ttu-id="50196-104">**Funções adequadas**</span><span class="sxs-lookup"><span data-stu-id="50196-104">**Appropriate roles**</span></span>

- <span data-ttu-id="50196-105">Administrador global</span><span class="sxs-lookup"><span data-stu-id="50196-105">Global admin</span></span>

<span data-ttu-id="50196-106">Uma maior salvaguarda de privacidade e segurança estão entre as nossas principais prioridades.</span><span class="sxs-lookup"><span data-stu-id="50196-106">Greater privacy safeguards and security are among our top priorities.</span></span> <span data-ttu-id="50196-107">Sabemos que a melhor defesa é a prevenção e que somos tão fortes quanto o nosso elo mais fraco.</span><span class="sxs-lookup"><span data-stu-id="50196-107">We know that the best defense is prevention and that we are only as strong as our weakest link.</span></span> <span data-ttu-id="50196-108">É por isso que precisamos que todos os nossos ecossistemas atuem e garantam a proteção de segurança adequadas.</span><span class="sxs-lookup"><span data-stu-id="50196-108">That is why we need everyone in our ecosystem to act and ensure appropriate security protections are in place.</span></span> <span data-ttu-id="50196-109">Recomendamos vivamente que todos os parceiros permitam a autenticação de vários fatores (MFA) para os seus utilizadores no seu inquilino parceiro.</span><span class="sxs-lookup"><span data-stu-id="50196-109">We strongly recommend all partners enable multi-factor authentication (MFA) for their users in their partner tenant.</span></span> 

## <a name="add-multi-factor-authentication-for-your-users"></a><span data-ttu-id="50196-110">Adicionar autenticação multi-factor para os seus utilizadores</span><span class="sxs-lookup"><span data-stu-id="50196-110">Add multi-factor authentication for your users</span></span>

<span data-ttu-id="50196-111">Deve ser o administrador global da sua empresa para completar esta tarefa.</span><span class="sxs-lookup"><span data-stu-id="50196-111">You must be the global admin for your company to complete this task.</span></span>

<span data-ttu-id="50196-112">É mais fácil ativar o MFA para os seus utilizadores à medida que os adiciona ao seu inquilino AZure AD.</span><span class="sxs-lookup"><span data-stu-id="50196-112">It is easiest to enable MFA for your users as you add them to your Azure AD tenant.</span></span>

1. <span data-ttu-id="50196-113">Inscreva-se no [portal Azure](https://portal.azure.com) e, em seguida, vá para a **gestão do Utilizador**.</span><span class="sxs-lookup"><span data-stu-id="50196-113">Sign into the [Azure portal](https://portal.azure.com) and then go to **User management**.</span></span>
1. <span data-ttu-id="50196-114">Selecione **a autenticação de vários fatores.**</span><span class="sxs-lookup"><span data-stu-id="50196-114">Select **Multi-factor authentication**.</span></span>
1. <span data-ttu-id="50196-115">Selecione o utilizador que pretende ativar e, em seguida, selecione **Ative**.</span><span class="sxs-lookup"><span data-stu-id="50196-115">Select the user you want to enable and then select **Enable**.</span></span>

<span data-ttu-id="50196-116">Isto permitirá o MFA para este utilizador.</span><span class="sxs-lookup"><span data-stu-id="50196-116">This will enable MFA for this user.</span></span> <span data-ttu-id="50196-117">Ativado significa que o utilizador será solicitado a configurar a sua verificação de MFA quando iniciar o seu seru.</span><span class="sxs-lookup"><span data-stu-id="50196-117">Enabled means that the user will be asked to set up their MFA verification when they sign in for the first time.</span></span> <span data-ttu-id="50196-118">Posteriormente, ao iniciar o sôm, será-lhes solicitado que lhes forneçam um código que lhes seja enviado através de e-mail ou mensagem de texto (dependendo do que configurarem).</span><span class="sxs-lookup"><span data-stu-id="50196-118">Thereafter, at sign in, they will be asked to provide a code sent to them either through email or text message (depending on which they set up).</span></span>  

:::image type="content" source="images/MFA/securityverification.png" alt-text="Especificar como verificar":::

>[!NOTE]
><span data-ttu-id="50196-120">Pode **impor aos** seus utilizadores a utilização de MFA utilizando os mesmos passos acima e selecionando **Enforce**.</span><span class="sxs-lookup"><span data-stu-id="50196-120">You can **Enforce** your users to use MFA by using same steps as above and selecting **Enforce**.</span></span> <span data-ttu-id="50196-121">Para saber mais, leia [Ativar a autenticação multi-factor Azure por utilizador para garantir eventos de entrada.](/azure/active-directory/authentication/howto-mfa-userstates)</span><span class="sxs-lookup"><span data-stu-id="50196-121">To learn more, read [Enable per-user Azure Multi-Factor Authentication to secure sign-in events](/azure/active-directory/authentication/howto-mfa-userstates).</span></span> 

<span data-ttu-id="50196-122">Todos os utilizadores começam **desativados.**</span><span class="sxs-lookup"><span data-stu-id="50196-122">All users start out **Disabled**.</span></span> <span data-ttu-id="50196-123">Quando inscreve os utilizadores na autenticação multi-factor Azure por utilizador, o seu estado muda para **Enabled**.</span><span class="sxs-lookup"><span data-stu-id="50196-123">When you enroll users in per-user Azure Multi-Factor Authentication, their state changes to **Enabled**.</span></span> <span data-ttu-id="50196-124">Quando os utilizadores ativados iniciaram o seu registo e completam o processo de registo, as alterações de estado para **Aplicadas**.</span><span class="sxs-lookup"><span data-stu-id="50196-124">When enabled users sign in and complete the registration process, their state changes to **Enforced**.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="50196-125">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="50196-125">Next steps</span></span>

- [<span data-ttu-id="50196-126">Atribuir funções e permissões a utilizadores</span><span class="sxs-lookup"><span data-stu-id="50196-126">Assign roles and permissions to users</span></span>](permissions-overview.md)