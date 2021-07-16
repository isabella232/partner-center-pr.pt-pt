---
title: Atribuir funções & permissões aos utilizadores
ms.topic: article
ms.date: 10/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba quais as funções mais bem possíveis para os utilizadores da sua empresa que gerem transações comerciais, referências, incentivos ou membros mpn no Partner Center.
author: hemas
ms.author: hemas
ms.localizationpriority: high
ms.custom: SEOMAY.20, contperf-fy21q1
ms.openlocfilehash: a9cca322d7a37dce099c5bec44530b2006da7758
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/16/2021
ms.locfileid: "114373662"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a>Atribuir funções e permissões aos utilizadores de uma empresa que necessite de trabalhar no Partner Center

**Funções adequadas**: Administração global | Administração de administração de utilizadores | Administrador sócio da MPN

Configura o seu perfil de parceiro, incluindo nome legal e morada, detalhes de apoio, isenções de impostos, informações bancárias e o contacto principal para a sua empresa. Próximo passo: Configurar os seus utilizadores com senhas e funções para que possam começar a trabalhar no Partner Center consigo.

## <a name="set-up-your-employees-to-work-in-partner-center"></a>Configurar os seus colaboradores para trabalhar no Partner Center

Você determina os tipos de acesso que os seus utilizadores têm para Partner Center pelas funções e permissões que lhes dá. As funções estão relacionadas com o(s) programa(s) em que o seu negócio está envolvido. Por exemplo, se o seu negócio for um negócio Fornecedor de Soluções em Nuvem (CSP), não só terá as funções de gestão de inquilinos standard Azure Ative Directory (Azure AD), como a administração global, mas precisará de papéis específicos do programa CSP. Cada programa tem papéis específicos.

>[!Note]
> As funções de inquilino da AZure AD incluem funções de administrador global, administração de utilizadores e CSP. As funções não-Azure-AD são as funções que não gerem o inquilino, e incluem a administração de parceiros MPN (Microsoft Partner Network), administração de perfil de negócios, administração de encaminhamento, administração de incentivos e utilizador de incentivos. 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a>Gerir transações comerciais em Partner Center (funções Azure AD e CSP)

|**Role**|**O que podem fazer**|**Saiba mais**|
|----------------------------------|---|:---------------------------------|
|Administrador global|* Pode aceder a todas as contas/serviços da Microsoft com plenos privilégios|[Manage your Partner Center account](partner-center-account-setup.md) (Gerir a conta do Partner Center)
|      |* Crie bilhetes de apoio para o Centro de Parceiros
||* Ver bilhetes de apoio a parceiros que criar
||* Ver acordos, listas de preços e ofertas
||* Ver, criar e gerir utilizadores parceiros|
||  Ver, criar e gerir ficheiros de faturação, faturas e recon
|Administração de gestão de utilizadores   | * Ver, criar e gerir utilizadores|[Gerencie os benefícios e ofertas de adesão da Microsoft Partner Network no Partner Center](manage-your-partner-network-benefits.md)
||* Ver todos os perfis de parceiros
||* Crie bilhetes de apoio para o Centro de Parceiros
||* Ver bilhetes de apoio a parceiros que criar
|Administrador de faturação | - Ver, criar e gerir ficheiros de faturação, faturas e recon|[Read your bill](billing.md) (Ler a sua fatura)
||* Ver preços
||* Crie bilhetes de apoio para o Centro de Parceiros
||* Ver bilhetes de apoio a parceiros que criar
|Utilizador predefinido|  Ver o meu perfil   |[Repor a palavra-passe](reset-my-pasword.md)
|Agente administrativo | * Gestão de clientes|[Ligar-se aos seus clientes](connect-with-your-customers.md)
||* Adicione a lista de dispositivos ao Centro de Parceiros
||* Criar e aplicar perfis em dispositivos
||* Gestão de assinaturas
||* Pedidos de saúde e serviço de serviço para os clientes
||* Solicitar privilégios de administrador delegado
||* Ver preços e ofertas
||* Faturação
||* Administrar em nome de um cliente
||* Registar um revendedor de valor acrescentado
||* Crie bilhetes de apoio para o Centro de Parceiros
||* Ver bilhetes de apoio a parceiros que criar|
|Agente comercial | * Gestão de clientes|[Fornecer suporte de faturação para os seus clientes e ajudar a responder às suas questões de faturação](provide-billing-support.md)
||* Adicione a lista de dispositivos ao Centro de Parceiros
||* Gestão de assinaturas
||* Ver bilhetes de apoio
||* Solicite uma relação com um cliente
||* Ver preços e ofertas
||* Gerir os condutores do cliente
||* Ver o contrato de cliente
||* Registar um revendedor de valor acrescentado
||* Crie bilhetes de apoio para o Centro de Parceiros
||* Ver bilhetes de apoio a parceiros que criar|
|Agente helpdesk| * Procurar e ver um cliente|[Aumente os problemas para a Microsoft e saiba quais os problemas mais adequados à escalada da Microsoft](escalate-problems-to-microsoft.md)
||* Editar detalhes do cliente
||* Ajude a resolver problemas de clientes com faturação ou gestão de subscrição
||* Solicitar apoio em nome dos clientes 
||* Gerir subscrições e questões de faturação em nome dos clientes
||* Crie bilhetes de apoio para o Centro de Parceiros
||* Ver bilhetes de apoio a parceiros que criar| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-azure-ad-role"></a>Fornecedor de painel de controlo (CPV). (papel da CSP e papel de AD não-Azure)

Os CPVs desenvolvem aplicações para utilização por parceiros CSP para lhes permitir integrar os seus sistemas com APIs do Partner Center. 

|**Role**   |**O que pode fazer**|**Saiba mais**|
|------------------------------|:----------------------------|----|
|Administrador global| Ver e gerir o seu perfil de Fornecedor de Painéis de Controlo (CPV)|[Inscreva-se como fornecedor de painéis de controlo para ajudar a integrar sistemas parceiros CSP com APIs do Partner Center](enroll-as-cpv.md)
||Ver e gerir qualquer um dos seus utilizadores que necessite de acesso às capacidades do CPV|

### <a name="guest-user-must-be-added-to-the-azure-ad-tenant"></a>Utilizador convidado (deve ser adicionado ao inquilino AZure AD)

|**Utilizador convidado**   | **Funções**|
|---------------------------|:--------------------|
||Administrador sócio da MPN|
||Administrador de perfil de negócios|
||Administração de referências|


## <a name="manage-mpn-membership-and-your-company"></a>Gerir a adesão à MPN e à sua empresa 

Estes papéis não são papéis de AD Azure. Estas funções gerem o negócio da empresa e não o inquilino.

|**Role** | **O que pode fazer**|**Saiba mais**|
|----------------------------|:----------------------------|-----|
|Administrador sócio da MPN|* Ver, criar e gerir pedidos de serviço de parceiros|[Comprar ou renovar uma subscrição do Microsoft Action Pack ou competências Silver e Gold](mpn-get-action-pack.md)
||* Ver perfis legais, empresariais, empresariais e MPN
||* Ver detalhes do utilizador e seus dados de competências
||* Ver competências
||* Ver e gerir benefícios
||* Ver e comprar ofertas mpn
||* Ver MPN oferece histórico de encomendas e faturas
||* Ver dados do indicador de contribuição do parceiro
||* Pode funcionar na ferramenta de validação do voucher|
||* Ver análise de dados do cliente
||* Ver outras funções de utilizador dentro da empresa, mas não pode atribuir funções
||* Crie bilhetes de apoio para o Centro de Parceiros
||* Ver bilhetes de apoio a parceiros que criar
|Administrador de conta| Adicionar localizações|[Gerir localizações](manage-locations.md)
|| Gerir perfis relacionados com as contas para as contas para as contas para as que é administrador 
||* Atribuir funções para utilizadores em arrendatários a funções não-Azure-AD 
||* Inscrever localizações em programas
||* Crie bilhetes de apoio para o Centro de Parceiros
||* Ver bilhetes de apoio a parceiros que criar

## <a name="manage-referrals"></a>Gerir referências

|**Role** | **O que pode fazer**|**Saiba mais**
|------------------------------|:-------------------------|---|
|Administração de referências|Criar e gerir tudo sob o separador Referências no Centro de Parceiros|[Gerir oportunidades de Venda conjunta](manage-co-sell-opportunities.md)
||    Pode ver e editar todas as oportunidades e pistas de co-venda
||    Pode atribuir membros da equipa para um acordo
||    Pode ver e editar perfis de negócio
||    Pode ver e registar ofertas para oportunidades que são marcadas como ganhas e elegíveis para registo de negócios
||    Pode criar e ver bilhetes de apoio
|Utilizador de referências|Criar e gerir oportunidades de co-venda apenas se fizerem parte da equipa |[Gerir oportunidades de Venda conjunta](manage-co-sell-opportunities.md)
||    Pode criar oportunidades de co-venda para os locais onde lhes é atribuído o papel.
||    Pode visualizar e registar ofertas para oportunidades que são marcadas como ganhas e elegíveis para registo de negócios se forem membros da equipa.
||    Pode criar e ver bilhetes de apoio
|Administrador de perfil de negócios|Criar e gerir perfis de negócio | [Gerir perfis de negócio](create-a-marketing-profile.md)
||    Pode criar e ver bilhetes de apoio

Juntamente com a nova função de utilizador de referências, estamos também a introduzir a margem de localização para as ofertas. A tabela abaixo explica o acesso às ofertas com base no local.

|**Âmbito** | **O que pode fazer** |
|------------------------------|:-------------------------|
|Empresa inteira | Tanto os administradores como os utilizadores têm acesso a criar ofertas para qualquer localização na sua empresa|
|| Administração de referência tem acesso a visualização e edição de todos os negócios |
|| Os utilizadores de referência têm acesso a visualização e edição de todas as ofertas apenas se fizerem parte da equipa |
|Um ou mais locais | Tanto os administradores como os utilizadores têm acesso a criar ofertas para a localização atribuída na sua empresa|
|| O administrador de referência tem acesso para visualizar e editar todos os negócios pertencentes aos locais atribuídos|
|| Os utilizadores de referência têm acesso a visualização e edição de todas as ofertas pertencentes aos locais atribuídos se fizerem parte da equipa|

## <a name="manage-incentives"></a>Gerir incentivos

|**Role** | **O que pode fazer**|**Saiba mais**
|------------------------------|:-------------------------|---|
|Administradores de incentivos|* Inicia e gere incentivos |[Use estes recursos para ajudá-lo a começar com incentivos](incentives-get-started-intro.md)
||* Pode ver e editar todos os aspetos dos programas de incentivos
||* Pode ver e editar dados bancários e fiscais
||* Ver descontos e ganhos cooperativos
||* Suporte de acesso
||* Pagamentos de incentivos de litígios|
|Utilizador de incentivos|* Pode ver programas de incentivos
||* Pode ver e iniciar pedidos de incentivos
||* Ver descontos e ganhos cooperativos
||* Crie bilhetes de apoio para o Centro de Parceiros
||* Ver bilhetes de apoio a parceiros que criar

## <a name="view-partner-center-insights-data"></a>Ver dados de Informações do Centro de Parceiros

|**Role** | **O que pode fazer**|**Saiba mais**|
|------------------------------|:-------------------------|---|
|Espectador de relatório executivo|Acesso a todos os conjuntos de dados de reporte, criar bilhetes de apoio a parceiros, ver bilhetes de apoio a parceiros que criar|[Relatórios do painel de avaliação disponíveis no Partner Center Informações](insights-overview-report.md)
|Espectador de relatório|Acesso a relatórios de dados com exceção das receitas e dados pessoais do cliente e dos colaboradores, criar bilhetes de apoio ao parceiro, ver bilhetes de apoio a parceiros que criar|

## <a name="next-steps"></a>Passos seguintes

- [Create user accounts and assign roles permissions](create-user-accounts-and-set-permissions.md) (Criar contas de utilizador e atribuir funções e permissões)
- [Verifique as informações da sua conta quando se inscrever num novo programa do Partner Center](verification-responses.md)
