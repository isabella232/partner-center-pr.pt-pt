---
title: Unir a sua conta de parceiro com outra conta de parceiro
description: Saiba como fundir a sua conta de parceiro com outra conta de parceiro no Partner Center - para empresas que são parceiros ativos da Microsoft no Partner Center.
ms.topic: article
author: parthpandyaMSFT
ms.author: parthp
ms.custom: seodec18
ms.date: 06/12/2020
ms.openlocfilehash: 26912daeae6648d49d1fda3ee148d46c8a3d6705
ms.sourcegitcommit: b4771fd0781d95551e65baa481a572291c729d7d
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/28/2020
ms.locfileid: "92795836"
---
# <a name="merge-your-partner-account-with-another-partner-account"></a>Unir a sua conta de parceiro com outra conta de parceiro

**Funções aplicáveis**

- Administrador de conta

Duas ou mais empresas que são parceiros ativos da Microsoft e têm contas no Partner Center podem optar por fundir as suas contas.

## <a name="what-happens-when-two-partners-elect-to-merge-their-partner-center-accounts"></a>O que acontece quando dois parceiros escolhem fundir as suas contas do Partner Center

- A organização parceira que iniciar a fusão será a conta global partner (PGA).

- A PGA da organização convidada torna-se uma localização da empresa de iniciação.

- Todas as localizações da conta de fusão tornam-se localizações ao abrigo da PGA.

- Assim que a fusão da conta estiver concluída, verá os detalhes da conta, como localizações e utilizadores dentro do perfil PGA. Não pode inverter este processo.

- Todos os IDs MPN para locais são preservados durante esta consolidação.

- Os papéis dos utilizadores são trazidos. Por exemplo, se um utilizador tivesse sido o administrador de incentivos para uma localização específica, continuaria a ter esse papel após a fusão e a poder ver os incentivos que viu antes da fusão.

- Os inquilinos da AD Azure e as contas CSP não são fundidos e não têm qualquer impacto.

- As ofertas publicadas e os dados do pipeline associados a ambas as empresas são preservados

### <a name="view-of-merged-accounts"></a>Vista das contas fundidas

:::image type="content" source="images/merge-accounts/account-merge.png" alt-text="Fusão de conta":::

## <a name="what-to-expect-if-you-have-been-invited-to-merge-your-partner-center-account-with-another-partner-center-account"></a>O que esperar se foi convidado a fundir a sua conta partner Center com outra conta partner Center

Caso decida aceitar o convite para fundir contas: · Os seus ID(s) (s) e locais mpn serão fundidos na PGA da conta parceira que o convidou.

- Os seus utilizadores serão colocados na conta fundida com as suas funções intactas.

- Os benefícios e competências existentes serão preservados para ambas as empresas após a fusão até à renovação. Na renovação, as contas serão tratadas como uma empresa e as regras de renovação padrão serão aplicadas.

## <a name="understand-the-impacts-to-programs-and-benefits-when-partners-elect-to-merge-accounts"></a>Compreender os impactos para programas e benefícios quando os parceiros escolhem fundir contas

- Todas as competências existentes (Gold/Silver), compras (como o Microsoft Action Pack) e benefícios associados são preservados durante a consolidação. Se ambas as empresas tiverem a mesma competência, mas uma é de ouro e a outra de prata, a competência com maior nível de proficiência será atribuída, e os parceiros terão um conjunto de benefícios de prata e um conjunto de benefícios de ouro para essa competência até à sua próxima renovação. 

- A data de aniversário mais alta para o Microsoft Action Pack será mantida após a fusão. Por exemplo, se a data de aniversário da empresa 1 for junho de 2020 para a renovação do Action Pack e a data de aniversário para a renovação do Action Pack para a empresa 2 é outubro de 2020, a Microsoft usará a data de outubro de 2020 como a nova data de aniversário para a empresa fundida.

- Durante a fusão da conta e até à sua próxima renovação, cada conta manterá o seu Action Pack e/ou benefícios de competência. Na renovação, aplicam-se as regras padrão do Action Pack e das regras de renovação de competências.

- Após a renovação, os benefícios que são incluídos com a obtenção de competências e o Action Pack são implementados para a conta global parceira da empresa parceira:

  - Microsoft Action Pack: A empresa parceira poderá adquirir um Action Pack por conta global parceira.

  - Competência: A empresa parceira receberá um pacote de benefícios fundamentais, associados à sua maior realização, além de benefícios específicos de competência para o qual o parceiro é elegível para conta global por parceiro.

- Todos os benefícios estão sujeitos ao guia de utilização da [Rede de Parceiros](https://aka.ms/partner-benefits-use-guide)da Microsoft. Por exemplo: um token O365 E3 ativado está funcional durante doze (12) meses após a ativação. Uma vez que um token tenha sido ativado para licenças de um inquilino, essas licenças não podem ser transferidas para outro inquilino.

- As associações de ID MCP para ambas as empresas serão mantidas e associadas à ID MPN da PGA.

- Os benefícios técnicos e de mercado são oferecidos como benefício principal da competência. Após a fusão, recomenda-se que verifique o seu banco e informações fiscais para garantir a exatidão.

- Se a sua empresa estiver no programa Azure Expert MSP, os benefícios são retidos até à renovação.

- Se a sua empresa obteve especializações avançadas, estas são mantidas em ambas as contas.

- Quaisquer vouchers de garantia de software são mantidos em ambas as contas. 

## <a name="invite-a-company-to-merge-their-partner-center-account-with-your-partner-center-account"></a>Convide uma empresa a fundir a sua conta Partner Center com a sua conta Partner Center

>[!Note]
>Para realizar a fusão da conta, tem de ser o administrador da **Conta** da sua empresa.

1. Selecione **Definições** do painel partner center. 

2. Selecione **Fusão de Conta** .

3. Adicione o ID MPN localizado no **perfil partner** da conta que pretende convidar a fundir-se consigo. Deve usar o mpn global do parceiro deles. Não pode usar uma identificação de MPN de localização.

4. Quando seleciona **a Merge,** é enviado um convite para a empresa parceira. Quando aceitarem o seu pedido, pode iniciar a fusão da conta no Partner Center. Se a empresa rejeitar o seu pedido de fusão de contas, pode explicar por que rejeitaram o pedido. Uma lista de todas as suas combinações de conta está disponível para si ao abrigo **do histórico da Merge.**
 
### <a name="example-of-two-companies-merging-accounts"></a>Exemplo de duas empresas que fundem contas

1. Contoso tem 

    a. um [ID MPN global de 11111111](https://partner.microsoft.com/pcv/accountsettings/connectedpartnerprofile) e um [IDs MPN de localização subordinada de 2222222](https://partner.microsoft.com/pcv/accountsettings/locationsprofile).
  
    b. um inquilino AD AZure = @contoso.com
 
    c. uma competência de ouro que expira 1 de outubro de 2020
2. Fabricam tem
 
    a.  um ID MPN global de 3333333 e dois IDs MPN de localização subordinada de 44444444 e 555555

    b.  um inquilino da AAD = @fabricam.com

    c.  duas competências de ouro que expiram 1 de dezembro de 2020
3.  Contoso compra Fabricam e vai [aqui](https://partner.microsoft.com/dashboard/account/merger) para iniciar um pedido de fusão
4.  Fabricam assina no Partner Center e vai para a mesma página que Contoso fez em passo #3, para aprovar o pedido de Contoso.
5.  A Contoso revê os detalhes da fusão nessa mesma página e fornece confirmação para avançar com a fusão da conta.
    
## <a name="next-steps"></a>Passos seguintes

- [Assign users roles and permissions](permissions-overview.md) (Atribuir funções e permissões de utilizador)

- [Verifique as informações do perfil do seu parceiro](update-your-partner-profile.md)

- [Adicione serviços partilhados azure partner para que os parceiros possam comprar subscrições Azure para seu próprio uso](shared-services.md)
