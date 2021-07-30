---
title: Edição Empresarial Migrate Dynamics 365
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Saiba como migrar as ofertas qualificadas dynamics 365 Business Edition para versões mais recentes antes de expirarem.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 2e8eca0a645656388516c4c25f0091713424caf0
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/29/2021
ms.locfileid: "114838296"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a>Migrate Dynamics 365 Business Edition Offers to newer versions (Migrar as Ofertas do Dynamics 365 Business Edition para versões mais recentes)

**Funções adequadas**: Administração global | Administração de administração de utilizadores | Agente administrativo | Agente comercial

A partir de 1 de janeiro de 2019, os clientes com subscrições da Dynamics 365 Business Edition já não podem renovar-se nestas ofertas antigas; as subscrições existentes não renovarão automaticamente quando expirarem. Na página de pormenor da subscrição, o estado de subscrição mudará para "Expira na [data]" de "Renovações automáticas em [data]".

Para garantir a continuidade dos clientes, deve transitar aqueles com subscrições caducadas para uma opção suportada, listada abaixo. Recomendamos que os clientes mudem os clientes para novas subscrições antes da data de fim anual da subscrição para evitar eventuais interrupções de serviço para os clientes.

Se utilizar a API (CREST ou Partner Center), pode encontrar subscrições caducadas avaliando a data final da subscrição juntamente com a renovação automática = Propriedade falsa. As subscrições em questão serão definidas para renovação automática=Falsa a 1 de janeiro de 2019. Pode mover os clientes para um novo plano a qualquer momento. 

## <a name="the-dynamics-365-business-editions-being-retired"></a>As Dynamics 365 Business Editions estão a ser aposentadas

- Dinâmica 365 para Finanças e Operações, Edição de Negócios
- Dinâmica 365 para Membros da Equipa, Edição de Negócios

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a>Dynamics Business Central - as novas ofertas da Dynamics 365 Business Edition

Com as novas ofertas da Dynamics Business Central, os seus clientes podem ligar as suas finanças, vendas, serviços e operações para agilizar processos de negócio, melhorar as interações dos clientes e tomar melhores decisões. A Dynamics 365 Business Central é baseada na nuvem e está disponível apenas através de parceiros de programa Fornecedor de Soluções em Nuvem (CSP).
Os clientes da Dynamics 365 Business Edition podem receber preços de transição descontados para as novas ofertas da Business Central até 30 de junho de 2020.

## <a name="transition-customers-to-new-product-plans"></a>Transição de clientes para novos planos de produtos

 A transferência de clientes de SKUs reformados para os mais recentes requer os seguintes passos nesta ordem:

- Comprar a nova subscrição
- Reatribuir licenças de utilizador atuais
- Cancelar subscrição antiga

## <a name="purchase-the-new-plan-for-your-customer"></a>Compre o novo plano para o seu cliente

1. Selecione **Clientes** a partir da navegação esquerda e, em seguida, selecione o cliente que pretende mover-se para a nova subscrição.
2. Selecione **Adicionar Subscrição**.
3. Selecione a subscrição que pretende adquirir no catálogo (neste caso, uma das opções acima), introduza o número de licenças e, em seguida, **selecione Enviar por isso**. 

O seu cliente terá agora a subscrição antiga e a nova. O seu próximo passo é reatribuir licenças aos utilizadores do cliente.

1. Selecione **clientes** a partir da navegação esquerda e, em seguida, selecione o cliente em que está a mover-se.
2. Selecione **Utilizadores e licenças.**
3. Para reatribuir uma licença a um utilizador, selecione o utilizador e, em seguida, **selecione Gerir licenças**. 
4. Na página **'Gerir licenças',** limpe a caixa de verificação da licença Dynamics 365 para Vendas/Cliente a partir da caixa de verificação de licença Básica (Oferta Qualificada) e selecione um novo plano de serviço para a subscrição para a qual o cliente está a mover-se. 
5. Selecione **Submeter**. Fá-lo-ás por cada utilizador que precise da nova licença. 

Uma vez transferidas as licenças para a nova subscrição, pode cancelar a subscrição antiga. 

1. Selecione **clientes** a partir da navegação esquerda e, em seguida, selecione o cliente em que está a mover-se.
2. Na página de detalhes da subscrição, desafie a subscrição antiga para **Suspender** e selecione **Enviar**.

A subscrição antiga está agora suspensa e a nova subscrição está ativa. A subscrição suspensa será desavisionada automaticamente após 120 dias. O seu cliente não incorrerá em custos adicionais para a subscrição antiga.
