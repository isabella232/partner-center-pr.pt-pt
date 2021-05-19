---
title: Configurar os seus utilizadores com a autenticação multifator
ms.topic: how-to
ms.date: 12/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Saiba como configurar os seus colaboradores com a MFA
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 5173526d0f65623311d5cd3a1061e8b9e93e9bb9
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151632"
---
# <a name="set-up-your-users-with-multi-factor-authentication"></a>Configurar os seus utilizadores com a autenticação multifator

**Funções apropriadas**: Administração global

Uma maior salvaguarda de privacidade e segurança estão entre as nossas principais prioridades. Sabemos que a melhor defesa é a prevenção e que somos tão fortes quanto o nosso elo mais fraco. É por isso que precisamos que todos os nossos ecossistemas atuem e garantam a proteção de segurança adequadas. Recomendamos vivamente que todos os parceiros permitam a autenticação de vários fatores (MFA) para os seus utilizadores no seu inquilino parceiro. 

## <a name="add-multi-factor-authentication-for-your-users"></a>Adicionar autenticação multi-factor para os seus utilizadores

Deve ser o administrador global da sua empresa para completar esta tarefa.

É mais fácil ativar o MFA para os seus utilizadores à medida que os adiciona ao seu inquilino AZure AD.

1. Inscreva-se no [portal Azure](https://portal.azure.com) e, em seguida, vá para a **gestão do Utilizador**.
1. Selecione **a autenticação de vários fatores.**
1. Selecione o utilizador que pretende ativar e, em seguida, selecione **Ative**.

Isto permitirá o MFA para este utilizador. Ativado significa que o utilizador será solicitado a configurar a sua verificação de MFA quando iniciar o seu seru. Posteriormente, ao iniciar o sôm, será-lhes solicitado que lhes forneçam um código que lhes seja enviado através de e-mail ou mensagem de texto (dependendo do que configurarem).  

:::image type="content" source="images/MFA/securityverification.png" alt-text="Especificar como verificar":::

>[!NOTE]
>Pode **impor aos** seus utilizadores a utilização de MFA utilizando os mesmos passos acima e selecionando **Enforce**. Para saber mais, leia [Ativar a autenticação multi-factor Azure por utilizador para garantir eventos de entrada.](/azure/active-directory/authentication/howto-mfa-userstates) 

Todos os utilizadores começam **desativados.** Quando inscreve os utilizadores na autenticação multi-factor do Diretório Ativo Azure por utilizador, o estado muda para **Enabled**. Quando os utilizadores ativados iniciaram o seu registo e completam o processo de registo, as alterações de estado para **Aplicadas**. 

## <a name="next-steps"></a>Passos seguintes

- [Atribuir funções e permissões a utilizadores](permissions-overview.md)