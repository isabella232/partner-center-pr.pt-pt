---
title: Unir a sua conta de parceiro com outra conta de parceiro
description: Saiba como fundir a sua conta de parceiro com outra conta de parceiro no Partner Center - para empresas que são parceiros ativos da Microsoft no Partner Center.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-account
author: parthpandyaMSFT
ms.author: parthp
ms.custom: seodec18
ms.date: 06/12/2020
ms.openlocfilehash: 4b913754dd73f99e8aa363d257a9ac658d190b6a
ms.sourcegitcommit: fceaca54b0ec695cf214209c09b4516e1b40866a
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/23/2021
ms.locfileid: "128322004"
---
# <a name="merge-your-partner-account-with-another-partner-account"></a>Unir a sua conta de parceiro com outra conta de parceiro

**Funções adequadas**: Administrador de conta

Duas ou mais empresas que são parceiros ativos da Microsoft e têm contas no Partner Center podem optar por fundir as suas contas.

## <a name="what-happens-when-two-partners-elect-to-merge-their-partner-center-accounts"></a>O que acontece quando dois parceiros escolhem fundir as suas contas do Partner Center

- A organização parceira que inicia a fusão será a conta global partner (PGA).

- A PGA da organização convidada torna-se uma localização da empresa de iniciação.

- Todas as localizações da conta de fusão tornam-se localizações ao abrigo da PGA.

- Assim que a fusão da conta estiver concluída, verá os detalhes da conta, como localizações e utilizadores dentro do perfil PGA. Não pode inverter este processo.

- Todos os IDs MPN para locais são preservados durante esta consolidação.

- Os papéis dos utilizadores são trazidos. Por exemplo, se um utilizador tivesse sido o administrador de incentivos para uma localização específica, continuaria a ter esse papel após a fusão e a poder ver os incentivos que viu antes da fusão.

- Os inquilinos da AD Azure e as contas CSP não são fundidos e não têm efeito.

- As ofertas publicadas e os dados do pipeline associados a ambas as empresas são preservados

### <a name="view-of-merged-accounts"></a>Vista das contas fundidas

:::image type="content" source="images/merge-accounts/account-merge.png" alt-text="Fusão de contas.":::

## <a name="what-to-expect-if-you-have-been-invited-to-merge-your-partner-center-account-with-another-partner-center-account"></a>O que esperar se foi convidado a fundir a sua conta partner Center com outra conta do Partner Center

Caso decida aceitar o convite para fundir contas: · Os seus ID(s) (s) e locais mpn serão fundidos na PGA da conta parceira que o convidou.

- Os seus utilizadores serão colocados na conta resultante da fusão com as suas funções intactas.

- Os benefícios e competências existentes serão preservados para ambas as empresas após a fusão até à renovação. Na renovação, as contas serão tratadas como uma empresa e as regras de renovação padrão serão aplicadas.

## <a name="understand-the-impacts-to-programs-and-benefits-when-partners-elect-to-merge-accounts"></a>Compreender os impactos para programas e benefícios quando os parceiros escolhem fundir contas

- Todas as competências existentes (Gold/Silver), compras (como o Microsoft Action Pack) e benefícios associados são preservadas durante a consolidação. Se ambas as empresas tiverem a mesma competência, mas uma é de ouro e a outra de prata, a competência com o nível mais elevado de proficiência será atribuída, e os parceiros terão um conjunto de benefícios de prata e um conjunto de benefícios de ouro para essa competência até à sua próxima renovação. 

- A data de aniversário mais alta para o Microsoft Action Pack será mantida após a fusão. Por exemplo, se a data de aniversário da empresa 1 for junho de 2020 para a renovação do Action Pack e a data de aniversário para a renovação do Action Pack para a empresa 2 é outubro de 2020, a Microsoft usará a data de outubro de 2020 como a nova data de aniversário para a empresa fundida.

- Durante a fusão da conta e até à sua próxima renovação, cada conta manterá o seu Action Pack e/ou benefícios de competência. Na renovação, aplicam-se as regras padrão do Action Pack e das regras de renovação de competências.

- Após a renovação, os benefícios que são incluídos na obtenção de competências e o Action Pack são implementados para a conta global parceira da empresa parceira:

  - Microsoft Action Pack: A empresa parceira poderá adquirir um Action Pack por conta global de parceiros.

  - Competência: A empresa parceira receberá um pacote de benefícios fundamentais, associados à sua maior realização, além de benefícios específicos de competência para o qual o parceiro é elegível para uma conta global por parceiro.

- Todos os benefícios estão sujeitos ao guia de [utilização da Rede de Parceiros](https://partner.microsoft.com/dashboard/account/merger)da Microsoft. Por exemplo: um token O365 E3 ativado está funcional durante 12 meses após a ativação. Uma vez que um token tenha sido ativado para licenças de um inquilino, essas licenças não podem ser transferidas para outro inquilino.

- As associações de ID MCP para ambas as empresas serão mantidas e associadas à ID MPN da PGA.

- Os benefícios técnicos e de mercado são oferecidos como benefício principal da competência. Após a fusão, recomenda-se que verifique o seu banco e informações fiscais para garantir a exatidão.

- Se a sua empresa estiver no programa Azure Expert MSP, os benefícios são retidos até à renovação.

- Se a sua empresa obteve especializações avançadas, estas são mantidas em ambas as contas.

- Quaisquer vouchers de garantia de software são mantidos em ambas as contas. 

- Não há efeito para a DPOR ou associação PAL. Quaisquer contribuições de receitas associadas começarão a fluir para a nova Conta Global de Parceiros

## <a name="invite-a-company-to-merge-their-partner-center-account-with-your-partner-center-account"></a>Convide uma empresa para fundir a sua conta Partner Center com a sua conta Partner Center

>[!Note]
>Para realizar a fusão da conta, tem de ser o administrador da **Conta** da sua empresa.

1. Selecione **Definições** no painel de instrumentos do Centro de Parceiros. 

2. Selecione **Fusão de Conta**.

3. Adicione o ID MPN localizado no **perfil partner** da conta que pretende convidar para se fundir consigo. Deve usar o mpn global do parceiro deles. Não pode usar uma identificação de MPN de localização.

4. Quando seleciona **a Merge,** é enviado um convite para a empresa parceira. Quando aceitarem o seu pedido, pode iniciar a fusão da conta no Partner Center. Se a empresa rejeitar o seu pedido de fusão de contas, pode explicar por que rejeitaram o pedido. Uma lista de todas as suas combinações de conta está disponível para si no histórico **da Fusão.**
 
### <a name="example-of-two-companies-merging-accounts"></a>Exemplo de duas empresas que fundem contas

1. Contoso, Ltd. 

    a. um [ID MPN global de 1111111](https://partner.microsoft.com/pcv/accountsettings/connectedpartnerprofile) e um [ID de MPN de localização](https://partner.microsoft.com/pcv/accountsettings/locationsprofile)subordinada de 2222222 .
  
    b. um inquilino AD AZure = @contoso.com
 
    c. uma competência de ouro que expira 1 de outubro de 2020
2. Fabrikam, Inc.
 
    a. um ID MPN global de 3333333 e dois IDs MPN de localização subordinada de 4444444 e 5555555

    b.  um inquilino AD AZure = @fabrikam.com

    c.  duas competências de ouro que expiram 1 de dezembro de 2020
3.  Contoso compra Fabrikam e vai ao [Partner Center](https://partner.microsoft.com/dashboard/account/merger) para iniciar um pedido de fusão.
4.  Fabrikam assina no Partner Center e vai para a mesma página que Contoso fez em passo #3, para aprovar o pedido de Contoso.
5.  A Contoso revê os detalhes da fusão nessa mesma página e fornece confirmação para avançar com a fusão da conta.
6.  Após a fusão, a conta da empresa apresentará como:

    a.  Uma empresa chamada Contoso com um ID MPN global de 1111111 e 4 IDs MPN de localização subordinada de 2222222, 3333333, 4444444 e 5555555
    
    b.  Terá dois inquilinos da AD Azure ( @contoso.com @fabrikam.com +) que têm acesso à mesma conta partner Center
    
    c.  Terá dois pacotes de benefícios de competência, um que expira a 1 de outubro de 2020 e outro que expira a 1 de dezembro de 2020. Poderão renovar-se como um único pacote de benefícios de competência a 1 de dezembro de 2020. Quando renovarem, a Contoso manterá as três competências, embora só possam manter um pacote de benefícios únicos.
    
7.  Os administradores da Contoso continuarão a gerir as funções do Partner Center para @contoso.com os utilizadores. Os administradores da Fabrikam continuarão a gerir as funções do Partner Center para @fabrikam.com os utilizadores. Os administradores de Contoso só podem administrar os utilizadores de Fabrikam se forem convidados como convidados para o inquilino de Fabrikam.
8.  Contoso poderia decidir ignorar o @fabrikam.com inquilino, e reeditar os empregados da Fabrikam novas @contoso.com credenciais com novos papéis e permissões.

## <a name="next-steps"></a>Passos seguintes

- [Assign users roles and permissions](permissions-overview.md) (Atribuir funções e permissões de utilizador)

- [Verifique as informações do perfil do seu parceiro](update-your-partner-profile.md)

- [Adicione serviços partilhados a azure partner para que os parceiros possam comprar subscrições Azure para seu próprio uso](shared-services.md)
