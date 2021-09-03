---
title: Gerir ofertas de produtos de mercado &
ms.topic: how-to
ms.date: 07/02/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Utilizando o Partner Center, saiba como os Fornecedores de Soluções Cloud podem gerir ofertas ISV de terceiros compradas para clientes do mercado comercial.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 14901b47b7363b2d87861be43a7071d9f23545cc
ms.sourcegitcommit: 09d2c10491244775e656b48fce35b5648262ce59
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/03/2021
ms.locfileid: "123457927"
---
# <a name="manage-commercial-marketplace-products-and-offers-for-your-customers"></a>Gerir produtos e ofertas de marketplace comercial para os seus clientes


**Funções adequadas**: Administração global | Agente administrativo

Os parceiros do programa Fornecedor de Soluções em Nuvem (CSP) podem usar o portal Partner Center para comprar muitas ofertas ou subscrições isv SaaS para os seus clientes no mercado comercial. Uma vez que você compra uma oferta, você tem várias maneiras de geri-la.

## <a name="view-or-edit-a-subscription"></a>Ver ou editar uma subscrição

Depois de adquirir uma subscrição de um editor ISV de terceiros, pode revê-la ou editá-la da seguinte forma:

1. Inscreva-se no painel partner [center](https://partner.microsoft.com/dashboard)e, em seguida, selecione **Clientes** do menu de navegação à esquerda.

2. Selecione um cliente apropriado e, em seguida, **selecione Subscrições**. Isto lista quaisquer subscrições baseadas em licença que tenha comprado para o cliente.

3. Na coluna **Subscrição,** selecione a subscrição que pretende visualizar ou editar. Isto dá-lhe mais informações para configurar ou providenciar a oferta. (Se for necessária mais ação sobre a oferta, poderá também ver um estado de "Ação Necessária" apresentado na coluna Status. Isto também pode ser acompanhado por um link para o site da editora ISV.)

4. Uma vez selecionada a subscrição que pretende visualizar ou editar, a página de detalhes da subscrição permite-lhe editar a subscrição e fazer coisas como:

    - Alterar o apelido de subscrição

    - Adicionar/diminuir o número de licenças na subscrição

    - Cancelar a subscrição

    - Desativar renovação automática

    - Adicione um ID de revendedor indireto, se aplicável

> [!NOTE]
> Poderá ter de completar determinados passos definidos pela editora ISV antes de poder efetuar algumas alterações numa subscrição, tais como cancelar uma subscrição.

## <a name="assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer"></a>Atribuir licenças e ativar uma subscrição em nome de um cliente

Ao adquirir uma oferta de Software como Serviço (SaaS) fornecida por um editor independente de Fornecedor de Software (ISV) no mercado comercial, o editor da ISV ajuda a gerir o processo de atribuição de licenças e ativar a subscrição em nome do seu cliente.

O editor deve fornecer-lhe um link personalizado e um código de autorização que identifique a sua compra específica.

1. Pode encontrar este link personalizado da editora ISV de algumas formas:

   - Pode ver o link da página de confirmação que aparece depois de adquirir uma oferta ISV SaaS. Para encontrar este link na página, procure e selecione **Vá ao site da editora.**

   - Pode ver o link na página de Subscrições específica do cliente. Este link de editor aparece na linha associada à oferta ISV ou subscrição adquirida para o cliente.

   - Pode [recuperar o link utilizando APIs do Partner Center](/partner-center/develop/get-activation-link-by-order-line-item).

   > [!NOTE]
   > Para isso em nome do seu cliente, poderá necessitar de copiar o link personalizado, colar-o num browser privado e inserir as credenciais do cliente.

2. Assim que estiver no site ou sistema do editor ISV, o editor informá-lo-á de quaisquer medidas adicionais que necessite de tomar para completar o processo de configuração do cliente e a prestação ou atribuir licenças.

3. Como parceiro no programa CSP que está a trabalhar em nome do seu cliente, é responsável por executar as seguintes tarefas:

    - Envie todas as informações necessárias ao editor.

    - Envie qualquer URL necessário diretamente para o seu cliente (ou de outra forma comunicar diretamente detalhes sobre esta subscrição ao seu cliente)

4. Assim que fornecer as informações necessárias ao editor, o editor fornecerá e atribuirá licenças apropriadas. A faturação da subscrição só começará depois dos seguintes eventos ocorrerem:

    - A editora ISV atribuiu com sucesso licenças apropriadas

    - A editora ISV confirmou à Microsoft (através de uma API de cumprimento separada, SaaS) que a configuração da conta foi concluída com sucesso

## <a name="cancel-a-license-based-saas-subscription-from-an-isv-publisher"></a>Cancelar uma assinatura SaaS baseada em licença de um editor isv

Quando subscreve um produto SaaS baseado em licença oferecido por um editor ISV dentro do mercado comercial, tem a opção de cancelar a subscrição dentro do período de cancelamento designado. Este período de cancelamento muda dependendo se tem uma subscrição mensal ou anual. Também pode escolher se renova automaticamente a subscrição.

Para obter mais informações sobre os períodos de cancelamento que se aplicam, como cancelar ou como renovar automaticamente uma subscrição, consulte [Cancelar uma subscrição](create-a-new-subscription.md#cancel-a-subscription).

## <a name="add-or-remove-licenses-for-a-saas-subscription"></a>Adicionar ou remover licenças para uma subscrição do SaaS

Para ofertas de mercado comercial SaaS, pode adicionar ou remover licenças de utilizador para uma subscrição do cliente.

1. Inscreva-se no painel partner [center](https://partner.microsoft.com/dashboard)e, em seguida, selecione **Clientes** do menu de navegação à esquerda.

2. Selecione um cliente apropriado e, em seguida, **selecione Subscrições**. Isto lista quaisquer subscrições baseadas em licença que tenha comprado para o cliente.

3. Na coluna **Subscrição,** selecione a subscrição que pretende modificar.

4. Na página de detalhes da subscrição, localize o campo **Quantidade.** É aqui que pode aumentar ou diminuir o número de licenças.

5. Alterar a quantidade e, em seguida, selecionar **Enviar por isso .**

## <a name="manage-subscriptions-using-partner-center-apis"></a>Gerir subscrições usando APIs do Partner Center

Também pode utilizar APIs do Partner Center para realizar a gestão do ciclo de vida e gerir faturas para as suas subscrições. Para obter mais informações, consulte [Criar uma subscrição para produtos de mercado comercial.](/partner-center/develop/create-subscription-azure-marketplace-products)

## <a name="next-steps"></a>Passos seguintes

- [Comprar ofertas de mercado comercial](csp-commercial-marketplace-purchase.md)
- [Conheça a faturação no mercado comercial](csp-commercial-marketplace-billing.md)
