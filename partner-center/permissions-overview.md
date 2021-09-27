---
title: Atribuir funções e permissões a utilizadores
ms.topic: article
ms.date: 09/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-account
description: Saiba quais as funções que são melhores para os utilizadores da sua empresa que gerem transações comerciais, referências, incentivos ou membros mpn no Partner Center.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: high
ms.custom: SEOMAY.20, contperf-fy21q1
ms.openlocfilehash: 46d17de1ba7572c72162cfd38143ed9aa084c5c7
ms.sourcegitcommit: d731813da1d31519dc2dc583d17899e5cf4ec1b2
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/27/2021
ms.locfileid: "129075772"
---
# <a name="assign-roles-and-permissions-to-users"></a>Atribuir funções e permissões a utilizadores

**Funções adequadas**: Administração global | Administração de administração de utilizadores | Administrador sócio da MPN

Você definiu o seu perfil de parceiro, incluindo nome legal e endereço, detalhes de suporte, isenções de impostos de arquivo, informações bancárias e o contacto principal para a sua empresa. O seu próximo passo é configurar os seus utilizadores com senhas e funções para que possam começar a trabalhar no Partner Center consigo.

## <a name="set-up-your-employees-to-work-in-partner-center"></a>Configurar os seus colaboradores para trabalhar no Partner Center

Você determina os tipos de acesso que os seus utilizadores têm para Partner Center pelas funções e permissões que lhes dá. As funções estão relacionadas com o(s) programa(s) em que o seu negócio está envolvido. Por exemplo, se o seu negócio for um negócio Fornecedor de Soluções em Nuvem (CSP), não só terá as funções de gestão de inquilinos standard Azure Ative Directory (Azure AD), como a administração global, mas precisará de papéis específicos do programa CSP. Cada programa tem papéis específicos.

> [!NOTE]
> As funções de inquilino da AZure AD incluem funções de administrador global, administração de utilizadores e CSP. As funções não-Azure-AD são as funções que não gerem o inquilino, e incluem a administração parceira mpn (Microsoft Partner Network), administração de perfil de negócios, administração de encaminhamento, administração de incentivos e utilizador de incentivos. 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a>Gerir transações comerciais em Partner Center (funções Azure AD e CSP)

|**Role**|**O que podem fazer**| **Área de trabalho** | **Saiba mais**|
|----------------------------------|---|---|:---------------------------------|
|Administrador global|* Pode aceder a todas as contas/serviços da Microsoft com privilégios completos| Definições da conta | [Manage your Partner Center account](partner-center-account-setup.md) (Gerir a conta do Partner Center) |
||* Crie bilhetes de apoio para o Partner Center | Ajuda + suporte |
||* Ver bilhetes de apoio a parceiros que criar | Ajuda + suporte |
||* Ver acordos, listas de preços e ofertas | Preços |
||* Ver, criar e gerir utilizadores parceiros | Definições da conta |
||  Ver, criar e gerir ficheiros de faturação, faturas e recon | Faturação |
| Administrador de gestão de utilizadores   | * Ver, criar e gerir utilizadores| Benefícios | [Gerencie os benefícios e ofertas de adesão da Microsoft Partner Network no Partner Center](manage-your-partner-network-benefits.md)
||* Ver todos os perfis de parceiros | Clientes |
||* Crie bilhetes de apoio para o Centro de Parceiros | Ajuda + suporte |
||* Ver bilhetes de apoio a parceiros que criar | Ajuda + suporte |
|Administrador de faturação | - Ver, criar e gerir ficheiros de faturação, faturas e recon| Faturação | [Read your bill](billing.md) (Ler a sua fatura)
||* Ver preços | Faturação |
||* Crie bilhetes de apoio para o Centro de Parceiros | Ajuda + suporte |
||* Ver bilhetes de apoio a parceiros que criar | Ajuda + suporte |
|Utilizador predefinido|  Ver o meu perfil   | Definições da conta | [Repor a palavra-passe](reset-my-pasword.md)
|Agente administrativo | * Gestão do cliente| Clientes | [Ligar-se aos seus clientes](connect-with-your-customers.md)
||* Adicione a lista de dispositivos ao Centro de Parceiros | Definições da conta |
||* Criar e aplicar perfis em dispositivos | Definições da conta |
||* Gestão de assinaturas | Definições da conta |
||* Pedidos de saúde e serviço de serviço para os clientes | Ajuda + suporte |
||* Solicitar privilégios de administrador delegado | Definições da conta |
||* Ver preços e ofertas | Preços |
||* Faturação | Faturação |
||* Administrar em nome de um cliente | Definições da conta |
||* Registar um revendedor de valor acrescentado | Definições da conta |
||* Crie bilhetes de apoio para o Centro de Parceiros | Ajuda + suporte |
||* Ver bilhetes de apoio a parceiros que criar | Ajuda + suporte |
|Agente comercial | * Gestão do cliente| Faturação | [Fornecer suporte de faturação para os seus clientes e ajudar a responder às suas questões de faturação](provide-billing-support.md)
||* Adicione a lista de dispositivos ao Centro de Parceiros | Definições da conta |
||* Gestão de assinaturas | Definições da conta |
||* Ver bilhetes de apoio | Ajuda + suporte |
||* Solicite uma relação com um cliente | Clientes |
||* Ver preços e ofertas | Preços |
||* Gerir os condutores do cliente | Referências |
||* Ver o contrato de cliente | Clientes |
||* Inscreva um revendedor de valor acrescentado | Definições da conta |
||* Crie bilhetes de apoio para o Centro de Parceiros | Ajuda + suporte |
||* Ver bilhetes de apoio a parceiros que criar | Ajuda + suporte |
|Agente helpdesk| * Procurar e ver um cliente| Ajuda + suporte | [Aumente os problemas para a Microsoft e saiba quais os problemas mais adequados à escalada da Microsoft](escalate-problems-to-microsoft.md)
||* Editar detalhes do cliente  | Ajuda + suporte |
||* Ajude a resolver problemas de clientes com faturação ou gestão de subscrição | Ajuda + suporte |
||* Solicitar apoio em nome dos clientes | Ajuda + suporte |
||* Gerir subscrições e questões de faturação em nome dos clientes | Faturação |
||* Crie bilhetes de apoio para o Centro de Parceiros | Ajuda + suporte |
||* Ver bilhetes de apoio a parceiros que criar  | Ajuda + suporte |

### <a name="control-panel-vendor-cpv-csp-role-and-non-azure-ad-role"></a>Fornecedor de painéis de controlo (CPV). (papel CSP e papel de AD não-Azure)

Os CPVs desenvolvem aplicações para utilização por parceiros CSP para lhes permitir integrar os seus sistemas com APIs do Partner Center.

|**Role**                   | **O que pode fazer**      | **Área de trabalho** | **Saiba mais**|
|------------------------------|:----------------------------|---------------|---------------|
|Administrador global| Ver e gerir o seu perfil de Fornecedor de Painéis de Controlo (CPV)|  | [Inscreva-se como Fornecedor de Painel de Controlo para ajudar a integrar sistemas parceiros CSP com APIs do Partner Center](enroll-as-cpv.md)
||Ver e gerir qualquer um dos seus utilizadores que necessite de acesso às capacidades do CPV |  |

### <a name="guest-user-must-be-added-to-the-azure-ad-tenant"></a>Utilizador convidado (deve ser adicionado ao inquilino AZure AD)

| **Utilizador convidado**    | **Funções**            |
|----------------------|:------------------------|
|                      | Administrador sócio da MPN       |
|                      | Administrador de perfil de negócios  |
|                      | Administração de referências         |

## <a name="manage-mpn-membership-and-your-company"></a>Gerir a adesão à MPN e à sua empresa

Estes papéis **não** são papéis de AD Azure. São usados para gerir o negócio da empresa em vez do inquilino.

| **Role** | **O que pode fazer** | **Área de trabalho** | **Saiba mais**|
|----------------------------|:----------------------------|-----|
|Administrador sócio da MPN|* Ver, criar e gerir pedidos de serviço de parceiros| Membership | [Comprar ou renovar uma subscrição do Microsoft Action Pack ou competências Silver e Gold](mpn-get-action-pack.md) |
| |* Ver perfis legais, empresariais, empresariais e MPN | Definições da conta |
| |* Ver detalhes do utilizador e seus dados de competências | Membership |
| |* Ver competências | Membership |
| |* Ver e gerir benefícios | Benefícios |
| |* Ver e comprar ofertas mpn | Membership |
| |* Ver MPN oferece histórico de encomendas e faturas | Membership |
| |* Ver dados do indicador de contribuição do parceiro | Membership |
| |* Pode funcionar na ferramenta de validação do voucher | Membership |
| |* Ver análise de dados do cliente | Informações |
| |* Ver outras funções de utilizador dentro da empresa, mas não pode atribuir funções | Definições da conta |
| |* Crie bilhetes de apoio para o Centro de Parceiros | Ajuda + suporte |
| |* Ver bilhetes de apoio a parceiros que criar | Ajuda + suporte |
| Administrador de conta| Adicionar localizações| Definições da conta | [Gerir localizações](manage-locations.md)
| |* Gerir perfis relacionados com as contas para as contas para as contas que está a administrar | Definições da conta |
| |* Atribuir funções para utilizadores em arrendatários a funções não-Azure-AD | Definições da conta |
| |* Inscrever localizações em programas |  |
| |* Crie bilhetes de apoio para o Centro de Parceiros | Ajuda + suporte |
| |* Ver bilhetes de apoio a parceiros que criar | Ajuda + suporte |

## <a name="manage-referrals"></a>Gerir referências

|**Role** | **O que pode fazer**| **Área de trabalho** | **Saiba mais** |
|------------------------------|:---|-----------------------|---|
|Administração de referências|Criar e gerir tudo sob o separador Referências no Centro de Parceiros| Referências | [Gerir oportunidades de Venda conjunta](manage-co-sell-opportunities.md)
||    Pode ver e editar todas as oportunidades e pistas de co-venda | Referências |
||    Pode atribuir membros da equipa para um acordo | Referências |
||    Pode ver e editar perfis de negócio | Referências |
||    Pode ver e registar ofertas para oportunidades que são marcadas como ganhas e elegíveis para registo de negócios | Referências |
||    Pode criar e ver bilhetes de apoio | Ajuda + suporte |
|Utilizador de referências|Criar e gerir oportunidades de co-venda apenas se fizerem parte da equipa | Referências | [Gerir oportunidades de Venda conjunta](manage-co-sell-opportunities.md)
||    Pode criar oportunidades de co-venda para os locais onde lhes é atribuído o papel. | Referências |
||    Pode ver e registar ofertas para oportunidades que são marcadas como ganhas e elegíveis para registo de negócios se forem membros da equipa. | Referências |
||    Pode criar e ver bilhetes de apoio | Ajuda + suporte |
|Administrador de perfil de negócios|Criar e gerir perfis de negócio | Referências | [Gerir perfis de negócio](create-a-marketing-profile.md)
||    Pode criar e ver bilhetes de apoio | Ajuda + suporte |

Juntamente com a nova função de utilizador de referências, estamos também a introduzir a margem de localização para as ofertas. A tabela abaixo explica o acesso às ofertas com base no local.

|**Âmbito** | **O que pode fazer** | **Área de trabalho** |
|------------------------------|:-----------------|--------|
|Empresa inteira | Tanto os administradores como os utilizadores têm acesso a criar ofertas para qualquer localização na sua empresa| Referências |
|| A administração de referência tem acesso a visualização e edição de todos os negócios | Referências |
|| Os utilizadores de referência têm acesso a visualização e edição de todas as ofertas apenas se fizerem parte da equipa | Referências |
|Um ou mais locais | Tanto os administradores como os utilizadores têm acesso a criar ofertas para a localização atribuída na sua empresa| Referências |
|| A administração de referência tem acesso para visualizar e editar todos os negócios pertencentes aos locais atribuídos| Referências |
|| Os utilizadores de referência têm acesso a visualização e edição de todas as ofertas pertencentes aos locais atribuídos se fizerem parte da equipa| Referências |

## <a name="manage-incentives"></a>Gerir incentivos

|**Role** | **O que pode fazer**| **Área de trabalho** | **Saiba mais** |
|---------|:-------------------|---------------|----------------|
|Administradores de incentivos|* Inicia e gere incentivos | Incentivos | [Use estes recursos para ajudá-lo a começar com incentivos](incentives-get-started-intro.md) |
||* Pode ver e editar todos os aspetos dos programas de incentivos | Incentivos |
||* Pode ver e editar detalhes bancários e fiscais | Incentivos |
||* Ver descontos e ganhos cooperativos | Incentivos |
||* Suporte de acesso | Ajuda + suporte |
||* Pagamentos de incentivos de litígios | Incentivos |
|Utilizador de incentivos|* Pode ver programas de incentivos | Incentivos ||
||* Pode ver e iniciar pedidos de incentivos | Incentivos |
||* Ver descontos e ganhos cooperativos | Incentivos |
||* Crie bilhetes de apoio para o Centro de Parceiros | Ajuda + suporte |
||* Ver bilhetes de apoio a parceiros que criar | Ajuda + suporte |

## <a name="view-partner-center-insights-data"></a>Ver dados de Informações do Centro de Parceiros

|**Role** | **O que pode fazer** | **Área de trabalho** | **Saiba mais** |
|---------|:--------------------|---------------|----------------|
|Espectador de relatório executivo|Acesso a todos os conjuntos de dados de reporte, criar bilhetes de apoio a parceiros, ver bilhetes de apoio a parceiros que criar| Informações | [Relatórios do painel de visão geral disponíveis no Partner Center Informações](insights-overview-report.md) |
|Espectador de relatório|Acesso a relatórios de dados com exceção das receitas e dados pessoais do cliente e dos colaboradores, criar bilhetes de apoio ao parceiro, ver bilhetes de apoio a parceiros que criar | Informações | |

## <a name="next-steps"></a>Passos seguintes

- [Create user accounts and assign roles permissions](create-user-accounts-and-set-permissions.md) (Criar contas de utilizador e atribuir funções e permissões)
- [Verificar as informações da conta ao inscrever-se num novo programa do Centro de Parceiros](verification-responses.md)
