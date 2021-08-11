---
title: Anúncios de abril de 2021
description: Anúncios de abril de 2021 para o Microsoft Partner Center, incluindo novas capacidades, promoções, ofertas, mercados ou alterações às ofertas existentes.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-announcements
author: brentserbus
ms.author: brserbus
ms.custom:
- announcement
- references_regions
ms.localizationpriority: high
ms.date: 04/29/2021
ms.openlocfilehash: e5f2b8f3c4041f3c533abd9512b68879222b330c7301a4227aeb04188f9fe068
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/06/2021
ms.locfileid: "115688182"
---
# <a name="april-2021-announcements"></a>Anúncios de abril de 2021

Esta página fornece os anúncios para o Microsoft Partner Center para abril de 2021.

## <a name="readiness-updated-csp-customer-address-validation-api-going-live-in-june-testing-capability-now-available"></a><a name="10"></a>Prontidão: Validação de endereço do cliente CSP atualizada API em direto em junho; capacidade de teste agora disponível

### <a name="categories"></a>Categorias

- Data: 2021-04-30
- Preparação

### <a name="summary"></a>Resumo

Para ajudar parceiros e clientes a gerir o seu negócio com base na confiança, vamos convidar parceiros para testar alterações na API de Endereço Validado para todos os países do mundo.

### <a name="impacted-audience"></a>Audiência impactada

Parceiros de conta direta da CSP e fornecedores indiretos que criam novos ou atualizaram os detalhes do endereço dos clientes existentes

### <a name="details"></a>Detalhes

A Microsoft tem confiança. Estamos empenhados em fornecer um método compatível, seguro e seguro de validação de endereços do cliente para transação de subscrições de clientes no programa CSP. A partir de 31 de março de 2021, introduzimos alterações à API de Endereço Validado. Convidamos parceiros a testar a API antes do go-live no final de junho de 2021. 

Note que estas alterações afetam apenas a API do Endereço Validado. Criar APIs de Perfil de Faturação de Clientes e Atualização não são afetados. Embora o endereço sugerido não tenha atualmente de ser usado com a API do Cliente Criar, é altamente recomendado.

A resposta devolverá uma das seguintes mensagens de estado:

| Estado     | Descrição |    Número de endereços sugeridos devolvidos |
|-------|---------------|-------------------|
|Envio verificado | O endereço é verificado e pode ser enviado para. | Único |
|Verificado | O endereço está verificado. | Único |
|Interação necessária | O endereço sugerido foi alterado significativamente e precisa de confirmação do utilizador. | Único |
|Parcial de rua | A rua dada no endereço é parcial e precisa de mais informações. | Múltiplos — máximo de três |
|Instalações parciais | As instalações dadas (número de edifício, número de suite, entre outras) são parciais e precisam de mais informações. | Múltiplos — máximo de três |
|Vários | Existem vários campos que são parciais no endereço (potencialmente também incluindo a parcial da rua e as instalações parciais). | Múltiplos — máximo de três |
|Nenhuma | O endereço está incorreto. | Nenhuma |
|Não validado | O endereço não pôde ser enviado através do processo de validação. | Nenhuma |

Os códigos postais dos EUA devolverão mais quatro dígitos + hífen, por exemplo, 12345-6789.

### <a name="next-steps"></a>Passos seguintes

- Reveja a documentação técnica e questione frequentemente na [coleção de parceiros dedicados](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) para obter uma orientação mais detalhada.
- Prepare-se para incorporar as alterações utilizando a API do Partner Center e a experiência do utilizador web. 
- Partilhe o seu ID do inquilino da caixa de areia com o especialista em assuntos (Ali Khaki) a ser incluído no voo de teste, para que possa começar a preparar-se para a atualização. 
- Se estiver a utilizar uma solução de fornecedor de painéis de controlo (CPV), consulte o seu CPV.

### <a name="questions"></a>Perguntas?

Se precisar de apoio para as suas operações com a Microsoft, contacte o suporte do seu parceiro Yammer grupo ou abra um pedido de [serviço.](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8)

_______________
## <a name="new-location-for-partner-center-api-swagger-documentation"></a><a name="9"></a>Nova localização para a documentação da API Swagger do Partner Center

### <a name="categories"></a>Categorias

- Data: 2021-04-26
- Capacidades

### <a name="summary"></a>Resumo

Os documentos da API Swagger do Centro Parceiro foram migrados do anterior site de [documentação da Swagger](https://apidocs.microsoft.com/services/partnercenter) para um [novo site de documentação swagger.](/rest/api/partner-center-rest/)

### <a name="impacted-audience"></a>Audiência impactada

Parceiros de conta direta e Fornecedores Indiretos que participam no programa Fornecedor de Soluções em Nuvem (CSP) que estão a utilizar as APIs do Partner Center

### <a name="details"></a>Detalhes

A partir de 26 de abril de 2021, a documentação da API Swagger do Partner Center, incluindo o conteúdo da API de Repouso, está localizada num [novo site.](/rest/api/partner-center-rest/) O antigo local ficará inacessível após várias semanas.

### <a name="benefits"></a>Benefícios

A documentação da API Swagger do Centro Parceiro fornecerá uma função **try it.** Para utilizar esta função, terá de ter um Token Bearer, que pode gerar seguindo os passos listados na [Autenticação do Centro de Parceiros.](/partner-center/develop/partner-center-authentication#app--user-authentication)

### <a name="next-steps"></a>Passos seguintes

Partilhe esta informação dentro da sua organização para que a equipa adequada possa rever e atualizar os seus processos.

### <a name="questions"></a>Perguntas?

Para questões sobre estas ofertas, consulte as suas comunidades Yammer relevantes.

________________
## <a name="cloud-solution-provider-csp-software-return-period-policy-and-download-link-expiry-notice"></a><a name="8"></a>Fornecedor de Soluções em Nuvem (CSP) política de devolução de software e aviso de expiração do link de descarregamento

### <a name="categories"></a>Categorias

- Data: 2021-04-21
- Capacidades

### <a name="summary"></a>Resumo

Existem alterações na política do período de devolução do software CSP e na expiração do link de descarregamento.

### <a name="impacted-audience"></a>Audiência impactada

Parceiros que transacionam ofertas de subscrição de software perpétuo ou software em CSP

### <a name="details"></a>Detalhes

Note as seguintes notificações importantes relativas a compras perpétuas de software e subscrição de software através do Partner Center:

#### <a name="software-return-period-policy"></a>Política do período de devolução do software

A partir de 1 de junho de 2021, o período de devolução das ofertas de software em CSP, conforme indicado no Microsoft Partner Agreement (MPA), passará de 60 dias da data de encomenda para 30 dias a contar da data da encomenda.

Após a apresentação de uma encomenda de uma oferta de software, os parceiros terão 30 dias a contar da data da encomenda para submeter quaisquer revisões a tal encomenda:

- Qualquer licença de software perpétuo devolvida dentro do período de devolução de 30 dias receberá um crédito total do preço de compra pago.

- Qualquer produto de subscrição de software devolvido dentro do período de devolução de 30 dias receberá um crédito prostimado do preço de compra pago.

Esta mensagem é um seguimento das nossas comunicações por email enviadas em dezembro de 2020 e abril de 2021 a todos os parceiros da CSP relativamente ao período de devolução e outras atualizações à MPA. Consulte esses avisos para obter todos os detalhes sobre as alterações que afetam a MPA.

#### <a name="software-download-link-expiry"></a>Expiração do link de descarregamento de software

A partir de 3 de junho de 2021, os links de descarregamento de software para compras perpétuas de software e produtos de subscrição de software através do Partner Center terão uma data de validade de cinco dias a partir do download inicial. O prazo de validade será aplicável a todas as compras até 3 de junho de 2021, bem como a 3 de junho de 2021.

### <a name="next-steps"></a>Passos seguintes

Reveja o período de devolução do [CSP e o link de descarregamento expirando faQ,](https://partner.microsoft.com/resources/detail/csp-software-return-period-download-expiry-faq-pdf)e informe todas as equipas apropriadas dentro da sua organização destas alterações:

### <a name="questions"></a>Perguntas?

Para questões sobre estas ofertas, consulte as suas comunidades Yammer relevantes.

________________
## <a name="open-licensing-program-transitioning-resellers-to-the-cloud-solution-provider-csp-program"></a><a name="7"></a>Programa de Licenciamento Aberto: Revendedores de transição para o programa Fornecedor de Soluções em Nuvem (CSP)

### <a name="categories"></a>Categorias

- Data: 2021-04-19
- Cresça o seu negócio

### <a name="summary"></a>Resumo

Esta comunicação detalha como se preparar para as alterações que estão para breve no programa open licensing.

### <a name="impacted-audience"></a>Audiência impactada

CSP e parceiros de Licença Aberta

### <a name="details"></a>Detalhes

Em 2020, a Microsoft [anunciou](https://blogs.partner.microsoft.com/mpn/general-availability-of-perpetual-software-licenses-in-the-cloud-solution-provider-program/) que as licenças de software perpétuos estarão amplamente disponíveis para parceiros e clientes através do programa Fornecedor de Soluções em Nuvem (CSP). O primeiro marco foi alcançado em janeiro de 2021, quando as ofertas comerciais de software perpétuo ficaram disponíveis. O próximo marco-chave acontecerá em julho de 2021, quando as ofertas do [sector público](https://aka.ms/openlicensepublicsector) ficarem disponíveis. Também [comunicámos](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) que a partir de 1 de janeiro de 2022, nenhuma nova compra de licença de software ou renovações de Software Assurance ou serviços online pode ser feita através do programa Open License.

A transição do software perpétuo para o programa CSP na nova experiência de comércio ajudará os parceiros a expandir as oportunidades para oferecer soluções diversas e serviços geridos. Isto também vai acelerar a transição dos clientes para a nuvem.  Para ajudar a garantir uma transição suave tanto para os nossos parceiros como para os nossos clientes, fizemos estes ajustes e materiais para acelerar esta transformação digital:

#### <a name="april-2021"></a>abril de 2021

[Disponível:](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/)Abrir materiais de transição licença-csp para revendedores

#### <a name="july-2021"></a>julho de 2021

##### <a name="csp"></a>CSP

- 1 de julho: Licenças de software perpétuos disponíveis para clientes do sector público

- 7 de julho: Visual Studio Pro e Get Genuine Windows Agreement licenças de software perpétuos disponíveis para todos os segmentos

##### <a name="open-value"></a>Valor Aberto

- 1 de julho: SKUs adicionais disponíveis no programa Open Value para educação e sem fins lucrativos, oferecendo ofertas semelhantes ao programa De Licença Aberta

##### <a name="open-license"></a>Licença Aberta

- 1 de julho: A Microsoft deixará de lançar novas ofertas no programa Open License.

#### <a name="january-2022"></a>janeiro de 2022

- 1 de janeiro: Não podem ser feitas novas compras ou renovações através do programa Licença Aberta

### <a name="next-steps"></a>Passos seguintes

#### <a name="csp-indirect-providers"></a>Fornecedores indiretos da CSP

Utilize os próximos meses para ajudar os revendedores open license orientando para o programa CSP, assistindo a eventos comunitários parceiros e usando os materiais de transição Open License-to-CSP para revendedores:

- [Abra materiais de transição licença-para-CSP para revendedores](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/)— Apresentação geral personalizável, modelo de e-mail, guia de revendedor indireto CSP e muito mais para ajudá-lo a conduzir a adoção para os seus revendedores em escala.

- [CSP Partner Community Events](https://globalpbocomm.eventbuilder.com/GlobalCSP) organizados pela Microsoft Business Operations.  Junte-se às várias sessões para aprender básicos de CSP (CSP Fundamentals) ou ficar atualizado, e fazer perguntas sobre Software em CSP (Q&A Sessions).

- (Em breve) Sessão de formação centrada no revendedor indireto da CSP, organizada pela Microsoft Business Operations.

#### <a name="open-license-resellers"></a>Revendedores de Licença Aberta

- Se a sua organização não estiver atualmente inscrita no programa CSP, contacte o seu distribuidor para obter informações sobre como começar. Ligação com um fornecedor indireto [aqui.](https://partner.microsoft.com/membership/cloud-solution-provider/find-a-provider)

- Se a sua organização já está inscrita no programa CSP, saiba mais sobre software perpétuo em CSP [aqui.](https://partner.microsoft.com/resources/collection/software-in-csp)

### <a name="questions"></a>Perguntas?

Para mais perguntas sobre estas ofertas, consulte as suas comunidades Yammer relevantes.

________________
## <a name="now-live-global-promo-readiness-guide"></a><a name="6"></a>Agora ao vivo: Guia global de prontidão promocional

### <a name="categories"></a>Categorias

- Data: 2021-04-16
- Capacidades

### <a name="summary"></a>Resumo

A Prontidão de Lançamento publicou um novo [guia global de prontidão promocional](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) na galeria de recursos de prontidão de operações. Este guia proporciona uma visão consolidada de todas as [promoções globais ativas.](https://partner.microsoft.com/resources/collection/global-promo-readiness-guide-collection#/)

### <a name="impacted-audience"></a>Audiência impactada

Todos os parceiros de licenciamento de volume (VL), Dynamics Price List (DPL) e Fornecedor de Soluções em Nuvem (CSP)

### <a name="details"></a>Detalhes

Os parceiros da Microsoft partilharam connosco a necessidade de fornecer uma visão consolidada de todas as promoções globais com detalhes de suporte. Você queria este guia consolidado para ajudá-lo a usar promoções com a confiança de que toda a informação disponível será facilmente acessível em um local central e conveniente.

A partir de abril de 2021, a Microsoft atualizará este guia mensalmente, estando disponível numa coleção dedicada global promo promoinginess Guide na galeria de recursos de prontidão de operações.

As ligações a este guia também serão incluídas nas seguintes coleções:

- [A coleção de calendário](https://partner.microsoft.com/resources/collection/csp-announcement-calendar#/)de lançamento, que proporciona uma visão centralizada das próximas mudanças e lançamentos.

- [Coleções comunitárias](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/), que contêm materiais de apoio para as nossas chamadas mensais de parceiros, destacando as próximas mudanças e temas oportunos de interesse operacional.

- [Newsletters de parceiros](https://partner.microsoft.com/resources/collection/csp-monthly-update#/), tais como CSP Monthly Update

Como lembrete mensal, também publicaremos um anúncio do Partner Center com cada nova edição do guia global de prontidão promocional.

### <a name="next-steps"></a>Passos seguintes

No início de cada mês, encontrará o mais recente [guia global de prontidão promocional](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) na galeria de recursos de [prontidão de operações.](https://partner.microsoft.com/resources)

Partilhe esta informação com os contactos adequados nas suas organizações e informe-nos de quão útil o guia é através do "Foi útil esta página?" botão no final de cada página.

________________
## <a name="april-cloud-solution-provider-csp-community-update-and-reminders"></a><a name="5"></a>Atualização e lembretes da comunidade Fornecedor de Soluções em Nuvem de abril (CSP)

### <a name="categories"></a>Categorias

- Data: 2021-04-16
- | comunitários Convites e lembretes

### <a name="summary"></a>Resumo

Os recursos comunitários da CSP estão disponíveis a pedido e atualizados mensalmente para mantê-lo informado e preparado para a mudança no programa CSP.

### <a name="impacted-audience"></a>Audiência impactada

Parceiros de conta direta da CSP e fornecedores indiretos

### <a name="details"></a>Detalhes

Este mês, os recursos incluem os seguintes tópicos-chave:

- [Atualização para evolução do programa CSP e alterações do programa Open License](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/)

- [Alterações aos requisitos de embarque de clientes da CSP em determinadas regiões](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/)

- [Novo formato para a nova fatura PDF do comércio no programa CSP](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/)

Dentro da [coleção comunitária CSP,](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/)você encontrará:

- A [newsletter de Atualização Mensal da CSP,](https://partner.microsoft.com/resources/detail/csp-monthly-update-april-2021-global)que agrega anúncios, atualizações, eventos e lembretes recentes num documento de fácil leitura.

- O [Calendário de Anúncios da CSP,](https://partner.microsoft.com/resources/detail/csp-announcement-calendar-april-2021)que fornece uma visão de linha do tempo das próximas alterações que afetam o programa.

- O novo [calendário de lançamento do produto,](https://partner.microsoft.com/resources/detail/product-launch-calendar-april-pdf)onde pode ver os próximos lançamentos e ofertas de produtos.

- [A CSP lança recursos](https://partner.microsoft.com/resources/collection/april-2021-csp-launch-topics-collection#/) de atualização com conteúdo fácil de consumir em mudanças operacionais chave.

- [Refreshers e lembretes](https://partner.microsoft.com/resources/detail/csp-april-2021-refreshers-and-reminders-pdf) sobre os principais tópicos da CSP que recebem interesse e consultas.

#### <a name="csp-community-call-qas"></a>CSP Community Call Q&As

A Chamada Comunitária Q&Como estão disponíveis para o ajudar com questões relacionadas com as próximas alterações. Registe-se agora para a CSP Community Call Q&Tal como está a decorrer em abril, maio e junho. Estes irão focar-se nos mais recentes lançamentos, atualizações importantes e lembretes.

[Registe-se aqui.](https://globalpbocomm.eventbuilder.com/GlobalCSP)

### <a name="next-steps"></a>Passos seguintes

Reveja os recursos comunitários e registe-se para a Chamada Comunitária Q&A.

Para garantir que obtém o máximo da Chamada Comunitária Q&A, reveja o conteúdo da comunidade a pedido e envie as suas perguntas até 48 horas antes da chamada.

### <a name="questions"></a>Perguntas?

A chamada comunitária mensal CSP Q&A é o melhor local para questões relacionadas com alterações no programa CSP. Todos os meses, reveja o material e envie as suas perguntas com antecedência para que possamos passar a sessão sobre os tópicos que são mais importantes para si.

Para mais informações, contacte [o Suporte.](https://partner.microsoft.com/dashboard/support/csp/servicerequests/create?category=csp)

________________
## <a name="final-reminder-deprecation-of-get-qualification-on-may-6-2021"></a><a name="4"></a>Lembrete final: Depreciação da qualificação do GET em 6 de maio de 2021

### <a name="categories"></a>Categorias

- Data: 2021-05-04

- Capacidades

### <a name="impacted-audience"></a>Audiência impactada

Parceiros que vendem ofertas académicas, sem fins lucrativos e Nuvem da Comunidade Governamental (GCC) através do programa Fornecedor de Soluções em Nuvem utilizando a API do Partner Center

### <a name="details"></a>Detalhes

Este anúncio é um seguimento das melhorias do Partner Center [lançadas em dezembro.](./2020-december.md#1) Como parte desse lançamento, foram implementadas novas APIs get e post qualifications e, consequentemente, **a qualificação get existente será aposentada no dia 6 de maio de 2021**. Nessa altura, terás de te ter transitado para usar as novas APIs do Post Partner Center. As novas APIs post permitir-lhe-ão adquirir ofertas de Educação, enquanto as novas APIs GET permitir-lhe-ão adquirir ofertas pré-qualificadas sem fins lucrativos e GCC.

### <a name="next-steps"></a>Passos seguintes

- **Atualize as novas APIs** para uma transição bem sucedida e oportuna.

- **Reveja as novas alterações e guia** do Centro de Parceiros na API nos recursos de prontidão de operações: [Melhorias do processo de validação do processo de validação do cliente do Partner Center Education](https://partner.microsoft.com/resources/collection/partner-center-edu-validation-enhancements#/).

- Partilhe esta informação com as equipas apropriadas dentro da sua organização e com os seus revendedores para ajudá-los a prepararem-se para estas mudanças.

### <a name="questions"></a>Perguntas?

Para quaisquer questões relacionadas com esta notificação, contacte [o Suporte do Centro de Parceiros](https://partner.microsoft.com/dashboard/support/referrals/servicerequests?category=referrals).

### <a name="change-log"></a>Change log

- 4 de maio de 2021: Lembrete final da próxima depreciação da qualificação do GET

- 9 de abril de 2021: Lembrete da próxima depreciação da qualificação do GET 

- Fevereiro: Prazos atualizados para depreciação das qualificações GET & PUT

- Janeiro: Lembrete das próximas depreciações das qualificações GET & PUT

________________
## <a name="new-format-for-the-new-commerce-pdf-invoice-in-csp"></a><a name="3"></a>Novo formato para o novo comércio fatura PDF em CSP

### <a name="categories"></a>Categorias

- Data: 2021-04-05
- Capacidades

### <a name="summary"></a>Resumo

A Microsoft está a introduzir um novo formato para a nova fatura PDF do comércio no programa Fornecedor de Soluções em Nuvem (CSP) para apresentar detalhes de faturação por detalhes do produto em vez da descrição do SKU.

### <a name="impacted-audience"></a>Audiência impactada

Parceiros transacionando através do programa CSP

### <a name="details"></a>Detalhes

A partir de maio de 2021, a Microsoft está a introduzir um novo formato para a nova fatura PDF do comércio no programa CSP para apresentar detalhes de faturação por detalhes do produto em vez da descrição do SKU. Com esta nova atualização, vamos agregar os itens de linha por tipo de produto enquanto exibimos todos os produtos numa linha individual.

Os parceiros vão notar esta alteração que entra em vigor na sua fatura de maio para o período de faturação entre 1 de abril de 2021 e 30 de abril de 2021. As ofertas afetadas são Microsoft Azure As assinaturas Reserved Instance, Azure (plano Azure) e Marketplace.

Quaisquer pedidos de crédito-rebill feitos após a atualização do formato da fatura serão gerados no novo formato.

#### <a name="partner-benefits"></a>Benefícios do parceiro

Esta atualização irá oferecer as seguintes melhorias à experiência de faturação para os parceiros:

- Tamanho da fatura reduzida ao mesmo tempo que retém dados críticos

- Alinhamento do formato aos padrões da indústria para faturas compactas e fáceis de utilizar 

Os seguintes elementos não serão afetados:

- Página de resumo de faturação na fatura PDF

- APIs de faturação existentes

- Ficheiros de reconciliação (os ficheiros Recon podem ser utilizados para recuperar dados granulares.) 

- Faturas de encargos baseadas em licenças e de utilização

### <a name="next-steps"></a>Passos seguintes

Reveja as informações sobre este tópico na [galeria de recursos de prontidão de operações](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/) no site do parceiro da Microsoft. Para mais informações sobre faturação e tópicos fiscais, incluindo recursos de faturação, faturas, faturação de CSP e impostos, visite [a secção de Faturação](../billing.md) no Partner Center.

________________
## <a name="changes-to-the-cloud-solution-provider-csp-customer-onboarding-requirements"></a><a name="2"></a>Alterações aos requisitos de embarque do cliente Fornecedor de Soluções em Nuvem (CSP)

### <a name="categories"></a>Categorias

- Data: 2021-04-02
- Ofertas/Mercados

### <a name="summary"></a>Resumo

Como parte do nosso compromisso de ajudar parceiros e clientes a gerir o seu negócio com base na confiança, vamos solicitar informações adicionais ao cliente, a partir de 25 de março de 2021.

### <a name="impacted-audience"></a>Audiência impactada

Parceiros de conta direta da CSP e fornecedores indiretos que tenham clientes novos ou existentes nos países listados na secção seguinte

### <a name="details"></a>Detalhes

A Microsoft tem confiança. Estamos empenhados em fornecer um método de validação de clientes conforme, seguro e seguro para a transação de subscrições de clientes no programa CSP. No dia 25 de março de 2021, apresentaremos melhorias no Partner Center API e na interface de utilizador (UI) que afetarão os parceiros que cumprem ambos os seguintes critérios:

- O parceiro tem uma relação de faturação direta com a Microsoft (o que significa que o parceiro é ou um parceiro de conta direta ou um fornecedor indireto).

- O parceiro negoceia com clientes novos ou existentes nos seguintes países:

    - Tailândia
    - Vietname
    - Turquia
    - Polónia
    - África do Sul
    - Índia
    - Brasil
    - Iraque
    - Mianmar
    - Sudão do Sul
    - Arábia Saudita
    - Emirados Árabes Unidos
    - Venezuela

Os parceiros que satisfaçam os critérios terão de submeter o ID de registo da empresa de um cliente (também conhecido como organização do cliente INN) e o número de telefone quando atualizarem ou criarem uma subscrição para esse cliente. Estes parceiros também podem introduzir um nome do meio opcional para o cliente.

Note que quando adicionar o ID de registo da sua empresa deve usar o seu ID de imposto de negócio e não o ID pessoal do cliente.

Os parceiros que fazem negócios com clientes novos ou já existentes nos seguintes países já foram a bordo com um lançamento anterior em novembro de 2020.

- Arménia
- Azerbaijão
- Bielorrússia
- Hungria
- Cazaquistão
- Quirguistão
- Moldávia
- Rússia
- Tajiquistão
- Ucrânia
- Usbequistão

Os parceiros com clientes no resto do mundo terão a capacidade, no final de março de 2021, de introduzir o ID de registo da empresa, número de telefone e nome do meio para os clientes como detalhes opcionais.

### <a name="next-steps"></a>Passos seguintes

- Reveja a documentação técnica e questione frequentemente na coleção de [parceiros](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) dedicados para obter uma orientação mais detalhada.
- Prepare-se para incorporar as alterações utilizando a API do Partner Center e a experiência do utilizador web. A API/SDKs estará disponível para testes.
- Certifique-se de submeter os dados adicionais ao embarcar em novos clientes ou modificar os dados do cliente existentes.
- Se estiver a utilizar uma solução de fornecedor de painéis de controlo (CPV), consulte o seu CPV.

### <a name="questions"></a>Perguntas?

Contacte o seu consultor fiscal ou o fisco local se tiver alguma questão relacionada com o ID de registo da empresa (também chamado INN ou TIN). A Microsoft não pode fornecer orientações sobre questões fiscais.

Se precisar de apoio com as suas operações com a Microsoft, abra um [pedido de serviço](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).

## <a name="view-this-months-product-launches-and-offers"></a><a name="1"></a>Veja os lançamentos e ofertas deste mês

### <a name="categories"></a>Categorias

- Data: 2021-04-01
- Capacidades
 
### <a name="summary"></a>Resumo

O calendário de lançamento do produto de abril de 2021 já foi publicado.

### <a name="impacted-audience"></a>Audiência impactada

Todos os parceiros que transfiram através do programa Fornecedor de Soluções em Nuvem (CSP)

### <a name="details"></a>Detalhes

O calendário de [lançamento do produto](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) de abril de 2021 já está disponível na galeria de recursos de prontidão operações. Veja aqui os próximos lançamentos e ofertas de produtos.

### <a name="next-steps"></a>Passos seguintes

Reveja o [calendário de lançamento](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/)do produto e partilhe a informação com as partes interessadas apropriadas na sua organização.  

### <a name="questions"></a>Perguntas?

Para mais perguntas sobre estas ofertas, consulte as suas comunidades Yammer relevantes.