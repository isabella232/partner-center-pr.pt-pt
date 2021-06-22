---
title: Resolução de problemas configurando a sua conta Partner Center ou problemas de renovação de MPN
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Problemas de resolução de problemas ao tentar matricular-se no Partner Center. Respostas abordam desafios com métodos de pagamento, esquecendo palavras-passe, e muito mais.
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4fc1a43b4d525d9221ac7e4db56f5f278404e3f5
ms.sourcegitcommit: bce54ddb9fff7332a03d6aa228ba9414a87d76b7
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/22/2021
ms.locfileid: "112431758"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a><span data-ttu-id="97c4f-104">Configuração de conta de resolução de problemas ou problemas de renovação de MPN</span><span class="sxs-lookup"><span data-stu-id="97c4f-104">Troubleshoot account setup or MPN renewal issues</span></span>

<span data-ttu-id="97c4f-105">**Funções adequadas**: Administração global | Administrador sócio da MPN</span><span class="sxs-lookup"><span data-stu-id="97c4f-105">**Appropriate roles**: Global admin | MPN partner admin</span></span>
 
<span data-ttu-id="97c4f-106">Aqui ficam algumas sugestões para resolver problemas comuns que surgem ao configurar a sua conta Partner Center.</span><span class="sxs-lookup"><span data-stu-id="97c4f-106">Here are some suggestions for troubleshooting common issues that arise when setting up your Partner Center account.</span></span>

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a><span data-ttu-id="97c4f-107">O que acontece se estiver a migrar do Centro de Membros de Parceiros e não puder editar quaisquer campos de informação da empresa</span><span class="sxs-lookup"><span data-stu-id="97c4f-107">What happens if you are migrating from Partner Membership Center and you can't edit any company information fields</span></span>

<span data-ttu-id="97c4f-108">Nos casos em que a sua empresa já tenha presença no Partner Center (por exemplo, uma conta Cloud Solution Provider (CSP) – será mostrado um ecrã apenas de leitura.</span><span class="sxs-lookup"><span data-stu-id="97c4f-108">In cases where your company already has a presence in Partner Center (for example, a Cloud Solution Provider (CSP) account) – you will be shown a read-only screen.</span></span> <span data-ttu-id="97c4f-109">Este ecrã apresentará todas as informações sobre a sua empresa tal como existe no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="97c4f-109">This screen will display all the information about your company as it exists in Partner Center.</span></span>

<span data-ttu-id="97c4f-110">Não podes alterar os detalhes deste ecrã.</span><span class="sxs-lookup"><span data-stu-id="97c4f-110">You can't change the details on this screen.</span></span> <span data-ttu-id="97c4f-111">Isto é por design e não por um erro.</span><span class="sxs-lookup"><span data-stu-id="97c4f-111">This is by design and not an error.</span></span>

<span data-ttu-id="97c4f-112">Para prosseguir, **selecione Aceitar** e, em seguida, selecione **Continue**.</span><span class="sxs-lookup"><span data-stu-id="97c4f-112">To proceed, select **Accept**, and then select **Continue**.</span></span>


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a><span data-ttu-id="97c4f-113">Se o departamento de TI tiver desligado **inscreva-se no Partner Center**</span><span class="sxs-lookup"><span data-stu-id="97c4f-113">If the IT department has turned off **Sign up for Partner Center**</span></span>

<span data-ttu-id="97c4f-114">Você vê esta mensagem porque os utilizadores virais são desativado, ou porque a Inscrição Viral é desativada no inquilino do Azure Ative Directory (AD).</span><span class="sxs-lookup"><span data-stu-id="97c4f-114">You see this message because viral users are disabled, or because Viral Sign-up is disabled on the Azure Active Directory (AD) tenant.</span></span> <span data-ttu-id="97c4f-115">O administrador Global para a sua conta Azure AD pode permitir as funcionalidades necessárias executando o seguinte comando PowerShell:</span><span class="sxs-lookup"><span data-stu-id="97c4f-115">The Global admin for your Azure AD account can enable required features by running the following PowerShell command:</span></span>

<span data-ttu-id="97c4f-116">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span><span class="sxs-lookup"><span data-stu-id="97c4f-116">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span></span>

<span data-ttu-id="97c4f-117">Para mais informações, leia [o Self-service inscreva-se.](/azure/active-directory/users-groups-roles/directory-self-service-signup)</span><span class="sxs-lookup"><span data-stu-id="97c4f-117">For more information, read [Self-service sign up](/azure/active-directory/users-groups-roles/directory-self-service-signup).</span></span>

## <a name="you-forgot-your-password"></a><span data-ttu-id="97c4f-118">Esqueceu-se da sua senha.</span><span class="sxs-lookup"><span data-stu-id="97c4f-118">You forgot your password</span></span>

<span data-ttu-id="97c4f-119">Se esqueceu a sua palavra-passe, na página de iniciar scontabilidade, selecione **Não pode aceder à sua conta?**</span><span class="sxs-lookup"><span data-stu-id="97c4f-119">If you have forgotten your password, on the sign-in page, select **Can't access your account?**.</span></span> <span data-ttu-id="97c4f-120">Esta opção permite-lhe redefinir a sua palavra-passe ou pedir ao seu administrador Global para lhe atribuir novas credenciais.</span><span class="sxs-lookup"><span data-stu-id="97c4f-120">This option lets you reset your password or ask your Global admin to assign you new credentials.</span></span>

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a><span data-ttu-id="97c4f-121">No ecrã "Fale-nos da sua empresa", recebe um erro de "Algo correu mal"</span><span class="sxs-lookup"><span data-stu-id="97c4f-121">On the “Tell us about your company” screen, you receive a “Something went wrong” error</span></span>

<span data-ttu-id="97c4f-122">Esta mensagem de erro geralmente aparece se utilizar inadvertidamente caracteres, espaços ou código de país no número de telefone da sua empresa.</span><span class="sxs-lookup"><span data-stu-id="97c4f-122">This error message usually shows up if you inadvertently use special characters, spaces, or country code in your company phone number.</span></span> <span data-ttu-id="97c4f-123">O valor introduzido no campo Número de Telefone só pode conter um máximo de 10 caracteres.</span><span class="sxs-lookup"><span data-stu-id="97c4f-123">The value entered in the Phone Number field can only contain a maximum of 10 characters.</span></span>


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a><span data-ttu-id="97c4f-124">A compra do seu cartão de crédito está a receber uma mensagem de erro afirmando que "a sua encomenda foi recusada.</span><span class="sxs-lookup"><span data-stu-id="97c4f-124">Your credit card purchase is receiving an error message stating that “Your order was declined.</span></span> <span data-ttu-id="97c4f-125">Por favor, verifique as suas informações"</span><span class="sxs-lookup"><span data-stu-id="97c4f-125">Please verify your information”</span></span>


<span data-ttu-id="97c4f-126">Utilize sempre o endereço correspondente ao seu cartão de crédito e não à sua entidade legal.</span><span class="sxs-lookup"><span data-stu-id="97c4f-126">Always use the address corresponding to your credit card rather than your legal entity.</span></span> <span data-ttu-id="97c4f-127">Além disso, certifique-se de que o código postal está correto e corresponde ao endereço que utiliza.</span><span class="sxs-lookup"><span data-stu-id="97c4f-127">Also, make sure the zip code is correct and corresponds to the address you use.</span></span>

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a><span data-ttu-id="97c4f-128">Pretende mudar de pagamento offline para método de pagamento online</span><span class="sxs-lookup"><span data-stu-id="97c4f-128">You want to switch from offline payment to online payment method</span></span> 

<span data-ttu-id="97c4f-129">Terá de cancelar a encomenda original e recomprar utilizando o método de pagamento preferido.</span><span class="sxs-lookup"><span data-stu-id="97c4f-129">You will need to cancel the original order and repurchase using the preferred payment method.</span></span>

<span data-ttu-id="97c4f-130">Para cancelar uma encomenda:</span><span class="sxs-lookup"><span data-stu-id="97c4f-130">To cancel an order:</span></span>

1. <span data-ttu-id="97c4f-131">No painel Partner Center, selecione o **separador Ofertas de Adesão.**</span><span class="sxs-lookup"><span data-stu-id="97c4f-131">In the Partner Center dashboard, select the **Membership Offers** tab.</span></span>

2. <span data-ttu-id="97c4f-132">Selecione **cancelar pedido**</span><span class="sxs-lookup"><span data-stu-id="97c4f-132">Select **Cancel order**</span></span>

3. <span data-ttu-id="97c4f-133">Aparecerá uma janela de confirmação e deve confirmar-se para cancelar a encomenda inicial.</span><span class="sxs-lookup"><span data-stu-id="97c4f-133">A confirmation window will appear and you must confirm in order to cancel the initial order.</span></span>

## <a name="next-steps"></a><span data-ttu-id="97c4f-134">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="97c4f-134">Next steps</span></span>

- <span data-ttu-id="97c4f-135">[Manage your Partner Center account](partner-center-account-setup.md) (Gerir a conta do Partner Center)</span><span class="sxs-lookup"><span data-stu-id="97c4f-135">[Manage your Partner Center account](partner-center-account-setup.md)</span></span>
- [<span data-ttu-id="97c4f-136">Como ler o seu projeto de lei e arquivo de reconhecimento</span><span class="sxs-lookup"><span data-stu-id="97c4f-136">How to read your bill and recon file</span></span>](read-your-bill.md)
