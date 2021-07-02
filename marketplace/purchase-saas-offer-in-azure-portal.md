---
title: Como comprar uma oferta saaS no portal Azure
description: Saiba como encontrar e comprar uma oferta SaaS no portal Azure.
author: mingshen-ms
ms.author: mingshen
ms.reviewer: dannyevers
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: how-to
ms.date: 06/29/2021
ms.openlocfilehash: a124e4c5bb31a1fbb744bf2c5e1ea65a356bdd54
ms.sourcegitcommit: 1d09ccaaa54f167b0c63e99761172ebe84e89f2e
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/02/2021
ms.locfileid: "113221445"
---
# <a name="purchase-a-saas-offer-in-azure-portal"></a>Comprar uma oferta SaaS no portal Azure

Este artigo explica as diferentes opções e requisitos para pesquisar, tentar e comprar uma oferta de software-as-a-service (SaaS) a partir do portal Azure.

## <a name="create-a-saas-subscription"></a>Criar uma subscrição SaaS

Para adquirir uma subscrição SaaS, precisa de uma conta de utilizador Azure com acesso a uma subscrição Azure apropriada. Esta subscrição será usada para faturação, bem como para compartimentalização dos seus recursos de nuvem adquiridos. Para saber mais sobre as subscrições do Azure, consulte [Criar uma subscrição adicional do Azure.](/azure/cost-management-billing/manage/create-subscription)

No portal Azure, selecione a oferta desejada do SaaS na secção **Marketplace.**

Uma subscrição de Software-as-a-Service oferece o direito de usar um serviço por um determinado período de tempo através de uma subscrição online em vez de instalação local em computadores individuais. Uma subscrição é um acordo para usar uma ou mais plataformas ou serviços em nuvem, para os quais os encargos se acumulam com base numa taxa de licença por utilizador ou no consumo de recursos baseados na nuvem. Uma organização pode ter várias subscrições de SaaS.

As restrições às subscrições do SaaS incluem:

- Sem assinaturas de estudantes.
- Não Visual Studio subscrição da Enterprise.
- Sem subscrições de crédito grátis.
- Para ofertas pagas, é necessário um instrumento de pagamento.

## <a name="saas-offers-discovery-in-azure-portal"></a>SaaS oferece descoberta no portal Azure

Uma vez que você está no portal Azure, existem algumas maneiras de reduzir a sua pesquisa para se concentrar nas ofertas do SaaS.

### <a name="narrowing-your-search"></a>Reduzindo a sua pesquisa

Na página inicial, sob os **serviços Azure** selecione **+ Criar um recurso** ou **Marketplace**. Ou use o atalho **G + N** em qualquer lugar da plataforma.

- Reduza os resultados às ofertas do SaaS utilizando o filtro **'Tipo oferta'** e, em seguida, selecione **SaaS**.
- Use a barra de pesquisa global na área de navegação superior, para encontrar uma oferta específica de SaaS.

Encontre uma [oferta Private SaaS](/marketplace/private-offers) selecionando o banner no topo da página inicial do **Marketplace.** Nem todas as ofertas, ou planos estão disponíveis em todas as geografias e algumas podem aparecer apenas para certos inquilinos.

A vista filtrada mostra cada oferta SaaS disponível representada por um título. Selecione um para ver a página de detalhes do produto. Que inclui as seguintes secções:

- Visão geral – detalhes sobre o serviço, marketing e materiais de aprendizagem
- Planos + Preços – cada oferta incluirá pelo menos um plano com diferentes termos e preços de faturação
- Informações de utilização + Suporte – inclui ID Publisher, ID de oferta e ID do plano
- Avaliação e Avaliações da oferta específica do SaaS

## <a name="available-billing-models-plansskus-for-saas-offers"></a>Modelos de faturação disponíveis (planos/SKUs) para ofertas saas

Cada oferta saas terá um ou mais planos. Cada oferta tem um modelo de preços associado: taxa fixa ou por utilizador. Cada preço do plano é taxa recorrente, que pode ser zero dólares (quaisquer preços cotados são apenas para fins e não se destinam a refletir custos reais). Esta taxa é forfedária ou preço por utilizador. Tipos de planos disponíveis:

- **Planos mensais** – taxa mensal recorrente; taxa mensal plana ou por utilizador que é paga com uma recorrência mensal. Quando o prazo terminar, o plano será renovado automaticamente.
- **Planos anuais** – taxa anual recorrente; taxa anual plana ou por utilizador que é paga com uma recorrência anual. Quando o prazo terminar, o plano será renovado automaticamente.
- **Medidores personalizados** – juntamente com as taxas recorrentes, um plano de tarifa fixa também pode incluir dimensões personalizadas opcionais para o uso excessivo não incluído na taxa fixa. Cada dimensão representa uma unidade faturada. Este é um custo variável que muda de acordo com o uso de unidades medidos, tais como: largura de banda, bilhetes ou e-mail processado. Será cobrado de acordo com o seu consumo destas dimensões mensalmente. Por favor, note que o consumo excessivo só começa quando utiliza todas as unidades de medição incluídas na taxa fixa.
- **Teste gratuito** – em alguns casos, o plano inclui um período experimental de um mês, durante o qual pode utilizar o software gratuitamente.  Uma vez terminado o período experimental, será cobrado de acordo com o seu plano. As ofertas de teste não são compatíveis com os contadores personalizados.

Estes modelos de preços estão disponíveis para planos públicos e privados.

## <a name="saas-purchase-experience"></a>Experiência de compra saaS

1. Na página do produto, selecione um plano que atenda às suas necessidades e continue a **configurar + subscrever**
2. Como parte do processo de compra, você será redirecionado para o **separador Básicos** e você será obrigado a:
    1. Defina qual *subscrição* gostaria de utilizar para faturação. A subscrição Azure que utiliza deve ter um método de compra válido definido para o mesmo. Deve ter o nível de permissão certo ou ter um grupo de recursos sob essa subscrição com o nível certo de permissões. Além disso, o seu país de faturação deve ser um país onde a oferta está disponível para compra. As subscrições Azure sem um método de pagamento válido (por exemplo, uma subscrição msdn) só podem ser usadas para comprar planos gratuitos
    1. Escolha ou crie um ** Grupo de Recursos* a que o recurso SaaS pertencerá.
    1. Digite um *Nome* para a subscrição de SaaS para identificá-lo facilmente mais tarde. Uma vez comprado, não pode mudar o nome.
    1. Em **Plano,** verá o plano que selecionou na página detalhada do produto (PDP). Se ainda não fez uma seleção ativa no PDP, verá o plano padrão. Pode alterar a sua seleção selecionando o link **do plano Change.** Selecione o termo de faturação relevante e, em seguida, escolha outro plano. Poderá alterar o plano após a compra, se a editora o apoiar. No entanto, não poderá alterar o prazo de mensal para anual ou de anual para mensal.
    1. Nos casos em que o modelo de preços seja *por utilizador,* poderá ser-lhe exigido que especifique o número de *Utilizadores*. O preço que vê mudará com base na subscrição, plano e termo que selecionou.
3. Proceda ao separador **Tags** - *As etiquetas* são pares chave/valor definidos pelo utilizador, que podem ser colocados diretamente num recurso ou num grupo de recursos. Pode utilizar tags para encontrar facilmente o seu recurso SaaS mais tarde. A Azure suporta atualmente até 50 tags por grupo de recursos e recursos. As etiquetas podem ser colocadas num recurso no momento da criação ou adicionadas a um recurso existente.
4. Continue a **rever + Subscreva** para analisar a oferta e planear detalhes.
    1. Rever *Termos de utilização,* *Alterações* e Política de *Privacidade* do editor e também para o Azure Marketplace
    1. Pode ser-lhe pedido que adicione os seus dados de contacto
    1. Rever *detalhes básicos* e *tags*
5. Após confirmação, **selecione Subscrever**.

## <a name="saas-subscription-and-configuration"></a>Assinatura e configuração do SaaS

Quando seleciona subscrever, uma mensagem afirma: "A sua subscrição SaaS está em andamento". Este processo deve levar alguns minutos, não feche a janela até que esteja terminado.

Uma vez concluída a subscrição, uma mensagem afirma que a subscrição do SaaS está concluída, e deve configurar a conta para começar a desfrutar da sua compra. Também receberá um e-mail solicitando-lhe para ativar a nova subscrição. Se não for você que irá configurar a conta SaaS, envie este e-mail para a pessoa relevante.

Para completar o processo e começar a usar o SaaS, é obrigado a começar a configurar a sua subscrição. Ao selecionar o botão **Configure agora,** irá redirecioná-lo para o site da editora.

Também pode verificar o estado da subscrição selecionando o ícone 'bell' no canto superior direito do cabeçalho.

Se não concluir o processo de configuração dentro de *30 dias,* esta subscrição saaS será automaticamente *eliminada*. A faturação começará depois de a sua conta estar configurada no site da editora.

Mensagens de erro que poderá encontrar durante o processo:

- O *nome do* plano do plano selecionado não pode ser adquirido numa subscrição gratuita
  - Atualize a sua conta, consulte https://aka.ms/UpgradeFreeSub mais detalhes.

- A compra falhou porque não conseguimos encontrar um cartão de crédito válido, nem um método de pagamento associado à sua subscrição Azure.
  - Utilize uma subscrição Azure diferente ou adicione um cartão de crédito ou método de pagamento atual para esta subscrição e redaveja.

- O *nome do plano selecionado* do nome da *oferta* pela editora *editora não* está disponível para compra de acordo com as regras definidas pelo seu Administrador de TI.
  - Contacte o seu administrador de TI.

- O *nome do plano selecionado* pelo *editor* *de oferta* não está disponível para compra devido às configurações do mercado privado efetuada pelo administrador de TI do seu inquilino.
  - Contacte o seu Administrador de TI

- A compra falhou porque o prazo de faturação solicitado é vazio ou inválido.
  - Tente comprar um plano diferente/termo de faturação.

- A compra falhou porque não pudemos verificar a sua assinatura de um acordo legal.
  - Redaçar. Se o erro persistir, tente fazer a compra utilizando diferentes subscrições ou suporte de contacto da Azure.

- A compra da *oferta DE OFERTAID* pela *editora editorID* falhou. Esta oferta não está disponível para compra.
  - Tente novamente mais tarde. Se, passado uma hora, continuar a receber esta mensagem de erro, contacte o suporte.  

- A aquisição do *plano de ofertaID* da *ofertaid* pela *editora editorid* falhou. Este plano não está atualmente disponível para compra.
  - Tente novamente mais tarde. Se, passado uma hora, continuar a receber esta mensagem de erro, contacte o suporte. 

- O *endereço de e-mail* do cliente com *o objeto id ObjectID* não tem autorização para executar *a implementação implementação Depôração Desaídua* sobre o Grupo *de Recursos de âmbito; O DeploymentScope* ou o âmbito de aplicação é inválido.  
  - Receberá esta mensagem se não tiver as permissões certas no Grupo de Recursos/Subscrição Azure.  
    Se o acesso foi concedido recentemente, por favor refresque as suas credenciais.  
    Para implantar recursos num grupo de recursos tem de ter pelo menos acesso ao Contribuinte. Verifique o seu estado de acesso em **Grupos de Recursos** e, em seguida, **Controlo de Acesso**. Isto mostra quem é o 'Proprietário', a quem pode pedir para atribuí-lo como 'Contribuinte'.

- A subscrição utilizada para esta compra não permite compras no Marketplace.  
  - Por favor, use uma subscrição diferente ou peça ao seu administrador para alterar a definição para esta subscrição e retentou novamente.

## <a name="next-steps"></a>Passos seguintes

- Se já comprou uma oferta no mercado, vá a [Billing e Facturaing](/marketplace/billing-invoicing)
- Você também pode saber mais sobre as opções [de planos privados.](/marketplace/private-offers)
