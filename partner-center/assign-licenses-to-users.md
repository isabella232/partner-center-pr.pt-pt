---
title: Gerir utilizadores para contas de clientes
ms.topic: how-to
ms.date: 02/25/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Gerir os utilizadores para os seus clientes no Partner Center - criar contas de utilizador, adicionar ou remover licenças de utilizador, redefinir palavras-passe e eliminar ou restaurar as contas do utilizador.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 0e2bb4ceb146174da83e9c08a9ff030380298bd0
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/03/2021
ms.locfileid: "101756080"
---
# <a name="manage-users-and-user-licenses-for-customer-accounts"></a><span data-ttu-id="602d1-103">Gerir utilizadores e licenças de utilizador para contas de clientes</span><span class="sxs-lookup"><span data-stu-id="602d1-103">Manage users and user licenses for customer accounts</span></span> 

<span data-ttu-id="602d1-104">**Funções adequadas**</span><span class="sxs-lookup"><span data-stu-id="602d1-104">**Appropriate roles**</span></span>

- <span data-ttu-id="602d1-105">Administrador global</span><span class="sxs-lookup"><span data-stu-id="602d1-105">Global admin</span></span>
- <span data-ttu-id="602d1-106">Administração de gestão de utilizadores</span><span class="sxs-lookup"><span data-stu-id="602d1-106">User management admin</span></span>
- <span data-ttu-id="602d1-107">Agente administrativo</span><span class="sxs-lookup"><span data-stu-id="602d1-107">Admin agent</span></span>


<span data-ttu-id="602d1-108">Pode criar e eliminar novos utilizadores na conta de um cliente.</span><span class="sxs-lookup"><span data-stu-id="602d1-108">You can create and delete new users in a customer's account.</span></span> <span data-ttu-id="602d1-109">Também pode restaurar uma ou mais contas de utilizador que apagou anteriormente no prazo de 30 dias após a eliminação.</span><span class="sxs-lookup"><span data-stu-id="602d1-109">You can also restore one or more user accounts that you previously deleted within 30 days of the deletion.</span></span> <span data-ttu-id="602d1-110">As atribuições anteriores do utilizador também serão restauradas (assumindo que as dotações anteriores estão disponíveis).</span><span class="sxs-lookup"><span data-stu-id="602d1-110">The user's previous subscription assignments will also be restored (assuming their previous allocations are available).</span></span>

<span data-ttu-id="602d1-111">Ao comprar novas subscrições para um cliente, o cliente deve dar-lhe uma lista de todos os utilizadores que precisarão de contas, permissões do utilizador e quais os serviços de que cada utilizador necessita.</span><span class="sxs-lookup"><span data-stu-id="602d1-111">When you buy new subscriptions for a customer, the customer should give you a list of all the users who will need accounts, their user permissions, and which services each user needs.</span></span>  

>[!NOTE]
><span data-ttu-id="602d1-112">A secção de **Utilizadores e licenças** do separador **Cliente** mostra todos os utilizadores criados no inquilino de um cliente específico, incluindo utilizadores que tenham licenças compradas a outro parceiro CSP ou a partir de outro canal de compra.</span><span class="sxs-lookup"><span data-stu-id="602d1-112">The **Users and licenses** section of **Customer** tab shows all users created in a specific customer’s tenant, including users that have licenses purchased from another CSP partner or from another purchasing channel.</span></span>

<span data-ttu-id="602d1-113">Pode [atribuir subscrições a vários utilizadores de](bulk-license-provisioning-for-multiple-users.md) uma só vez importando os nomes utilizando um [ficheiro de folha de cálculo compatível com Excel .csv](adding-multiple-users-to-a-customer-account.md).</span><span class="sxs-lookup"><span data-stu-id="602d1-113">You can [assign subscriptions to multiple users](bulk-license-provisioning-for-multiple-users.md) at one time by importing the names using an [Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span>

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a><span data-ttu-id="602d1-114">Criar contas de utilizador para um cliente</span><span class="sxs-lookup"><span data-stu-id="602d1-114">Create user accounts for a customer</span></span>

1. <span data-ttu-id="602d1-115">Inscreva-se no painel do Centro [de Parceiros](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="602d1-115">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="602d1-116">No menu Partner Center, selecione **Clientes,** em seguida, escolha um cliente da lista.</span><span class="sxs-lookup"><span data-stu-id="602d1-116">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="602d1-117">No menu do cliente, selecione **Utilizadores e licenças.**</span><span class="sxs-lookup"><span data-stu-id="602d1-117">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="602d1-118">Para cada utilizador que adicionar, **selecione Adicionar subscrição,** em seguida, preencha as informações, incluindo permissões e licenças.</span><span class="sxs-lookup"><span data-stu-id="602d1-118">For each user you add, select **Add subscription**, then fill out the information, including permissions and licenses.</span></span> <span data-ttu-id="602d1-119">**Guarde** as suas alterações.</span><span class="sxs-lookup"><span data-stu-id="602d1-119">**Save** your changes.</span></span>

5. <span data-ttu-id="602d1-120">Certifique-se de que regista o nome de utilizador e a palavra-passe temporária para enviar ao utilizador.</span><span class="sxs-lookup"><span data-stu-id="602d1-120">Be sure to record the user name and temporary password to send to the user.</span></span>

6. <span data-ttu-id="602d1-121">Se estiver a adicionar vários utilizadores um de cada **vez, utilize outro utilizador**.</span><span class="sxs-lookup"><span data-stu-id="602d1-121">If you are adding multiple users one at a time use **Add another user**.</span></span>

7. <span data-ttu-id="602d1-122">Também pode adicionar vários utilizadores de uma só vez [importando um ficheiro de folha de cálculo compatível com Excel .csv](adding-multiple-users-to-a-customer-account.md).</span><span class="sxs-lookup"><span data-stu-id="602d1-122">You can also add multiple users at once by [importing an Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span> <span data-ttu-id="602d1-123">Pode esperar até terminar com todo o conjunto antes de enviar e-mails ou imprimir os nomes e senhas do ecrã de confirmação.</span><span class="sxs-lookup"><span data-stu-id="602d1-123">You can wait until you're done with the whole set before emailing or printing the names and passwords from the confirmation screen.</span></span>

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a><span data-ttu-id="602d1-124">Adicionar ou remover licenças de utilizador para um cliente</span><span class="sxs-lookup"><span data-stu-id="602d1-124">Add or remove user licenses for a customer</span></span>

<span data-ttu-id="602d1-125">As seguintes medidas aplicam-se à adição ou remoção de licenças de utilizador para produtos Microsoft.</span><span class="sxs-lookup"><span data-stu-id="602d1-125">The following steps apply to adding or removing user licenses for Microsoft products.</span></span> <span data-ttu-id="602d1-126">Para adicionar ou remover licenças de utilizador para subscrições SaaS baseadas em licenças no mercado comercial, consulte [Adicionar ou remover licenças para uma subscrição SaaS](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).</span><span class="sxs-lookup"><span data-stu-id="602d1-126">To add or remove user licenses for license-based SaaS subscriptions in the commercial marketplace, see [Add or remove licenses for a SaaS subscription](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).</span></span>

1. <span data-ttu-id="602d1-127">Inscreva-se no painel do Centro [de Parceiros](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="602d1-127">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="602d1-128">No menu Partner Center, selecione **Clientes,** em seguida, escolha um cliente da lista.</span><span class="sxs-lookup"><span data-stu-id="602d1-128">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="602d1-129">No menu do cliente, selecione **Utilizadores e licenças.**</span><span class="sxs-lookup"><span data-stu-id="602d1-129">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="602d1-130">Escolha um ou mais utilizadores da lista.</span><span class="sxs-lookup"><span data-stu-id="602d1-130">Choose one or more users from the list.</span></span> <span data-ttu-id="602d1-131">Se, por exemplo, o cliente acaba de adquirir novas licenças e quiser atribuí-las a pessoas que ainda não as têm, pode utilizar os utilizadores do **Filtro por...** opção para encontrar o grupo certo.</span><span class="sxs-lookup"><span data-stu-id="602d1-131">If, for example, the customer just purchased new licenses and you wanted to assign them to people who don't have them yet, you can use the **Filter users by...** option to find the right group.</span></span>

5. <span data-ttu-id="602d1-132">Selecione **Licenças de Gestão**.</span><span class="sxs-lookup"><span data-stu-id="602d1-132">Select **Manage licenses**.</span></span> <span data-ttu-id="602d1-133">Faça as alterações e, em seguida, **Guarde**.</span><span class="sxs-lookup"><span data-stu-id="602d1-133">Make your changes, then **Save**.</span></span>

> [!NOTE]
> <span data-ttu-id="602d1-134">Para [os produtos Azure Marketplace,](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer)a atribuição e ativação de licenças é gerida através do Fornecedor Independente de Software (ISV) que publicou o produto.</span><span class="sxs-lookup"><span data-stu-id="602d1-134">For [Azure Marketplace products](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer), license assignment and activation is managed through the Independent Software Vendor (ISV) who published the product.</span></span>

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a><span data-ttu-id="602d1-135">Redefinir a palavra-passe de um utilizador para um cliente</span><span class="sxs-lookup"><span data-stu-id="602d1-135">Reset a user's password for a customer</span></span>

1. <span data-ttu-id="602d1-136">Inicie sessão no [dashboard](https://partner.microsoft.com/dashboard) do Centro de Parceiros.</span><span class="sxs-lookup"><span data-stu-id="602d1-136">Sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="602d1-137">No menu Partner Center, selecione **Clientes,** em seguida, escolha um cliente da lista.</span><span class="sxs-lookup"><span data-stu-id="602d1-137">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="602d1-138">No menu do cliente, selecione **Utilizadores e licenças.**</span><span class="sxs-lookup"><span data-stu-id="602d1-138">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="602d1-139">Escolha o utilizador na lista.</span><span class="sxs-lookup"><span data-stu-id="602d1-139">Choose the user from the list.</span></span>

4. <span data-ttu-id="602d1-140">Na parte inferior do ecrã, **selecione Redefinir a palavra-passe**.</span><span class="sxs-lookup"><span data-stu-id="602d1-140">At the bottom of the screen, select **Reset password**.</span></span> 

5. <span data-ttu-id="602d1-141">Envie a nova senha temporária para o utilizador.</span><span class="sxs-lookup"><span data-stu-id="602d1-141">Send the new temporary password to the user.</span></span>

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a><span data-ttu-id="602d1-142">Eliminar contas de utilizador para um cliente</span><span class="sxs-lookup"><span data-stu-id="602d1-142">Delete user accounts for a customer</span></span>

1. <span data-ttu-id="602d1-143">A partir do menu **Partner Center,** selecione **Clientes.**</span><span class="sxs-lookup"><span data-stu-id="602d1-143">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="602d1-144">Escolha o cliente na lista.</span><span class="sxs-lookup"><span data-stu-id="602d1-144">Choose the customer from the list.</span></span>

2. <span data-ttu-id="602d1-145">No menu do cliente, selecione **Utilizadores e licenças.**</span><span class="sxs-lookup"><span data-stu-id="602d1-145">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="602d1-146">Escolha o utilizador na lista.</span><span class="sxs-lookup"><span data-stu-id="602d1-146">Choose the user from the list.</span></span>

3. <span data-ttu-id="602d1-147">Na parte inferior do ecrã, **selecione Eliminar a conta de utilizador**.</span><span class="sxs-lookup"><span data-stu-id="602d1-147">At the bottom of the screen, select **Delete user account**.</span></span>

<span data-ttu-id="602d1-148">Se precisar de restaurar esta conta, pode encontrá-la no separador **utilizadores eliminados** da lista de **Utilizadores e licenças** do Cliente.</span><span class="sxs-lookup"><span data-stu-id="602d1-148">If you need to restore this account, you can find it in the **Deleted users** tab of the Customer's **Users and licenses** list.</span></span> <span data-ttu-id="602d1-149">Tem 30 dias para restaurar um utilizador apagado.</span><span class="sxs-lookup"><span data-stu-id="602d1-149">You have 30 days to restore a deleted user.</span></span>

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a><span data-ttu-id="602d1-150">Restaurar contas de utilizador eliminadas</span><span class="sxs-lookup"><span data-stu-id="602d1-150">Restore deleted user accounts</span></span>

1. <span data-ttu-id="602d1-151">A partir do menu **Partner Center,** selecione **Clientes,** em seguida, escolha o cliente da lista.</span><span class="sxs-lookup"><span data-stu-id="602d1-151">From the **Partner Center** menu, select **Customers**, then choose the customer from the list.</span></span>

2. <span data-ttu-id="602d1-152">Selecione **Utilizadores e licenças.**</span><span class="sxs-lookup"><span data-stu-id="602d1-152">Select **Users and licenses**.</span></span>

3. <span data-ttu-id="602d1-153">Selecione o separador **utilizadores eliminados ()** Deve ler **(1)** ou mais quando houver utilizadores eliminados que possam ser restaurados.</span><span class="sxs-lookup"><span data-stu-id="602d1-153">Select the **Deleted users ( )** tab. It should read **(1)** or greater when there are deleted users that can be restored.</span></span>

4. <span data-ttu-id="602d1-154">Selecione uma ou mais das caixas de verificação dos utilizadores eliminados e, em seguida, selecione **Restaurar**.</span><span class="sxs-lookup"><span data-stu-id="602d1-154">Select one or more of the deleted users' checkboxes and then select **Restore**.</span></span>

    <span data-ttu-id="602d1-155">Todas as contas de utilizador selecionadas reaparecerão na página **Utilizadores e licenças.**</span><span class="sxs-lookup"><span data-stu-id="602d1-155">All selected user accounts will reappear in the **Users and licenses** page.</span></span>

## <a name="next-steps"></a><span data-ttu-id="602d1-156">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="602d1-156">Next steps</span></span>

- [<span data-ttu-id="602d1-157">Assign or revoke licenses to multiple users (Atribuir ou revogar licenças para vários utilizadores)</span><span class="sxs-lookup"><span data-stu-id="602d1-157">Assign or revoke licenses to multiple users</span></span>](bulk-license-provisioning-for-multiple-users.md)

- [<span data-ttu-id="602d1-158">Criar vários utilizadores para uma conta de cliente</span><span class="sxs-lookup"><span data-stu-id="602d1-158">Create multiple users for a customer account</span></span>](adding-multiple-users-to-a-customer-account.md)