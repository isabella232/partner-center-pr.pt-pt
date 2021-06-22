---
title: Verifique o perfil da empresa
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como verificar os detalhes da sua empresa, como contacto primário, endereço e informações do programa. Também pode atualizar os seus endereços legais e de faturação.
author: parthpandyaMSFT
ms.author: parthp
ms.topic: how-to
ms.date: 04/12/2021
ms.localizationpriority: medium
ms.custom: contperf-fy21q4
ms.openlocfilehash: 49f5e30df241c8a29c3282c1958b39ebd9add36e
ms.sourcegitcommit: bce54ddb9fff7332a03d6aa228ba9414a87d76b7
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/22/2021
ms.locfileid: "112431730"
---
# <a name="verify-or-update-your-company-profile-information"></a>Verifique ou atualize as informações do perfil da empresa 

**Funções adequadas**: Administração global | Administrador de conta MPN

A primeira vez que assinar no Partner Center como administrador global, deverá confirmar que todos os detalhes da sua empresa estão corretos. Estes incluem contacto primário, nome e endereço de negócios legais e informações do programa. Se a sua empresa tiver mais de uma localização, reveja os seus dados de localização para obter uma precisão. Como administrador global, administrador billing ou agente de administração, também poderá ver e atualizar a sua faturação e informações fiscais.

O seu perfil de parceiro consiste na informação de negócios legal, nome de contacto primário e e-mail, nos programas em que a sua empresa participa e, se relevante, das suas outras empresas que estão agora fundidas no âmbito do seu negócio legal. Certifique-se de que o nome e endereço da Empresa no seu perfil de negócio legal estão isentos de erros ortográficos e abreviaturas, e corresponda exatamente aos seus registos formais de registo comercial da empresa. Se estiver a operar como proprietário único, tem de usar o nome da sua empresa como nome legal.


## <a name="locate-the-legal-business-profile"></a>Localize o perfil de negócio legal

1. No Partner Center, selecione o ícone **Definições** e, em seguida, selecione **as definições de Conta**.
 
1. Selecione **perfil de Organização**. 

2. Reveja os valores do **perfil de negócio legal,** **informações de contato primários** e **informações do Programa.**

Se fundiu as suas outras empresas no âmbito do seu negócio legal, também pode rever essa informação. 

## <a name="update-your-legal-business-profile"></a>Atualize o seu perfil de negócio legal 

Atualize o nome ou endereço da sua empresa legal no Partner Center.

>[!Important]
>- Para as contas da Microsoft Partner Network (MPN), tanto o administrador global como o administrador de conta podem atualizar o nome da empresa legal.
>- Para as contas de revendedor indiretos Cloud Solution Provider (CSP), apenas o administrador Global pode atualizar o nome da empresa legal. 
>- Os sócios de contas diretas e os fornecedores indiretos não podem alterar o nome legal da sua empresa se o estado de verificação da conta for **autorizado.** Se precisar de alterar o nome, tem de criar um [bilhete De Apoio.](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=eb74583c-61b3-2124-bffc-00920e0ae772)



1. No Partner Center, selecione **Definições**, selecione **definições de Conta** e, em seguida, selecione **o perfil da Organização**.

2. Selecione **Legal** e, em seguida, selecione o perfil de negócio legal (Parceiro ou Revendedor) que pretende atualizar.

1. Selecione **Update** ao lado do nome/endereço da empresa e altere os detalhes.
 
1. Quando selecionar **Enviar por ela,** a sua identidade legal será reavaliada. Reavaliamos apenas o que mudou.

1. Se a verificação falhar, aprenda a [corrigir o problema](verification-responses.md).

>[!Important]
>Se é sócio da CSP, não pode mudar o país associado à sua morada legal. O seu país de endereço legal está ligado ao seu inquilino e serviços, bem como à moeda com que negoceia. Para saber mais sobre as atualizações do país da MPN, leia  [as atualizações do país da MPN](manage-locations.md#change-country-of-partner-global-account).


### <a name="who-can-update-legal-business-name-and-when"></a>Quem pode atualizar o nome legal do negócio e quando

|**Programa**|**Quem pode atualizar o nome da empresa**|**Quando (estado) pode ser atualizado**|**Permitido**|
|---------------------|:-------------------------------|:------------|:-----------------|
MPN|Administração global; Administrador de conta|Autorizado; pendente; rejeitado| Permitido|
|CSP: Revendedor indireto|Administrador global|Autorizado; pendente; rejeitado| Permitido|


## <a name="update-your-mpn-global-business-account"></a>Atualize a sua Conta Global de Negócios MPN

Durante a sua migração do Partner Membership Center para Partner Center, se a conta de negócios errada foi identificada como o negócio legal, pode alterá-la para a conta de negócios legal correta.

Para então fazer estas atualizações, você precisa ser o administrador global ou administrador de conta. Saiba como [gerir as suas contas de localização MPN Global](manage-locations.md)


## <a name="update-your-mpn-id-associated-with-your-csp-account"></a>Atualizar o seu ID da MPN associado à sua conta do CSP

Para atualizar o ID MPN associado à sua conta CSP:

1. Inscreva-se no [painel de instrumentos](https://partner.microsoft.com/dashboard/home) do Partner Center como administrador global com as suas credenciais de conta CSP e, em seguida, selecione **Definições**. (As suas credenciais MPN e CSP podem ser diferentes.)
 
1. Selecione **identificadores** a partir das **definições** de Conta .

1. Na secção **CSP,** utilize o link **'Atualização'** para atualizar o ID MPN associado à sua Conta CSP 


## <a name="update-your-csp-legal-billing-address"></a>Atualize o seu endereço de faturação legal CSP

Se você é o administrador global, administrador de faturação ou agente administrativo, pode alterar o endereço que aparece na sua fatura no seu **perfil de pagamento e imposto**. No entanto, não poderá alterar o nome da empresa na fatura devido a uma limitação do sistema de faturas.

:::image type="content" source="images/billing-profile.png" alt-text="Captura de ecrã da área onde a informação de faturação é adicionada.":::

|**Campo**  |**Descrição**|  
|---------------------|:------------------|
|Nome da Empresa Bill-to|O nome da empresa que aparece na Bill-To informação na sua fatura CSP.  Isto não é editável no Centro parceiro.  Para atualizar, crie um bilhete de apoio.|
|Endereço Bill-to|O endereço bill-to mostrado na fatura da CSP. Pode ser atualizado a partir do [perfil de Billing.](https://partner.microsoft.com/dashboard/account/v3/accountsettings/billingprofile#commercial)|
|Contato Bill-to|Os dados de contacto de faturação (nome próprio, apelido, número primário) para a conta CSP.  Pode ser atualizado a partir do [perfil de Billing.](https://partner.microsoft.com/dashboard/account/v3/accountsettings/billingprofile#commercial)|
|Número de PO|O número da Ordem de Compra apresentada na fatura do parceiro. Pode ser atualizado a partir do [perfil de Billing.](https://partner.microsoft.com/dashboard/account/v3/accountsettings/billingprofile#commercial)|
|ID do imposto da empresa|As empresas de alguns países podem fornecer o seu [número de imposto sobre o valor acrescentado (IVA) ou equivalente local.](./organization-tax-info.md) Para atualizar o seu NIF, tem de ser administrador Global, administrador de faturação ou agente de administração.|
|Moeda de Faturação|A moeda de faturação da sua conta CSP é determinada pelo país legal da conta CSP.  Isto não pode ser alterado uma vez que a conta CSP é criada.|

## <a name="next-steps"></a>Passos seguintes

- [Verifique o seu estado de verificação](verification-responses.md)

- [Gerir localizações de MPN](manage-locations.md)