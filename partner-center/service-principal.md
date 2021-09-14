---
title: Diretor de serviço AZure AD
ms.topic: how-to
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-enroll
description: Descubra como adicionar um diretor de serviço ao seu inquilino AZure AD. Fazê-lo significa adicionar uma aplicação AD Azure (principal serviço) no Partner Center.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: a7851d270ad51a5a06ebc7d7725a2ae5c803419b
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/13/2021
ms.locfileid: "126247109"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a>Adicione uma aplicação AD AZure (principal serviço) no Partner Center

**Funções apropriadas**: Administração global

No programa Mercado Comercial no Partner Center, pode agora adicionar uma aplicação de Microsoft Azure Ative Directory (Azure AD) (principal serviço) como utilizador na sua conta Partner Center. (Conseguiu fazê-lo anteriormente na sua conta Cloud Partner Portal (CPP). Agora que emigrou para o Partner Center, a conta do CPP é apenas de leitura.)
 
>[!Note] 
>O diretor de serviço é sinónimo de aplicação Azure AD.

## <a name="add-an-azure-ad-application-service-principal"></a>Adicione uma aplicação AD AZure (principal serviço)

1. A partir do painel Partner Center, selecione **Definições** e, em seguida, selecione **as definições de Desenvolvedor**.

2. Selecione **Utilizadores** e, em seguida, **selecione Adicionar Aplicações AD Azure**.

3. Selecione uma aplicação AD Azure existente ou crie uma nova.

4. Se criar uma nova aplicação AD Azure, inclua as seguintes informações:  

   - **URL de resposta**: O URL onde os utilizadores podem iniciar sação para utilizar a sua aplicação AD Azure.

   - **App ID URI**: Um identificador lógico para a aplicação Azure AD que é apresentado quando envia um único pedido de inscrição para Azure AD.

   - **Funções de segurança**: O **Gestor** de Funções (o mesmo que o papel de 'Proprietário' no CPP) e o **Desenvolvedor** (o mesmo papel de 'Contribuinte' no CPP) aplicam-se ao programa de Marketplace Comercial no Partner Center, podendo ser associados a esta Aplicação AD Azure.  

## <a name="next-steps"></a>Passos seguintes

- [Visão geral do mercado comercial no Partner Center](csp-commercial-marketplace-overview.md)