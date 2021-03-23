---
title: Anúncios de março de 2021
description: Março de 2021 anúncios para o Microsoft Partner Center, incluindo novas capacidades, promoções, ofertas, mercados ou alterações às ofertas existentes.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.custom: announcement
ms.localizationpriority: high
ms.date: 03/22/2021
ms.openlocfilehash: a3172b78d41a966b52a824703a7f15f163467d63
ms.sourcegitcommit: 715368e56fe669d29c7981906e08bc8d7d5d62a4
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/23/2021
ms.locfileid: "104880740"
---
# <a name="march-2021-announcements"></a>Anúncios de março de 2021

Esta página fornece os anúncios para o Microsoft Partner Center para março de 2021.

________________
## <a name="corrections-made-to-march-1-2021-perpetual-software-price-list"></a><a name="14"></a>Correções feitas até 1 de março de 2021 lista de preços perpétuos de software

### <a name="categories"></a>Categorias

- Data: 2021-03-23
- Ofertas/Mercados

### <a name="impacted-audience"></a>Audiência impactada

Fornecedores indiretos e parceiros de conta direto que transfiram software perpétuo no programa Cloud Solution Provider 

### <a name="details"></a>Detalhes

A lista de preços do software perpétuo publicada a 1 de março de 2021 incluía mercados que não deveriam ter estado lá. A lista de preços perpétuos de software foi atualizada em 17 de março de 2021 com as correções. Estas correções só se aplicavam:

- ID do produto: DF77X4D43RKT 
- Nome do produto: Windows 10 Home to Pro Upgrade para o Microsoft 365 Business
- Mercados removidos ou não apoiados: AE, AF, AL, AM, AO, BA, BB, BD, BH, BM, BN, BO, BR, BS, BW, BY, BZ, CI, CL, CM, CO, CR, CW, CW, DO, DZ, EC, EG, ET, FJ, FO, GE, GH, GT, HN, IL, IN, IQ, JM, JO, KE, KG, KN, KW, KY, KZ, LB, LK, LY, MA, MC, MD, ME, MN, MN, , NI, NP, OM, PA, PE, PH, PK, PR, PY, QA, RS, RU, RW, SG, SN, SV, TH, TJ, TM, TN, TT, TZ, UA, UG, UY, UZ, VE, VN, YE, ZM, ZW

Estas alterações aplicam-se apenas ao produto acima referido. Outros produtos não tinham correções. 

### <a name="next-steps-and-resources"></a>Próximos passos e recursos

- Os parceiros que transacionam software perpétuo devem descarregar a mais recente lista de preços perpétuos de software.
- Consulte os [códigos dos países](https://docs.microsoft.com/azure/marketplace/commercial-marketplace-co-sell-countries) da região para um mapeamento amigável da abreviatura de duas letras para os países.
________________
## <a name="sdk-release-on-net-standard-v1170"></a><a name="13"></a> Lançamento SDK em .NET Standard (v1.17.0)

### <a name="categories"></a>Categorias

- Data: 2021-03-23

- Capacidades
 
### <a name="impacted-audience"></a>Audiência impactada

Parceiros Direct Bill e Fornecedores Indiretos que participam no programa CSP que estão a utilizar o Partner Center .NET SDK.

### <a name="details"></a>Detalhes

A partir de 23 de março de 2020, os Parceiros podem começar a descarregar a versão do [MicrosoftPartnerCenter.NETSDK (NuGet Gallery | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0), juntamente com [amostras atualizadas](https://github.com/Microsoft/Partner-Center-DotNet-Samples)do Centro De Parceiros Públicos SDK GitHub . Esta versão inclui atualizações aos seguintes métodos:

#### <a name="audit-updated-new-operation-types"></a>Auditoria Atualizada: Novos tipos de operação

Adicione novos [tipos de operação](https://docs.microsoft.com/partner-center/develop/auditing-resources) para saber quando o cliente aprovou e encerrou o DAP.

- DapAdminRelationshipApproved

- DapAdminRelationshipTerminated

#### <a name="audit-updated-new-resource-and-operation-types"></a>Auditoria Atualizada: Novos tipos de recursos e de operação

Adicionou novos [tipos de recursos e de operação](https://docs.microsoft.com/partner-center/develop/auditing-resources) para apoiar o cenário de função do diretório do cliente.

- Novo tipo de recurso "CustomerDirectoryRole"

- Tipos de operação "AddUserMember" e "RemoveUserMember"

#### <a name="sdk-updates-to-customer-accounts"></a>Atualizações SDK para contas de clientes

- Suporte para GET /clientes/{customer-tenant-id}/directSignedMicrosoftCustomerAgreementStatus

- GET /clientes/{cliente-inquilino-id}/qualificações

- POST /clientes/{customer_id}/qualificações?código={validação Código}

#### <a name="additional-changes"></a>Alterações adicionais

As seguintes alterações são introduzidas como parte do Novo Comércio, e estão atualmente disponíveis apenas por convite para parceiros que fazem parte da experiência técnica M365/D365 New Commerce. Os parceiros que não fazem parte da pré-visualização técnica do Novo Comércio não devem notar impactos e devem ser compatíveis com retroparos.

- Alterações no catálogo:

  - GET /products/{product-id}/skus/{sku-id}

- Compra e Gestão:
  - GET /clientes/{clienteId}/subscrições
  - GET /clientes/{customerId}/subscrições/{subscriçãoD}
  - PATCH /clientes/{customerId}/subscrições/{subscriçãoD}
  - GET /clientes/{customerId}/subscrições/{subscriçãoD}/transitioneligibilities
  - GET /clientes/{customerId}/subscrições/{subscriçãoId}/transições
  - POST /clientes/{customerId}/subscrições/{subscriçãoD}/transições

### <a name="next-steps"></a>Passos Seguintes

- Descarregue a versão mais recente [do MicrosoftPartnerCenter.NETSDK (NuGet Gallery | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0)
- Faça o download e reveja as amostras do [GitHub](https://github.com/Microsoft/Partner-Center-DotNet-Samples)

________________
## <a name="csp-commercial-marketplace-offer-and-fy21-csp-incentives-for-eligible-offers"></a><a name="12"></a>Oferta de mercado comercial da CSP e incentivos ao CDS para ofertas elegíveis

### <a name="categories"></a>Categorias

- Data: 2021-03-18
- Capacidades

### <a name="impacted-audience"></a>Audiência impactada

Fornecedores indiretos e parceiros de conta direta no programa Cloud Solution Provider 

### <a name="details"></a>Detalhes

Os fornecedores indiretos e parceiros de conta direta no programa Cloud Solution Provider podem vender ofertas de terceiros e ganhar um incentivo de desconto para cada oferta de terceiros elegível transacionada no Partner Center ou no portal Azure. O incentivo será sob a forma de um desconto nas vendas faturadas para as ofertas elegíveis e está **disponível até 30 de junho de 2021**.  

Continue a aprender sobre este incentivo CSP Commercial Marketplace Offer abaixo e contacte os seus clientes hoje para identificar as ofertas certas para permitir o seu sucesso contínuo e transformação digital.

Fazemos parcerias com fornecedores de software independentes (ISVs) para trazer as mais recentes soluções IaaS e SaaS para o mercado para os clientes da Microsoft. Os editores da ISV têm a opção de permitir a venda das suas ofertas através do canal parceiro da Microsoft. As nossas ofertas elegíveis para incentivos enquadram-se em duas categorias:

- Selecione ofertas de terceiros SaaS e IaaS com o estado de co-venda do Azure IP. 

- Aplicações SaaS integradas com Equipas ou pelo menos duas aplicações de produtividade Microsoft 365, tais como PowerPoint, Word, Excel, Outlook ou SharePoint.

### <a name="next-steps-and-resources"></a>Próximos passos e recursos

- Saiba mais sobre o ganho [de Incentivos a Parceiros](https://partner.microsoft.com/membership/partner-incentives) para a venda de aplicações elegíveis para o mercado, as aplicações elegíveis para incentivos. Novas ofertas são adicionadas mensalmente.  
- [Cloud Solution Provider recursos de incentivo de parceiro de conta direta](https://partner.microsoft.com/asset/collection/cloud-solution-provider-direct-partner-incentive-resources#/)
- [Recursos de incentivo indiretos do Fornecedor de Soluções Cloud](https://partner.microsoft.com/asset/collection/cloud-solution-provider-indirect-provider-incentive-resources#/)
- Reveja esta [apresentação](https://partner.microsoft.com/resources/detail/partner-center-cm-for-csp-overview-pdf) para saber mais sobre a venda das aplicações de marketplace comercial. Confira os recursos adicionais [aqui.](https://partner.microsoft.com/resources/collection/partner-center-cm-for-csp-collection#/) 
- Explore o catálogo de marketplace comercial no [Partner Center](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-discover) ou no [portal Azure](https://ms.portal.azure.com/#home)
- Utilize [APIs](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market) para integrar apps no mercado da sua empresa
- Contacte os ISVs com os que está interessado em fazer negócios
- Os fornecedores indiretos precisam de integrar usando APIs e guiar revendedores em que apps vender

### <a name="questions"></a>Perguntas?  

Consulte [este artigo](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-overview) para obter uma visão geral do mercado comercial no Partner Center.

Se precisar de assistência adicional, pode criar um pedido de apoio no Partner Center. Saiba mais em [https://aka.ms/IncentivesSupport](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=1) .

________________
## <a name="power-bi-premium-offer-naming-and-prerequisite-update"></a><a name="11"></a>Power BI Premium oferece nomeação e atualização pré-requisito

### <a name="categories"></a>Categorias

- Data: 2021-03-18
- Capacidades

### <a name="summary"></a>Resumo

A lista final de preços de 1 de abril de 2021 será atualizada para adicionar clareza ao nome e/ou informação pré-requisito para ofertas de Power BI Premium Per User.

### <a name="impacted-audience"></a>Audiência impactada

Cloud Solution Provider (CSP) parceiros diretos e indiretos

### <a name="details"></a>Detalhes

A lista final de preços de 1 de abril de 2021 será atualizada para adicionar clareza ao nome e/ou informação pré-requisito para ofertas de Power BI Premium Per User.

Até que a lista final de preços seja atualizada, utilize as informações nesta secção para garantir que o produto correto é encomendado.

Os seguintes detalhes mostram o SKU afetado e os detalhes pré-requisitos.

| Oferta nome de exibição na pré-visualização da lista de preços de 1 de março |  Nome de exibição de oferta atualizado na lista final de preços de 1 de abril| ID da oferta |
| ------ | ----------- | ----------- |
| Power BI Premium por utilizador Add-On (Preços de Pessoal sem fins lucrativos)  |  Power BI Premium por utilizador Add-On **(Office)** (Preço do Pessoal sem fins lucrativos)   | 31c03289-47ab-4ab0-8df1-03742c127ac6   |

Os clientes são obrigados a ter qualquer um dos seguintes pré-requisitos para comprar esta oferta:

| Oferta nome de exibição | ID da oferta |
| ------ | ----------- |
| Microsoft 365 E5 (Preços do Pessoal sem fins lucrativos)  |  31bedf01-9e57-4ece-a53a-d3656a563931   |
|   Microsoft 365 E5 sem Audio Conferencing (Preços de Pessoal sem fins lucrativos)|  b456810a-c414-4e07-98fc-ef74e8175a09|
|   Escritório 365 E5 (Preços do Pessoal sem fins lucrativos)| ce139fe5-8bd5-47ed-a5be-07c286f8b9e    |
|   Julgamento do Escritório 365 E5 (Preço do Pessoal Sem Fins Lucrativos)|  2f192efe-608a-4c9c-9d19-2b0b70b0962e|
|   Escritório 365 E5 sem Audio Conferencing (Preços do Pessoal Sem Fins Lucrativos)|  c3897426-9f49-4eaf-9b4d-7d9a1c72aef7|

A seguinte oferta Power BI Premium tem um pré-requisito necessário para a compra:

| Oferta nome de exibição | ID da oferta |
| ------ | ----------- |
|   Power BI Premium por utilizador Add-On (Preços de Pessoal sem fins lucrativos)|  ef0b895b-681b-4026-a5b1-dda182a57d40 |

Os clientes são obrigados a ter este pré-requisito para a compra desta oferta:

| Oferta nome de exibição | ID da oferta |
| ------ |----------|
| Power BI Pro (Preços do Pessoal Sem Fins Lucrativos)  |   cabdfc93-5786-4224-bfd3-35d58f833b35 |

### <a name="next-steps"></a>Passos seguintes

Reveja os recursos sobre este tema e partilhe esta informação com as partes interessadas apropriadas na sua organização.  

### <a name="questions"></a>Perguntas?

Para quaisquer questões sobre estas ofertas, consulte as suas comunidades Yammer relevantes. 

## <a name="march-price-updates-for-microsoft-365-f3"></a><a name="10"></a> Atualizações de preços de março para o Microsoft 365 F3

### <a name="categories"></a>Categorias

- Data: 2021-03-16
- Ofertas/Mercados

### <a name="summary"></a>Resumo

Os preços incorretos de março de 2021 foram corrigidos para a Microsoft 365 F3 British Pound (GBP) e Euro (EUR).

### <a name="impacted-audience"></a>Audiência impactada

Parceiros que compram o Microsoft 365 F3 em GBP ou EUR entre 1 de março e 17 de março de 2021 através do programa Cloud Solution Provider (CSP).

### <a name="details"></a>Detalhes

A Microsoft resolveu preços incorretos para o Microsoft 365 F3. Os preços incorretos foram para GBP e EUR e apenas para ofertas adquiridas entre 1 de março e 17 de março de 2021. As ofertas e moedas impactadas estão listadas abaixo. 

| Nome da oferta | Moeda | ID da oferta | Material ID |
| ------ |----------- |----------- |----------- |
| Microsoft 365 F3 (Caridade) | GBP | 57b722c2-c435-4bfb-9bc8-80509213a13a | AAD-11626 |
| Microsoft 365 F3 (Comercial) | EUR| 3451a3b0-8cda-44a7-bad7-c30be81c4aaa | AAA-89898 |
 
As listas de preços base de licença de março e abril foram atualizadas a 16 de março, 17:00 horas.

### <a name="next-steps"></a>Passos seguintes

- Os parceiros devem reencaitar as atuais listas de preços baseadas em licenças, tanto em março como na pré-visualização de abril, com estas correções de preços, se aplicável.  
- A Microsoft entrará em contacto com parceiros impactados nas próximas semanas por e-mail para os informar dos próximos passos relacionados com a correção das transações afetadas.

### <a name="questions"></a>Perguntas?

Para mais perguntas, verifique as suas comunidades CSP Yammer relevantes.

________________

## <a name="update-a-legal-company-name-through-partner-center"></a><a name="9"></a> Atualize um nome legal da empresa através do Partner Center

### <a name="categories"></a>Categorias

- Data: 2021-03-16
- Escala de & de eficiência de unidade

### <a name="summary"></a>Resumo

A partir de março de 2021, os parceiros da Microsoft Partner Network (MPN) e os revendedores indiretos cloud Solution Provider (CSP) podem atualizar o nome da empresa legal através do Partner Center.

### <a name="impacted-audience"></a>Audiência impactada

Parceiros MPN e revendedores indiretos CSP (não aplicáveis aos parceiros de conta direta da CSP)

### <a name="details"></a>Detalhes

A partir de março de 2021, os parceiros mpn e revendedores indiretos da CSP podem atualizar o nome da sua empresa legal através do Partner Center de forma compatível e self-serve. Com esta nova funcionalidade, os parceiros deixarão de precisar de submeter um bilhete de suporte do Partner Center para atualizar o nome da empresa. Isto poupará um tempo significativo para os parceiros na realização destas atividades. 

Para saber mais, consulte [Atualizar o seu perfil de negócio legal.](../update-your-partner-profile.md#update-your-legal-business-profile)

>[!NOTE]
>Certifique-se de que o nome da empresa no seu perfil de negócio legal está livre de erros ortográficos e abreviaturas, e corresponde exatamente aos seus registos formais de registo comercial da empresa. Para obter mais informações sobre a atualização do seu perfil de organização, consulte para [verificar o seu perfil de organização.](../update-your-partner-profile.md#update-your-legal-business-profile)

### <a name="next-steps"></a>Passos seguintes

Partilhe esta informação dentro da sua organização para que a equipa adequada possa rever e atualizar os seus processos.

### <a name="questions"></a>Perguntas?

Para mais perguntas, verifique as suas comunidades CSP Yammer relevantes.

________________
## <a name="update-to-cloud-solution-provider-csp-program-evolution-and-open-license-program-changes"></a><a name="8"></a> Atualização para a evolução do programa do Fornecedor de Soluções de Nuvem (CSP) e alterações do programa Open License

### <a name="categories"></a>Categorias

- Data: 2021-03-15
- Capacidades

### <a name="summary"></a>Resumo

Novas ofertas de software perpétuo do sector comercial e público estão a chegar ao programa Cloud Solution Provider (CSP), juntamente com alterações ao programa open licensing.

### <a name="impacted-audience"></a>Audiência impactada

Distribuidores comerciais e revendedores geridos que vendem através do programa Open License, bem como todos os parceiros da CSP que transacionam software perpétuo

### <a name="details"></a>Detalhes

Em setembro de 2020, a Microsoft [anunciou](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) uma série de passos na nossa jornada de transformação digital para expandir oportunidades aos parceiros no programa CSP, incluindo a disponibilidade de software no local para parceiros. Estas mudanças permitem que os parceiros cresçam o seu negócio e aumentem o seu alcance, aproveitando as licenças de software na CSP, posicionando-as para o sucesso no mundo atual em nuvem. Também capacitam as transições dos clientes para a nuvem e dão aos parceiros a flexibilidade necessária para ambientes de nuvem híbrida do cliente.

Na continuação desta transformação digital, anunciamos as seguintes alterações:

- 1 de julho de 2021: Não serão adicionados novos SKUs, produtos ou promoções à lista de preços do programa Open License.

- 7 de julho de 2021: Duas ofertas comerciais, Get Genuine Windows e Visual Studio Professional, e ofertas do setor público (governo, educação e sem fins lucrativos – ver [anúncio](./2020-december.md#9)) serão adicionadas à lista de preços perpétuos de software da CSP.  A lista de preços pode ser encontrada na secção de Software da página [de venda > de preços & Ofertas](https://partnercenter.microsoft.com/pcv/sales) no Partner Center e será republica nesta data.

Para obter detalhes completos sobre a evolução do programa CSP e alterações no programa Open License, consulte os **Próximos Passos** abaixo.

### <a name="next-steps"></a>Passos Seguintes:

- Evolução do Programa CSP: Reveja o [software perpétuo nos](https://partner.microsoft.com/resources/collection/software-in-csp#/) materiais de prontidão do programa Cloud Solution Provider. Use este [mapa de prontidão](https://partner.microsoft.com/resources/detail/software-in-csp-readiness-map-pdf) para localizar rapidamente as informações certas para o seu papel.

- Alterações no programa De Licença Aberta: Rever a evolução do [programa CSP e o programa Open License altera os](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/) materiais de prontidão. Use este [mapa de prontidão](https://partner.microsoft.com/resources/detail/csp-open-evolution-to-a-better-experience-readiness-map-pdf) para localizar rapidamente as informações certas para o seu papel.

### <a name="questions"></a>Perguntas

Para mais perguntas, verifique as suas comunidades CSP Yammer relevantes.

_______________
## <a name="update-to-a-previous-announcement-premium-assessments-an-add-on-to-compliance-manager"></a><a name="7"></a>Atualização para um anúncio anterior: Avaliações Premium, um add-on ao Compliance Manager

### <a name="categories"></a>Categorias

- Data: 2021-03-15
- Expandir o seu negócio

### <a name="summary"></a>Resumo

As ofertas de julgamento não deveriam ter sido listadas na lista de preços e serão removidas.

### <a name="impacted-audience"></a>Audiência impactada

Parceiros transacionando através do Cloud Solution Provider

### <a name="details"></a>Detalhes

As ofertas de julgamento não deviam ter sido incluídas na lista de preços. Estes serão removidos da lista de preços de 1 de maio de 2021.

O anúncio original está [aqui.](./2021-february.md#4)

### <a name="additional-resources"></a>Recursos adicionais

- [Segurança e conformidade microsoft 365 E5](https://www.microsoft.com/licensing/product-licensing/microsoft-365-enterprise?activetab=m365-enterprise:primaryr5)

- [Construir e gerir avaliações no Microsoft Compliance Manager - Microsoft 365 Compliance](/microsoft-365/compliance/compliance-manager-assessments)

### <a name="next-steps"></a>Passos seguintes

Reveja os recursos sobre este tema e partilhe esta informação com as partes interessadas apropriadas na sua organização.

### <a name="questions"></a>Perguntas?

Para questões sobre estas ofertas, consulte as suas comunidades Yammer relevantes.

________________
## <a name="migrate-your-solutions-from-one-commercial-partner-ocp-go-to-market-gtm-to-the-microsoft-commercial-marketplace"></a><a name="6"></a> Migrar as suas soluções de One Commercial Partner (OCP) go-to market (GTM) para o mercado comercial da Microsoft

### <a name="categories"></a>Categorias

- Data: 2021-03-12
- Capacidades

### <a name="summary"></a>Resumo

A partir de 29 de março de 2021, começará a experimentar capacidades limitadas de um Parceiro Comercial (OCP) no mercado (GTM). Encorajamo-lo a migrar as suas soluções para o mercado comercial no Partner Center.

### <a name="impacted-audience"></a>Audiência impactada

Organizações co-vendem com soluções no OCP GTM

### <a name="details"></a>Detalhes

Em dezembro de 2020, iniciámos a nossa viagem desde a ferramenta Microsoft OCP GTM até ao mercado comercial da Microsoft no Partner Center. Esta transição expande as capacidades do mercado comercial onde pode mostrar as suas soluções a milhões de clientes, partilhar oportunidades bidirecionalmente com outros vendedores da Microsoft e parceiros e vender soluções inovadoras em conjunto.

O próximo marco na transição terá lugar no dia 29 de março de 2021. É aí que começará a experimentar capacidades limitadas de OCP GTM, com alguns campos a tornarem-se apenas para ler. Se está atualmente a co-vender com soluções no OCP GTM, encorajamo-lo a migrar as suas soluções para o mercado comercial para tirar partido das suas capacidades e simplificar a sua experiência de publicação. 

Mudar-se para o mercado comercial faz do Partner Center o principal destino da experiência de co-venda. É onde pode continuar a crescer o seu negócio ligando as suas soluções aos nossos clientes partilhados através dos mesmos canais e experiências no produto que usamos para produtos da Microsoft. [Saiba mais sobre o mercado comercial.](https://blogs.partner.microsoft.com/mpn/getting-started-with-the-microsoft-commercial-marketplace/)

### <a name="next-steps"></a>Passos seguintes

- Se ainda não mexeu nas suas soluções, siga as instruções detalhadas no guia de [transição](/azure/marketplace/co-sell-solution-migration) ou veja o [tutorial de vídeo passo a passo](https://partner.microsoft.com/asset/detail/ocp-gtm-to-the-microsoft-commercial-marketplace-mp4) para completar todas as atividades de migração e começar a publicar as suas soluçãos no mercado comercial.

- Para questões relacionadas com a experiência de capacidade limitada no OCP GTM, consulte os [requisitos de Co-venda para publicar no mercado comercial da Microsoft FAQ](https://partner.microsoft.com/resources/detail/co-sell-requirements-publish-commercial-marketplace-faq-pdf). (Ver a secção "OCP GTM limited capabilities starting March 29, 2021.")

### <a name="questions"></a>Perguntas?

[Contacte o Suporte](https://partner.microsoft.com/support/?stage=1) se tiver alguma dúvida ou precisar de mais informações.

________________
## <a name="expanding-the-new-commerce-experience-in-the-cloud-solution-provider-csp-program-for-azure-to-russia"></a><a name="5"></a>Expandir a nova experiência de comércio no programa Cloud Solution Provider (CSP) para o Azure à Rússia

### <a name="categories"></a>Categorias

- Data: 2021-03-10
- Capacidades

### <a name="impacted-audience"></a>Audiência impactada

Todos os parceiros na Rússia transacionam através do programa Cloud Solution Provider (CSP).

### <a name="details"></a>Detalhes

A partir de 10 de março de 2021, estamos entusiasmados por anunciar a disponibilidade da nova experiência de **comércio na CSP para o Azure na Rússia.** Esta experiência irá dinamizar e melhorar a forma como os clientes compram e consomem serviços Azure. Também dará aos parceiros do programa CSP uma visão consistente dos preços do Azure através de moções de vendas, preços USD para consistência global, alinhamento de datas de faturação e acesso à Azure Cost Management.

### <a name="next-steps"></a>Passos seguintes

Existem vários recursos disponíveis introduzindo a nova experiência de comércio Azure e fornecendo informações adicionais. Encontre as últimas FAQs, decks, vídeo e muito mais na Galeria de [Recursos de Atualizações do Programa CSP.](https://partner.microsoft.com/resources/collection/new-azure-experience-in-csp#/)

________________
## <a name="partner-center-software-license-key-and-download-fulfillment"></a><a name="4"></a>Chave de licença de software Partner Center e cumprimento de descarregamento

### <a name="categories"></a>Categorias

- Data: 2021-03-04
- Capacidades

### <a name="summary"></a>Resumo

O software Partner Center descarregamento e capacidade de cumprimento da chave da licença foi reintegrado.

### <a name="impacted-audience"></a>Audiência impactada

Todos os parceiros do Cloud Solution Provider (CSP) transacionando encomendas de software de subscrição perpétua e servidor através do Partner Center

### <a name="details"></a>Detalhes

Em resposta ao feedback do parceiro, estamos a reinstaurar a capacidade de cumprimento do Partner Center para obter chaves de software e licença para ordens de software de subscrição perpétua e servidor. Será restaurado ao seu estado anterior antes de ser removido em 19 de janeiro de 2021. (Ver o [anúncio](2020-september.md#17).)

Note que as chaves de licença de software e links de descarregamento são valiosos e altamente procurados por ativos de propriedade intelectual. Se vazadas, podem ser rapidamente esgotadas dos seus limites de ativação e causar uma experiência negativa de cliente e parceiro.

### <a name="next-steps"></a>Passos seguintes

Reveja os seguintes recursos para instruções de utilização e orientações importantes sobre a distribuição das chaves do software:

- [Vender software no local através do programa CSP](../csp-on-premise-software.md)
- [Guia de operações](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf) do Centro Parceiro (Consulte a **secção de distribuição de chaves de software.)**

### <a name="questions"></a>Perguntas?

Se tiver mais perguntas sobre este aviso, consulte as suas comunidades Yammer relevantes.

________________
## <a name="migrate-your-deals-from-partner-sales-connect-psc-to-partner-center"></a><a name="3"></a>Migrar as suas ofertas de Partner Sales Connect (PSC) para Partner Center

### <a name="categories"></a>Categorias

- Data: 2021-03-04
- Capacidades

### <a name="summary"></a>Resumo

A Partner Sales Connect (PSC) passará para o acesso apenas à leitura a partir de 31 de março de 2021, pelo que pedimos que comece a migrar as suas ofertas do PSC para o Partner Center.

### <a name="impacted-audience"></a>Audiência impactada

Parceiros com negócios no PSC

### <a name="details"></a>Detalhes

Como parte do nosso compromisso comum com o crescimento, **co-vender com** a Microsoft é o caminho para que **você seja descoberto, entregue a sua experiência e expanda a sua pegada de cliente** para resultados positivos do cliente. Com uma oferta média **3,5 vezes mais rápida** do que o normal, gerir a sua experiência de co-venda no Partner Center permite-lhe vender através dos canais de clientes diretos, parceiro e vendedor da Microsoft, e gerir todo o seu pipeline de referência num local.

**O PSC** passará a **ter acesso apenas** a leitura a partir de 31 de março de **2021,** por isso pedimos-lhe que inicie a sua mudança para o Partner Center e aceda a estas melhorias de capacidade: 

- **Encaminhamento mais preciso** das ofertas que partilha com a Microsoft para o vendedor certo, com base no tipo de assistência que necessita.
- **Validação de elegibilidade do negócio inicial** para soluções elegíveis para incentivos e para cumprir os critérios do programa ISV Connect, simplificando o processo de aprovação e a prova final de execução (POE).
- **Experiência de utilizador sem emenda** para gerir todas as suas oportunidades de co-venda e vendas qualificadas lidera num só local.

Também adicionámos recentemente novas funcionalidades no Partner Center para ajudar no seu movimento:

- [Operações a granel para co-vender oportunidades](../bulk-operations.md)
- [Recurso de migração de acordo](../psc-to-pc.md) (ver a secção **de migração do PSC Deals.)**

Utilizando a experiência de co-venda no Partner Center, as suas equipas de vendas terão mais tempo para se concentrarem em nutrir leads e oportunidades, fechar ofertas e criar relações duradouras com o cliente.

### <a name="next-steps"></a>Passos seguintes

Utilize o [guia de transição](../psc-to-pc.md) do Centro de Parceiros para o acompanhar através dos passos para migrar as suas ofertas do PSC para o Partner Center.

### <a name="questions"></a>Perguntas?

Para mais perguntas, contacte [o Support](https://partner.microsoft.com/support/?stage=1).

________________
## <a name="new-microsoft-dynamics-365-products-and-offers-available-on-april-1-2021"></a><a name="2"></a>Novos produtos e ofertas microsoft Dynamics 365 disponíveis a 1 de abril de 2021

### <a name="categories"></a>Categorias

- Data: 2021-03-04
- Capacidades

### <a name="summary"></a>Resumo

No dia 1 de abril de 2021, a Microsoft lançará vários novos produtos e ofertas para o programa Cloud Solution Provider (CSP).

### <a name="impacted-audience"></a>Audiência impactada

Todos os parceiros que transacionam através do programa Cloud Solution Provider (CSP)

### <a name="details"></a>Detalhes

No dia 1 de abril de 2021, a Microsoft lançará os seguintes novos produtos e ofertas:

- Power BI Premium por utilizador
- Expansão geo e segmento usl de voz do cliente e marketing USL

**Power BI Premium por utilizador**

A Microsoft introduzirá as primeiras ofertas do Power BI Premium por utilizador. O Power BI Premium é atualmente vendido apenas numa construção de capacidade. Power BI Premium Per User fornece acesso a inteligência empresarial (BI) e capacidades de análise. O seu licenciamento individual flexível atende às pequenas e médias empresas.

Reveja os [detalhes de lançamento](/power-platform-release-plan/2020wave2/power-bi/planned-features) do Power BI para saber mais sobre esta oferta.


**Oferecer detalhes**

Note que o nome da oferta difere ligeiramente da pré-visualização da lista de preços.

| Nome da oferta | ID da oferta |
| ------ |----------- |
| Power BI Premium por utilizador | 9c810018-9356-4903-95ab-eeb956289290 | 
| Power BI Premium Por Utilizador para Docente | 3affc44f-f372-4ad5-8657-aadd9574fce0 | 
| Power BI Premium Por Utilizador para Estudantes | 657eea87-d0b0-4c89-8c8e-9b04395bd940 | 
| Power BI Premium por Utilizador (Preço do Pessoal sem fins lucrativos) | 7a0a856c-059f-45dd-9d26-ae27992e706a | 
| Power BI Premium por utilizador Add-On | 244ff87e-5925-44a0-bf31-cea189719b58 | 
| Power BI Premium por utilizador Add-On para a Faculdade | 5da849bd-b8f7-4340-b4f4-3a9eaeb8987e | 
| Power BI Premium por utilizador Add-On para estudantes | cf62d70d-5af5-422a-bda8-97936402ac8e | 
| Power BI Premium por utilizador Add-On (Preços de Pessoal sem fins lucrativos) | 31c03289-47ab-4ab0-8df1-03742c127ac6 | 

**Expansão geo e segmento usl de voz do cliente e marketing USL**

No seguimento do lançamento de dezembro de 2020, as ofertas de Voz e Marketing USL da Dynamics 365 foram alteradas para adicionar novos países e MAIS SKUs sem fins lucrativos e educativos.

| Nome da oferta | ID da oferta |
| ------ |----------- |
| Dinâmica 365 Customer Voice USL (Preços de pessoal sem fins lucrativos) | 7a8642a5-481e-4906-a642-b56dbeeb62a0 |
| Dinâmica 365 Voz do Cliente USL para Faculdade | 85162d70-9676-4cf6-a4bc-a0d6672f2657 |

Visite as seguintes páginas para saber mais sobre estas ofertas:

- [Página inicial da Página inicial da Voz do Serviço ao Cliente Dynamics 365](https://dynamics.microsoft.com/customer-voice/overview/)
- [Página inicial de Marketing Dynamics 365](https://dynamics.microsoft.com/customer-voice/overview/)

### <a name="next-steps"></a>Passos seguintes

Reveja os recursos sobre este tema e partilhe esta informação com as partes interessadas apropriadas na sua organização.  

### <a name="questions"></a>Perguntas?

Para quaisquer questões sobre estas ofertas, consulte as suas comunidades Yammer relevantes. 

________________
## <a name="microsoft-universal-print-now-available-in-some-suites"></a><a name="1"></a> Microsoft Universal Print já disponível em algumas suites

### <a name="categories"></a>Categorias

- Data: 2021-03-33
- Capacidades

### <a name="summary"></a>Resumo

A Microsoft Universal Print estará disponível para transacionar dentro de suites Microsoft 365 selecionadas e como um addon autónomo a partir de 1 de março de 2021.

### <a name="impacted-audience"></a>Audiência impactada

Todos os parceiros que transacionam através do programa Cloud Solution Provider (CSP)

### <a name="details"></a>Detalhes

[Universal Print](https://aka.ms/universalprint) é um serviço de impressão Microsoft 365 que remove a necessidade de servidores de impressão no local e permite que os dispositivos Windows imprimam para impressoras registadas no Azure. Estará disponível para transações a partir de 1 de março de 2021.

Os trabalhadores beneficiam da impressão sem condutor, da descoberta da impressora baseada em localização e de uma experiência de impressão intuitiva sem curva de aprendizagem. Os dispositivos que se unem ao Azure Ative Directory (Azure AD) utilizam credenciais AZure AD existentes para imprimir de forma segura. Os administradores gerem a impressão utilizando o portal Azure e podem facilmente ligar impressoras com suporte nativo para impressão universal. A Impressão Universal pode ser implantada com impressoras não compatíveis utilizando o software de conector de impressão universal.

A Universal Print será reensitada no lançamento para Windows E3, A3, E5 e A5, e Microsoft 365 BP, F3, E3, A3, E5 e A5.  

**Oferecer detalhes**

Note que o nome da oferta difere ligeiramente da pré-visualização da lista de preços.

| Nome da oferta | ID da oferta | Material ID |
| ------ |----------- |----------- |  
| Universal Print volume add-on (500 empregos) - Microsoft 365  | cb131356-45ee-4ae2-8537-873b706c8e75     | 9BI-00004   |
| Complemento de volume de impressão universal (500 empregos) para docentes - Microsoft 365   | 477bee81-9872-43d6-91d3-c72390bfcf49   | 9BK-00004   |
| Complemento de volume de impressão universal (500 empregos) - Windows    | d3ddc493-5741-4e0d-a02d-07edbb72e   | 9BI-00002   |
| Complemento de volume de impressão universal (500 empregos) para docentes - Windows   |  d0862f05-80f5-4fd4-8432-fe72dd893cc7  | 9BK-00002   |

### <a name="next-steps"></a>Passos seguintes

Familiarize-se com a tabela de preços e a [visão geral](/universal-print/fundamentals/universal-print-whatis)da Impressão Universal . Partilhe esta informação com todos os contactos apropriados na sua organização.

### <a name="questions"></a>Perguntas?

Para quaisquer questões sobre estas ofertas, consulte as suas comunidades Yammer relevantes.
