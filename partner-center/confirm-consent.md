---
title: Confirme a aceitação do cliente do Microsoft Customer Agreement
description: Saiba como confirmar a aceitação do cliente do Acordo de Cliente da Microsoft. Isto pode ser necessário para encomendar produtos e serviços da Microsoft para os clientes.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 06/30/2020
ms.openlocfilehash: aacca72e9af45b2777364734c2b07dbe8101989d
ms.sourcegitcommit: 22af0997d52a87417b62f44fb0a7d711bec77b35
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/19/2020
ms.locfileid: "92530656"
---
# <a name="updated-method-to-confirm-customer-acceptance-of-the-microsoft-customer-agreement"></a>Método atualizado para confirmar a aceitação do cliente do Acordo de Cliente da Microsoft

**Aplica-se a**

-  Partner Center

**Funções adequadas**

- Agente administrativo
- Agente comercial

> [!NOTE]
> O recurso Do Acordo é atualmente suportado pelo Partner Center apenas na nuvem pública da Microsoft. Não é aplicável a:
> * Centro de Parceiros operado pela 21Vianet
> * Centro de Parceiros para Microsoft Cloud Germany
> * Centro de Parceiros para Microsoft Cloud para governo dos EUA

>[!NOTE]
>A partir de 31 de janeiro de 2020, todos os clientes, existentes e novos, devem assinar o novo Acordo de Clientes da Microsoft. Para saber mais, leia [Confirme a aceitação do cliente do Acordo de Cliente da Microsoft.](confirm-customer-agreement.md)

Como parceiro, precisa de obter a aceitação do Acordo de Cliente da Microsoft antes de poder encomendar produtos e serviços da Microsoft para esse cliente. Para melhor ajudar os parceiros a cumprir os requisitos de conformidade, a Microsoft pede aos parceiros que confirmem a aceitação, fornecendo os seguintes detalhes sobre a pessoa que aceitou o acordo:

- Nome próprio

- Apelido

- Endereço de e-mail

- Número de telefone (opcional)

- Data de aceitação

Os parceiros de conta direta e os Fornecedores Indiretos devem confirmar a aceitação do Cliente do Microsoft Customer Agreement ao transagir através do Partner Center ou da Partner Center API. A confirmação é *obrigatória.*

Se não for fornecida confirmação para um determinado cliente:

- Não poderá criar novas encomendas para este cliente.

- Não poderá alterar a contagem de licenças das assinaturas existentes baseadas em licenças para este cliente.

A confirmação da aceitação do cliente pode ser feita através do Partner Center ou da API do Partner Center. Para isso através da API do Centro De Parceiros, consulte os seguintes tópicos:

- [Obtenha a confirmação do consentimento do cliente](/partner-center/develop/get-confirmation-of-customer-consent)

- [Obtenha metadados de acordo](/partner-center/develop/get-agreement-metadata)

- [Confirme o consentimento do cliente](/partner-center/develop/confirm-customer-consent)

Isto aplica-se tanto aos ambientes de produção como de caixas de areia.

## <a name="confirm-customer-acceptance-for-a-new-customer"></a>Confirme a aceitação do cliente para um novo cliente

Utilize o seguinte procedimento para confirmar a aceitação do cliente enquanto cria um novo inquilino de cliente no Partner Center. Deves ser um agente administrativo ou agente comercial para fazer isto.

1. Selecione **Clientes** , e depois **Novo cliente** e, em seguida, selecione **informações de Conta** .

2. Insira a informação sobre o contacto **da Empresa** e **da Primária.**

   :::image type="content" source="images/mca/mca1.png" alt-text="Informações da empresa":::

3. Ao abrigo do **contrato de cliente da Microsoft,** selecione O cliente **aceitou o mais recente contrato de cliente da Microsoft.**

4. Nos termos **da data de aceitação** do Acordo, insira a data adequada. Não pode marcar isto para uma data futura.

5. Insira os detalhes do utilizador que forneceu a aceitação.

   :::image type="content" source="images/mca/MCA3.png" alt-text="Informações da empresa":::

   Por predefinição, é apresentada a informação do utilizador de contacto primário. Se isto não estiver correto, selecione **Update** e, em seguida, insira o **Nome Próprio** , **Apelido,** **endereço de e-mail** e * número de *telefone* (opcional) da pessoa que aceitou o acordo.

6. Selecione **Seguinte** para continuar com os passos restantes para criar o inquilino do cliente.

## <a name="confirm-customer-acceptance-for-an-existing-customer"></a>Confirme a aceitação do cliente para um cliente existente

Deves ser um agente administrativo ou agente comercial para fazer isto.

1. Selecione **Clientes** e, em seguida, encontre e selecione o cliente que deseja ver.

2. Selecione **informação de Conta** .

3. Ao abrigo do **contrato de cliente da Microsoft,** selecione **Update** .

   :::image type="content" source="images/mca/mca4.png" alt-text="Informações da empresa":::

4. Introduza o **Nome Próprio** , **Apelido,** **endereço de e-mail** e número de **telefone** (opcional) do utilizador que aceitou o acordo.

5. Nos termos **da data de aceitação** do Acordo, insira a data adequada. Não pode marcar isto para uma data futura.

6. Selecione **Guardar e continuar** .

## <a name="confirm-customer-acceptance-while-creating-new-order-for-an-existing-customer"></a>Confirme a aceitação do cliente ao criar uma nova encomenda para um cliente existente

Se tentar criar uma nova encomenda para um cliente existente que não tenha confirmado antes, receberá um pedido para completar a confirmação. Utilize o seguinte procedimento para o fazer.

1. Introduza o **Nome Próprio** , **Apelido,** **endereço de e-mail** e número de **telefone** (opcional) do utilizador que aceitou o acordo.

2. Nos termos **da data de aceitação** do Acordo, insira a data adequada. Não pode marcar isto para uma data futura.

3. Selecione **Guardar e continuar** .

## <a name="retrieve-confirmation-of-customer-acceptance-for-an-existing-customer"></a>Recuperar a confirmação da aceitação do cliente para um cliente existente

Pode obter a confirmação da aceitação do cliente para um cliente existente que forneceu anteriormente utilizando o procedimento abaixo. Deves ser um agente administrativo ou agente comercial para fazer isto.

1. Selecione **Clientes** e, em seguida, encontre e selecione o cliente que deseja ver.

2. Selecione **informação de Conta** .

3. De acordo com **o contrato de cliente da Microsoft,** verá se foi ou não fornecida confirmação para este cliente.

## <a name="next-steps"></a>Passos seguintes

- [Confirme a aceitação do Cliente do Microsoft No programa de parceiros CSP](confirm-customer-agreement.md)

- [Atestar a aceitação do Acordo de Cliente da Microsoft em nome do seu cliente](attest-acceptance-customer-agreement.md)