---
title: Gerir utilizadores para contas de clientes
ms.topic: how-to
ms.date: 09/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: Gerir os utilizadores para os seus clientes no Partner Center - criar contas de utilizador, adicionar ou remover licenças de utilizador, redefinir palavras-passe e eliminar ou restaurar as contas de utilizador.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: eb4163a2db470bec7c09c4a800f01becce4e21d3
ms.sourcegitcommit: e1da62b36420d78bf44e3962358d0af65ebc3402
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/27/2021
ms.locfileid: "129088896"
---
# <a name="manage-users-and-user-licenses-for-customer-accounts"></a>Gerir utilizadores e licenças de utilizador para contas de clientes 

**Funções adequadas**: Administração global | Administração de administração de utilizadores | Agente administrativo

Pode criar e eliminar novos utilizadores na conta de um cliente. Também pode restaurar uma ou mais contas de utilizador que apagou anteriormente no prazo de 30 dias após a eliminação. As atribuições anteriores do utilizador também serão restauradas (assumindo que as dotações anteriores estão disponíveis).

Ao comprar novas subscrições para um cliente, o cliente deve dar-lhe uma lista de todos os utilizadores que precisarão de contas, permissões de utilizador e quais os serviços de que cada utilizador necessita.

> [!NOTE]
> A secção de **Utilizadores e licenças** do separador **Cliente** mostra todos os utilizadores criados no inquilino específico de um cliente, incluindo utilizadores que tenham licenças compradas a outro parceiro CSP ou a partir de outro canal de compra.

Pode [atribuir subscrições a vários utilizadores de](bulk-license-provisioning-for-multiple-users.md) uma só vez importando os nomes utilizando um [ficheiro de .csv compatível com Excel](adding-multiple-users-to-a-customer-account.md).

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a>Criar contas de utilizador para um cliente

> [!NOTE]
> Para saber mais sobre a interface de espaços de trabalho, consulte [o Centro de Parceiros.](get-around-partner-center.md#turn-workspaces-on-and-off)

#### <a name="workspaces-view"></a>[Vista de espaços de trabalho](#tab/workspaces-view)

1. A partir do [painel Partner Center](https://partner.microsoft.com/dashboard), selecione o azulejo **cliente** e, em seguida, selecione o cliente da lista de Clientes.

2. No menu do cliente, selecione **Utilizadores e licenças.**

3. Para cada utilizador que adicionar, **selecione Adicionar subscrição,** em seguida, preencha as informações, incluindo permissões e licenças. **Guarde** as suas alterações.

4. Certifique-se de que regista o nome de utilizador e a palavra-passe temporária para enviar ao utilizador.

5. Se estiver a adicionar vários utilizadores um de cada **vez, adicione outro utilizador**.

6. Também pode adicionar vários utilizadores de uma só vez [importando um ficheiro de folha de cálculo .csv compatível com Excel.](adding-multiple-users-to-a-customer-account.md) Pode esperar até terminar com todo o conjunto antes de enviar e-mails ou imprimir os nomes e senhas do ecrã de confirmação.

#### <a name="current-view"></a>[Vista atual](#tab/current-view)

1. A partir do [painel de instrumentos Partner Center](https://partner.microsoft.com/dashboard), selecione **Clientes,** em seguida, selecione o cliente da lista de Clientes.

2. No menu do cliente, selecione **Utilizadores e licenças.**

3. Para cada utilizador que adicionar, **selecione Adicionar subscrição,** em seguida, preencha as informações, incluindo permissões e licenças. **Guarde** as suas alterações.

4. Certifique-se de que regista o nome de utilizador e a palavra-passe temporária para enviar ao utilizador.

5. Se estiver a adicionar vários utilizadores um de cada **vez, adicione outro utilizador**.

6. Também pode adicionar vários utilizadores de uma só vez [importando um ficheiro de folha de cálculo .csv compatível com Excel.](adding-multiple-users-to-a-customer-account.md) Pode esperar até terminar com todo o conjunto antes de enviar e-mails ou imprimir os nomes e senhas do ecrã de confirmação.

* * *

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a>Adicionar ou remover licenças de utilizador de um cliente

As seguintes medidas aplicam-se à adição ou remoção de licenças de utilizador para produtos Microsoft. Para adicionar ou remover licenças de utilizador para subscrições SaaS baseadas em licenças no mercado comercial, consulte [Adicionar ou remover licenças para uma subscrição SaaS](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).

> [!NOTE]
> Para saber mais sobre a interface de espaços de trabalho, consulte [o Centro de Parceiros.](get-around-partner-center.md#turn-workspaces-on-and-off)

#### <a name="workspaces-view"></a>[Vista de espaços de trabalho](#tab/workspaces-view)

1. A partir do [painel Partner Center](https://partner.microsoft.com/dashboard), selecione o azulejo **cliente** e, em seguida, selecione o cliente da lista de Clientes.

2. No menu do cliente, selecione **Utilizadores e licenças.**

3. Escolha um ou mais utilizadores na lista. Se, por exemplo, o cliente acaba de adquirir novas licenças e quiser atribuí-las a pessoas que ainda não as têm, pode utilizar os utilizadores do **Filtro por...** opção de encontrar o grupo certo.

4. Selecione **Gerir licenças**. Faça as alterações e, em seguida, **Guarde**.

> [!NOTE]
> Para [os produtos Azure Marketplace,](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer)a atribuição e ativação de licenças é gerida através do Fornecedor Independente de Software (ISV) que publicou o produto.

#### <a name="current-view"></a>[Vista atual](#tab/current-view)

1. A partir do [painel de instrumentos Partner Center](https://partner.microsoft.com/dashboard), selecione **Clientes,** em seguida, selecione o cliente da lista de Clientes.

2. No menu do cliente, selecione **Utilizadores e licenças.**

3. Escolha um ou mais utilizadores na lista. Se, por exemplo, o cliente acaba de adquirir novas licenças e quiser atribuí-las a pessoas que ainda não as têm, pode utilizar os utilizadores do **Filtro por...** opção de encontrar o grupo certo.

4. Selecione **Gerir licenças**. Faça as alterações e, em seguida, **Guarde**.

> [!NOTE]
> Para [os produtos Azure Marketplace,](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer)a atribuição e ativação de licenças é gerida através do Fornecedor Independente de Software (ISV) que publicou o produto.

* * *

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a>Redefinir a palavra-passe de um utilizador para um cliente

> [!NOTE]
> Para saber mais sobre a interface de espaços de trabalho, consulte [o Centro de Parceiros.](get-around-partner-center.md#turn-workspaces-on-and-off)

#### <a name="workspaces-view"></a>[Vista de espaços de trabalho](#tab/workspaces-view)

1. Faça o [sômis](https://partner.microsoft.com/dashboard)no painel Partner Center, selecione o azulejo **do Cliente** e, em seguida, selecione o cliente da lista de Clientes.

2. No menu do cliente, selecione **Utilizadores e licenças.** Escolha o utilizador na lista.

3. Na parte inferior do ecrã, **selecione Redefinir a palavra-passe**.

4. Envie a nova senha temporária para o utilizador.

#### <a name="current-view"></a>[Vista atual](#tab/current-view)

1. Inscreva-se no [painel de instrumentos do Centro de Parceiros,](https://partner.microsoft.com/dashboard)selecione **Clientes** e, em seguida, selecione o cliente da lista de Clientes.

2. No menu do cliente, selecione **Utilizadores e licenças.** Escolha o utilizador na lista.

3. Na parte inferior do ecrã, **selecione Redefinir a palavra-passe**.

4. Envie a nova senha temporária para o utilizador.

* * *

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a>Eliminar contas de utilizador para um cliente

> [!NOTE]
> Para saber mais sobre a interface de espaços de trabalho, consulte [o Centro de Parceiros.](get-around-partner-center.md#turn-workspaces-on-and-off)

#### <a name="workspaces-view"></a>[Vista de espaços de trabalho](#tab/workspaces-view)

1. A partir do [painel Partner Center](https://partner.microsoft.com/dashboard), selecione o azulejo **cliente** e, em seguida, selecione o cliente da lista de Clientes.

2. No menu do cliente, selecione **Utilizadores e licenças.** Escolha o utilizador na lista.

3. Na parte inferior do ecrã, **selecione Eliminar a conta de utilizador**.

Se precisar de restaurar esta conta, pode encontrá-la no separador **utilizadores eliminados** da lista de **Utilizadores e licenças** do Cliente. Tem 30 dias para restaurar um utilizador apagado.

#### <a name="current-view"></a>[Vista atual](#tab/current-view)

1. A partir do [painel de instrumentos Partner Center](https://partner.microsoft.com/dashboard), selecione **Clientes,** em seguida, selecione o cliente da lista de Clientes.

2. No menu do cliente, selecione **Utilizadores e licenças.** Escolha o utilizador na lista.

3. Na parte inferior do ecrã, **selecione Eliminar a conta de utilizador**.

Se precisar de restaurar esta conta, pode encontrá-la no separador **utilizadores eliminados** da lista de **Utilizadores e licenças** do Cliente. Tem 30 dias para restaurar um utilizador apagado.

* * *

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a>Restaurar contas de utilizador eliminadas

> [!NOTE]
> Para saber mais sobre a interface de espaços de trabalho, consulte [o Centro de Parceiros.](get-around-partner-center.md#turn-workspaces-on-and-off)

#### <a name="workspaces-view"></a>[Vista de espaços de trabalho](#tab/workspaces-view)

1. A partir do [painel Partner Center](https://partner.microsoft.com/dashboard), selecione o azulejo **cliente** e, em seguida, selecione o cliente da lista de Clientes.

2. Selecione **Utilizadores e licenças**.

3. Selecione o separador **utilizadores eliminados ()** Deve ler **(1)** ou mais quando houver utilizadores eliminados que possam ser restaurados.

4. Selecione uma ou mais das caixas de verificação dos utilizadores eliminados e, em seguida, selecione **Restaurar**.

    Todas as contas de utilizador selecionadas reaparecerão na página **Utilizadores e licenças.**

#### <a name="current-view"></a>[Vista atual](#tab/current-view)

1. A partir do [painel de instrumentos Partner Center](https://partner.microsoft.com/dashboard), selecione **Clientes,** em seguida, selecione o cliente da lista de Clientes.

2. Selecione **Utilizadores e licenças**.

3. Selecione o separador **utilizadores eliminados ()** Deve ler **(1)** ou mais quando houver utilizadores eliminados que possam ser restaurados.

4. Selecione uma ou mais das caixas de verificação dos utilizadores eliminados e, em seguida, selecione **Restaurar**.

    Todas as contas de utilizador selecionadas reaparecerão na página **Utilizadores e licenças.**

* * *

## <a name="next-steps"></a>Passos seguintes

- [Assign or revoke licenses to multiple users (Atribuir ou revogar licenças para vários utilizadores)](bulk-license-provisioning-for-multiple-users.md)

- [Criar vários utilizadores para uma conta de cliente](adding-multiple-users-to-a-customer-account.md)