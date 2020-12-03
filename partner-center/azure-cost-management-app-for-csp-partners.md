---
title: Gestão de Custos do Azure para CSPs
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como registar a aplicação web Cloudyn e use uma chave secreta para ela no Partner Center para que possa usar a app para rastrear o uso e os custos do cliente Azure.
author: aparnagkrishnan
ms.author: aparnag
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: defa691a3bc70cbda45f01cb447d89364a49e3b8
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534998"
---
# <a name="track-customer-azure-usage-and-costs-with-the-azure-cost-management-app-for-csp-partners"></a>Acompanhe o uso do cliente Azure e os custos com a app de gestão de custos Azure para parceiros CSP  

**Funções adequadas**

- Administrador global
- Agente administrativo

[Obtenha mais informações sobre a Azure Cost Management](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a>Before you begin
Antes de poder utilizar a Azure Cost Management, certifique-se de que cumpre os seguintes requisitos:

- É um parceiro no programa Cloud Solution Provider.
- Você tem a capacidade de criar uma aplicação web Partner Center API.

## <a name="overview"></a>Descrição geral

A Cloudyn é uma aplicação web que permite rastrear e gerir o quanto os seus clientes estão a usar o Azure e os custos dessa utilização. Usa-o através da API do Centro Parceiro.

## <a name="register-your-web-app-in-the-partner-center"></a>Registe a sua aplicação web no Centro de Parceiros
Quando regista uma aplicação web Azure Ative Directory no Partner Center, permite o acesso à API do Partner Center. 
1.  Inscreva-se no [Partner Center](https://partnercenter.microsoft.com/pcv/dashboard/overview) utilizando [uma conta global de administrador ou agente administrativo.](create-user-accounts-and-set-permissions.md)
2.  A partir do **Partner Center**, selecione Gestão de **aplicações de contas.** &gt; **[App management](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)**
3.  Na secção **Aplicação Web,** clique em **Adicionar nova aplicação web.**
<br> **Nota:** Se já criou uma aplicação web, pode saltar o passo 3.
4.  Copie e guarde o **Commerce ID** GUID e o **App ID** GUID para a sua aplicação web. Você precisará de ambos os IDs para usar o teste gratuito de 30 dias da app de gestão de custos Azure.

## <a name="add-a-secret-key-to-your-app"></a>Adicione uma chave secreta à sua aplicação
1. Na descida ao lado do botão **Adicionar,** selecione uma duração de 1 ou 2 anos.
2. Clique **na tecla Adicionar**. 
3. Copie e guarde o valor da chave secreta. Vai precisar disto para o julgamento gratuito de 30 dias.<br>
   > [!NOTE]  
   > As chaves secretas da aplicação são como senhas com datas de validade mais longas. Guarde o valor da chave num local seguro para utilização futura.

## <a name="next-steps"></a>Passos seguintes
Inicie um [julgamento gratuito de 30 dias.](https://go.microsoft.com/fwlink/?linkid=857895)
Precisa dos seguintes detalhes para iniciar o julgamento:
- Signo do Centro parceiro em credenciais
- Commerce ID GUID
- App ID GUID
- Valor chave segredo da aplicação
