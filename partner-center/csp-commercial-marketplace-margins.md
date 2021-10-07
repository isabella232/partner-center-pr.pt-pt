---
title: Descubra margens - mercado comercial
ms.topic: how-to
ms.date: 10/06/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Saiba como os parceiros Fornecedor de Soluções em Nuvem (CSP) podem usar o Partner Center para descobrir as margens configuradas por Fornecedores de Software Independentes (ISVs).
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8d7b5f077b3ea3f98f87121634427842db0a0f03
ms.sourcegitcommit: 77737d8f986a1afb3d923c130936e2f73ce07879
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/07/2021
ms.locfileid: "129661379"
---
# <a name="discover-margins-configured-by-independent-software-vendors-isvs"></a>Descubra as margens configuradas por Fornecedores independentes de software (ISVs)

**Funções adequadas**: Administração global | Administrador de faturação | Agente administrativo | Agente comercial | Agente helpdesk

Os Fornecedores independentes de Software (ISVs) podem oferecer descontos de margem para algumas ofertas de marketplace comercial a fornecedores específicos de soluções cloud (CSPs). Estas margens incentivam os CSPs a vender estas ofertas aos seus clientes.

> [!NOTE]
> A funcionalidade de descontos de margem ISV para CSP está atualmente disponível como **pré-visualização pública** enquanto continuamos a recolher feedback e a melhorar as experiências.

## <a name="notes-about-the-public-preview"></a>Notas sobre a pré-visualização do público

A capacidade de margens ISV para CSP permite ao ISV criar descontos direcionados para CSPs específicos. Esta capacidade está disponível agora, mas em visualização pública. Isto significa que a funcionalidade é totalmente funcional e utilizável enquanto continuamos a melhorar as experiências globais do mercado da CSP. A funcionalidade será declarada já não na pré-visualização, uma vez que melhoramos a experiência do parceiro. Não existem prazos específicos para isso e os Parceiros CSP podem continuar a utilizar a funcionalidade de descontos como está.

### <a name="public-preview-improvement-areas"></a>Áreas públicas de melhoria da pré-visualização

- Disponibilidade de oferta appSource: Algumas ofertas de marketplace CSP, principalmente ofertas appSource, demoram mais tempo a integrar e disponibilizar no Centro de Parceiros. Alguns parceiros podem estar à procura de ofertas do AppSource, mas podem ter de esperar até serem disponibilizadas. À medida que o tempo passa, a equipa do Partner Center irá fazer melhorias na latência entre o momento em que um ISV cria uma oferta e quando estiver disponível.
- As margens são atualmente definidas como descontos percentuais de um produto de mercado CSP SKU. Para a frente, há aspirações a integrar o ponto de preços em futuras tabelas de preços. Até que isso aconteça, os parceiros podem emparelhar o sku do produto na lista de margens (e ASA associada) com o produto da lista de preços de mercado SKUs para prever os valores de carga.
- Algumas ofertas de marketplace com teste habilitado, não relacionadas com descontos de margem, mostram como **valores de $.00** na experiência de navegação no mercado. Os parceiros devem ter o cuidado de compreender que estes ensaios serão renovados para os montantes pagos no final do seu mandato. 
- As ofertas exclusivas podem estar disponíveis para os parceiros. Atualmente, estes não estão na lista de preços do mercado. Até lá, os parceiros terão de encontrar os preços para eles, utilizando a experiência de navegação no mercado para o produto para o qual querem preços.

## <a name="view-margins-in-partner-center"></a>Ver margens no Partner Center

Um CSP pode ver margens que os ISVs configuraram para eles na página de margens:

> [!NOTE]
> Para saber mais sobre a interface de espaços de trabalho, consulte [o Centro de Parceiros.](get-around-partner-center.md#turn-workspaces-on-and-off)

#### <a name="workspaces-view"></a>[Vista de espaços de trabalho](#tab/workspaces-view)

1. Inscreva-se no [painel partner center](https://partner.microsoft.com/dashboard) e selecione o azulejo de **preços.**

2. Selecione **margens**. Os parceiros verão uma lista de ofertas de marketplace para as quais os ISVs têm margens configuradas.

3. Os parceiros da CSP podem navegar na lista de margens disponíveis ou **descarregar** os dados num formato delimitado em vírgula.

#### <a name="current-view"></a>[Vista atual](#tab/current-view)

1. Inscreva-se no painel partner [center](https://partner.microsoft.com/dashboard)e, em seguida, selecione **CSP** do menu de navegação à esquerda.

2. Selecione **Venda,** seguido de **Margins**. Os parceiros verão uma lista de ofertas de marketplace para as quais os ISVs têm margens configuradas.

3. Os parceiros da CSP podem navegar na lista de margens disponíveis ou **descarregar** os dados num formato delimitado em vírgula.

* * *

## <a name="margins-overview"></a>Visão geral das margens

Os ISVs que estabeleceram relações com a CSP Partners podem querer oferecer descontos de margem para incentivar o CSP Partner a vender as ofertas aos seus clientes. Nestes casos, o Parceiro CSP negoceia frequentemente uma margem com um ISV ou o ISV pode fornecer uma margem sem consultar um Parceiro CSP. O ISV pode oferecer uma margem em ofertas baseadas em licenças ou em consumo. As margens baseadas no consumo aplicam-se apenas aos produtos ISV, e não a quaisquer produtos de consumo Azure com os quais o produto ISV possa trabalhar.

## <a name="margins-and-pricing"></a>Margens e preços

A lista de preços do mercado partner center contém os preços csp originais para ofertas. As listas de preços do mercado da CSP são partilhadas em todos os parceiros e contêm preços de retalho. Os parceiros aplicam então o desconto percentual de margem para o produto SKU que querem comprar para entender o preço final do artigo antes de o comprarem. Os parceiros da CSP também verão os preços de retalho na folha de preços do Azure através do portal Azure (apenas para produtos à base de consumo). Verão igualmente pormenores sobre a margem que lhes é alargada nesta folha de preços. 

## <a name="purchasing-offers"></a>Ofertas de compra

Os parceiros da CSP adquirem a sua margem configurada simplesmente comprando a oferta de marketplace no [Partner Center](https://partner.microsoft.com) ou implantando o produto a partir do portal Microsoft [Azure](https://portal.azure.com). O parceiro transaccionante receberá o desconto de margem sem ter de dar mais um passo. Os parceiros não podem optar por fora da margem, se o ISV o configurar para o CSP, o desconto será aplicado.

As margens são aplicáveis a qualquer transação que o parceiro executa e se aplique a qualquer um dos seus clientes. O Parceiro CSP não precisa de aceitar uma proposta e não é obrigado a transacionar uma oferta ISV, mas se o fizerem, e tiverem uma margem, será automaticamente aplicada. 

## <a name="margins-and-indirect-resellers"></a>Margens e Revendedores Indiretos

As margens são disponibilizadas apenas aos parceiros faturados pela Microsoft, transacionando parceiros como fornecedores indiretos e parceiros de conta direto. Um ISV não pode fornecer uma margem diretamente a um revendedor indireto, mas o fornecedor indireto pode decidir passar uma margem para o seu revendedor indireto. Os fornecedores indiretos podem optar por passar a margem para o seu revendedor indireto, mas não são obrigados a. 

## <a name="terms-and-billing"></a>Termos e faturação

Os parceiros podem verificar que a margem foi aplicada para ofertas baseadas no consumo usando as funcionalidades de gestão de custos Azure no portal Azure. Os parceiros podem verificar se a margem foi pedida para ofertas baseadas em licenças, revendo o seu ficheiro de reconciliação no final do seu ciclo de faturação.

Cada margem tem uma data de início e fim. A redução de preço baseada no desconto de margem é aplicada ao termo da compra. Um parceiro pode recomprar a mesma oferta após o seu mandato para obter um novo termo com margem. As renovações aplicam a margem se a renovação ocorrer dentro das datas de início e fim da margem. As datas de fim de uma margem alinham-se sempre até ao final do mês. 

## <a name="margins-for-metered-billing"></a>Margens para faturação medido

Alguns produtos CSP vêm com faturação medido. Se o parceiro da CSP aumentar os lugares para ofertas com faturação medida, o preço da parte baseada no direito dos encargos manterá o desconto até ao final do período de subscrição anual, mas a margem aplicada ao preço da faturação prevista não será mantida após o período final da margem. A solução aqui é que os ISVs criem uma nova margem para esse parceiro CSP até ao final do período de subscrição. 

## <a name="margins-notifications"></a>Notificações de margens

Não existe nenhuma notificação proactiva a menos que o ISV contacte o CSP por e-mail e confirme que estendeu uma margem. O parceiro CSP poderá visualizar todas as margens disponíveis através do separador Margens no Centro de Parceiros.   

### <a name="recon-files"></a>Arquivos de reconhecimento

O parceiro da CSP encontrará detalhes das margens que lhes são estendidas no ficheiro recon de compras **recorrentes e únicas** uma vez geradas. Dados importantes no ficheiro de reconhecimento para explicar as margens:

- A UnitPrice permanecerá conforme o preço fixado pelo ISV.  

- A EffectiveUnitPrice mostrará o preço após a aplicação da margem.  

- A Descrição do Preçoadjustment conterá detalhes sobre a margem fornecida ao parceiro CSP. 

## <a name="discover-and-operationalize-margins-using-the-partner-center-apis"></a>Descubra e operacionalize as margens utilizando as APIs do Partner Center

Os parceiros podem utilizar a interface de utilizador do Partner Center ou as APIs para visualizar ou exportar as margens disponíveis para eles.

### <a name="apis-to-retrieve-margins"></a>APIs para recuperar margens

Os parceiros podem operacionalizar os dados ligando para as APIs abaixo. Cada uma destas APIs devolve uma lista de margens a que o parceiro tem acesso, definida pelo ISV. Ambas as APIs devolvem os mesmos dados.

- [Obter Margins](/partner-center/develop/get-margins) devolve dados em formato de resultados da API

- [Baixar Margens](/partner-center/develop/download-margins) devolve dados em formato delimitado em vírgula

### <a name="apis-to-discover-marketplace-offers"></a>APIs para descobrir ofertas de marketplace

Os parceiros do programa CSP também podem usar APIs para devolver uma lista de margens disponíveis para eles. As ofertas elegíveis serão apenas as ofertas saaS ISV disponíveis para o parceiro vender através do mercado Partner Center. Os parceiros podem obter uma lista de ofertas do Marketplace SaaS [através da obtenção de uma lista de ofertas para um mercado.](/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market)

Os parceiros da CSP podem usar as APIs do Partner Center para puxar a lista de ofertas transacionáveis de software como serviço (SaaS) e submeter encomendas para os seus clientes. Para obter mais informações, consulte [Criar uma subscrição para produtos de mercado comercial.](/partner-center/develop/create-subscription-azure-marketplace-products)

Os parceiros da CSP podem usar o portal Azure UX para visualizar todas as ofertas de marketplace. Podem utilizar as seguintes APIs para puxar a lista de ofertas de VM do mercado e submeter encomendas para os seus clientes.  
- [VMs: Obtenha uma lista de VMs oferece APIs](/azure/virtual-machines/windows/cli-ps-findimage)
- [VMs: APIs de compra (CLI, PowerShell, ARM)](/azure/virtual-machines/linux/quick-create-cli) 

Não existe filtro no portal Azure para as ofertas que optam por serem vendidas via CSP. Os parceiros terão de rever a tabela de preços para perceber quais as ofertas que podem ser transpostas através da CSP. Não existem APIs do portal Azure disponíveis atualmente para transacionar ofertas de mercado saaS ou aplicações geridas. 

Para obter mais informações sobre a experiência da CSP no mercado, leia a [visão geral do mercado comercial.](csp-commercial-marketplace-overview.md)

## <a name="next-steps"></a>Passos seguintes

- [Descrição geral do marketplace comercial](csp-commercial-marketplace-overview.md)
- [Comprar ofertas de mercado comercial](csp-commercial-marketplace-purchase.md)
- [Guia de incentivos da CSP](https://aka.ms/partnerincentives)
