---
title: Migrar Dinâmicas 365 subscrições
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como migrar de subscrições básicas e qualificadas da Dynamics 365 para uma nova subscrição antes de expirarem as subscrições existentes.
author: Brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5ba6992eff64031aed0dafeb5a5010983396ab63
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151649"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a>Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions (Migrar o Dynamics 365 e o Customer Engagement Plan da versão Básica (ofertas qualificadas) para versões mais recentes)

**Funções adequadas**: Administração global | Administração de administração de utilizadores | Agente administrativo | Agente comercial

A partir de 1 de janeiro de 2019, os clientes com Dinâmica 365 para Vendas/Plano de Envolvimento com o Cliente a partir de assinaturas Básicas (Ofertas Qualificadas) já não podem renovar estas ofertas antigas; as subscrições existentes não renovarão automaticamente quando expirarem. Na página de pormenor da subscrição, o estado de subscrição mudará para "Expira na [data]" de "Renovações automáticas em [data]". 

Para garantir a continuidade dos clientes, deve transitar aqueles com subscrições caducadas para uma opção suportada, listada abaixo. Recomendamos que os clientes mudem os clientes para novas subscrições antes da data de fim anual da subscrição para evitar eventuais interrupções de serviço para os clientes.

Se utilizar a API (CREST ou Partner Center), pode encontrar subscrições caducadas avaliando a data final da subscrição juntamente com a renovação automática = Propriedade falsa. As subscrições em questão serão definidas para renovação automática=Falsa a 1 de janeiro de 2019. Pode mover os clientes para um novo plano a qualquer momento. 

### <a name="the-dynamics-365-offers-being-retired"></a>A Dynamics 365 oferece a reforma

- Dinâmica 365 para Venda Enterprise Edition CRMOL Basic (Oferta Qualificada)
- Dinâmica 365 para Venda Enterprise Edition CRMOL Basic (Oferta Qualificada) para Faculdade
- Dinâmica 365 para Sales Enterprise Edition CRMOL Basic (Oferta Qualificada) para Estudantes
- Dinâmica 365 para Venda Enterprise Edition (Preço do Governo) CRMOL Basic (Oferta Qualificada)
- Dinâmica 365 para Venda Enterprise Edition Da SA para CRM Basic (Oferta Qualificada)
- Dinâmica 365 para Venda Enterprise Edition From SA for CRM Basic (Oferta Qualificada) para Faculdade
- Dinâmica 365 para Venda Enterprise Edition From SA for CRM Basic (Oferta Qualificada) para Estudantes
- Dinâmica 365 para Venda Enterprise Edition (Preço do Governo) A partir de SA para CRM Basic (Oferta Qualificada)
- Dinâmica 365 para Venda Enterprise Edition Add-On para CRM Basic (Oferta Qualificada)
- Dinâmica 365 para Venda Enterprise Edition Add-On para CRM Basic (Oferta Qualificada) para Faculdade
- Dinâmica 365 para Venda Enterprise Edition Add-On para CRM Basic (Oferta Qualificada) para Estudantes
- Dinâmica 365 para Venda Enterprise Edition (Preço do Governo) Add-On para CRM Basic (Oferta Qualificada)
- Dinâmica 365 Plano de Envolvimento com o Cliente Enterprise Edition CRMOL Basic (Oferta Qualificada)
- Dinâmica 365 Plano de Envolvimento com o Cliente Enterprise Edition (Preço do Governo) CRMOL Basic (Oferta Qualificada)
- Dinâmica 365 Plano de Envolvimento com o Cliente Enterprise Edition CRMOL Basic (Oferta Qualificada) para Estudantes
- Dinâmica 365 Plano de Envolvimento com o Cliente Enterprise Edition CRMOL Basic (Oferta Qualificada) para Faculdade
- Dinâmica 365 Plano de Envolvimento com o Cliente Edição Empresarial da SA para CRM Basic (Oferta Qualificada)
- Dinâmica 365 Plano de Envolvimento com o Cliente Enterprise Edition (Preço do Governo) A partir de SA para CRM Basic (Oferta Qualificada)
- Dinâmica 365 Plano de Envolvimento com o Cliente Edição Empresarial da SA para CRM Basic (Oferta Qualificada) para Estudantes
- Dinâmica 365 Plano de Envolvimento com o Cliente Edição Empresarial da SA para CRM Basic (Oferta Qualificada) para Faculdade
- Dinâmica 365 Plano de Envolvimento com o Cliente Enterprise Edition Add-On para CRM Basic (Oferta Qualificada)
- Dinâmica 365 Plano de Envolvimento com o Cliente Enterprise Edition (Preço do Governo) Add-On para CRM Basic (Oferta Qualificada)
- Dinâmica 365 Plano de Envolvimento com o Cliente Enterprise Edition Add-On para CRM Basic (Oferta Qualificada) para Estudantes
- Dinâmica 365 Plano de Envolvimento com o Cliente Enterprise Edition Add-On para CRM Basic (Oferta Qualificada) para Faculdade



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a>Dinâmica 365 para Plano de Venda/Envolvimento do Cliente a partir de planos básicos de substituição (Ofertas Qualificadas)

**Ofertas aposentadas**   

- Dinâmica 365 para Vendas da CRM Basic ou CRMOL Basic (Oferta Qualificada)
- Dinâmica 365 Plano de Envolvimento do Cliente da CRM Basic ou CRMOL Basic (Oferta Qualificada)

**Opções de substituição**
- Dinâmica 365 para Profissional de Vendas (NOVO)
- Dinâmica 365 para Profissional de Vendas (NOVO)
- Dynamics 365 for Customer Service
- Dinâmica 365 Plano de Envolvimento do Cliente ou
- Dinâmica 365 Membros da equipa



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
 

 



