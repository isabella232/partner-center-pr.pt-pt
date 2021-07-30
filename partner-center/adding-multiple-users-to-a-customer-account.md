---
title: Adicionar vários utilizadores para uma conta de cliente
ms.topic: how-to
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: Para adicionar vários utilizadores à conta de um cliente, faça o upload de um ficheiro de dados para o Partner Center utilizando o formato de ficheiro separado em vírgula (.csv).
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 907d1267164df267acab08675b4b9388fbf14474
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/29/2021
ms.locfileid: "114839435"
---
# <a name="upload-a-csv-file-of-users-to-a-customers-account"></a>Faça o upload de um ficheiro .csv de utilizadores para a conta de um cliente


**Funções apropriadas**: Administração global

Adicione vários utilizadores à conta de um cliente de uma só vez, enviando um ficheiro de dados no formato de ficheiro de valor separado em vírgula (.csv) para o Centro de Parceiros. 

## <a name="create-the-file-of-customer-users-and-upload-to-customer-account"></a>Crie o ficheiro dos utilizadores do cliente e faça upload para a conta do cliente

1. Crie um ficheiro de dados de valor separado (.csv) com os dados acima descritos. Guarde o ficheiro para que possa navegar para ele num passo posterior. Consulte [o ficheiro Fields for .csv para importar vários utilizadores para uma conta de cliente.](file-customer-users.md) 

2. Inscreva-se no painel do Centro [de Parceiros](https://partner.microsoft.com/dashboard).

3. No menu Partner Center, selecione **Clientes,** em seguida, escolha um cliente da lista.

4. Selecione o separador **Utilizadores e Licenças** do cliente e, em seguida, selecione **utilizadores upload**.

5. Informação **do utilizador do Upload**, selecione **Procurar**.

6. No seletor de ficheiros, selecione o seu ficheiro de dados e, em seguida, selecione **Abrir**.

7. Selecione **Validar**.

    **Nota**  A maioria dos erros de criação de conta são causados por problemas de ficheiros de dados, incluindo falta de informação, endereços de e-mail mal formados ou duplicados, ou demasiados registos no ficheiro.

8. Depois de o Centro de Parceiros validar o ficheiro, selecione a **Localização** Geográfica para os novos utilizadores.
9. Selecione **Guardar**.
10. Faça o download da informação de senha temporária para os utilizadores.

    >[!IMPORTANT]
    > Certifique-se de baixar o ficheiro com as senhas temporárias agora, uma vez que não poderá fazê-lo mais tarde. Os novos utilizadores devem aceder à sua nova conta utilizando a senha temporária para as suas novas contas.

11. Os novos utilizadores são automaticamente atribuídos permissões de **Can use licenças e serviços**. 

## <a name="next-steps"></a>Passos seguintes

- [Dê permissão aos clientes no Partner Center para comprarem os seus próprios produtos ou serviços](give-customers-permission.md)
