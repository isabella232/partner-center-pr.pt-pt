---
title: Gerir localizações na sua conta de parceiro
ms.topic: how-to
ms.date: 02/05/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Saiba como adicionar uma nova localização e como a localização MPN ID é usada em programas de incentivo, negócios de CSP, subscrições e outras transações.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c5ac31b772c6757468c5ea9d463643731571b31f
ms.sourcegitcommit: d37a3f353426e52dfbbac577b7576f9c3f6d2ddf
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/06/2021
ms.locfileid: "99624277"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a>Gerencie as localizações da sua conta MPN e adicione uma nova localização


**Funções adequadas**

- Administrador global
- Administrador de conta

A localização MPN ID identifica cada localização específica da sua empresa. Utiliza a localização MPN ID para se inscrever em programas de incentivo, para transacionar negócios do Cloud Solution Provider (CSP) e outras transações comerciais. O ID MPN global é utilizado para atividades não transacionais, tais como pedidos de apoio.

## <a name="the-following-is-a-typical-scenario"></a>Segue-se um cenário típico:

A Contoso tem a sua conta global Partner (PGA) no Reino Unido. Este é o seu negócio legal registrado, e o seu ID MPN global é usado para gerir todos os negócios não transacionais. A Contoso também tem contas de localização partner (PLA) equivalentes a subsidiárias ou divisões em outro local no Reino Unido, França e EUA. Na estrutura da Conta MPN, estas PLAs são representadas como IDs MPN de localização única. As PLAs são utilizadas para negócios transacionais, como CSP ou programas de incentivos. Os pagamentos estão ligados a locais específicos. 

>[!NOTE]
>Há uma relação 1-1 entre um inquilino da CSP e uma identificação de localização MPN.

:::image type="content" source="images/locations/locations1.png" alt-text="Estrutura das localizações da MPN":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a>Pré-requisitos para adicionar uma nova conta para uma empresa de CSP

Para adicionar uma nova conta de negócios da CSP, comece por garantir que cumpriu os pré-requisitos.

1. Você deve ter uma identificação MPN de localização no país onde você quer fazer negócios com CSP. Para criar uma nova localização MPN, leia "Adicionar uma localização MPN" abaixo.
  
1. Para criar uma nova inscrição de Revendedor Indireto CSP, leia [Trabalhar com fornecedores indiretos](indirect-reseller-tasks-in-partner-center.md#get-started) 

>[!NOTE] 
 >Lembre-se de assinar com as **novas** credenciais para a **nova** conta CSP. Não use as suas credenciais existentes como Partner Center irá reconhecê-lo como tendo já uma conta.

2. Aceite o Acordo de Parceiro da Microsoft e ative a conta.

1. Se quiser inscrever-se como parceiro direct Bill, leia [requisitos para parceiros direct Bill](direct-partner-new-requirements.md)

## <a name="view-your-mpn-locations"></a>Ver as suas localizações de MPN

1. Inscreva-se no painel partner [Center](https://partner.microsoft.com/dashboard/home) com as suas credenciais de conta MPN. (As suas credenciais MPN podem ser diferentes das suas credenciais de CSP) 
 
1. A partir do ícone **Definições,** selecione **definições de conta**, **perfil de organização,** **Legal**. 

1. No **separador Partner** verifique se não existe uma mensagem de erro de banner a pedir-lhe para corrigir locais migrados a partir de PMC. Se houver, siga as instruções e fixe os locais. 

3. Se não houver uma mensagem de erro, então a partir de  **Definições**, selecione  **Definições** de Conta , **Perfil da Organização,** **Identificadores**.

4. Encontre o ID MPN com o Tipo "Localização" que corresponda ao país desta conta CSP e use-o para pesquisar abaixo e completar a associação.

5. Se não conseguir encontrar o ID MPN de localização que corresponda à conta CSP que pretende utilizar, pode adicionar uma nova localização que irá criar um novo ID MPN. Consulte **a localização mpn** abaixo.

## <a name="add-an-mpn-location"></a>Adicione uma localização MPN

1. Inscreva-se usando a conta MPN no Partner Center. (As suas credenciais MPN podem ser diferentes das suas credenciais CSP) . A conta MPN deve ter privilégios de Administração Global ou Administração de Contas. 

1. A partir do **ícone Definições,** selecione as **definições de Conta** e, em seguida, selecione o perfil da **Organização**.

2. Selecione **Legal** e, em seguida, no separador **Parceiro,** selecione **localizações de Negócios** e clique em **Adicionar uma localização.**

3. Forneça os dados necessários, incluindo o nome comercial, endereço e contato para a localização que pretende adicionar à sua empresa.
 
1. Clique **em Adicionar localização**. Isto criará um novo ID MPN para o novo local que pode utilizar para transações e incentivos da CSP.

:::image type="content" source="images/legal-biz.png" alt-text="Adicione um novo negócio legal":::

> [!NOTE]
> Uma vez que uma localização é adicionada no Centro de Parceiros, não pode ser removida. Verá **MPN** no menu esquerdo do Partner Center se tiver usado o ID MPN correto para iniciar sins.

## <a name="change-country-of-partner-global-account"></a>Mudar país de conta global partner 

1. Inscreva-se usando a conta MPN no Partner Center. (As suas credenciais MPN podem ser diferentes das suas credenciais CSP) . A conta MPN deve ter privilégios de Administração Global ou Administração de Contas. 

2. No separador **Partner,** vá às localizações do **Negócios** e verifique a lista de locais para garantir que o local que deseja como entidade legal está listado. 
 
1. Para adicionar uma localização, clique em **Adicionar uma localização** e, no voo para fora, forneça os detalhes necessários, incluindo o nome do negócio, endereço e contacto primário para a localização que pretende adicionar à sua empresa. 
 
1. Selecione **Mude o seu país** junto ao **país/região** drop-down e siga os passos. 

:::image type="content" source="images/lbp.png" alt-text="Os dados do perfil de negócio legal voam para fora":::

5. Clique em **Guardar**.

6. O país da conta global da MPN será alterado para o novo país legal.
  
## <a name="next-steps"></a>Passos seguintes

- Conheça o [processo de verificação.](verification-responses.md)
