---
title: Como confirmar que o seu cliente aceitou o Acordo de Cliente da Microsoft para o programa CSP
description: Fornecedor de Soluções em Nuvem parceiros (CSP) precisam confirmar a aceitação do cliente do Acordo de Cliente da Microsoft antes de encomendar serviços Microsoft para os clientes.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 03/24/2021
ms.openlocfilehash: ed3b888791dad1e875db64b7ccbe20e7b0a8b4bbd71fb7c83cc677ee2d5f2d3a
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/06/2021
ms.locfileid: "115680111"
---
# <a name="how-to-confirm-that-your-customer-has-accepted-the-microsoft-customer-agreement-to-the-csp-program"></a>Como confirmar que o seu cliente aceitou o Acordo de Cliente da Microsoft para o programa CSP

**Funções adequadas**: Agente administrador | Agente comercial


Os clientes têm duas opções para a forma como aceitam o Acordo de Cliente da Microsoft.

**Opção 1**: Atestado parceiro de aceitação do cliente - O Parceiro pode confirmar a aceitação do cliente utilizando o Partner Center API/SDK ou através do painel partner Center.

**Opção 2**: Aceitação direta do cliente - O parceiro pode convidar o cliente através de um URL para rever e aceitar o acordo no Centro de Administração Microsoft 365.

## <a name="access-microsoft-customer-agreement-template"></a>Aceder ao modelo de Acordo de Cliente da Microsoft

Pode descarregar manualmente a versão mais recente do modelo do Microsoft Customer Agreement a partir [daqui.](https://aka.ms/customeragreement) O Microsoft Customer Agreement é específico por país. Ao solicitar o modelo do Contrato de Cliente da Microsoft, certifique-se de selecionar o país correto com base na localização do cliente.

## <a name="option-1-confirm-customer-acceptance-in-partner-center"></a>Opção 1: Confirmar a aceitação do cliente no Partner Center

Os parceiros de conta direta podem confirmar a aceitação do Cliente do Microsoft Customer Agreement no Partner Center para clientes novos e existentes. Os revendedores indiretos não podem atestar em nome dos seus clientes e precisam de trabalhar com o seu Fornecedor Indireto para obter o atestado concluído.

### <a name="confirm-customer-acceptance-for-new-customers"></a>Confirme a aceitação do cliente para novos clientes

Quando criar um novo inquilino de clientes no Partner Center, utilize os seguintes passos para confirmar a aceitação do Cliente do Microsoft Customer Agreement. Deve ser um agente administrativo ou agente comercial para executar estes passos.

1. Selecione **Clientes**, e depois **Novo cliente**.

2. Informação em **Conta,** introduza informação para a empresa e o seu contacto principal.

3. De acordo com o **acordo da Microsoft,** selecione a caixa para atestar que o cliente aceitou o Acordo de Cliente da Microsoft.

4. Nos termos **da data de aceitação** do Acordo, insira a data adequada. Não pode marcar isto para uma data futura.

5. Certifique-se de que as informações de contacto do utilizador primário apresentadas estão corretas. Se estiver incorreto, selecione **Update** e introduza as informações precisas para a pessoa que aceitou o acordo.

6. Selecione **Next** para continuar a criar o inquilino do cliente.

   :::image type="content" source="images/mca/newcustomeragreement.jpg" alt-text="Novo cliente.":::  

### <a name="confirm-customer-acceptance-for-existing-customers"></a>Confirme a aceitação do cliente para os clientes existentes

Deve ser um agente administrativo ou agente comercial para fazer isto:

1. Selecione **Clientes**. Encontre e selecione o cliente.

2. Selecione **informação de Conta**.

3. Ao abrigo **do Microsoft Customer Agreement**, selecione **Update**.

4. Introduza o **Nome Próprio**, **Apelido,** **endereço de e-mail** e **Telefone número** (opcional) da pessoa que aceitou o acordo. Nos termos **da data de aceitação** do Acordo, insira a data adequada. Não pode marcar isto para uma data futura.

5. **Selecione Save** e continue.

   :::image type="content" source="images/mcua2-update2.png" alt-text="Cliente existente.":::

### <a name="retrieve-confirmation-of-customer-acceptance"></a>Recuperar a confirmação da aceitação do cliente

Para obter a confirmação de que um cliente existente aceitou o Acordo de Cliente da Microsoft, utilize os seguintes passos. Deves ser um agente administrativo ou agente comercial para fazer isto.

1. Selecione **Clientes** e, em seguida, encontre e selecione o cliente que deseja ver.

2. Selecione **informação de Conta**.

3. De acordo com **o contrato de cliente da Microsoft,** consulte se a confirmação foi ou não fornecida por este cliente.

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a>Confirme a aceitação do cliente usando Partner Center API/SDK

Pode utilizar a API/SDK do Partner Center para confirmar a aceitação do cliente do Microsoft Customer Agreement. Para mais informações sobre a API/SDK, consulte:

- [Obter metadados de contrato para o Contrato de Cliente Microsoft](/partner-center/develop/get-customer-agreement-metadata)

- [Confirmar aceitação do cliente do Contrato de Cliente Microsoft](/partner-center/develop/confirm-customer-consent-customer-agreement)

- [Obter confirmação da aceitação do cliente do Contrato de Cliente Microsoft](/partner-center/develop/get-confirmation-of-customer-agreement)

- [Obtenha um link de descarregamento para o modelo do Contrato de Cliente da Microsoft](/partner-center/develop/download-customer-agreement-template)

## <a name="option-2-customer-acceptance-in-microsoft-365-admin-center"></a>Opção 2: Aceitação do cliente no Administração Microsoft 365 Center

Os parceiros podem convidar clientes novos e existentes, através de um URL, a rever e aceitar o acordo dentro do Administração Microsoft 365 Center. As próximas secções mostram-lhe como:

- Crie um novo cliente e convide o cliente a rever e aceitar o acordo.

- Convide um novo cliente a rever e a aceitar a relação e o acordo do revendedor.

- Convide um cliente existente a rever e a aceitar o acordo.

>[!NOTE]
> Pode utilizar [a API/SDK do Partner Center](/partner-center/develop/get-direct-sign-status-of-customer-agreement) para obter o estado da aceitação direta de um cliente do Acordo de Cliente da Microsoft.  

## <a name="create-a-new-customer-and-invite-the-customer-to-review-and-accept-the-agreement"></a>Crie um novo cliente e convide o cliente a rever e aceitar o acordo

Use os seguintes passos para criar um novo cliente no Partner Center e, em seguida, convidá-los a rever e aceitar o Acordo de Cliente da Microsoft dentro Administração Microsoft 365 Center.

1. A partir do separador **Clientes** dentro do Partner Center, **selecione Adicionar cliente.**

2. Informação **em Conta**, introduza informações sobre o novo cliente em todas as áreas requeridas, incluindo o nome da empresa do cliente e o contacto primário.

3. De acordo com **o Cliente,** o Cliente selecionado **será solicitado a aceitar o Acordo de Cliente da Microsoft no Administração Microsoft 365 Center**. Preencha todos os outros campos necessários na página.

4. Selecione **Seguinte: Reveja** então continue os passos para criar o inquilino do cliente. 

>[!NOTE] 
>Os novos clientes não podem fazer uma compra até aceitarem o Acordo de Cliente da Microsoft.  

   :::image type="content" source="images/mca/create-new-customer.jpg" alt-text="Criar um novo cliente.":::

5. Quando chegar ao ecrã **de Confirmação** no novo fluxo de trabalho do cliente, guarde as credenciais do cliente. Terá de dar estas credenciais ao seu cliente mais tarde.

6. Fora do Partner Center, crie e envie um e-mail que convida o cliente a aceitar o Acordo de Cliente da Microsoft no Administração Microsoft 365 Center. Certifique-se de incluir estes itens no e-mail:

   - Um link para este [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (Inscrição obrigatória)

   - As credenciais do cliente que guardou no passo 5.

7. O cliente receberá então o convite de e-mail do parceiro e selecionará o [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).

8. O cliente assina no Administração Microsoft 365 Center utilizando as credenciais de cliente que forneceu.

9. O cliente verifica a caixa para aceitar o acordo de Cliente da Microsoft.

## <a name="invite-a-new-customer-to-review-and-accept-the-reseller-relationship-and-microsoft-customer-agreement"></a>Convide um novo cliente a rever e aceitar a relação de revendedor e o Acordo de Cliente da Microsoft 

Utilize os seguintes passos para convidar um novo cliente a rever e aceitar a relação de revendedor e o Acordo de Cliente da Microsoft. 

1. A partir do separador **Clientes** dentro do Partner Center, selecione Solicite um link **de relacionamento revendedor.** 

2. Será gerado um modelo de e-mail automático, incluindo texto e um URL parametrizado que direciona o cliente para o Centro de Administração Microsoft 365.

3. Pode personalizar o modelo de e-mail gerado automaticamente e, em seguida, selecionar **Copy para clipboard** ou **Abrir no e-mail**.

4. Utilize este modelo de e-mail para convidar o cliente a aceitar o pedido **de relacionamento do revendedor** e o **Acordo de Cliente da Microsoft.** (Nota: No convite por e-mail, certifique-se de que o parceiro também inclui o URL que foi fornecido automaticamente, bem como as credenciais de cliente que foram criadas recentemente.)

   :::image type="content" source="images/mca/createrelationship.png" alt-text="criar uma relação.":::

5. O cliente recebe convite via e-mail e clica no URL parametrizado. 

6. O cliente utiliza credenciais que fornece dentro de e-mail para iniciar sinse no Administração Microsoft 365 Center.

7. O cliente verifica a caixa para aceitar a relação de **revendedor** e **o Acordo de Cliente da Microsoft.** 

8. Dentro do mesmo URL, o cliente é capaz de ver uma lista consolidada de diferentes parceiros com os quais está a trabalhar. Podem selecionar um parceiro para ver detalhes.

   :::image type="content" source="images/mca/accept.jpg" alt-text="Aceite um acordo.":::


## <a name="invite-an-existing-customer-to-review-and-accept-the-agreement"></a>Convide um cliente existente a rever e aceitar o acordo

Utilize os seguintes passos para convidar um cliente existente a rever e aceitar o Acordo de Cliente da Microsoft. 

1. Crie o e-mail do cliente com o URL incorporado convidando o seu cliente a aceitar o Acordo de Cliente da Microsoft.

2. O seu cliente recebe o convite por e-mail e clica no [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement). 

3. O cliente introduz as suas credenciais no Administração Microsoft 365 Center.

4. O seu cliente verifica a caixa para aceitar o Acordo de Cliente da Microsoft. 

5. Dentro do mesmo URL, o cliente pode ver a lista consolidada de diferentes parceiros com quem está a trabalhar. Podem selecionar um parceiro para ver detalhes.

   :::image type="content" source="images/mca/customeraccept.png" alt-text="cliente.":::

>[!NOTE]
>Em certos cenários, os clientes podem não ser capazes de aceitar diretamente o Acordo de Cliente da Microsoft. Para saber mais sobre estas situações, leia Dois cenários onde precisa de atestar em nome do seu cliente, abaixo.

## <a name="two-scenarios-where-you-need-to-attest-on-behalf-of-your-customer"></a>Dois cenários em que precisa de atestar em nome do seu cliente

Existem dois cenários em que os clientes podem não ser capazes de aceitar diretamente o Acordo de Cliente da Microsoft dentro do Administração Microsoft 365 Center.

**Cenário 1**: Um cliente existente adquiriu qualquer um dos seguintes através de uma relação de parceiro existente: ofertas, subscrições de software ou software, Instâncias Reservadas ou Plano Azure. O cliente está agora a tentar fazer qualquer nova compra (excluindo a renovação automática). Quando esse cliente clicar no URL, receberão a mensagem "Por favor contacte o seu Parceiro para confirmar a sua aceitação do Acordo de Cliente da Microsoft."  

**Para resolver:** Tem de atestar em nome do cliente.

:::image type="content" source="images/mca/accept-scenario-1.png" alt-text="Screenshot da página Administração Microsoft 365 Center pedindo-lhe para contactar o seu parceiro para confirmar a aceitação do Acordo de Cliente da Microsoft.":::

**Cenário 2**: Um cliente existente adquiriu qualquer uma das seguintes ofertas, subscrições de software e software, Instâncias Reservadas e Plano Azure. O cliente está agora a tentar fazer qualquer nova compra com um novo parceiro.

Quando o cliente clicar no URL para Administração Microsoft 365 Center para aceitar a nova relação de parceiro e o acordo, eles receberão a mensagem "Por favor contacte o seu Parceiro para confirmar a sua aceitação do Acordo de Cliente da Microsoft."  

**Para resolver:** Tem de atestar em nome do cliente.  

## <a name="confirm-that-a-customer-has-accepted-the-agreement"></a>Confirme que um cliente aceitou o acordo

Se tentar criar uma nova encomenda para um cliente existente que não tenha confirmado antes, receberá um pedido para completar a confirmação. Utilize o seguinte procedimento para o fazer.

1. Introduza o **Nome Próprio**, **Apelido,** **endereço de e-mail** e **Telefone número** (opcional) do utilizador que aceitou o acordo.

2. Nos termos **da data de aceitação** do Acordo, insira a data adequada. Não pode marcar isto para uma data futura.

3. Selecione **Guardar e continuar**. 

## <a name="next-steps"></a>Passos seguintes

- [Verificar ou atualizar as informações do perfil da empresa](update-your-partner-profile.md)
- [Contratos de Cliente Microsoft (por região, idioma)](Agreements.md)
