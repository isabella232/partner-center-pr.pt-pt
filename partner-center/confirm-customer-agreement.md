---
title: Confirm customer acceptance of the Microsoft Customer Agreement (Confirmar a aceitação do cliente do Contrato de Cliente Microsoft)
description: Saiba como confirmar a aceitação do cliente do Acordo de Cliente da Microsoft. Os participantes do programa Cloud Solution Provider (CSP) precisam de encomendar produtos e serviços da Microsoft aos clientes.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 05/05/2020
ms.openlocfilehash: 45a34473ff63875af8bd07962ea836661bc948ee
ms.sourcegitcommit: 22af0997d52a87417b62f44fb0a7d711bec77b35
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/19/2020
ms.locfileid: "92530638"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-customer-agreement-in-the-csp-partner-program"></a>Confirme a aceitação do Cliente do Microsoft No programa de parceiros CSP

**Aplica-se a**

- Partner Center
- Microsoft 365 Admin Center

**Funções adequadas**

- Agente administrativo
- Agente comercial

No dia 1 de outubro de 2019, a Microsoft introduziu o **Microsoft Customer Agreement** no programa CSP para substituir o Microsoft Cloud Agreement. Leia [orientações](indirect-reseller-tasks-in-partner-center.md) adicionais para revendedores indiretos. Para facilitar a migração dos parceiros para o novo acordo, ambos os acordos coexistiram no programa da CSP até 31 de janeiro de 2020. A partir de 1 de fevereiro de 2020, o Microsoft Customer Agreement substituiu o Microsoft Cloud Agreement.

Os clientes têm duas opções para aceitar o Acordo de Cliente da Microsoft. 

**Opção 1** : Atestado parceiro de aceitação do cliente - O Parceiro pode confirmar a aceitação do cliente utilizando o Partner Center API/SDK ou através do painel partner Center.

**Opção 2** : Aceitação direta do cliente - O parceiro pode convidar o cliente através de um URL para rever e aceitar o acordo no Microsoft 365 Admin Center.

## <a name="access-microsoft-customer-agreement-template"></a>Aceder ao modelo de Acordo de Cliente da Microsoft

Pode descarregar manualmente a versão mais recente do modelo do Microsoft Customer Agreement a partir [daqui.](https://aka.ms/customeragreement) O Microsoft Customer Agreement é específico por país. Ao solicitar o modelo do Contrato de Cliente da Microsoft, certifique-se de selecionar o país correto com base na localização do cliente.

## <a name="option-1-confirm-customer-acceptance-in-partner-center"></a>Opção 1: Confirmar a aceitação do cliente no Partner Center

Os parceiros podem confirmar a aceitação do Cliente do Microsoft Customer Agreement no Partner Center para clientes novos e existentes. Os revendedores não podem atestar em nome dos seus clientes e precisam de trabalhar com o seu Fornecedor Indireto para obter o atestado concluído.

### <a name="confirm-customer-acceptance-for-new-customers"></a>Confirme a aceitação do cliente para novos clientes

Quando criar um novo inquilino de clientes no Partner Center, utilize os seguintes passos para confirmar a aceitação do Cliente do Microsoft Customer Agreement. Deve ser um agente administrativo ou agente comercial para executar estes passos.

1. Selecione **Clientes** , e depois **Novo cliente** .

2. Informação em **Conta,** introduza informação para a empresa e o seu contacto principal.

3. De acordo com o **acordo da Microsoft,** selecione a caixa para atestar que o cliente aceitou o Acordo de Cliente da Microsoft.

4. Nos termos **da data de aceitação** do Acordo, insira a data adequada. Não pode marcar isto para uma data futura.

5. Certifique-se de que as informações de contacto do utilizador primário apresentadas estão corretas. Se estiver incorreto, selecione **Update** e introduza as informações precisas para a pessoa que aceitou o acordo.

6. Selecione **Next** para continuar a criar o inquilino do cliente.

   :::image type="content" source="images/mca/newcustomeragreement.jpg" alt-text="Novo cliente":::  

### <a name="confirm-customer-acceptance-for-existing-customers"></a>Confirme a aceitação do cliente para os clientes existentes

Deve ser um agente administrativo ou agente comercial para fazer isto:

1. Selecione **Clientes** . Encontre e selecione o cliente.

2. Selecione **informação de Conta** .

3. Ao abrigo **do Microsoft Customer Agreement** , selecione **Update** .

4. Introduza o **Nome Próprio** , **Apelido,** **endereço de e-mail** e número de **telefone** (opcional) da pessoa que aceitou o acordo. Nos termos **da data de aceitação** do Acordo, insira a data adequada. Não pode marcar isto para uma data futura.

5. **Selecione Save** e continue.

   :::image type="content" source="images/mcua2-update2.png" alt-text="Novo cliente":::

### <a name="retrieve-confirmation-of-customer-acceptance"></a>Recuperar a confirmação da aceitação do cliente

Pode obter a confirmação de que um cliente existente aceitou o Acordo de Cliente da Microsoft utilizando os seguintes passos. Deves ser um agente administrativo ou agente comercial para fazer isto.

1. Selecione **Clientes** e, em seguida, encontre e selecione o cliente que deseja ver.

2. Selecione **informação de Conta** .

3. De acordo com **o contrato de cliente da Microsoft,** consulte se a confirmação foi ou não fornecida por este cliente.

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a>Confirme a aceitação do cliente usando Partner Center API/SDK

Pode utilizar a API/SDK do Partner Center para confirmar a aceitação do cliente do Microsoft Customer Agreement. Para mais informações sobre a API/SDK, consulte:

- [Obtenha metadados de acordo para o Acordo de Cliente da Microsoft](/partner-center/develop/get-customer-agreement-metadata)

- [Confirme a aceitação do cliente do Microsoft Customer Agreement](/partner-center/develop/confirm-customer-consent-customer-agreement)

- [Obtenha a confirmação da aceitação do cliente do Microsoft Customer Agreement](/partner-center/develop/get-confirmation-of-customer-agreement)

- [Obtenha um link de descarregamento para o modelo do Contrato de Cliente da Microsoft](/partner-center/develop/download-customer-agreement-template)

## <a name="option-2-customer-acceptance-in-microsoft-365-admin-center"></a>Opção 2: Aceitação do cliente no Microsoft 365 Admin Center

Os parceiros podem convidar clientes novos e existentes, através de um URL, a rever e aceitar o acordo dentro do Microsoft 365 Admin Center. As próximas secções mostram-lhe como:

- Crie um novo cliente e convide o cliente a rever e aceitar o acordo.

- Convide um novo cliente a rever e a aceitar a relação e o acordo do revendedor.

- Convide um cliente existente a rever e a aceitar o acordo.

>[!NOTE]
> Pode utilizar [a API/SDK do Partner Center](/partner-center/develop/get-direct-sign-status-of-customer-agreement) para obter o estado da aceitação direta de um cliente do Acordo de Cliente da Microsoft.  

## <a name="create-a-new-customer-and-invite-the-customer-to-review-and-accept-the-agreement"></a>Crie um novo cliente e convide o cliente a rever e aceitar o acordo

Use os seguintes passos para criar um novo cliente no Partner Center e, em seguida, convidá-los a rever e aceitar o Acordo de Cliente da Microsoft dentro do Microsoft 365 Admin Center.

1. A partir do separador **Clientes** dentro do Partner Center, **selecione Adicionar cliente.**

2. Informação **em Conta** , introduza informações sobre o novo cliente em todas as áreas requeridas, incluindo o nome da empresa do cliente e o contacto primário.

3. De acordo com o **Cliente** , selecione a primeira opção, **o Cliente será solicitado a aceitar o Acordo de Cliente da Microsoft no Microsoft 365 Admin Center** . Preencha todos os outros campos necessários na página.

4. Selecione **Seguinte: Reveja** então continue os passos para criar o inquilino do cliente. 

>[!NOTE] 
>Os novos clientes não podem fazer uma nova compra até aceitarem o Acordo de Cliente da Microsoft.  

   :::image type="content" source="images/mca/create-new-customer.jpg" alt-text="Novo cliente":::

5. Quando chegar ao ecrã **de Confirmação** no novo fluxo de trabalho do cliente, guarde as credenciais do cliente. Terá de dar estas credenciais ao seu cliente mais tarde.

6. Fora do Partner Center, crie e envie um e-mail que convida o cliente a aceitar o Acordo de Cliente da Microsoft no Microsoft 365 Admin Center. Certifique-se de incluir estes itens no e-mail:

   - Um link para este [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (Inscrição obrigatória)

   - As credenciais do cliente que guardou no Passo 5.

7. O cliente receberá então o convite de e-mail do parceiro e selecionará o [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).

8. O cliente assina no Microsoft 365 Admin Center utilizando as credenciais de cliente previamente recebidas do parceiro.

9. Em seguida, o cliente verifica a caixa para aceitar o acordo de Cliente da Microsoft.

## <a name="invite-a-new-customer-to-review-and-accept-the-reseller-relationship-and-microsoft-customer-agreement"></a>Convide um novo cliente a rever e aceitar a relação de revendedor e o Acordo de Cliente da Microsoft 

Utilize os seguintes passos para convidar um novo cliente a rever e aceitar a relação de revendedor e o Acordo de Cliente da Microsoft. 

1. A partir do separador **Clientes** dentro do Partner Center, selecione Solicite um link **de relacionamento revendedor.** 

2. Será gerado um modelo de e-mail automático, incluindo texto e um URL parametrizado que direciona o cliente para o Microsoft 365 Admin Center.

3. Pode personalizar o modelo de e-mail gerado automaticamente e, em seguida, selecionar **Copy para clipboard** ou **Abrir no e-mail** .

4. Utilize este modelo de e-mail para convidar o cliente a aceitar o pedido **de relacionamento do revendedor** e o **Acordo de Cliente da Microsoft.** (Nota: No convite por e-mail, certifique-se de que o parceiro também inclui o URL que foi fornecido automaticamente, bem como as credenciais de cliente que foram criadas recentemente.)

   :::image type="content" source="images/mca/createrelationship.png" alt-text="Novo cliente":::

5. O cliente recebe convite via e-mail e clica no URL parametrizado. 

6. O cliente utiliza credenciais fornecidas pelo parceiro dentro do e-mail para assinar no Microsoft 365 Admin Center.

7. O cliente verifica a caixa para aceitar a relação de **revendedor** e **o Acordo de Cliente da Microsoft.** 

8. Dentro do mesmo URL, o cliente é capaz de ver uma lista consolidada de diferentes parceiros com os quais está a trabalhar. Podem selecionar um parceiro para ver detalhes.

   :::image type="content" source="images/mca/accept.jpg" alt-text="Novo cliente":::


## <a name="invite-an-existing-customer-to-review-and-accept-the-agreement"></a>Convide um cliente existente a rever e aceitar o acordo

Utilize os seguintes passos para convidar um cliente existente a rever e aceitar o Acordo de Cliente da Microsoft. 

1. Crie o e-mail do cliente com o URL incorporado convidando o seu cliente a aceitar o Acordo de Cliente da Microsoft.

2. O seu cliente recebe o convite por e-mail e clica no [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement). 

3. O cliente introduz as suas credenciais no Microsoft 365 Admin Center.

4. O seu cliente verifica a caixa para aceitar o Acordo de Cliente da Microsoft. 

5. Dentro do mesmo URL, o cliente pode ver a lista consolidada de diferentes parceiros com quem está a trabalhar. Podem selecionar um parceiro para ver detalhes.

   :::image type="content" source="images/mca/customeraccept.png" alt-text="Novo cliente":::

>[!NOTE]
>Em certos cenários, os clientes podem não ser capazes de aceitar diretamente o Acordo de Cliente da Microsoft. Para saber mais sobre estas situações, consulte [dois cenários onde precisa de atestar em nome do seu cliente.](attest-acceptance-customer-agreement.md)

### <a name="historical-timeline-details"></a>Detalhes históricos da linha do tempo

| Date | Marco | Detalhes |
|------------|------------|--------------------------------|
|01 de agosto de 2019| Pré-visualização UX disponível na caixa de areia| Os parceiros podem confirmar a aceitação do Cliente do Microsoft Customer Agreement utilizando o painel de instrumentos partner Center no ambiente de caixa de areia CSP. Os parceiros com acesso ao ambiente de caixa de areia CSP pré-visualizam as alterações da experiência do utilizador. Os parceiros sem acesso a sandbox podem aprender sobre as mudanças neste tópico.|
|03 de setembro de 2019|A pré-visualização da API está disponível na caixa de areia.|O parceiro pode confirmar a aceitação do Cliente do Microsoft Customer Agreement utilizando a API do Partner Center em ambiente de caixa de areia CSP. Os parceiros da API podem aproveitar esta oportunidade para visualizar as alterações da API e começar a trabalhar na integração da API para apoiar o novo acordo.|
|20 de setembro de 2019|.NET SDK pré-visualização está disponível na caixa de areia.|O parceiro pode confirmar a aceitação do Cliente do Microsoft Customer Agreement utilizando o Partner Center .NET SDK em ambiente de caixa de areia CSP. Os parceiros da API podem aproveitar esta oportunidade para visualizar as alterações .NET SDK e começar a trabalhar na integração da API para apoiar o novo acordo.|
|01 de outubro de 2019|Microsoft Customer Agreement disponível na produção|A Microsoft introduz o Acordo de Cliente da Microsoft no programa CSP para substituir o Microsoft Cloud Agreement. Os parceiros podem confirmar a aceitação do Cliente do Microsoft Customer Agreement utilizando o painel de instrumentos partner center e a API em produção. O Microsoft Cloud Agreement continua suportado no programa de parceiros CSP. No entanto, os parceiros são aconselhados a começar a migrar para o Microsoft Customer Agreement. Novas compras e alterações na contagem de licenças às subscrições existentes exigirão a confirmação do parceiro do Acordo de Cliente da Microsoft ou do Microsoft Cloud Agreement. Algumas novas ofertas (por exemplo, o novo plano Azure) exigirão a confirmação do Acordo de Cliente da Microsoft.|
|31 de janeiro de 2020|Microsoft Cloud Agreement removido da produção|O Microsoft Cloud Agreement já não é aceite no âmbito do programa de parceiros CSP. Novas compras e alterações na contagem de licenças às subscrições existentes exigirão que o parceiro forneça a confirmação do Acordo de Cliente da Microsoft. Este requisito aplica-se a novos clientes e clientes existentes que possam ter aceitado previamente o Microsoft Cloud Agreement.|
|3 de fevereiro de 2020|O Parceiro tem agora a opção de convidar o cliente através de um URL para rever e aceitar o acordo no Microsoft 365 Admin Center autenticado. | O cliente pode aceitar o Acordo de Cliente da Microsoft no Microsoft 365 Admin Center. A aceitação direta do cliente do acordo no Microsoft 365 Admin Center confirma a aprovação dos termos. 