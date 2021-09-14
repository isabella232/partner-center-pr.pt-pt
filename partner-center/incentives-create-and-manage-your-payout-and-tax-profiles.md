---
title: Perfis fiscais e de pagamento no Centro de Parceiros
ms.topic: how-to
ms.date: 04/15/2021
description: Crie e gere o seu perfil de pagamento e impostos para que possa ser pago pelos seus incentivos. Inclui criar, gerir e usar perfis diferentes.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.openlocfilehash: a6d578c2ad09e1f8bb03f520d659f1a9b1e199a9
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/13/2021
ms.locfileid: "126248122"
---
# <a name="create-and-manage-incentives-payout-and-tax-profiles-in-partner-center"></a>Criar e gerir incentivos no pagamento e perfis fiscais no Partner Center

**Funções adequadas**: Incentivos administrativos | Administração de contas | Administração global

Para receber o pagamento pelos seus programas de incentivos para uma determinada localização MPN, tem de completar a inscrição ao associar um perfil de pagamento e perfil fiscal válido ao programa e à localização MPN. A Microsoft utilizará este perfil de pagamento e perfil fiscal para emitir os pagamentos. Poderá ser permitida a utilização de transferências bancárias eletrónicas ou de notas de crédito para efeitos de pagamento, dependendo das regras do programa de incentivos. 

## <a name="roles-currencies-and-multiple-microsoft-incentive-programs"></a>Funções, moedas e vários programas de incentivo da Microsoft

É importante entender a informação abaixo antes de começar com o seu pagamento e perfil fiscal.

### <a name="roles-and-permissions"></a>Funções e permissões

Você deve ser um Incentivo Admin para inserir informação bancária e fiscal para pagamentos de incentivos. Se for um ADMINISTRADOR MPN/Conta, pode atribuir-se a si próprio e/ou a um colega para ser o Administrador de Incentivos.

Se precisar de solicitar permissões de Administração de Incentivos, contacte o seu MPN Admin ou a Global Admin. Pode descobrir quem na sua empresa tem estas funções ao inscrever-se no [painel de instrumentos](https://partner.microsoft.com/dashboard/)do Partner Center. A partir do ícone **Definições** no topo direito, selecione **Gestão do Utilizador** e, em seguida, filtre no Global Admin.

Incentivos Os utilizadores podem ver os ganhos de incentivo e os detalhes e relatórios de pagamento, mas não podem editar detalhes bancários e fiscais.

### <a name="choose-your-disbursement-currency"></a>Escolha a sua moeda de desembolso

Os pagamentos de incentivos são feitos na moeda que selecionou quando configura o seu perfil de pagamento. Os pagamentos serão calculados usando uma taxa de câmbio definida mensalmente pela Microsoft. Será responsável por quaisquer alterações de valor devido à moeda selecionada.

### <a name="using-different-profiles-for-different-microsoft-programs"></a>Usando diferentes perfis para diferentes programas da Microsoft

Se a sua empresa estiver matriculada em vários programas de incentivo, pode utilizar a mesma conta de pagamento para todos eles, ou optar por utilizar diferentes contas de pagamento para diferentes programas.

## <a name="create-and-manage-payout-and-tax-profiles-in-partner-center"></a>Criar e gerir perfis de pagamento e impostos no Partner Center

As secções abaixo irão acompanhar-te através do processo de criação e gestão de perfis de pagamento e impostos no Partner Center.

>[!IMPORTANT]
>Você deve ser um administrador de incentivo para criar ou gerir perfis de pagamento e impostos no Partner Center. As funções de incentivo devem ser atribuídas a cada localização MPN ao abrigo de cada programa de incentivo. Para obter mais informações sobre como adicionar administradores de incentivo no Partner Center, consulte [Criar contas de utilizador](create-user-accounts-and-set-permissions.md).

## <a name="access-the-payout-and-tax-section-in-partner-center"></a>Aceda à secção de pagamentos e impostos no Partner Center

1. Inscreva-se no painel de [instrumentos](https://partner.microsoft.com/dashboard/) do Partner Center utilizando a sua conta de Azure Ative Directory (Azure AD) (conta da empresa) ou o endereço de e-mail apropriado se um for atribuído.

   - Vários domínios podem ser registados dentro de uma conta AD Azure. Contacte o seu administrador Global para determinar quais os domínios associados.
   - Se só conseguir iniciar scontabilidade com o @onmicrosoft.com domínio e precisar de domínios adicionais, contacte o administrador da conta para adicionar domínios adicionais à conta Azure AD.
   - Se lhe for solicitado que selecione **conta de trabalho ou escola** ou conta **pessoal,** selecione **Trabalho ou conta escolar**.

2. Selecione o ícone de engrenagem para abrir o menu **Definições** e, em seguida, selecione **as definições de Conta**.

3. No menu **de definições de conta,** selecione **Payout e tax**.

## <a name="assign-payout-and-tax-profiles-to-individual-programs"></a>Atribuir perfis de pagamento e impostos a programas individuais

1. Inscreva-se no [painel partner center](https://partner.microsoft.com/dashboard/)e, em seguida, selecione o ícone de engrenagem para abrir o menu **Definições.** 

2. Selecione **as definições de Conta,** expanda a **secção de Pagamento e Imposto**, e, em seguida, selecione Payout e tax profile **assignment**. 
   
   Será apresentada uma lista dos seus programas. Selecione a seta ao lado de um programa para ver os detalhes do perfil. 

3. No menu de entrega **do Perfil Fiscal,** selecione o perfil de imposto que deseja ou selecione a opção para criar um novo perfil. Quando selecionar a opção para criar um novo perfil, será redirecionado adequadamente.  **Selecione Continue** na janela pop-up. O processo de criação de um novo perfil fiscal é fornecido abaixo.

4. Selecione **o método de pagamento**.

   - Se selecionou **a transferência bancária electrónica** como método de pagamento, selecione o perfil de pagamento que pretende ou selecione a opção de criar um novo perfil. Quando selecionar a opção para criar um novo perfil, será redirecionado adequadamente. Selecione Continue na janela pop-up. O processo de criação de um novo perfil de pagamento foi fornecido abaixo.

   - Se tiver selecionado **a Nota de Crédito** como método de pagamento, então complete a verificação. Isto confirma que o número SAP referenciado pertence à sua organização.

    >[!NOTE]
    >Se houver várias entidades empresariais da Microsoft listadas, deve selecionar um perfil de pagamento para cada entidade.

    >[!NOTE]
    >A disponibilidade do método de pagamento depende das regras do programa de incentivos.

    - Se a sua localização MPN ID for paga por uma subsidiária local da Microsoft por um determinado programa de incentivos e permitir a nota de crédito LRD (distribuidor de risco limitado) como método de pagamento, então o seu perfil de pagamento será pré-povoado com o método de pagamento LRD Credit Note. Na linha de método de pagamento de nota de crédito LRD para o respetivo programa de incentivos e localização MPN ID, verá **Confirmado** ou **Verificação Necessário** como o estado na secção de perfil de pagamento.
    
       **Selecione Verificação necessária** para confirmar e verificar os detalhes de identificação do inquilino CSP que estão associados à localização MPN e método de pagamento para receber o pagamento da nota de crédito. Na caixa de diálogo Detalhes de **Nota de Crédito,** reveja e verifique se o ID do Inquilino CSP e os dados fornecidos estão corretos. Se lhe for apresentado mais do que um ID de inquilino, selecione cuidadosamente o ID do inquilino do CSP no qual deseja receber pagamentos. Em seguida, **selecione Confirme** para reconhecer que os detalhes da sua empresa estão corretos, e que o pagamento de incentivo deve ser feito para o ID do inquilino CSP que você selecionou.
 
      Se o estado mostrar **confirmado,** a atribuição do ID do inquilino da CSP foi concluída e não é necessária qualquer outra ação. Pode ainda selecionar Confirmado para ver os detalhes da atribuição.
   
      Nos países que exigem explicitamente aos parceiros o pedido de aplicação de uma isenção fiscal, haverá a opção de aplicar a isenção fiscal junto ao perfil fiscal na secção de perfil fiscal do programa de incentivos e localização MPN. A verificação desta caixa aplicará benefícios de isenção fiscal à sua nota de crédito de incentivo. 
   
      Atualmente, o método de pagamento LRD Credit Note está disponível apenas para parceiros austrália, Nova Zelândia e Canadá para o programa de incentivo ao comércio microsoft. Se você é um parceiro de conta direta ou fornecedor indireto nestes três países inscritos para o programa MCI e você não vê a nota de crédito LRD como o método de pagamento disponível, então confirme que o seu ID do inquilino está associado com a conta de localização mpn do parceiro relevante. Para mais informações sobre isto, leia [como atualizar o seu perfil de organização.](update-your-partner-profile.md)

    
5. Selecione a **Moeda**.

6. Quando tiver concluído todos os campos de pagamento, **selecione Enviar por isso.**

## <a name="set-up-a-default-bank-profile"></a>Configurar um perfil bancário predefinido

Pode configurar perfis bancários predefinidos e atribuí-los a localizações do MPN. Estes perfis predefinidos serão utilizados pela Microsoft para posteriores inscrições para essa localização do MPN. 

1. Inscreva-se no [painel partner center](https://partner.microsoft.com/dashboard/)e, em seguida, selecione o ícone de engrenagem para abrir o menu **Definições.**   

2. Selecione **as definições de Conta,** expanda a secção **de Pagamento e Imposto** e, em seguida, selecione Payout e tax **profiles**. 

3. **Selecione Gerir os perfis predefinidos** na secção perfis de **pagamento.** 

4. Para criar um perfil bancário predefinido, **selecione Adicionar um perfil bancário predefinido**. 

5. Selecione um perfil bancário da lista de perfis bancários disponíveis da sua empresa, selecione a moeda a utilizar com este perfil bancário e, em seguida, selecione a lista de localizações mpn para as quais pretende que este perfil predefinido se aplique.

6. Selecione **Feito** uma vez concluídas as seleções. O botão Done não será clicável até que todos os campos necessários estejam concluídos. 

>[!NOTE]
>O mesmo banco e emparelhamento de moedas pode ser aplicado em vários locais. Se a localização MPN tiver sido atribuída uma combinação de perfil padrão e moeda uma vez, deixará de aparecer na localização para futuras atribuições de perfil predefinido. Se a seleção predefinida for eliminada, a localização MPN reaparecerá para futuras atribuições de perfil predefinido. Cada perfil bancário e combinação de moedas é adicionado como uma linha única e editável.

7. Uma vez adicionadas todas as alterações necessárias, **selecione Save**.  

## <a name="create-your-bank-profile"></a>Crie o seu perfil bancário

Os perfis bancários são criados a nível da empresa. Isto permite que um perfil bancário seja atribuído em vários programas de ID e incentivos de MPN dentro de uma empresa. Pode haver exceções na aplicação do perfil bancário a diferentes países, uma vez que podem ser aplicadas diferentes regras bancárias e fiscais.

>[!NOTE]
>Nas páginas seguintes, são necessários campos com asterisco. Se não sabe o que é um campo, selecione o ícone da informação. 

1. Na página **Detalhes,** preencha os seguintes campos: **Nome do perfil:** Introduza um nome único para identificar este perfil de pagamento.
    **Localização da conta bancária:** O país onde está localizado o banco da sua empresa.
    **Método de pagamento:** O método de pagamento preferido para o Partner Center é a transferência bancária electrónica.

2. Selecione **Seguinte**.

3. Na página da **conta Do Banco,** insira a sua informação. Os campos mostrados nesta página variam de país para país. 

4. Selecione **Seguinte**.

5. Na página **do Beneficiário,** insira as informações apropriadas. O beneficiário é a pessoa na sua empresa que o banco entraria em contacto se precisasse de discutir a sua conta.

6. Quando os campos estiverem concluídos, selecione **Terminar** e, em seguida, selecione **Confirmar** para criar o seu perfil bancário.

Será redirecionado para a página **de pagamentos e perfis fiscais.** O estado do seu novo perfil refletirá **a validação pendente** da Microsoft até que a validação esteja concluída. Este processo pode demorar até 48 horas. Uma vez concluída a validação, o seu estado de perfil refletirá quer **aprovado** quer **ação necessária**. Se **for necessário** agir, repita os passos acima, fornecendo as informações necessárias. 

## <a name="create-your-tax-profile"></a>Crie o seu perfil fiscal

Utilize o seguinte procedimento para fornecer à Microsoft as informações fiscais necessárias para a sua organização. As páginas desta secção são dinâmicas e variam de acordo com o seu país ou região. Se precisar de ajuda para identificar as informações fiscais corretas, contacte as fontes governamentais apropriadas no seu país.

Para empresas parceiras nas Américas, se necessitar de informações sobre o preenchimento dos formulários W8 ou W9, os seguintes endereços levam-no ao site do IRS:

- [http://www.irs.gov/pub/irs-pdf/iw8.pdf](http://www.irs.gov/pub/irs-pdf/iw8.pdf)
- [http://www.irs.gov/pub/irs-pdf/iw9.pdf](http://www.irs.gov/pub/irs-pdf/iw9.pdf)

>[!IMPORTANT]
> Insira apenas detalhes para a sua empresa. Nunca introduza detalhes pessoais.

1. Na página **'Perfil de** Negócios', preencha os campos necessários e, em seguida, selecione **Seguinte**. 

2. Na página **Configuração,** selecione a opção que se aplica à sua empresa.

   - Selecione a opção à esquerda se a sua empresa for incorporada apenas nos Estados Unidos, ou se este perfil for para um indivíduo.
   - Selecione a opção à direita se a sua empresa estiver incorporada fora dos Estados Unidos e, em seguida, selecione o seu país/região da lista.

3. Selecione **Seguinte**. 

4. Na página de estado do **Imposto,** insira as informações necessárias e, em seguida, selecione **Seguinte**. Os campos nesta página variam por país. seus detalhes. 

5. Na página **de documentação adicional,** os campos necessários e selecione **Seguinte**. 

6. **Selecione Procurar** para carregar quaisquer documentos necessários pelo seu país ou região. Quando o nome do documento for mostrado, selecione **Upload**. 

7. Se precisar de remover o documento, selecione **Remover**.

8. Para guardar e continuar, **selecione Terminar**.

9. **Selecione Confirme** na mensagem pop-up. Você será levado de volta para a página **de pagamento e configuração de impostos.**
 
## <a name="update-expired-tax-profiles"></a>Atualizar perfis de impostos caducados

1. Inscreva-se no [painel partner center](https://partner.microsoft.com/dashboard/)e, em seguida, selecione o ícone de engrenagem para abrir o menu **Definições.**

1. Selecione **as definições de Conta,** expanda a secção **de Pagamento e Imposto** e, em seguida, selecione Payout e tax **profile**.

1. Selecione **perfil fiscal**.

1. Verifique a **data de validade** da coluna e navegue para o perfil fiscal que está caducado ou prestes a expirar.

1. Selecione **Editar**.

1. Na secção de formulário fiscal, atualize os formulários fiscais fornecendo os novos detalhes. 

## <a name="next-steps"></a>Passos seguintes

- [Questões comuns sobre pagamentos e impostos](payout-faq.yml)
