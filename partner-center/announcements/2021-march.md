---
title: Anúncios de março de 2021
description: Março de 2021 anúncios para o Microsoft Partner Center, incluindo novas capacidades, promoções, ofertas, mercados ou alterações às ofertas existentes.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-announcements
author: brentserbus
ms.author: brserbus
ms.custom: announcement
ms.localizationpriority: high
ms.date: 04/02/2021
ms.openlocfilehash: 28af0cecf14530554a0a17cdc2a45925f3e5d45376483fa1eb680575fdad3854
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/06/2021
ms.locfileid: "115688017"
---
# <a name="march-2021-announcements"></a>Anúncios de março de 2021

Esta página fornece os anúncios para o Microsoft Partner Center para março de 2021.

## <a name="readiness-changes-to-the-cloud-solution-provider-csp-customer-address-validation-api-going-live-in-june-testing-capability-now-available"></a><a name="19"></a>Prontidão: Alterações à validação do endereço do cliente Fornecedor de Soluções em Nuvem (CSP) A API vai em direto em junho; capacidade de teste agora disponível

### <a name="categories"></a>Categorias

- Data: 2021-03-30
- Preparação

### <a name="summary"></a>Resumo

Para ajudar parceiros e clientes a gerir o seu negócio com base na confiança, vamos convidar parceiros para testar alterações na API de Endereço Validado para todos os países do mundo.

### <a name="impacted-audience"></a>Audiência impactada

Parceiros de conta direto da CSP e fornecedores indiretos que criam novos ou atualizam os dados de endereço dos clientes existentes.

### <a name="details"></a>Detalhes

A Microsoft tem confiança. Estamos empenhados em fornecer um método compatível, seguro e seguro de validação de endereços do cliente para transação de subscrições de clientes no programa CSP. A partir de 31 de março de 2021, introduzimos alterações na API do Endereço Validado que convidamos os parceiros a testar, antes de irmos ao vivo com as mudanças em junho de 2021.

As alterações afetam apenas a API do Endereço Validado. Criar APIs de Perfil de Faturação de Clientes e Atualização não são impactados.

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

Os códigos postais dos EUA devolverão mais 4 dígitos + hífen - por exemplo, 12345-6789.

Uma vez que um endereço é submetido para validação através da API de Endereço Validado, o seguinte esquema de resposta será devolvido:

```csharp

// <summary>
/// Object represents the address validation response.
/// </summary>

public class AddressValidationResponse
{
   /// <summary>
   /// Gets or sets the original address
   /// </summary>
   /// <value>
   /// Original Address
   /// </value>
   public Address OriginalAddress { get; set; }

   /// <summary>
   /// Gets or sets the suggested addresses
   /// </summary>
   /// <value>
   /// Suggested Addresses
   /// </value>
   public List<Address> SuggestedAddresses { get; set; }

   /// <summary>
   /// Gets or sets the validation status
   /// </summary>
   /// <value>
   /// Status
   /// </value>
   public string Status { get; set; }

   /// <summary>
   /// Gets or sets the validation message
   /// </summary>
   /// <value>
   /// Validation Message
   /// </value>
   public string ValidationMessage { get; set; }
   ```

Dê uma olhada nesta resposta da amostra. Note que para os EUA, a resposta devolverá um sufixo adicional de quatro dígitos para a linha de código postal se introduzir apenas cinco dígitos para o código postal.

```csharp

"suggested_address": {
              "Country": "US",
              "region": "WA",
              "city": "Redmond",
              "address_line1": "1 Microsoft Way",
              "postal_Code": "98052-8300"
},
"original_address": {
              "Country": "US",
              "region": "WA",
              "city": "Redmond",
              "address_line1": "1 Micro Way",
              "postal_Code": "98052"
},
"status":  "InteractionRequired",
"validation_message": "Address field invalid for property: ‘Street’"
}
```

### <a name="next-steps"></a>Passos seguintes

- Partilhe o seu ID do inquilino da caixa de areia com o especialista em assuntos (Ali Khaki) a ser incluído no voo de teste, para que possa começar a preparar-se para a atualização.

- Se estiver a utilizar uma solução de fornecedor de painéis de controlo (CPV), consulte o seu CPV.

### <a name="questions"></a>Perguntas?

Se precisar de apoio para as suas operações com a Microsoft, contacte o seu parceiro Yammer grupo.

### <a name="change-log"></a>Registo de alteração:

- 31 de março de 2020: Publicação original

- 30 de abril de 2021: Atualizações para resposta à amostra e detalhes do código postal

________________
## <a name="new-exchange-admin-center-eac-experience"></a><a name="18"></a>Experiência do Centro de Administração de Novas Exchange (EAC)

### <a name="categories"></a>Categorias

- Data: 2021-03-29
- Capacidades

### <a name="summary"></a>Resumo

A partir de 27 de abril de 2021, o centro de administração Exchange (EAC) vai lançar uma nova experiência que melhorará a eficiência do dia-a-dia para os utilizadores.

### <a name="impacted-audience"></a>Audiência impactada

Administradores delegados que acedem a Exchange através do Partner Center

### <a name="details"></a>Detalhes

A partir de 27 de abril de 2021, os parceiros que navegam para Exchange através do Partner Center serão redirecionados para o novo EAC.

Esta nova experiência está atualmente disponível como pré-visualização, e os administradores podem ativar esta experiência selecionando o toggle no canto superior direito dentro do clássico EAC. Também podem navegar para o novo EAC selecionando o banner "Experimente agora" que é exibido em todas as páginas.

Os benefícios do novo CEA incluem:

- Informações adicionadas, relatórios e mecanismos de alerta para problemas relacionados com o fluxo de correio. 

- Dashboards personalizados para aumentar a produtividade.

Para ajudá-lo a navegar através da nova experiência, os vídeos estão disponíveis na secção **Guia de & formação** sobre a nova experiência EAC. Estes dar-lhe-ão uma visão geral de como pode utilizar melhor o novo portal.

>[!NOTE]
>Com esta mudança, a experiência clássica da EAC não será depreciada. Será notificado com muita antecedência antes de qualquer alteração ser implementada.

### <a name="next-steps"></a>Passos seguintes

- Confira os [recursos sobre este tema,](https://partner.microsoft.com/resources/collection/new-exchange-admin-center-experience#/)onde pode ver imagens da nova experiência.

- Partilhe esta informação com as partes interessadas apropriadas na sua organização. 

### <a name="questions"></a>Perguntas?

Para quaisquer questões sobre estas alterações, consulte as suas comunidades Yammer relevantes.

________________
## <a name="microsoft-operations-introducing-the-product-launch-calendar"></a><a name="17"></a>Microsoft Operations: Introdução do calendário de lançamento do produto

### <a name="categories"></a>Categorias

- Data: 2021-03-25
- Ofertas | Local de trabalho moderno

### <a name="summary"></a>Resumo

Em resposta ao feedback dos parceiros, a Microsoft Operations irá agilizar as comunicações para lançamentos de produtos.

### <a name="impacted-audience"></a>Audiência impactada

Fornecedor de Soluções em Nuvem parceiros (CSP)

### <a name="details"></a>Detalhes

A Microsoft está empenhada em melhorar continuamente as experiências dos parceiros. Recebemos comentários seus de que tem recebido demasiadas comunicações da Microsoft, incluindo anúncios duplicados para lançamentos de produtos.

Em resposta ao seu feedback, a Microsoft dinamizou a experiência de prontidão para lançamentos de produtos para novas ofertas existentes.

Disponibilizamos-lhe agora uma única visão mensal dos lançamentos de produtos, publicada na galeria de recursos de prontidão operações. Esta [visão](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) mensal do calendário de lançamento do produto substituirá as comunicações individuais de lançamento de produtos na galeria de recursos de prontidão de Operações e nos anúncios do Partner Center.

Você também pode acessá-lo calendário de [lançamento](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) de produtos a partir de [coleções comunitárias, vistas](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) [de calendário](https://partner.microsoft.com/resources/assets#/?type=collection&search=Calendar&sort=updated)e [newsletters CSP.](https://partner.microsoft.com/resources/collection/csp-monthly-update#/) Iremos notificá-lo quando publicarmos o calendário de lançamento de produtos de cada mês com um anúncio na galeria de recursos de prontidão opera.

Você ainda pode encontrar informações sobre ofertas novas e existentes na lista de preços pré-visualização e registos de alteração de lista de preços, bem como em blogs de produtos, guias de licenciamento e páginas de marketing de produtos.

A alteração aplicar-se-á aos lançamentos para os seguintes produtos:

- Dinâmica no local
- Microsoft 365
- Microsoft Dynamics 365
- Windows
- Servidor  
- Ferramentas
- Teams e Telco

Continuaremos a enviar anúncios específicos para lançamentos de produtos que requerem detalhes de prontidão das operações.

### <a name="next-steps"></a>Passos seguintes

Reveja os recursos sobre este tema e partilhe esta informação com as partes interessadas apropriadas na sua organização.

### <a name="questions"></a>Perguntas?

Para mais perguntas sobre estas ofertas, consulte as suas comunidades Yammer relevantes.

________________
## <a name="changes-to-csp-customer-onboarding-requirements"></a><a name="16"></a>Alterações aos requisitos de embarque do cliente CSP

### <a name="categories"></a>Categorias

- Data: 2021-03-25
- Capacidades

### <a name="summary"></a>Resumo

Como parte do nosso compromisso de ajudar parceiros e clientes a gerir o seu negócio com base na confiança, vamos solicitar informações adicionais ao cliente, a partir de 25 de março de 2021.

### <a name="impacted-audience"></a>Audiência impactada

Fornecedor de Soluções em Nuvem (CSP) parceiros de conta direta e fornecedores indiretos que tenham clientes novos ou existentes nos países listados na secção seguinte

### <a name="details"></a>Detalhes

A Microsoft tem confiança. Estamos empenhados em fornecer um método de validação de clientes conforme, seguro e seguro para a transação de subscrições de clientes no programa CSP. No dia 25 de março de 2021, apresentaremos melhorias no Partner Center API e na interface de utilizador (UI) que afetarão os parceiros que cumprem ambos os seguintes critérios:

1. O parceiro tem uma relação de faturação direta com a Microsoft (o que significa que o parceiro é ou um parceiro de conta direta ou um fornecedor indireto).

2. O parceiro negoceia com clientes novos ou existentes nos seguintes países:

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

Os parceiros que satisfaçam os critérios terão de submeter o **ID** de registo da empresa de um cliente (também conhecido como organização do cliente **INN)** e o número de **telefone** quando estiverem a bordo de novos clientes ou modificar os dados do cliente existentes. Estes parceiros também podem introduzir um **nome do meio** opcional para o cliente.

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

Os parceiros com clientes no resto do mundo terão a capacidade, no dia 25 de março de 2021, de introduzir o ID de registo da **empresa,** **número de telefone** e nome do **meio** para os clientes como detalhes opcionais.

### <a name="next-steps"></a>Passos seguintes

- Reveja a documentação técnica e questione frequentemente na [coleção de parceiros dedicados](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) para obter uma orientação mais detalhada.

- Prepare-se para incorporar as alterações utilizando a API do Partner Center e a experiência do utilizador web. A API/SDKs estará disponível para testes.

- Certifique-se de submeter os dados adicionais ao embarcar em novos clientes ou modificar os dados do cliente existentes.

- Se estiver a utilizar uma solução de fornecedor de painéis de controlo (CPV), consulte o seu CPV.

### <a name="questions"></a>Perguntas?

Contacte o seu consultor fiscal ou o fisco local se tiver alguma questão relacionada com o identificador legal (também chamado INN ou TIN). A Microsoft não pode fornecer orientações sobre questões fiscais.

Se precisar de apoio nas suas operações com a Microsoft, [abra um pedido de serviço](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).

________________
## <a name="corrections-made-to-march-1-2021-perpetual-software-price-list"></a><a name="15"></a>Correções feitas até 1 de março de 2021 lista de preços perpétuos de software

### <a name="categories"></a>Categorias

- Data: 2021-03-23
- Ofertas/Mercados

### <a name="impacted-audience"></a>Audiência impactada

Fornecedores indiretos e parceiros de conta direta que transfiram software perpétuo no programa Fornecedor de Soluções em Nuvem 

### <a name="details"></a>Detalhes

A lista de preços do software perpétuo publicada a 1 de março de 2021 incluía mercados que não deveriam ter estado lá. A lista de preços perpétuos de software foi atualizada em 17 de março de 2021 com as correções. Estas correções só se aplicavam:

- ID do produto: DF77X4D43RKT 
- Nome do produto: Windows 10 Home para Pro atualização para Microsoft 365 Negócios
- Mercados removidos ou não apoiados: AE, AF, AL, AM, AO, BA, BB, BD, BH, BM, BN, BO, BR, BS, BW, BY, BZ, CI, CL, CM, CO, CR, CW, DO, DZ, EC, EG, ET, FJ, FO, GE, GH, GT, HN, IL, IN, IQ, JM, JO, KE, KG, KN, KW, KY, KZ, LB, LK, LY, MA, M, M, MD, MED, , MN, MO, MU, NA, NG, NI, NP, OM, PA, PE, PH, PK, PR, PY, QA, RS, RU, RW, SG, SN, SV, TH, TJ, TM, TN, TT, TZ, UA, UG, UY, UZ, VE, VN, YE, ZM, ZW

Estas alterações aplicam-se apenas ao produto acima referido. Outros produtos não tinham correções. 

### <a name="next-steps-and-resources"></a>Próximos passos e recursos

- Os parceiros que transacionam software perpétuo devem descarregar a mais recente lista de preços perpétuos de software.
- Consulte os [códigos dos países](/azure/marketplace/commercial-marketplace-co-sell-countries) da região para um mapeamento amigável da abreviatura de duas letras para os países.
________________
## <a name="sdk-release-on-net-standard-v1170"></a><a name="14"></a> Lançamento SDK em .NET Standard (v1.17.0)

### <a name="categories"></a>Categorias

- Data: 2021-03-23

- Capacidades
 
### <a name="impacted-audience"></a>Audiência impactada

Parceiros Direct Bill e Fornecedores Indiretos que participam no programa CSP que estão a utilizar o Partner Center .NET SDK.

### <a name="details"></a>Detalhes

A partir de 23 de março de 2020, os Parceiros podem começar a descarregar a versão do [MicrosoftPartnerCenter.NETSDK (NuGet Gallery | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0), juntamente com [amostras](https://github.com/Microsoft/Partner-Center-DotNet-Samples)atualizadas do Centro De Parceiros SDK GitHub . Esta versão inclui atualizações aos seguintes métodos:

#### <a name="audit-updated-new-operation-types"></a>Auditoria Atualizada: Novos tipos de operação

Adicione novos [tipos de operação](/partner-center/develop/auditing-resources) para saber quando o cliente aprovou e encerrou o DAP.

- DapAdminRelationshipApproved

- DapAdminRelationshipTerminated

#### <a name="audit-updated-new-resource-and-operation-types"></a>Auditoria Atualizada: Novos tipos de recursos e de operação

Adicionou novos [tipos de recursos e de operação](/partner-center/develop/auditing-resources) para apoiar o cenário de função do diretório do cliente.

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
- Baixar e rever as [amostras de GitHub](https://github.com/Microsoft/Partner-Center-DotNet-Samples)

________________
## <a name="csp-commercial-marketplace-offer-and-fy21-csp-incentives-for-eligible-offers"></a><a name="13"></a>Oferta de mercado comercial da CSP e incentivos ao CDS para ofertas elegíveis

### <a name="categories"></a>Categorias

- Data: 2021-03-18
- Capacidades

### <a name="impacted-audience"></a>Audiência impactada

Fornecedores indiretos e parceiros de conta direto no programa Fornecedor de Soluções em Nuvem 

### <a name="details"></a>Detalhes

Os fornecedores indiretos e parceiros de conta direta no programa Fornecedor de Soluções em Nuvem podem vender ofertas de terceiros e ganhar um incentivo de desconto para cada oferta de terceiros elegível transacionada no Partner Center ou no portal Azure. O incentivo será sob a forma de um desconto nas vendas faturadas para as ofertas elegíveis e está **disponível até 30 de junho de 2021**.  

Continue a aprender sobre este incentivo CSP Commercial Marketplace Offer abaixo e contacte os seus clientes hoje para identificar as ofertas certas para permitir o seu sucesso contínuo e transformação digital.

Fazemos parcerias com fornecedores de software independentes (ISVs) para trazer as mais recentes soluções IaaS e SaaS para o mercado para os clientes da Microsoft. Os editores da ISV têm a opção de permitir a venda das suas ofertas através do canal parceiro da Microsoft. As nossas ofertas elegíveis para incentivos enquadram-se em duas categorias:

- Selecione ofertas de terceiros SaaS e IaaS com o estado de co-venda do Azure IP. 

- Aplicações SaaS integradas com Teams ou pelo menos duas aplicações de produtividade Microsoft 365, tais como PowerPoint, Word, Excel, Outlook ou SharePoint.

### <a name="next-steps-and-resources"></a>Próximos passos e recursos

- Saiba mais sobre o ganho [de Incentivos a Parceiros](https://partner.microsoft.com/membership/partner-incentives) para a venda de aplicações elegíveis para o mercado, as aplicações elegíveis para incentivos. Novas ofertas são adicionadas mensalmente.  
- [Fornecedor de Soluções em Nuvem recursos de incentivo diretos para parceiros de conta](https://partner.microsoft.com/asset/collection/cloud-solution-provider-direct-partner-incentive-resources#/)
- [Fornecedor de Soluções em Nuvem recursos de incentivo indiretos do prestador](https://partner.microsoft.com/asset/collection/cloud-solution-provider-indirect-provider-incentive-resources#/)
- Reveja esta [apresentação](https://partner.microsoft.com/resources/detail/partner-center-cm-for-csp-overview-pdf) para saber mais sobre a venda das aplicações de marketplace comercial. Confira os recursos adicionais [aqui.](https://partner.microsoft.com/resources/collection/partner-center-cm-for-csp-collection#/) 
- Explore o catálogo de marketplace comercial no [Partner Center](../csp-commercial-marketplace-discover.md) ou no [portal Azure](https://ms.portal.azure.com/#home)
- Utilize [APIs](/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market) para integrar apps no mercado da sua empresa
- Contacte os ISVs com os que está interessado em fazer negócios
- Os fornecedores indiretos precisam de integrar usando APIs e guiar revendedores em que apps vender

### <a name="questions"></a>Perguntas?  

Consulte [este artigo](../csp-commercial-marketplace-overview.md) para obter uma visão geral do mercado comercial no Partner Center.

Se precisar de assistência adicional, pode criar um pedido de apoio no Partner Center. Saiba mais em [https://aka.ms/IncentivesSupport](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=1) .

________________
## <a name="power-bi-premium-offer-naming-and-prerequisite-update"></a><a name="12"></a>Power BI Premium oferecem nomeação e atualização pré-requisito

### <a name="categories"></a>Categorias

- Data: 2021-03-18
- Capacidades

### <a name="summary"></a>Resumo

A lista final de preços de 1 de abril de 2021 será atualizada para adicionar clareza ao nome e/ou informações pré-requisitos para Power BI Premium ofertas por Utilizador.

### <a name="impacted-audience"></a>Audiência impactada

Fornecedor de Soluções em Nuvem (CSP) parceiros diretos e indiretos

### <a name="details"></a>Detalhes

A lista final de preços de 1 de abril de 2021 será atualizada para adicionar clareza ao nome e/ou informações pré-requisitos para Power BI Premium ofertas por Utilizador.

Até que a lista final de preços seja atualizada, utilize as informações nesta secção para garantir que o produto correto é encomendado.

Os seguintes detalhes mostram o SKU afetado e os detalhes pré-requisitos.

| Oferta nome de exibição na pré-visualização da lista de preços de 1 de março |  Nome de exibição de oferta atualizado na lista final de preços de 1 de abril| ID da oferta |
| ------ | ----------- | ----------- |
| Power BI Premium Por Add-On de utilizador (preços de pessoal sem fins lucrativos)  |  Power BI Premium Por Add-On de utilizador **(Office)** (Preços do Pessoal sem fins lucrativos)   | 31c03289-47ab-4ab0-8df1-03742c127ac6   |

Os clientes são obrigados a ter qualquer um dos seguintes pré-requisitos para comprar esta oferta:

| Oferta nome de exibição | ID da oferta |
| ------ | ----------- |
| Microsoft 365 E5 (Preços do Pessoal Sem Fins Lucrativos)  |  31bedf01-9e57-4ece-a53a-d3656a563931   |
|   Microsoft 365 E5 sem AudioConferência (Preços do Pessoal Sem Fins Lucrativos)|  b456810a-c414-4e07-98fc-ef74e8175a09|
|   Office 365 E5 (Preços do Pessoal sem fins lucrativos)| ce139fe5-8bd5-47ed-a5be-07c286f8b9e    |
|   Office 365 E5 (Preço do Pessoal Sem Fins Lucrativos)|  2f192efe-608a-4c9c-9d19-2b0b70b0962e|
|   Office 365 E5 sem AudioConferência (Preços do Pessoal Sem Fins Lucrativos)|  c3897426-9f49-4eaf-9b4d-7d9a1c72aef7|

A seguinte oferta Power BI Premium tem um pré-requisito necessário para a compra:

| Oferta nome de exibição | ID da oferta |
| ------ | ----------- |
|   Power BI Premium Por Add-On de utilizador (preços de pessoal sem fins lucrativos)|  ef0b895b-681b-4026-a5b1-dda182a57d40 |

Os clientes são obrigados a ter este pré-requisito para a compra desta oferta:

| Oferta nome de exibição | ID da oferta |
| ------ |----------|
| Power BI Pro (Preços do Pessoal Sem Fins Lucrativos)  |   cabdfc93-5786-4224-bfd3-35d58f833b35 |

### <a name="next-steps"></a>Passos seguintes

Reveja os recursos sobre este tema e partilhe esta informação com as partes interessadas apropriadas na sua organização.  

### <a name="questions"></a>Perguntas?

Para quaisquer questões sobre estas ofertas, consulte as suas comunidades Yammer relevantes. 

## <a name="march-price-updates-for-microsoft-365-f3"></a><a name="11"></a>Atualizações de preços de março para Microsoft 365 F3

### <a name="categories"></a>Categorias

- Data: 2021-03-16
- Ofertas/Mercados

### <a name="summary"></a>Resumo

Os preços de março de 2021 estão corrigidos para Microsoft 365 F3 Libra Britânica (GBP) e Euro (EUR).

### <a name="impacted-audience"></a>Audiência impactada

Os parceiros que compram Microsoft 365 F3 em GBP ou EUR entre 1 de março e 17 de março de 2021 através do programa Fornecedor de Soluções em Nuvem (CSP).

### <a name="details"></a>Detalhes

A Microsoft resolveu preços incorretos para Microsoft 365 F3. Os preços incorretos foram para GBP e EUR e apenas para ofertas adquiridas entre 1 de março e 17 de março de 2021. As ofertas e moedas impactadas estão listadas abaixo. 

| Nome da oferta | Moeda | ID da oferta | Material ID |
| ------ |----------- |----------- |----------- |
| Microsoft 365 F3 (Caridade) | GBP | 57b722c2-c435-4bfb-9bc8-80509213a13a | AAD-11626 |
| Microsoft 365 F3 (Comercial) | EUR| 3451a3b0-8cda-44a7-bad7-c30be81c4aaa | AAA-89898 |
 
As listas de preços base de licença de março e abril foram atualizadas a 16 de março, 17:00 horas.

### <a name="next-steps"></a>Passos seguintes

- Os parceiros devem reencaitar as atuais listas de preços baseadas em licenças, tanto em março como na pré-visualização de abril, com estas correções de preços, se aplicável.  
- A Microsoft entrará em contacto com parceiros impactados nas próximas semanas por e-mail para os informar dos próximos passos relacionados com a correção das transações afetadas.

### <a name="questions"></a>Perguntas?

Para mais perguntas, verifique as suas comunidades Yammer CSP relevantes.

________________

## <a name="update-a-legal-company-name-through-partner-center"></a><a name="10"></a> Atualize um nome legal da empresa através do Partner Center

### <a name="categories"></a>Categorias

- Data: 2021-03-16
- Escala de & de eficiência de unidade

### <a name="summary"></a>Resumo

A partir de março de 2021, os parceiros da Microsoft Partner Network (MPN) e os revendedores indiretos Fornecedor de Soluções em Nuvem (CSP) podem atualizar o nome da empresa legal através do Partner Center.

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

Para mais perguntas, verifique as suas comunidades Yammer CSP relevantes.

________________
## <a name="update-to-cloud-solution-provider-csp-program-evolution-and-open-license-program-changes"></a><a name="9"></a>Atualização para a evolução do programa Fornecedor de Soluções em Nuvem (CSP) e alterações do programa Open License

### <a name="categories"></a>Categorias

- Data: 2021-03-15
- Capacidades

### <a name="summary"></a>Resumo

Novas ofertas de software perpétuo do sector comercial e público estão a chegar ao programa Fornecedor de Soluções em Nuvem (CSP) juntamente com alterações ao programa open licensing.

### <a name="impacted-audience"></a>Audiência impactada

Distribuidores comerciais e revendedores geridos que vendem através do programa Open License, bem como todos os parceiros da CSP que transacionam software perpétuo

### <a name="details"></a>Detalhes

Em setembro de 2020, a Microsoft [anunciou](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) uma série de passos na nossa jornada de transformação digital para expandir oportunidades aos parceiros no programa CSP, incluindo a disponibilidade de software no local para parceiros. Estas mudanças permitem que os parceiros cresçam o seu negócio e aumentem o seu alcance, aproveitando as licenças de software na CSP, posicionando-as para o sucesso no mundo atual em nuvem. Também capacitam as transições dos clientes para a nuvem e dão aos parceiros a flexibilidade necessária para ambientes de nuvem híbrida do cliente.

Na continuação desta transformação digital, anunciamos as seguintes alterações:

- 1 de julho de 2021: Não serão adicionados novos SKUs, produtos ou promoções à lista de preços do programa Open License.

- 7 de julho de 2021: Duas ofertas comerciais, Get Genuine Windows e Visual Studio Professional, e ofertas do setor público (governo, educação e sem fins lucrativos – ver [anúncio](./2020-december.md#9)) serão adicionadas à lista de preços perpétuos de software da CSP.  A lista de preços pode ser encontrada na secção de Software da página [de venda > de preços & Ofertas](https://partnercenter.microsoft.com/pcv/sales) no Partner Center e será republica nesta data.

Para obter detalhes completos sobre a evolução do programa CSP e alterações no programa Open License, consulte os **Próximos Passos** abaixo.

### <a name="next-steps"></a>Passos Seguintes:

- Evolução do Programa CSP: Reveja o [software Perpétuo nos materiais de](https://partner.microsoft.com/resources/collection/software-in-csp#/) prontidão do programa Fornecedor de Soluções em Nuvem. Use este [mapa de prontidão](https://partner.microsoft.com/resources/detail/software-in-csp-readiness-map-pdf) para localizar rapidamente as informações certas para o seu papel.

- Alterações no programa De Licença Aberta: Rever a evolução do [programa CSP e o programa Open License altera os](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/) materiais de prontidão. Use este [mapa de prontidão](https://partner.microsoft.com/resources/detail/csp-open-evolution-to-a-better-experience-readiness-map-pdf) para localizar rapidamente as informações certas para o seu papel.

### <a name="questions"></a>Perguntas

Para mais perguntas, verifique as suas comunidades Yammer CSP relevantes.

_______________
## <a name="update-to-a-previous-announcement-premium-assessments-an-add-on-to-compliance-manager"></a><a name="8"></a>Atualização para um anúncio anterior: Premium Assessments, um add-on ao Compliance Manager

### <a name="categories"></a>Categorias

- Data: 2021-03-15
- Expandir o seu negócio

### <a name="summary"></a>Resumo

As ofertas de julgamento não deveriam ter sido listadas na lista de preços e serão removidas.

### <a name="impacted-audience"></a>Audiência impactada

Parceiros transacionando através de Fornecedor de Soluções em Nuvem

### <a name="details"></a>Detalhes

As ofertas de julgamento não deviam ter sido incluídas na lista de preços. Estes serão removidos da lista de preços de 1 de maio de 2021.

O anúncio original está [aqui.](./2021-february.md#4)

### <a name="additional-resources"></a>Recursos adicionais

- [Microsoft 365 E5 segurança e conformidade](https://www.microsoft.com/licensing/product-licensing/microsoft-365-enterprise?activetab=m365-enterprise:primaryr5)

- [Construir e gerir avaliações no Microsoft Compliance Manager - Microsoft 365 Compliance](/microsoft-365/compliance/compliance-manager-assessments)

### <a name="next-steps"></a>Passos seguintes

Reveja os recursos sobre este tema e partilhe esta informação com as partes interessadas apropriadas na sua organização.

### <a name="questions"></a>Perguntas?

Para questões sobre estas ofertas, consulte as suas comunidades Yammer relevantes.

________________
## <a name="migrate-your-solutions-from-one-commercial-partner-ocp-go-to-market-gtm-to-the-microsoft-commercial-marketplace"></a><a name="7"></a> Migrar as suas soluções de One Commercial Partner (OCP) go-to market (GTM) para o mercado comercial da Microsoft

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
## <a name="programmatic-access-to-commercial-marketplace-analytics"></a><a name="6"></a>Acesso programático à análise do mercado comercial

### <a name="categories"></a>Categorias

- Data: 2021-03-10
- Capacidades

### <a name="summary"></a>Resumo

Os parceiros podem agora aceder programáticamente a relatórios de análise para monitorizar as vendas, avaliar o desempenho e otimizar ofertas no mercado comercial.

### <a name="impacted-audience"></a>Audiência impactada

Parceiros com ofertas no mercado comercial.

### <a name="details"></a>Detalhes

A API para aceder a relatórios de marketplace comercial permite-lhe agendar relatórios personalizados dos seus dados de análise assíncronos.

A capacidade permite-lhe definir consultas e modelos de reporte com base nas suas necessidades, definir um horário e obter relatórios atempadamente e de confiança em intervalos programados.

### <a name="next-steps"></a>Passos seguintes

Para saber mais, consulte [Começar com acesso programático à análise.](/azure/marketplace/analytics-get-started)

### <a name="questions"></a>Perguntas?

Contacte [o Suporte](https://go.microsoft.com/fwlink/?linkid=2165533) se tiver mais perguntas.

________________
## <a name="expanding-the-new-commerce-experience-in-the-cloud-solution-provider-csp-program-for-azure-to-russia"></a><a name="5"></a>Expandir a nova experiência de comércio no programa Fornecedor de Soluções em Nuvem (CSP) para o Azure à Rússia

### <a name="categories"></a>Categorias

- Data: 2021-03-10
- Capacidades

### <a name="impacted-audience"></a>Audiência impactada

Todos os parceiros na Rússia transacionam através do programa Fornecedor de Soluções em Nuvem (CSP).

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

Todos os Fornecedor de Soluções em Nuvem parceiros (CSP) transting encomendas de software de subscrição perpétua e servidor através do Partner Center

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
## <a name="migrate-your-deals-from-partner-sales-connect-psc-to-partner-center"></a><a name="3"></a>Migrar as suas ofertas de Ligação de Vendas de Parceiros (PSC) para Partner Center

### <a name="categories"></a>Categorias

- Data: 2021-03-04
- Capacidades

### <a name="summary"></a>Resumo

A Partner Sales Ligação (PSC) passará para o acesso apenas à leitura a partir de 31 de março de 2021, pelo que pedimos que comece a migrar as suas ofertas do PSC para o Partner Center.

### <a name="impacted-audience"></a>Audiência impactada

Parceiros com negócios no PSC

### <a name="details"></a>Detalhes

Como parte do nosso compromisso comum com o crescimento, **co-vender com** a Microsoft é o caminho para que **você seja descoberto, entregue a sua experiência e expanda a sua pegada de cliente** para resultados positivos do cliente. Com uma oferta média **3,5 vezes mais rápida** do que o normal, gerir a sua experiência de co-venda no Partner Center permite-lhe vender através dos canais de clientes diretos, parceiro e vendedor da Microsoft, e gerir todo o seu pipeline de referência num local.

**O PSC** passará a **ter acesso apenas** a leitura a partir de 31 de março de **2021,** por isso pedimos-lhe que inicie a sua mudança para o Partner Center e aceda a estas melhorias de capacidade: 

- **Encaminhamento mais preciso** das ofertas que partilha com a Microsoft para o vendedor certo, com base no tipo de assistência que necessita.
- **Validação de elegibilidade do negócio inicial** para soluções elegíveis para incentivos e para cumprir os critérios do programa isv Ligação, simplificando o processo de aprovação e a prova final de execução (POE).
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

No dia 1 de abril de 2021, a Microsoft lançará vários novos produtos e ofertas para o programa Fornecedor de Soluções em Nuvem (CSP).

### <a name="impacted-audience"></a>Audiência impactada

Todos os parceiros que transfiram através do programa Fornecedor de Soluções em Nuvem (CSP)

### <a name="details"></a>Detalhes

No dia 1 de abril de 2021, a Microsoft lançará os seguintes novos produtos e ofertas:

- Power BI Premium Por Utilizador
- Expansão geo e segmento usl de voz do cliente e marketing USL

**Power BI Premium Por Utilizador**

A Microsoft introduzirá as primeiras ofertas de Power BI Premium por utilizador. Power BI Premium é atualmente vendida apenas numa construção de capacidade. Power BI Premium Por Utilizador fornece acesso a inteligência empresarial (BI) e capacidades de análise. O seu licenciamento individual flexível atende às pequenas e médias empresas.

Reveja os [detalhes Power BI de lançamento](/power-platform-release-plan/2020wave2/power-bi/planned-features) para saber mais sobre esta oferta.


**Oferecer detalhes**

Note que o nome da oferta difere ligeiramente da pré-visualização da lista de preços.

| Nome da oferta | ID da oferta |
| ------ |----------- |
| Power BI Premium Por Utilizador | 9c810018-9356-4903-95ab-eeb956289290 | 
| Power BI Premium Por Utilizador para Faculdade | 3affc44f-f372-4ad5-8657-aadd9574fce0 | 
| Power BI Premium Por Utilizador para Estudantes | 657eea87-d0b0-4c89-8c8e-9b04395bd940 | 
| Power BI Premium Por Utilizador (Preços do Pessoal sem fins lucrativos) | 7a0a856c-059f-45dd-9d26-ae27992e706a | 
| Power BI Premium Por Add-On de utilizador | 244ff87e-5925-44a0-bf31-cea189719b58 | 
| Power BI Premium Por Add-On de utilizador para faculdade | 5da849bd-b8f7-4340-b4f4-3a9eaeb8987e | 
| Power BI Premium Por Add-On de utilizador para estudantes | cf62d70d-5af5-422a-bda8-97936402ac8e | 
| Power BI Premium Por Add-On de utilizador (preços de pessoal sem fins lucrativos) | 31c03289-47ab-4ab0-8df1-03742c127ac6 | 

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

- Data: 2021-03-03
- Capacidades

### <a name="summary"></a>Resumo

A Microsoft Universal Print estará disponível para transacionar dentro de Microsoft 365 suites selecionadas e como um addon autónomo a partir de 1 de março de 2021.

### <a name="impacted-audience"></a>Audiência impactada

Todos os parceiros que transfiram através do programa Fornecedor de Soluções em Nuvem (CSP)

### <a name="details"></a>Detalhes

[Universal Print](https://aka.ms/universalprint) é um serviço de impressão Microsoft 365 que remove a necessidade de servidores de impressão no local, e permite que Windows dispositivos imprimam para impressoras registadas em Azure. Estará disponível para transações a partir de 1 de março de 2021.

Os trabalhadores beneficiam da impressão sem condutor, da descoberta da impressora baseada em localização e de uma experiência de impressão intuitiva sem curva de aprendizagem. Os dispositivos que se unem ao Azure Ative Directory (Azure AD) utilizam credenciais AZure AD existentes para imprimir de forma segura. Os administradores gerem a impressão utilizando o portal Azure e podem facilmente ligar impressoras com suporte nativo para impressão universal. A Impressão Universal pode ser implantada com impressoras não compatíveis utilizando conector de Impressão Universal software.

A Universal Print será reabastetada no lançamento para Windows E3, A3, E5 e A5, e Microsoft 365 BP, F3, E3, A3, E5 e A5.  

**Oferecer detalhes**

Note que o nome da oferta difere ligeiramente da pré-visualização da lista de preços.

| Nome da oferta | ID da oferta | Material ID |
| ------ |----------- |----------- |  
| Complemento de volume de impressão universal (500 empregos) - Microsoft 365  | cb131356-45ee-4ae2-8537-873b706c8e75     | 9BI-00004   |
| Complemento de volume de impressão universal (500 postos de trabalho) para docentes - Microsoft 365   | 477bee81-9872-43d6-91d3-c72390bfcf49   | 9BK-00004   |
| Complemento de volume de impressão universal (500 empregos) - Windows    | d3ddc493-5741-4e0d-a02d-07edbb72e   | 9BI-00002   |
| Complemento de volume de impressão universal (500 postos de trabalho) para docentes - Windows   |  d0862f05-80f5-4fd4-8432-fe72dd893cc7  | 9BK-00002   |

### <a name="next-steps"></a>Passos seguintes

Familiarize-se com a tabela de preços e a [visão geral](/universal-print/fundamentals/universal-print-whatis)da Impressão Universal . Partilhe esta informação com todos os contactos apropriados na sua organização.

### <a name="questions"></a>Perguntas?

Para quaisquer questões sobre estas ofertas, consulte as suas comunidades Yammer relevantes.