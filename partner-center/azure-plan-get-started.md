---
title: Comece a sua mudança para o plano Azure
description: Saiba o que você e os seus clientes precisam de saber sobre a utilização do plano de pagamento da Azure, incluindo os primeiros passos, precauções de segurança e como começar.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
author: amitravat
ms.author: amrava
ms.custom: SEOAPR.20
ms.localizationpriority: High
ms.date: 12/02/2019
ms.openlocfilehash: 40bf84ed47c946b84f511693d9f8351b3ffa5a95
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/09/2021
ms.locfileid: "123961070"
---
# <a name="begin-using-pay-as-you-go-rates-with-the-azure-plan"></a>Comece a usar as taxas de pagamento com o plano Azure

**Funções adequadas**: Agente administrador | Agente comercial


A Microsoft introduziu uma nova experiência de comércio no Partner Center.  Com esta nova experiência de comércio, os parceiros terão acesso aos serviços Azure a preços de pagamento para clientes ao abrigo do Microsoft Customer Agreement.

Este plano simplifica a experiência de compra - você pode ter várias subscrições Azure em um plano Azure. Já não precisa de submeter uma encomenda separada por assinatura Azure. E nesta nova experiência comercial para o Azure, alinhamo-nos com um único princípio global de preços que permite aos parceiros da CSP oferecer ao Azure os preços publicados.

As necessidades de transformação digital dos nossos clientes requerem novas competências dos parceiros. Muitos clientes procuram parceiros para fornecer serviços acima e além da transação para tornar a sua viagem na nuvem mais suave e ajudar a consumir os serviços Azure de forma eficiente. Os parceiros da Microsoft desempenham um papel crítico em todas as fases do ciclo de vida do cliente. Este tipo de serviços parceiros estão em curso e incluem a monitorização imobiliária da Azure, a gestão de políticas e governação, a criação e configuração de afinação, o suporte técnico e uma variedade de outros serviços. Exigem que um parceiro esteja intimamente familiarizado com o ambiente Azure do cliente e tenha uma governação e controlo contínuos e adequados dos recursos subjacentes que gerem. Os parceiros de faturação que fornecem esta gestão de operações em nuvem 24 X 7 tornar-se-ão elegíveis para um **Partner que ganhou crédito pelos serviços geridos** para esse trabalho.

## <a name="make-sure-your-customers-have-signed-the-microsoft-customer-agreement"></a>Certifique-se de que os seus clientes assinaram o Acordo de Cliente da Microsoft

Desde 1 de outubro de 2019, está disponível o Microsoft Customer Agreement, um acordo perpétuo que simplifica e dinamiza a experiência de compra de clientes com um processo totalmente digital. Todos os clientes que queiram tirar partido da nova experiência de comércio na CSP para a Azure devem assinar o Acordo de Cliente da Microsoft.

Os parceiros que pretendam negociar ao abrigo do novo plano Azure e fazer uma nova encomenda devem confirmar a aceitação do Cliente da Microsoft utilizando o painel de instrumentos do Partner Center e a API em produção.

A partir de 1 de fevereiro de 2020, o atual Microsoft Cloud Agreement é removido do programa CSP. A partir desse momento, será necessária a confirmação do parceiro (atestado) da aceitação do cliente para o novo Acordo de Cliente da Microsoft para todas as outras ofertas, incluindo Microsoft 365, Dynamics 365 e Azure existente. Os parceiros da CSP não poderão fazer uma nova encomenda para o cliente sem aestestação do Acordo de Cliente da Microsoft.

Para mais detalhes, leia [Confirme a aceitação do cliente do Acordo de Cliente da Microsoft](confirm-customer-agreement.md)

## <a name="security-and-access-control-practices"></a>Práticas de segurança e controlo de acessos

Para ajudar a salvaguardar parceiros e clientes, estamos a introduzir um conjunto de requisitos de segurança obrigatórios para assessores, fornecedores de painéis de controlo e parceiros que participam no programa Fornecedor de Soluções em Nuvem.

Os parceiros que não implementarem os requisitos de segurança obrigatórios não poderão negociar no programa de Fornecedor de Soluções em Nuvem ou gerir os inquilinos dos clientes aproveitando os direitos de administração dos delegados, uma vez que estes requisitos são cumpridos. Estamos em fase de estabelecer uma data de execução técnica para os requisitos e notificaremos os parceiros da data com informações detalhadas.

## <a name="actions-to-take-to-implement-mfa"></a>Ações a tomar para implementar o MFA

Dada a natureza altamente privilegiada de ser um parceiro, precisamos garantir que cada utilizador tem um desafio MFA para cada autenticação. Isto pode ser realizado através de uma das seguintes formas:

- Implementação Azure AD Premium e garantir que a autenticação de vários fatores (MFA) é aplicada a cada utilizador
- Implementação dos [incumprimentos de segurança Azure AD](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)
- Implementar uma solução de terceiros e garantir que o MFA é aplicado a cada utilizador

A partir de 1 de agosto de 2019, todos os parceiros são obrigados a impor a autenticação de vários fatores para todos os utilizadores, incluindo contas de serviço, no seu inquilino parceiro. Informações detalhadas sobre estes requisitos de segurança podem ser encontradas nos [requisitos de segurança do Parceiro.](partner-security-requirements.md)

A Microsoft recomenda que os parceiros utilizem o RBAC de forma diligente, seguindo as melhores práticas ativadas através [de recursos Azure Ative Directory Privileged Identity Management.](/azure/active-directory/privileged-identity-management/pim-configure)

## <a name="read-more-about-the-azure-plan"></a>Leia mais sobre o plano Azure

- [Comprar o plano do Azure](purchase-azure-plan.md)

- [Comparar ofertas do Azure](compare-azure-offers.md)

- [Parceiro ganhou crédito - visão geral](partner-earned-credit.md)

- O parceiro obteve cálculos de crédito (PEC) e as funções e permissões elegíveis para ganhar créditos obtidos pelo parceiro estão disponíveis na sua lista de preços do Partner Center Dashboard (inscrição obrigatória).

## <a name="next-steps"></a>Passos seguintes 

- [Como o parceiro ganhou crédito é determinado - detalhes](partner-earned-credit-explanation.md)
- [Lista de preços do plano Azure explicada](azure-plan-price-list.md)
- [Transition your customer to Azure plan](azure-plan-transition.md) (Fazer a transição dos clientes para o plano do Azure)
- [Manage subscriptions and resources under the Azure plan](azure-plan-manage.md) (Gerir subscrições e recursos ao abrigo do plano do Azure)
- [A lista completa dos países/regiões onde o plano Azure está disponível](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3QN0x)