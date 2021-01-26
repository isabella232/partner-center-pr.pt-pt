---
title: Gerir localizações na sua conta de parceiro
ms.topic: how-to
ms.date: 01/25/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Saiba como adicionar uma nova localização e como a localização MPN ID é usada em programas de incentivo, negócios de CSP, subscrições e outras transações.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 38ea8a451f51d80998643e2a023420ea3efaa6ba
ms.sourcegitcommit: e99882e9b6c9b1a0f7427fb133693b1d977be76b
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/26/2021
ms.locfileid: "98773425"
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

## <a name="prerequisites-in-order-to-add-a-new-account-location-for-a-csp-business"></a>Pré-requisitos para adicionar uma nova localização de conta para uma empresa de CSP

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

1. A partir do **ícone Definição,** selecione as **definições da Organização**.

2. Selecione **Legal** e, em seguida, selecione **Localizações.**

3. **Selecione Adicione uma localização** e insira os detalhes do endereço da localização que pretende adicionar à sua empresa, bem como um contacto primário para a localização.

> [!NOTE]
> Uma vez que uma localização é adicionada no Centro de Parceiros, não pode ser removida. Verá **MPN** no menu esquerdo do Partner Center se tiver usado o ID MPN correto para iniciar sins.

## <a name="change-global-partner-account-location"></a>Alterar localização da conta de parceiro global

1. Nas **[localizações empresariais,](https://partner.microsoft.com/dashboard/account/v3/organization/legalinfo#mpn)** consulte a lista de locais para garantir que a localização desejada como entidade jurídica está listada. Se não for, adicione.

   :::image type="content" source="images/accountsettings/location1.png" alt-text="Screenshot da página de Localizações de Conta do Centro de Parceiros com lista de todas as localizações atuais.":::

2. Selecione **Legal** e, em seguida, selecione **Update legal business profile**
  
3. Selecione a região e entidade legal e **envie-a.**

  
## <a name="next-steps"></a>Próximos passos

- Conheça o [processo de verificação.](verification-responses.md)
