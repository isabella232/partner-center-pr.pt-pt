---
title: Criar subscrições de clientes no Partner Center
ms.topic: how-to
ms.date: 05/19/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: Saiba como vender subscrições aos seus clientes por produtos publicados pela Microsoft, bem como produtos SaaS publicados por ISVs de terceiros.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: 199e3dc42a0aa46c3e743e9e6fcb0ed585cd0303
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/29/2021
ms.locfileid: "114838024"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a>Create, suspend, or cancel customer subscriptions (Criar, suspender ou cancelar subscrições de clientes)

**Aplica-se a**: Partner Center | Centro de Parceiros para Microsoft Cloud for US Government

**Funções adequadas**: Agente administrador | Administrador de faturação | Administração global | Agente helpdesk | Agente comercial

Depois de ter criado um registo do seu cliente no Partner Center, pode vendê-los subscrições a produtos do catálogo. Isto inclui produtos publicados pela Microsoft e software como um serviço (SaaS) produtos publicados por fornecedores de software independentes de terceiros (ISVs) para o [mercado comercial.](https://azuremarketplace.microsoft.com/marketplace)

Algumas ofertas são limitadas a uma subscrição por cliente. Para ver uma lista das ofertas restritas, visite a página de Preços e Ofertas do Centro de Parceiros.

>[!IMPORTANT]
> Como parceiro no programa CSP, pode adquirir assinaturas SaaS **baseadas em licenças** ou **medidos** a editores da ISV dentro do Partner Center. Isto significa que pode adquirir qualquer oferta SaaS **baseada em licença** ou **medido** que o editor ISV lhe tenha disponibilizado, incluindo [ofertas exclusivas](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) às quais tem acesso. Para comprar ou gerir outras ofertas comerciais de marketplace a partir de ISVs (tais como ofertas baseadas em uso envolvendo aplicações Azure, Contentores ou VMs), você deve ir ao [portal Azure.](https://portal.azure.com/)

>[!NOTE]
>Todas as datas e horários no Partner Center são dadas na norma de tempo coordenada (UTC) do tempo universal. Isto pode diferir até 24 horas a partir da sua hora local.

## <a name="create-a-new-subscription"></a>Criar uma nova subscrição

1. Inicie sessão no [dashboard do Centro de Parceiros](https://partner.microsoft.com/dashboard).

2. No menu Partner Center, selecione **Clientes,** em seguida, escolha um cliente da lista.

3. Selecione **Adicionar subscrição**. O separador **Serviços Online** mostrará todas as ofertas disponíveis do Marketplace SaaS.

4. Para ver apenas certos tipos de subscrições, faça seleções nos filtros disponíveis:
   - **Publisher**: Escolha a **Microsoft** para ver apenas ofertas da Microsoft, ou **Partner** para ver produtos de marketplace comercial publicados pelos ISVs.
   - **Tipo de faturação**: Selecione o tipo de faturação de subscrição que pretende utilizar: **Licença** ou **Utilização**. Consulte [a faturação baseada em licença](license-based-billing.md) para obter informações que o ajudarão a decidir entre a frequência de faturação mensal e anual.
   - **Categoria**: Escolha **Empresa,** **Pequenas empresas,** ou **Trial.** Para obter informações sobre subscrições de teste, consulte [Oferecer aos seus clientes testes de produtos microsoft.](offer-your-customers-trials-of-microsoft-products.md)

5. Selecione as subscrições de produto que pretende comprar para o seu cliente. Os produtos que vê dependem do tipo de segmento de cliente (educação, governo, etc.) e dos filtros que aplicou. Algumas ofertas apresentadas no Mercado podem nem sempre estar disponíveis para um cliente específico ou um parceiro CSP específico. Isto pode ser porque:

   - O cliente já tem uma subscrição desse produto e só é permitido um

   - A subscrição do cliente pode ter sido suspensa (neste caso, pode reativar a subscrição em vez de comprar uma nova.)

   - Para as ofertas isv SaaS, pode haver algumas razões pelas quais a oferta não está disponível para compra: O ISV pode não suportar o país ou região de faturação do cliente; o ISV pode ter optado por não disponibilizar a oferta através do programa CSP; ou, o ISV pode ter feito a oferta [exclusiva](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) a apenas alguns parceiros da CSP. A oferta ISV também pode não ser transacionável através do Partner Center (por exemplo, contentores ou algumas ofertas baseadas em uso).  

6. Para cada subscrição que pretende adicionar, insira o número de licenças (se necessário) e selecione **Adicionar ao carrinho**.

7. Quando terminar de adicionar subscrições, selecione **'Rever'** e reveja a sua encomenda.

8. Depois de rever as suas encomendas e estiver pronto para comprar estas subscrições, selecione **Comprar**.

9. Depois de comprar uma subscrição para um cliente, ocorrerá o seguinte:

    - Pode rever ou editar a subscrição selecionando o nome de subscrição na página de **Subscrições** desse cliente. A partir daqui, pode selecionar licenças adicionais se alguma estiver disponível, alterar a quantidade de licenças ou suspender a subscrição.

    **Para assinaturas ISV SaaS (baseadas em licenças e contadores):**
    - Receberá um link para o site da editora ISV. Este link deve ajudá-lo a completar a implementação ou configuração da conta da subscrição do cliente.
      
    >[!NOTE]
    > Nem você nem o seu cliente receberão um e-mail com instruções para completar a configuração/provisionamento da conta para este tipo de subscrição ISV.)

    - Se a sua subscrição vier com um teste gratuito de 30 dias, o período experimental gratuito será aplicado automaticamente. Como parceiro no programa CSP, não pode renunciar ao período experimental gratuito nas ofertas que compra para os clientes. Uma vez terminada a duração do período experimental gratuito, o prazo de subscrição começará e a subscrição converter-se-á em estatuto pago. A subscrição irá então renovar automaticamente de acordo com o mesmo horário.
   
## <a name="update-subscriptions-with-add-ons"></a>Atualizar subscrições com suplementos 

Para adquirir um addon, o cliente deve primeiro ter uma subscrição base ativa.  Não pode comprar suplementos através do catálogo.

1. Inscreva-se no painel do Centro [de Parceiros](https://partner.microsoft.com/dashboard).

2. No menu Partner Center, selecione **Clientes,** em seguida, escolha um cliente da lista.

3. Escolha a subscrição que pretende gerir.

4. Abaixo da secção **'Estado',** encontram-se uma lista de Add-ons disponíveis para a subscrição.  

5. Atualize a quantidade de licenças para cada Add-on necessário. Em seguida, **submeta** as alterações.

A capacidade de adquirir addons através do Partner Center só está disponível para faturas diretas e fornecedores indiretos.
Apenas os complementos elegíveis são apresentados com base nos requisitos de base e na disponibilidade regional. Para obter mais informações sobre preços e ofertas, consulte a matriz de oferta de Cloud Reseller. A suspensão da subscrição base suspenderá também todos os suplementos associados.

As datas de início dos suplementos alinham-se com a subscrição base e os custos são calculados a partir da Data de início dos custos e da Data de fim dos custos, com os custos numa base pro-rata na primeira fatura. Para obter informações adicionais consulte, [faturação baseada em licença.](license-based-billing.md)


## <a name="suspend-or-cancel-a-subscription"></a>Suspender ou cancelar uma subscrição

Os parceiros podem suspender ou cancelar uma subscrição se solicitado pelo cliente, ou em casos de não pagamento ou fraude.

### <a name="suspend-a-subscription"></a>Suspender uma subscrição

Quando altera o estado de uma subscrição de **Suspenso,** os utilizadores não podem iniciar sôms ou aceder a serviços.

1. Inscreva-se no painel do Centro [de Parceiros](https://partner.microsoft.com/dashboard).

2. No menu Partner Center, selecione **Clientes,** em seguida, escolha um cliente da lista.

3. Escolha a subscrição que pretende gerir.

4. Na secção **Estado**, escolha **Suspenso**. Em seguida, **submeta** as alterações.

5. Todos os dados serão eliminados a menos que a subscrição seja reativada no prazo de 90 dias, ou 90 dias mais o número de dias entre o momento em que a conta foi aberta e o primeiro período de faturação (máximo de 120 dias).

Quando suspende uma subscrição, a data que vê abaixo do botão **Suspenso** indica quando a subscrição expirará automaticamente se não a reativar. 

>[!NOTE]
>As subscrições da CSP não têm um período de validade (como fazem as subscrições diretas da Web) durante o qual os serviços ainda funcionam, mas a subscrição não gera quaisquer encargos de faturação. As assinaturas CSP estão ativas ou suspensas (ou totalmente eliminadas).

### <a name="cancel-a-subscription"></a>Cancelar uma subscrição

Pode cancelar subscrições saaS baseadas em licenças de editores ISV de terceiros no [mercado comercial](csp-commercial-marketplace-overview.md)partner Center . Desde que cancele dentro do período de cancelamento, receberá um reembolso total.

Para ofertas ISV faturadas mensalmente:

- Se cancelar menos de 24 horas após a encomenda, receberá um crédito total na próxima fatura.

- Se cancelar mais de 24 horas após a encomenda, o cancelamento será agendado para a renovação.

Para ofertas faturadas anualmente:

- Se cancelar menos de 14 dias após a e realização do pedido, receberá um crédito total na próxima fatura.

- Se cancelar mais de 14 dias após a e realização da encomenda, o cancelamento será agendado para a renovação.

Depois destes períodos terminados, deixará de ver a opção de cancelar a subscrição.

> [!NOTE]
> Os serviços ISV baseados e medidos em uso (que utilizam máquinas virtuais ou contentores, por exemplo) não são elegíveis para devolução. Os serviços baseados na utilização podem ser desavisionados como um método de cancelamento. Uma vez que os encargos são cobrados após a utilização, estes serviços não são elegíveis para reembolso.

Para cancelar uma subscrição SaaS com base numa licença num editor do ISV, faça o seguinte:

1. Inscreva-se no painel do Centro [de Parceiros](https://partner.microsoft.com/dashboard).

2. No menu Partner Center, selecione **Clientes,** em seguida, escolha um cliente da lista.

3. Localize a subscrição que pretende cancelar.

4. Na coluna **'Estado',** **selecione Cancelar**. Em seguida, **submeta** as alterações.

5. Se aparecer uma caixa de diálogo, preencha os detalhes relevantes e, em seguida, **selecione Enviar por isso**.

6. Para confirmar o cancelamento, selecione **Sim, cancele**.

> [!NOTE]
> Também pode optar por cancelar uma subscrição do Azure Marketplace utilizando APIs. Para tal, consulte [cancelar uma subscrição do Azure Marketplace](/partner-center/develop/cancel-an-azure-marketplace-subscription).

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a>Escolha se renova automaticamente uma subscrição de mercado comercial

Por predefinição, as subscrições ativas estão definidas para se renovarem automaticamente quando o período de subscrição terminar. Para [subscrições de produtos de mercado comercial,](csp-commercial-marketplace-overview.md)pode optar opcionalmente por não renovar automaticamente a subscrição.

Para impedir que uma subscrição de mercado comercial ativo renove automaticamente:

1. Inscreva-se no painel do Centro [de Parceiros](https://partner.microsoft.com/dashboard).

2. No menu Partner Center, selecione **Clientes,** em seguida, escolha um cliente da lista.

3. Selecione **Subscrições**. Isto lista quaisquer subscrições baseadas em licença que tenha comprado para o cliente.

4. Na coluna **Subscrição,** selecione a subscrição que pretende modificar.

5. Na página de detalhes da subscrição, localize a secção **'Estado'** e desmarque a caixa **de renovação automática.**

6. Selecione **Submeter**.

## <a name="next-steps"></a>Passos seguintes

- [Compre produtos de mercado comercial para os seus clientes](csp-commercial-marketplace-purchase.md)

- [Gerir produtos de mercado comercial para os seus clientes](csp-commercial-marketplace-manage.md)

- [Descrição geral do marketplace comercial](csp-commercial-marketplace-overview.md)