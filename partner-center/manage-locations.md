---
title: Gerir as localizações na conta de parceiro
ms.topic: how-to
ms.date: 05/01/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-membership
description: Saiba como adicionar uma nova localização e como a localização MPN ID é usada em programas de incentivo, negócios de CSP, subscrições e outras transações.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 66ca3a24a810f61eae9feece5e64440fa531cda5
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/09/2021
ms.locfileid: "123959949"
---
# <a name="manage-your-mpn-account-locations-and-add-delete-a-location"></a>Gerencie as localizações da sua conta MPN e adicione (excluir) uma localização


**Funções adequadas**: Administração global | Administrador de conta

A localização MPN ID identifica cada localização específica da sua empresa. Utiliza a localização MPN ID para se inscrever em programas de incentivo, para transacionar Fornecedor de Soluções em Nuvem (CSP) e outras transações comerciais. O ID MPN global é utilizado para atividades não transacionais, tais como pedidos de apoio.

## <a name="the-following-scenario-is-typical"></a>O seguinte cenário é típico:

A Contoso tem a sua conta global Partner (PGA) no Reino Unido. A PGA é o seu negócio legal registado, e o seu ID MPN global é usado para gerir todos os negócios não transacionais. A Contoso também tem contas de localização partner (PLA) equivalentes a subsidiárias ou divisões em outro local no Reino Unido, França e EUA. Na estrutura da Conta MPN, estas PLAs são representadas como IDs MPN de localização única. As PLAs são utilizadas para negócios transacionais, como CSP ou programas de incentivos. Os pagamentos estão ligados a locais específicos. 

>[!NOTE]
>Há uma relação 1-1 entre um inquilino da CSP e uma identificação de localização MPN.

:::image type="content" source="images/locations/locations1.png" alt-text="Estrutura de localizações de MPN.":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a>Pré-requisitos para adicionar uma nova conta para uma empresa de CSP

Para adicionar uma nova conta de negócios da CSP, comece por garantir que cumpriu os pré-requisitos.

1. Você deve ter uma identificação MPN de localização no país onde você quer fazer negócios com CSP. Para criar uma nova localização MPN, leia "Adicionar uma localização MPN" abaixo.
  
1. Para criar uma nova inscrição de Revendedor Indireto CSP, leia [Trabalhar com fornecedores indiretos](indirect-reseller-tasks-in-partner-center.md#get-started) 

>[!NOTE] 
 >Lembre-se de assinar com as **novas** credenciais para a **nova** conta CSP. Não use as suas credenciais existentes como Partner Center irá reconhecê-lo como tendo já uma conta.

2. Aceite o Acordo de Parceiro da Microsoft e ative a conta.

1. Se quiser inscrever-se como parceiro direct Bill, leia [requisitos para parceiros direct Bill](direct-partner-new-requirements.md)

## <a name="view-and-update-your-mpn-locations"></a>Ver e atualizar as suas localizações de MPN

1. Inscreva-se no painel partner [Center](https://partner.microsoft.com/dashboard/home) com as suas credenciais de conta MPN. (As suas credenciais MPN podem ser diferentes das suas credenciais de CSP) 
 
1. A partir do ícone **Definições,** selecione **definições de conta,** **perfil de organização,** **Legal**. 

1. No **separador Partner,** verifique se não existe uma mensagem de erro de banner a pedir-lhe para corrigir locais migrados a partir de PMC.  Se as suas localizações não foram configuradas corretamente em PMC, e ainda não transitaram para PC, precisa atualizar essas localizações.

:::image type="content" source="images/locations/location-two.png" alt-text="O Screencap mostra como atualizar a localização.":::
 
4.  No ecrã de **localizações do PMC de revisão,** selecione **Update**.
Atualizar os seguintes campos:

- **Campo de nomes**: Certifique-se de que o nome da localização da empresa está correto. Se for apresentado um erro duplicado, tente mudar de, por exemplo, Contoso para Contoso, Inc.

- **Área de Entidade Jurídica**: Certifique-se de que escolheu a entidade jurídica a que a localização está ligada

- **Linha de endereço 1 & 2 campos**: Certifique-se de que o endereço está correto

- **Cidade & campos estado/província**: Certifique-se de que a combinação entre a cidade e o estado/província está correta. Há países onde será aplicado o menu suspenso para escolher o Estado/Província, e noutros países esse campo terá de ser inserido manualmente.

- **ZIP/ Código Postal :** Certifique-se de que o campo código postal está a corresponder ao seu País, Região, Cidade ou Endereço indicados.

- **Principais campos de informações de contacto**: Certifique-se de que os campos de primeiro e último nome estão preenchidos e que o endereço de e-mail indicado é um endereço de e-mail de trabalho e não pessoal (por exemplo, @outlook.com , @live.com etc.)

- **Telefone campo de números**: Certifique-se de que o número Telefone NÃO inclui caracteres especiais, espaços ou código de país. O valor introduzido no campo Telefone Número conterá sempre um máximo de 10 caracteres.

5. Se não houver uma mensagem de erro, então a partir de **Definições**, selecione **Conta Definições**, Perfil **da Organização,** **Identificadores**.

6. Encontre o ID MPN com o Tipo "Localização" que corresponda ao país desta conta CSP e use-o para completar a associação.

7. Se não conseguir encontrar o ID MPN de localização que corresponda à conta CSP que pretende utilizar, pode adicionar uma nova localização, que irá criar um novo ID MPN. Consulte **a localização mpn** abaixo.

## <a name="add-an-mpn-location"></a>Adicione uma localização MPN

1. Inscreva-se usando a conta MPN no Partner Center. (As suas credenciais MPN podem ser diferentes das suas credenciais de CSP.) A conta MPN deve ter privilégios de Administração Global ou Administração de Contas. 

1. A partir do **ícone Definições**, selecione as **definições de Conta** e, em seguida, selecione o perfil da **Organização**.

2. Selecione **Legal** e, em seguida, no separador **Parceiro,** selecione **localizações de Negócios** e selecione **Adicionar uma localização.**

3. Forneça os dados necessários, incluindo o nome comercial, endereço e contato para a localização que pretende adicionar à sua empresa.
 
1. Selecione **Localizar adicionar**. Isto criará um novo ID MPN para a nova localização que pode utilizar para transações e incentivos CSP.

:::image type="content" source="images/legal-biz.png" alt-text="Adicione um novo negócio legal.":::

> [!NOTE]
> Uma vez que uma localização é adicionada no Partner Center, não é possível removê-la. Verá **MPN** no menu esquerdo do Partner Center se tiver usado o ID MPN correto para iniciar sins.

## <a name="add-the-registration-number-id"></a>Adicione o ID número de registo

Se é um fornecedor indireto, parceiro de conta direta ou revendedor indireto e está a fazer negócios com clientes novos ou existentes nos seguintes países, tem de fornecer números de identificação de registo para o seu negócio. Se o país em que está a fazer negócios não estiver listado abaixo, o ID de registo é opcional.

- Arménia 
- Azerbaijão 
- Bielorrússia 
- Brasil 
- Hungria 
- Índia 
- Iraque 
- Cazaquistão 
- Quirguistão 
- Moldávia 
- Mianmar 
- Polónia 
- Rússia 
- Arábia Saudita 
- África do Sul 
- Sudão do Sul  
- Tajiquistão 
- Tailândia
- Turquia 
- Ucrânia 
- Emirados Árabes Unidos 
- Usbequistão 
- Venezuela
- Vietname 


Para mais informações, leia [as informações do número de ID do registo](reg-number-id.md)

## <a name="delete-a-location"></a>Excluir uma localização

Para eliminar uma localização da sua conta, terá de contactar o [Partner Support.](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b) Confirme se compreende o impacto desta ação. As localizações eliminadas não podem ser recuperadas e qualquer coisa ligada a esse ID MPN específico deixará de ser reconhecida ou ativa para a sua empresa.

## <a name="change-country-of-partner-global-account"></a>Mudar país de conta global partner 

1. Inscreva-se usando a conta MPN no Partner Center. (As suas credenciais MPN podem ser diferentes das suas credenciais de CSP.) A conta MPN deve ter privilégios de Administração Global ou Administração de Contas. 

2. No separador **Partner,** vá às localizações do **Negócios** e verifique a lista de locais para garantir que o local que deseja como entidade legal está listado. 
 
1. Para adicionar uma localização, clique em **Adicionar uma localização** e, no voo para fora, forneça os detalhes necessários, incluindo o nome do negócio, endereço e contacto primário para a localização que pretende adicionar à sua empresa. 
 
1. Selecione **Mude o seu país** ao lado da lista de drop-down **País/região** e siga os passos. 

:::image type="content" source="images/lbp.png" alt-text="Os dados legais do perfil de negócio saem.":::

5. Selecione **Guardar**.

6. O país da conta global da MPN será alterado para o novo país legal.
  
## <a name="next-steps"></a>Passos seguintes

- Conheça o [processo de verificação.](verification-responses.md)
