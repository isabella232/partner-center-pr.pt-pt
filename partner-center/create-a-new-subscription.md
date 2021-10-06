---
title: Criar subscrições de clientes no Partner Center
ms.topic: how-to
ms.date: 09/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: Saiba como vender subscrições aos seus clientes para produtos publicados pela Microsoft, bem como produtos SaaS publicados por ISVs de terceiros.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: c42e2e8dbc98bdf9ed0e2994bfb7ad49848aad76
ms.sourcegitcommit: b78e85a0bc62e3536b067417cb3db7899cda4f97
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/06/2021
ms.locfileid: "129565336"
---
# <a name="manage-customer-subscriptions"></a>Gerir subscrições de clientes

**Aplica-se a**: Partner Center | Centro de Parceiros para Microsoft Cloud for US Government

**Funções adequadas**: Agente administrador | Administrador de faturação | | de administração global Agente helpdesk | Agente comercial

Depois de ter criado um registo do seu cliente no Partner Center, pode vendê-los subscrições a produtos do catálogo. Isto inclui produtos publicados pela Microsoft e software como um serviço (SaaS) produtos publicados por fornecedores de software independentes de terceiros (ISVs) para o [mercado comercial.](https://azuremarketplace.microsoft.com/marketplace)

Algumas ofertas são limitadas a uma subscrição por cliente. Para ver uma lista das ofertas restritas, visite a página de **listas de preços** do Centro parceiro.

> [!IMPORTANT]
> Como parceiro no programa CSP, pode adquirir assinaturas SaaS **baseadas em licenças** ou **medidos** a editores da ISV dentro do Partner Center. Isto significa que pode comprar qualquer oferta SaaS **baseada em licença** ou **medido** que o editor ISV lhe tenha disponibilizado, incluindo [ofertas exclusivas](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) às quais tem acesso. Para comprar ou gerir outras ofertas comerciais de marketplace a partir de ISVs (como ofertas baseadas em uso envolvendo aplicações Azure, Contentores ou VMs), você deve ir ao [portal Azure.](https://portal.azure.com/)

> [!NOTE]
> Todas as datas e horários no Partner Center são dadas na norma de tempo coordenada (UTC) do tempo universal. Isto pode diferir até 24 horas a partir da sua hora local.

## <a name="create-a-new-subscription"></a>Criar uma nova subscrição

> [!NOTE]
> Para saber mais sobre a interface de espaços de trabalho, consulte [o Centro de Parceiros.](get-around-partner-center.md#turn-workspaces-on-and-off)

#### <a name="workspaces-view"></a>[Vista de espaços de trabalho](#tab/workspaces-view)

1. A partir do [painel Partner Center](https://partner.microsoft.com/dashboard), selecione o azulejo **cliente** e, em seguida, selecione o cliente da lista de Clientes.

2. Selecione **Adicionar subscrição**. O separador **Serviços Online** mostrará todas as ofertas disponíveis do Marketplace SaaS.

3. Para ver apenas certos tipos de subscrições, faça seleções nos filtros disponíveis:
   - **Publisher**: Escolha a **Microsoft** para ver apenas ofertas da Microsoft ou **Partner** para ver produtos de marketplace comercial publicados pelos ISVs.
   - **Tipo de faturação**: Selecione o tipo de faturação de subscrição que pretende utilizar: **Licença** ou **Utilização**. Consulte [a faturação baseada em licença](license-based-billing.md) para obter informações que o ajudarão a decidir entre a frequência de faturação mensal e anual.
   - **Categoria**: Escolha **Empresa,** **Pequenas empresas,** ou **Trial.** Para obter informações sobre subscrições de teste, consulte [Oferecer aos seus clientes testes de produtos microsoft.](offer-your-customers-trials-of-microsoft-products.md)

4. Selecione as subscrições de produto que pretende comprar para o seu cliente. Os produtos que vê dependem do tipo de segmento de cliente (educação, governo, etc.) e dos filtros que aplicou. Algumas ofertas apresentadas no Mercado podem nem sempre estar disponíveis para um cliente específico ou um parceiro CSP específico. Isto pode ser porque:
   - O cliente já tem uma subscrição desse produto e só é permitido um
   - A subscrição do cliente pode ter sido suspensa (Neste caso, pode reativar a subscrição em vez de comprar uma nova.)
   - Para as ofertas isv SaaS, pode haver algumas razões pelas quais a oferta não está disponível para compra: O ISV não pode suportar o país ou região de faturação do cliente; o ISV pode ter optado por não disponibilizar a oferta através do programa CSP; ou, o ISV pode ter feito a oferta [exclusiva](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) a apenas certos parceiros CSP. A oferta ISV também pode não ser transacionável através do Centro de Parceiros (por exemplo, contentores ou algumas ofertas baseadas em uso).  

5. Para cada subscrição que pretende adicionar, introduza o número de licenças (se necessário) e selecione **Adicionar ao carrinho**.

6. Quando terminar de adicionar subscrições, selecione **Rever** e rever a sua encomenda.

7. Uma vez revisto as suas encomendas e pronto para comprar estas subscrições, selecione **Comprar**.

8. Depois de comprar uma subscrição para um cliente, ocorrerá o seguinte:

    - Pode rever ou editar a subscrição selecionando o nome de subscrição na página de **Subscrições** desse cliente. A partir daqui, pode selecionar licenças adicionais se alguma estiver disponível, alterar a quantidade de licenças ou suspender a subscrição.

    **Para assinaturas ISV SaaS (baseadas em licenças e contadores):**
    - Receberá um link para o site da editora ISV. Este link deve ajudá-lo a completar a implementação ou a configuração da conta da subscrição do cliente.

    > [!NOTE]
    > Nem você nem o seu cliente receberão um e-mail com instruções para completar a configuração/provisionamento da conta para este tipo de subscrição ISV.)

    - Se a sua subscrição vier com um teste gratuito de 30 dias, o período experimental gratuito será aplicado automaticamente. Como parceiro no programa CSP, não pode renunciar ao período experimental gratuito nas ofertas que compra para os clientes. Uma vez terminada a duração do período experimental gratuito, o prazo de subscrição começará e a subscrição converter-se-á em estatuto pago. A subscrição irá então renovar automaticamente de acordo com o mesmo horário.

#### <a name="current-view"></a>[Vista atual](#tab/current-view)

1. A partir do [painel de instrumentos Partner Center](https://partner.microsoft.com/dashboard), selecione **Clientes,** em seguida, selecione o cliente da lista de Clientes.

2. Selecione **Adicionar subscrição**. O separador **Serviços Online** mostrará todas as ofertas disponíveis do Marketplace SaaS.

3. Para ver apenas certos tipos de subscrições, faça seleções nos filtros disponíveis:
   - **Publisher**: Escolha a **Microsoft** para ver apenas ofertas da Microsoft ou **Partner** para ver produtos de marketplace comercial publicados pelos ISVs.
   - **Tipo de faturação**: Selecione o tipo de faturação de subscrição que pretende utilizar: **Licença** ou **Utilização**. Consulte [a faturação baseada em licença](license-based-billing.md) para obter informações que o ajudarão a decidir entre a frequência de faturação mensal e anual.
   - **Categoria**: Escolha **Empresa,** **Pequenas empresas,** ou **Trial.** Para obter informações sobre subscrições de teste, consulte [Oferecer aos seus clientes testes de produtos microsoft.](offer-your-customers-trials-of-microsoft-products.md)

4. Selecione as subscrições de produto que pretende comprar para o seu cliente. Os produtos que vê dependem do tipo de segmento de cliente (educação, governo, etc.) e dos filtros que aplicou. Algumas ofertas apresentadas no Mercado podem nem sempre estar disponíveis para um cliente específico ou um parceiro CSP específico. Isto pode ser porque:
   - O cliente já tem uma subscrição desse produto e só é permitido um
   - A subscrição do cliente pode ter sido suspensa (Neste caso, pode reativar a subscrição em vez de comprar uma nova.)
   - Para as ofertas isv SaaS, pode haver algumas razões pelas quais a oferta não está disponível para compra: O ISV não pode suportar o país ou região de faturação do cliente; o ISV pode ter optado por não disponibilizar a oferta através do programa CSP; ou, o ISV pode ter feito a oferta [exclusiva](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) a apenas certos parceiros CSP. A oferta ISV também pode não ser transacionável através do Centro de Parceiros (por exemplo, contentores ou algumas ofertas baseadas em uso).  

5. Para cada subscrição que pretende adicionar, introduza o número de licenças (se necessário) e selecione **Adicionar ao carrinho**.

6. Quando terminar de adicionar subscrições, selecione **Rever** e rever a sua encomenda.

7. Uma vez revisto as suas encomendas e pronto para comprar estas subscrições, selecione **Comprar**.

8. Depois de comprar uma subscrição para um cliente, ocorrerá o seguinte:

    - Pode rever ou editar a subscrição selecionando o nome de subscrição na página de **Subscrições** desse cliente. A partir daqui, pode selecionar licenças adicionais se alguma estiver disponível, alterar a quantidade de licenças ou suspender a subscrição.

    **Para assinaturas ISV SaaS (baseadas em licenças e contadores):**
    - Receberá um link para o site da editora ISV. Este link deve ajudá-lo a completar a implementação ou a configuração da conta da subscrição do cliente.

    > [!NOTE]
    > Nem você nem o seu cliente receberão um e-mail com instruções para completar a configuração/provisionamento da conta para este tipo de subscrição ISV.)

    - Se a sua subscrição vier com um teste gratuito de 30 dias, o período experimental gratuito será aplicado automaticamente. Como parceiro no programa CSP, não pode renunciar ao período experimental gratuito nas ofertas que compra para os clientes. Uma vez terminada a duração do período experimental gratuito, o prazo de subscrição começará e a subscrição converter-se-á em estatuto pago. A subscrição irá então renovar automaticamente de acordo com o mesmo horário.

* * *

## <a name="update-subscriptions-with-add-ons"></a>Atualizar subscrições com suplementos

Para adquirir um addon, o cliente deve primeiro ter uma subscrição base ativa.  Não pode comprar suplementos através do catálogo.

1. Inscreva-se no painel do Centro [de Parceiros.](https://partner.microsoft.com/dashboard)

2. A partir do menu Partner Center, selecione **Clientes,** em seguida, escolha um cliente da lista.

3. Escolha a subscrição que pretende gerir.

4. Abaixo da secção **'Estado',** estão uma lista de Add-ons disponíveis para a subscrição.  

5. Atualize a quantidade de licenças para cada Add-on requerido. Em seguida, **submeta** as alterações.

A capacidade de adquirir addons através do Partner Center só está disponível para faturas diretas e fornecedores indiretos.
Apenas os complementos elegíveis são apresentados com base nos requisitos de base e na disponibilidade regional. Para obter mais informações sobre preços e ofertas, consulte a matriz de oferta de Cloud Reseller. A suspensão da subscrição base suspenderá também todos os suplementos associados.

As datas de início dos suplementos alinham-se com a subscrição base e os custos são calculados a partir da Data de início dos custos e da Data de fim dos custos, com os custos numa base pro-rata na primeira fatura. Para obter informações adicionais consulte, [faturação baseada em licença.](license-based-billing.md)


## <a name="suspend-or-cancel-a-subscription"></a>Suspender ou cancelar uma subscrição

Os parceiros podem suspender ou cancelar uma subscrição se solicitado pelo cliente, ou em casos de não pagamento ou fraude.

### <a name="suspend-a-subscription"></a>Suspender uma subscrição

Quando altera o estado de uma subscrição de **Suspenso,** os utilizadores não podem iniciar seduções ou aceder a serviços.

1. Inscreva-se no painel do Centro [de Parceiros.](https://partner.microsoft.com/dashboard)

2. A partir do menu Partner Center, selecione **Clientes,** em seguida, escolha um cliente da lista.

3. Escolha a subscrição que pretende gerir.

4. Na secção **Estado**, escolha **Suspenso**. Em seguida, **submeta** as alterações.

5. Todos os dados serão eliminados a menos que a subscrição seja reativada no prazo de 90 dias, ou 90 dias mais o número de dias entre o momento em que a conta foi aberta e o primeiro período de faturação (máximo de 120 dias).

Quando suspende uma subscrição, a data que vê abaixo do botão **Suspenso** indica quando a subscrição expirará automaticamente se não a reativar. 

> [!NOTE]
> As subscrições da CSP não têm um período de validade (como as subscrições diretas da Web têm) durante o qual os serviços ainda funcionam, mas a subscrição não gera quaisquer encargos de faturação. As assinaturas CSP estão ativas ou suspensas (ou totalmente eliminadas).

> [!NOTE]
> As novas mudanças de Comércio estão atualmente disponíveis apenas para parceiros que fazem parte da Microsoft 365/Dynamics 365 nova experiência técnica de experiência técnica.

Para suspender novas subscrições de comércio ou reativar novas subscrições de comércio suspensas, crie um pedido de serviço e suporte de contato.


### <a name="cancel-a-subscription"></a>Cancelar uma subscrição

Pode cancelar subscrições SaaS baseadas em licenças de editores ISV de terceiros dentro do [mercado comercial](csp-commercial-marketplace-overview.md)partner Center . Desde que cancele dentro do período de cancelamento, receberá um reembolso total.

Para ofertas ISV faturadas mensalmente:

- Se cancelar menos de 24 horas após a encomenda, receberá um crédito total na próxima fatura.

- Se cancelar mais de 24 horas após a encomenda, o cancelamento será agendado para a renovação.

Para ofertas faturadas anualmente:

- Se cancelar menos de 14 dias após a eção do pedido, receberá um crédito total na próxima fatura.

- Se você cancelar mais de 14 dias após a eção da encomenda, o cancelamento será agendado para ocorrer na renovação.

Depois destes períodos terminados, deixará de ver a opção de cancelar a subscrição.

> [!NOTE]
> Os serviços ISV baseados em utilização e medidos por terceiros (que utilizam máquinas virtuais ou contentores, por exemplo) não são elegíveis para devolução. Os serviços baseados na utilização podem ser desavisionados como um método de cancelamento. Uma vez que os encargos são cobrados após a utilização, estes serviços não são elegíveis para reembolso.

Para cancelar uma subscrição SaaS com base numa licença num editor do ISV, faça o seguinte:

1. Inscreva-se no painel do Centro [de Parceiros.](https://partner.microsoft.com/dashboard)

2. A partir do menu Partner Center, selecione **Clientes,** em seguida, escolha um cliente da lista.

3. Localize a subscrição que pretende cancelar.

4. Na coluna **'Estado',** **selecione Cancelar**. Em seguida, **submeta** as alterações.

5. Se aparecer uma caixa de diálogo, preencha os detalhes relevantes e, em seguida, **selecione Enviar por isso**.

6. Para confirmar o cancelamento, selecione **Sim, cancele**.

> [!NOTE]
> Também pode optar por cancelar uma subscrição do Azure Marketplace utilizando APIs. Para tal, consulte [cancelar uma subscrição do Azure Marketplace](/partner-center/develop/cancel-an-azure-marketplace-subscription).

## <a name="suspend-or-cancel-a-new-commerce-subscription"></a>Suspender ou cancelar uma nova subscrição de comércio

### <a name="suspend-a-new-commerce-subscription"></a>Suspender uma nova subscrição de comércio

> [!NOTE]
> As novas mudanças de Comércio estão atualmente disponíveis apenas para parceiros que fazem parte da Microsoft 365/Dynamics 365 nova experiência técnica de experiência técnica.

Em caso de não pagamento por parte do cliente, por vezes referido como o "cenário de dunning", os parceiros podem parar e retomar a sua subscrição para bloquear imediatamente o acesso do cliente aos serviços da subscrição.

Os parceiros podem parar e retomar uma subscrição a qualquer momento sem cancelamento. No entanto, a faturação dos parceiros continua durante a suspensão. 

A pausa nas subscrições do cliente irá desativar a sua capacidade de iniciar sing e usar os seus serviços até que a sua subscrição seja retomada. Todos os dados relacionados com a subscrição serão eliminados a menos que a subscrição seja reativada no prazo de 90 dias.

Pode fazer uma pausa numa subscrição utilizando o Partner Center:

1. Vá à página de subscrição do cliente e selecione a subscrição que pretende fazer uma pausa.

2. Selecione o botão de rádio **Suspender.**

3. No diálogo pop-up, selecione **OK**.

4. A subscrição estará agora em estado de pausa, e o parceiro continuará a ser cobrado para a subscrição.

A pausa é reversível através da interface de utilizador do Partner Center ou apIs que restaurarão imediatamente o acesso de um cliente aos serviços de uma subscrição.

> [!IMPORTANT]
> A pausa de uma subscrição irá desligar quaisquer definições de renovação automática e remover quaisquer alterações programadas existentes. A pausa de uma subscrição só afetará o acesso ao serviço do cliente, e a faturação do parceiro continuará enquanto estiver em estado de pausa.

### <a name="cancel-a-new-commerce-subscription"></a>Cancelar uma nova subscrição de comércio

> [!Note] 
> As novas mudanças de Comércio estão atualmente disponíveis apenas para parceiros que fazem parte da Microsoft 365/Dynamics 365 nova experiência técnica de experiência técnica.

Para novas ofertas de comércio, os parceiros podem cancelar a sua subscrição com um reembolso prosciente nas primeiras **72 horas** para qualquer prazo **(proção calculada diariamente)**.  

Após 72 horas, o cancelamento já não está disponível, e o parceiro será cobrado durante todo o prazo, mesmo que o cliente deixe de pagar, ou usando a subscrição (aplicável a qualquer plano de faturação).

Quando um cancelamento estiver concluído, o cliente perderá imediatamente o acesso ao serviço e o serviço não poderá ser restaurado. O estado para a assinatura não será recuperável.  

Se as licenças forem adicionadas a médio prazo, a mesma política de 72 horas aplica-se a qualquer redução de licenças adicionais. A redução das licenças adicionais deve ser feita através de **pedidos de apoio.**

## <a name="subscription-renewals"></a>Renovações de assinaturas

> [!NOTE]
> As novas mudanças de Comércio estão atualmente disponíveis apenas para parceiros que fazem parte da Microsoft 365/Dynamics 365 nova experiência técnica de experiência técnica.

Por predefinição, as subscrições ativas estão definidas para se renovarem automaticamente quando o período de subscrição terminar. Para [subscrições de produtos de mercado comercial,](csp-commercial-marketplace-overview.md)ou novas subscrições de comércio, pode optar opcionalmente por não renovar automaticamente a subscrição.

Para impedir que uma subscrição de mercado comercial ativo ou novas subscrições de comércio se renovem automaticamente:

1. Inscreva-se no painel do Centro [de Parceiros.](https://partner.microsoft.com/dashboard)

2. A partir do menu Partner Center, selecione **Clientes,** em seguida, escolha um cliente da lista.

3. Selecione **Subscrições**. Isto lista quaisquer subscrições baseadas em licença que tenha comprado para o cliente.

4. Na coluna **Subscrição,** selecione a subscrição que pretende modificar.

5. Na página de detalhes da subscrição, localize a secção **'Estado'** e desmarque a caixa **de renovação automática.**

6. Selecione **Submeter**.

### <a name="manage-new-commerce-renewals-with-scheduled-changes"></a>Gerir novas renovações de comércio com alterações programadas

> [!NOTE]
> As novas mudanças de Comércio estão atualmente disponíveis apenas para parceiros que fazem parte da Microsoft 365/Dynamics 365 nova experiência técnica de experiência técnica.

Algumas alterações às subscrições só podem acontecer no final de um período. Estas alterações podem ser programadas para que sejam convenientemente aplicadas no final do período. Exemplos de alterações que precisam de ser programadas:

- reduções de licenças
- Alterações ao termo de faturação
- Alterações na frequência de faturação

Outras alterações, como upgrades ou aumentos de licença, podem ser aplicadas durante o período.

As alterações de horário ocorrerão na renovação quando a subscrição se renovar para a próxima legislatura.

Pré-requisitos para alterações programadas:

- A subscrição está ativa 
- A renovação automática está a caminho
- SKU deve ser elegível para upgrade

Para agendar uma nova alteração a ocorrer na renovação:

1. Inscreva-se no painel do Centro de Parceiros.

2. Escolha um **cliente** na lista de clientes.

3. Escolha a subscrição que pretende gerir.

4. Selecione **Renovações de Gestão**.

5. Selecione uma alteração diferente para valor para SKU, quantidade, termo ou frequência de faturação:

   - **Corrente** é o valor atual da subscrição

   - **Alterar** para é o último valor guardado que quer ser aplicado na renovação da nova subscrição

6. Selecione **Submeter**.

7. As alterações ocorrerão na renovação.

Os parceiros podem aceder **a Manage Renovações** para visualizar, atualizar ou remover a alteração programada existente.

> [!NOTE]
> - Por defeito, os Ensaios converter-se-ão para o SKU equivalente pago no final do período experimental.
> - Para atualizações programadas do SKU, se a quantidade de licença não mudar, a reatribuição da licença de utilizador será automática, caso contrário terá de ser feita manualmente.
> - As alterações programadas guardadas são eliminadas se forem efetuadas atualizações intercalares à subscrição.

As alterações programadas guardadas são eliminadas quando são efetuadas as seguintes alterações intercalares:  

- A renovação automática é desligada 
- A quantidade é alterada 
- A subscrição está cancelada 
- SKU é atualizado 
- Julgamento é convertido 

## <a name="upgrades-in-new-commerce-subscriptions"></a>Atualizações em novas subscrições de comércio

Para o novo comércio, a atualização significa passar de uma subscrição paga para outra subscrição paga. As novas atualizações pagas ao comércio permitem ao cliente atualizar imediatamente do seu SKU atual para um com serviços adicionais. 

Os parceiros podem selecionar a subscrição a que pretendem atualizar quando a configuração da licença conta. Os parceiros podem selecionar uma **nova** subscrição ou selecionar uma subscrição **existente** se for elegível para a atualização. 

As atualizações podem ser de dois tipos: **Upgrade completo** e **atualização parcial**.

> [!NOTE]
> - As atualizações podem ser programadas para acontecer no final de um período de 20 000 ou podem ser iniciadas a médio prazo.
> - O início de uma atualização intercalar removerá as atualizações programadas existentes.
> - As atualizações só podem ser iniciadas a partir de subscrições no estado **Ativo.**

### <a name="full-upgrades"></a>Atualizações completas

Uma atualização completa é uma atualização no local, o que significa que todas ou mais licenças estão a ser atualizadas. Neste caso, o ID de subscrição permanece o mesmo, e as licenças são automaticamente atribuídas. No entanto, no caso de o cliente já ter adquirido o destino SKU a outro parceiro ou canal através do legado, será necessária uma atribuição manual. Se for necessária uma atribuição manual, o parceiro verá uma mensagem de aviso no Centro de Parceiros indicando que as licenças precisam de ser atribuídas manualmente. 

### <a name="partial-upgrades"></a>Atualizações parciais

As atualizações parciais permitem a um parceiro designar algumas licenças de um SKU para outro. A funcionalidade de atualização anterior nas assinaturas tradicionais baseadas em licenças apenas permitiu que todas as licenças fossem atualizadas. O novo comércio permite que um parceiro mova algumas licenças à sua conveniência. Isto dá ao parceiro mais controlo sobre a gestão de upgrades, permitindo-lhes mover alguns utilizadores para um novo SKU sem mover todos.

Detalhes parciais da atualização:

- Definido como parcial se a contagem de licença de upgrade for inferior à da subscrição inicial.
- Uma nova subscrição criada quando a atualização parcial terá as mesmas datas finais do prazo a partir da subscrição da atualização originária.

## <a name="increasing-and-reducing-licenses-in-new-commerce-subscriptions"></a>Aumentar e reduzir licenças em novas assinaturas de comércio

A contagem de licenças numa subscrição pode ser **aumentada** a qualquer momento, com ajustes de faturação refletidos na próxima fatura e ficheiro de reconciliação. 

A contagem de licenças numa subscrição pode ser **diminuída:**
- apenas nas primeiras 72 horas da altura em que a encomenda de subscrição foi colocada ou renovada pela **primeira vez.** 
- através do apoio ao cliente dentro de 72 horas, para licenças **adicionadas a meio**

Uma diminuição da contagem de licenças nas primeiras 72 horas de um termo de subscrição (após a compra ou renovação inicial) pode ser feita através de self-service no Partner Center ou através da API.

Uma redução da contagem de licenças para licenças adicionadas a meio do semestre só pode ser feita através do apoio ao cliente, nas primeiras 72 horas.

Em ambos os casos de redução de licença, você será reembolsado o **valor total menos valor pro-rated** para os dias que você   usou a subscrição **(proção calculada diariamente)**. 

Se **decorreram mais de 72 horas** desde que a encomenda de assinatura foi feita ou foram adicionadas licenças adicionais, a contagem de **licenças não pode** ser diminuída até à próxima janela de cancelamento na renovação.

## <a name="switching-billing-plans"></a>Mudar planos de faturação

Os parceiros têm a flexibilidade de mudar o seu plano de faturação e o seu termo de faturação em conjunto. Eles também têm a opção de mudar apenas o seu plano de faturação a meio do prazo, sem redefinir completamente o termo de faturação.

### <a name="just-changing-billing-frequency-scheduled-change"></a>Apenas alterando a frequência de faturação (Alteração Programada)

Os parceiros podem alterar apenas o plano de faturação através do Partner Center em apenas alguns passos, que entrarão em vigor no próximo ciclo de faturação:

1. Vá à página de subscrição do cliente e selecione a subscrição que pretende alterar.

2. Selecione o link **de frequência de faturação De gestão.**

3. Abrir-se-á um painel lateral que apresente a atual frequência de faturação e uma queda contendo as opções para alterar a frequência.

4. Uma vez selecionado um novo valor, as novas alterações de faturação ocorrerão no **próximo ciclo de faturação** (NÃO uma alteração imediata).

### <a name="changing-billing-frequency-along-with-billing-term-and-other-fields-immediate-change"></a>Alteração da frequência de faturação juntamente com o termo de faturação e outros campos (Mudança Imediata)

O parceiro pode alterar a frequência de faturação juntamente com o termo de faturação e outros campos através do Partner Center também, o que irá desencadear uma mudança imediata:

1. Vá à página de subscrição do cliente e selecione a subscrição que pretende alterar.

2. Altere a duração do prazo por seleção uma opção no dropdown. Isto abrirá mais uma entrega para mudar a frequência de faturação.

3. Selecione uma frequência de faturação diferente do dropdown.

4. Uma vez efetuadas as alterações e clicada, as novas alterações de faturação serão imediatamente **efetuadas**.

## <a name="next-steps"></a>Passos seguintes

- [Compre produtos de mercado comercial para os seus clientes](csp-commercial-marketplace-purchase.md)

- [Gerir produtos de mercado comercial para os seus clientes](csp-commercial-marketplace-manage.md)

- [Descrição geral do marketplace comercial](csp-commercial-marketplace-overview.md)
