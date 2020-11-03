---
title: Gerir localizações na sua conta de parceiro
ms.topic: article
ms.date: 10/12/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Saiba como adicionar uma nova localização e como a localização MPN ID é usada em programas de incentivo, negócios de CSP, subscrições e outras transações.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c6b0fc84636befedbc51aa0672ce19110eb4d9aa
ms.sourcegitcommit: 1719ff11409cd6953602b7798f8cfe821b8ea15e
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/15/2020
ms.locfileid: "92530428"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a>Gerencie as localizações da sua conta MPN e adicione uma nova localização

**Aplica-se a**

- Partner Center

**Funções adequadas**

- Administrador global
- Administrador de conta

A localização MPN ID identifica cada localização específica da sua empresa. Utiliza a localização MPN ID para se inscrever em programas de incentivo, para transacionar negócios do Cloud Solution Provider (CSP) e outras transações comerciais. O ID MPN global é utilizado para atividades não transacionais, tais como pedidos de apoio.

## <a name="the-following-is-a-typical-scenario"></a>Segue-se um cenário típico:

A Contoso tem a sua conta global Partner (PGA) no Reino Unido. Este é o seu negócio legal registrado, e o seu ID MPN global é usado para gerir todos os negócios não transacionais. A Contoso também tem contas de localização partner (PLA) equivalentes a subsidiárias ou divisões em outro local no Reino Unido, França e EUA. Na estrutura da Conta MPN, estas PLAs são representadas como IDs MPN de localização única. As PLAs são utilizadas para negócios transacionais, como CSP ou programas de incentivos. Os pagamentos estão ligados a locais específicos. 

>[!NOTE]
>Há uma relação 1-1 entre um inquilino da CSP e uma identificação de localização MPN.

:::image type="content" source="images/locations/locations1.png" alt-text="Estrutura das localizações da MPN":::

## <a name="prerequisites-in-order-to-add-a-new-location-for-a-csp-business"></a>Pré-requisitos para adicionar um novo local para uma empresa de CSP

Para adicionar uma nova localização comercial da CSP, existem vários pré-requisitos:

1. Você deve ter uma identificação mpn de localização no país onde você quer fazer negócios.

1. Precisa de um novo inquilino da AZure AD na [região de negócios](regional-authorization-overview.md) que ainda não esteja inscrito na CSP. Crie isto quando se inscrever na CSP.
 
3. Use o novo inquilino da AAD para se inscrever no programa CSP na região.
Fornecendo detalhes legais da empresa, incluindo o nome da empresa legal, endereço, detalhes de contato primário. Esta conta será submetida a verificação, por isso certifique-se de adicionar informações válidas.

>[!NOTE] 
 >Lembre-se de assinar com as **novas** credenciais para o **novo** inquilino da AD AZure. Não use as suas credenciais existentes como Partner Center irá reconhecê-lo como tendo já uma conta.

4. Aceite o Acordo de Parceiro da Microsoft e ative a conta.

## <a name="add-an-mpn-location"></a>Adicione uma localização MPN

1. Inscreva-se utilizando a conta MPN no Partner Center . A conta MPN deve ter privilégios de Administração Global ou Administração de Contas. 

1. A partir do **ícone Definição,** selecione as **definições do Parceiro** .

2. Selecione **Locais.**

3. **Selecione Adicione uma localização** e insira os detalhes do endereço da localização que pretende adicionar à sua empresa, bem como um contacto primário para a localização.

> [!NOTE]
> Uma vez que uma localização é adicionada no Centro de Parceiros, não pode ser removida. Verá **MPN** no menu esquerdo do Partner Center se tiver usado o ID MPN correto para iniciar sins.

## <a name="change-global-partner-account-location"></a>Alterar localização da conta de parceiro global

1. Na página **['Localizações',](https://partner.microsoft.com/pcv/accountsettings/locationsprofile)** consulte a lista de locais para garantir que o local que pretende como entidade legal está listado. Se não for, adicione.

   :::image type="content" source="images/updatepartnerprofile2.png" alt-text="Estrutura das localizações da MPN":::

2. Selecione **o perfil de Parceiro** e, em seguida, selecione Update legal business **profile**

   :::image type="content" source="images/updatepartnerprofile1.png" alt-text="Estrutura das localizações da MPN":::

3. Selecione a região e entidade legal e **envie-a.**

   :::image type="content" source="images/updatepartnerprofile3.png" alt-text="Estrutura das localizações da MPN":::

## <a name="next-steps"></a>Passos seguintes

- Conheça o [processo de verificação.](verification-responses.md)
