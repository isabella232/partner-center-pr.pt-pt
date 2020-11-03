---
title: Gerir utilizadores e licenças de utilizador para contas de clientes
ms.topic: how-to
ms.date: 05/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como gerir os utilizadores para os seus clientes no Partner Center, como criar contas de utilizador, adicionar ou remover licenças de utilizador, redefinir as palavras-passe do utilizador e eliminar ou restaurar as contas do utilizador.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: fc208283e0ed8c0f164a44cc9bd70260b8671c6e
ms.sourcegitcommit: 22af0997d52a87417b62f44fb0a7d711bec77b35
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/19/2020
ms.locfileid: "92530629"
---
# <a name="manage-users-and-user-licenses-for-customer-accounts"></a>Gerir utilizadores e licenças de utilizador para contas de clientes

**Aplica-se a**

- Partner Center

**Funções adequadas**

- Administrador global
- Administração de gestão de utilizadores
- Agente administrativo
- Agente comercial
- Agente helpdesk

Pode criar e eliminar novos utilizadores na conta de um cliente. Também pode restaurar uma ou mais contas de utilizador que apagou anteriormente no prazo de 30 dias após a eliminação. As atribuições anteriores do utilizador também serão restauradas (assumindo que as dotações anteriores estão disponíveis).

Ao comprar novas subscrições para um cliente, o cliente deve dar-lhe uma lista de todos os utilizadores que precisarão de contas, permissões do utilizador e quais os serviços de que cada utilizador necessita.  

Pode [atribuir subscrições a vários utilizadores de](bulk-license-provisioning-for-multiple-users.md) uma só vez importando os nomes utilizando um [ficheiro de folha de cálculo .csv compatível com o Excel.](adding-multiple-users-to-a-customer-account.md)

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a>Criar contas de utilizador para um cliente

1. Inscreva-se no painel do Centro [de Parceiros](https://partner.microsoft.com/dashboard).

2. No menu Partner Center, selecione **Clientes,** em seguida, escolha um cliente da lista.

3. No menu do cliente, selecione **Utilizadores e licenças.**

4. Para cada utilizador que adicionar, **selecione Adicionar subscrição,** em seguida, preencha as informações, incluindo permissões e licenças. **Guarde** as suas alterações.

5. Certifique-se de que regista o nome de utilizador e a palavra-passe temporária para enviar ao utilizador.

6. Se estiver a adicionar vários utilizadores um de cada **vez, utilize outro utilizador** .

7. Também pode adicionar vários utilizadores de uma só vez [importando um ficheiro de folha de cálculo .csv compatível com Excel.](adding-multiple-users-to-a-customer-account.md) Pode esperar até terminar com todo o conjunto antes de enviar e-mails ou imprimir os nomes e senhas do ecrã de confirmação.

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a>Adicionar ou remover licenças de utilizador para um cliente

As seguintes medidas aplicam-se à adição ou remoção de licenças de utilizador para produtos Microsoft. Para adicionar ou remover licenças de utilizador para subscrições SaaS baseadas em licenças no mercado comercial, consulte [Adicionar ou remover licenças para uma subscrição SaaS](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).

1. Inscreva-se no painel do Centro [de Parceiros](https://partner.microsoft.com/dashboard).

2. No menu Partner Center, selecione **Clientes,** em seguida, escolha um cliente da lista.

3. No menu do cliente, selecione **Utilizadores e licenças.**

4. Escolha um ou mais utilizadores da lista. Se, por exemplo, o cliente acaba de adquirir novas licenças e quiser atribuí-las a pessoas que ainda não as têm, pode utilizar os utilizadores do **Filtro por...** opção para encontrar o grupo certo.

5. Selecione **Licenças de Gestão** . Faça as alterações e, em seguida, **Guarde** .

> [!NOTE]
> Para [os produtos Azure Marketplace,](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer)a atribuição e ativação de licenças é gerida através do Fornecedor Independente de Software (ISV) que publicou o produto.

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a>Redefinir a palavra-passe de um utilizador para um cliente

1. Inscreva-se no painel do Centro [de Parceiros](https://partner.microsoft.com/dashboard).

2. No menu Partner Center, selecione **Clientes,** em seguida, escolha um cliente da lista.

3.  No menu do cliente, selecione **Utilizadores e licenças.** Escolha o utilizador na lista.

4.  Na parte inferior do ecrã, **selecione Redefinir a palavra-passe** . 

5.  Envie a nova senha temporária para o utilizador.

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a>Eliminar contas de utilizador para um cliente

1.  A partir do menu **Partner Center,** selecione **Clientes.** Escolha o cliente na lista.

2.  No menu do cliente, selecione **Utilizadores e licenças.** Escolha o utilizador na lista.

3.  Na parte inferior do ecrã, **selecione Eliminar a conta de utilizador** .

Se precisar de restaurar esta conta, pode encontrá-la no separador **utilizadores eliminados** da lista de **Utilizadores e licenças** do Cliente. Tem 30 dias para restaurar um utilizador apagado.

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a>Restaurar contas de utilizador eliminadas

1.  A partir do menu **Partner Center,** selecione **Clientes,** em seguida, escolha o cliente da lista.

2.  Selecione **Utilizadores e licenças.**

3.  Selecione o separador **utilizadores eliminados ()** Deve ler **(1)** ou mais quando houver utilizadores eliminados que possam ser restaurados.

4.  Selecione uma ou mais das caixas de verificação dos utilizadores eliminados e, em seguida, selecione **Restaurar** .

    Todas as contas de utilizador selecionadas reaparecerão na página **Utilizadores e licenças.**

## <a name="related-topics"></a>Tópicos relacionados


[Assign or revoke licenses to multiple users](bulk-license-provisioning-for-multiple-users.md) (Atribuir ou revogar licenças para vários utilizadores)

[Criar vários utilizadores para uma conta de cliente](adding-multiple-users-to-a-customer-account.md)