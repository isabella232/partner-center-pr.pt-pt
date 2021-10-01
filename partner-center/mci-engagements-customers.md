---
title: Página de clientes para compromissos com MCI
description: Utilize a página clientes dentro da secção de Compromissos do Programa De incentivo ao Comércio da Microsoft (MCI) para gerir os clientes.
author: Karthic83
ms.author: kashanum
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
ms.topic: how-to
ms.date: 09/29/2021
ms.custom: template-how-to
ms.openlocfilehash: bfa3185213abe5e166c3049602d3ca2dc16be70c
ms.sourcegitcommit: 6d29e7e6d700ee5638ba10ee12f75e37f993dae9
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/01/2021
ms.locfileid: "129365152"
---
# <a name="customers-page-for-mci-engagements"></a>Página de clientes para compromissos com MCI

**Funções adequadas**: Incentivos administrativos | Utilizador de incentivos

>[!NOTE]
>Isto aplica-se apenas para construir compromissos de intenção, isto é, workshops. 

A página **clientes** classifica os clientes por elegíveis, não elegíveis e completas para cada compromisso. A página está pré-exopultada com todos os clientes que forneceram consentimento para qualquer workshop no Partner Center. 

:::image type="content" source="images/incentives/customers-page.png" alt-text="Screenshot da página de Clientes." lightbox="images/incentives/customers-page.png":::

- O **separador Elegível** mostra todos os clientes elegíveis para o workshop. 
   - A coluna **Tipo** irá listar os clientes como "ativos" se tiver recebido o consentimento do cliente. Até lá, dirá "não começou".
- O **separador Não Elegível** mostra todos os clientes que não são elegíveis para o workshop por uma de três razões:  
   - O cliente não cumpre os critérios de elegibilidade para o noivado, 
   - O cliente deu consentimento a outro parceiro, ou 
   - O cliente já participou no workshop com outro parceiro. 
- O separador **Complete** mostra todos os clientes para os quais completou este workshop. Pode ver os detalhes da sua reclamação com este cliente selecionando a **reclamação do workshop 'Ver'** sob a coluna **Ação.**

Para qualquer compromisso, é-lhe exigido que adicione um cliente ou reclame um cliente (não ambos).

## <a name="add-a-customer"></a>Adicionar um cliente 
1. Selecione **+ Adicionar o cliente** na página cliente **do** envolvimento do workshop relevante utilizando o **separador Elegível.**
2. Forneça um ID de localização MPN para o workshop e o endereço de e-mail do cliente. O campo **TPID /Tenant ID** do cliente é opcional. Apenas os IDs de localização MPN que estão ambos inscritos no programa MCI e são elegíveis para este noivado aparecerão. Selecione **Seguinte**.
   - Se não fornecer um ID do inquilino ou iD principal dos pais (TPID) para o cliente, o sistema derivará o ID do inquilino a partir do endereço de e-mail do cliente. Em seguida, irá executar a verificação de elegibilidade do cliente para o workshop.
   - Se o ID do inquilino do cliente não puder ser encontrado usando o endereço de e-mail, você será solicitado para fornecer um endereço de e-mail diferente ou o ID/TPID do inquilino.
   - Se o ID/TPID do inquilino for fornecido, o sistema garantirá que o domínio de e-mail corresponde ao ID do inquilino. Se for encontrado um desfasamento, o sistema pedir-lhe-á que forneça uma razão.

   :::image type="content" source="images/incentives/add-customer-1.png" alt-text="Screenshot 1 de 3 mostrando como adicionar cliente." lightbox="images/incentives/add-customer-1.png":::

3. Escolha o workshop(s) para o qual gostaria de adicionar o cliente. Apenas esses workshops podem ser selecionados para os quais você e o seu cliente são elegíveis. Selecione **Seguinte**.

:::image type="content" source="images/incentives/add-customer-2.png" alt-text="Screenshot 2 de 3 mostrando como adicionar cliente." lightbox="images/incentives/add-customer-2.png":::

4. Reveja as informações e **selecione Adicionar cliente**. Terá a confirmação de que o cliente foi adicionado.

:::image type="content" source="images/incentives/add-customer-3.png" alt-text="Screenshot 3 de 3 mostrando como adicionar cliente." lightbox="images/incentives/add-customer-3.png":::

Deverá agora ver o cliente que adicionou nas respetivas páginas **clientes** para os compromissos do workshop selecionados no passo 3.

## <a name="claim-a-customer"></a>Reclamar um cliente 
O **separador Elegível** na página **clientes** será pré-carregado com uma lista de clientes que lhe são conhecidos, o parceiro, através de outros compromissos. Pode iniciar um workshop com qualquer um destes clientes. 
1. Selecione **O cliente 'Reclamar'** a partir da coluna **Ação.** 
2. Escolha um ID de localização MPN para o workshop. Apenas aparecerão os IDs de localização MPN que estão inscritos no programa DOM e que são elegíveis para este noivado. Selecione **Seguinte**.

   :::image type="content" source="images/incentives/claim-customer-1.png" alt-text="Screenshot 1 de 3 mostrando como reclamar o cliente." lightbox="images/incentives/claim-customer-1.png":::

3. Escolha o workshop(s) que pretende adicionar e, em seguida, selecione **Next**.

   :::image type="content" source="images/incentives/claim-customer-2.png" alt-text="Screenshot 2 de 3 mostrando como reclamar o cliente." lightbox="images/incentives/claim-customer-2.png":::

4. Reveja as informações e **selecione Adicionar cliente**. Terá a confirmação de que o cliente foi reclamado.

   :::image type="content" source="images/incentives/claim-customer-3.png" alt-text="Screenshot 3 de 3 mostrando como reclamar o cliente." lightbox="images/incentives/claim-customer-3.png":::

## <a name="ask-for-customer-consent"></a>Pedir o consentimento do cliente 
Se deseja realizar um workshop com um cliente, então precisa pedir consentimento ao cliente, que é o seu acordo para participar no workshop. Terá um total de 30 dias para obter o consentimento após a adição ou reclamação do cliente.

Depois de ter adicionado ou reclamado um cliente, verá quantos dias lhe restam para obter o consentimento na coluna de estado na página **Clientes.**
1. Selecione **o consentimento** do cliente do Gatilho a partir da coluna **Ação.** 
2. Forneça os e-mails e informações de contacto do cliente, juntamente com informações de contacto para a sua própria empresa. Em seguida, selecione **Seguinte**.

   :::image type="content" source="images/incentives/ask-consent-1.png" alt-text="Screenshot 1 de 2 mostrando como solicitar o consentimento do cliente." lightbox="images/incentives/ask-consent-1.png":::

3. Reveja os detalhes e **selecione Enviar por consentimento.** Será enviado um e-mail ao cliente para que possa aceitar ou recusar o workshop.
   - Se não tiver recebido o consentimento, pode enviar um lembrete clicando no link de consentimento do **cliente Resend** sob a coluna **Ação.**
   - Se um cliente foi recentemente adicionado mas recusa a participação no workshop, ou não responde dentro da linha temporal exigida, deixará de aparecer na página **clientes** para esse compromisso.

   :::image type="content" source="images/incentives/ask-consent-2.png" alt-text="Screenshot 2 de 2 mostrando como solicitar o consentimento do cliente." lightbox="images/incentives/ask-consent-2.png":::

Assim que o cliente der o seu consentimento, terá 90 dias para realizar o workshop.

## <a name="next-steps"></a>Passos seguintes
[Apresentar uma reclamação de workshop](/partner-center/mci-engagements-workshop)

[Visão geral e elegibilidade dos compromissos do MCI](/partner-center/mci-engagements)

[Use estes recursos para ajudá-lo a começar com incentivos](/partner-center/incentives-get-started-intro)

[Determine a elegibilidade do seu programa de incentivos](/partner-center/incentives-determined-your-program-eligibility)

[Inscrição e gestão de utilizadores no programa de incentivos](/partner-center/incentives-enroll)