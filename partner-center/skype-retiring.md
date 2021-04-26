---
title: Migrar alguns Skype para subscrições de negócios
description: Saiba como e quando migrar determinados clientes com o Skype expirado para o Plano De Negócios 1 para as novas versões do Office 365.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 06/03/2020
ms.openlocfilehash: f395987ef647fa6f7ed264c6476ddae419eabc34
ms.sourcegitcommit: 26e6b470756aa9c1b3b0b919301b0eb38a335a52
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/26/2021
ms.locfileid: "108002863"
---
# <a name="migrate-skype-for-business-online-plan-1-subscriptions-to-newer-office-365-versions"></a>Migrate Skype for Business Online Plan 1 subscriptions to newer Office 365 version (Migrar as subscrições do Skype para Empresas Online Plano 1 para a versão mais recente do Office 365)

**Funções adequadas**

- Agente comercial

O Skype for Business Online Plan 1 será reformado, a partir de 1 de agosto de 2018. Após essa data, os clientes deixarão de poder adquirir novas subscrições do Skype para o Plano de Negócios 1, e as subscrições existentes não renovarão automaticamente quando expirarem e não fornecerão uma opção de renovação. Na página de pormenor da subscrição, o estado de subscrição do Skype for Business Online Plan 1 mudou para "Expira na [data]" de "Renovações automáticas em [data]".  

Para garantir a continuidade dos clientes, deve transitar os clientes com subscrições do Skype expirando para o Plano Online 1 para uma opção SKU suportada, listada abaixo. Recomendamos que os clientes mudem os clientes para novas subscrições antes da data de fim anual da subscrição para evitar eventuais interrupções de serviço para os clientes. 

>[!NOTE]
>Tanto o Skype para o Plano Online 1 comercial como o governo SKUs estão reformados.

Se utilizar a API (CREST ou Partner Center), encontre subscrições caducadas avaliando a data final da subscrição juntamente com a renovação automática = Propriedade falsa. As subscrições do Skype for Business Online Plan 1 serão definidas para renovação automática=Falsa a 1 de setembro de 2018. Pode mover os clientes para um novo plano a qualquer momento. 

## <a name="skype-for-business-online-plan-1-replacement-plans"></a>Plano Skype para Plano Empresarial 1 planos de substituição

Com os novos planos, os seus clientes podem tirar partido das funcionalidades e funcionalidades mais recentes no Office 365. Os detalhes dos preços encontram-se na lista de preços e a matriz da lista de ofertas no Partner Center. 

- Opção 1: Escritório 365 Empresa F1
- Opção 2: Microsoft 365 Enterprise F1
- Opção 3: Outros planos do Office 365

|**Funcionalidade**    |**Opção 1**   |**Opção 2**   |**Opção 3**   |
|:-----------------|:-----------------|:-------------|:------------|
|Obtenha todas as funcionalidades incluídas no Skype para o Plano Online de Negócios 1|Yes   |Yes   |Yes   |
|IM e presença |Yes   |Yes   |Yes   |
|Peer-to-peer Audio e Vídeo sobre IP|Yes   |Yes   |Yes   
|Junte-se às reuniões como utilizador autenticado| Yes   |Yes   |Yes   |

## <a name="transition-customers-to-new-product-plans"></a>Transição de clientes para novos planos de produtos

A Microsoft oferece continuamente novos produtos e serviços aos nossos parceiros. Nestes casos, poderá ter de atualizar os clientes para novos serviços ou migrar as suas subscrições de SKUs que acabarão por ser encerradas. Os clientes migradores de SKUs reformados para os mais recentes requerem os seguintes passos:

- Comprar a nova subscrição
- Reatribuir licenças de utilizador atuais
- Cancelar subscrição antiga

### <a name="migrate-your-customers-to-new-plans"></a>Migrar os seus clientes para novos planos

1. Para adquirir a nova subscrição, a partir do **menu Partner Center**, selecione **Clientes,** selecione o cliente que pretende mover e, em seguida, selecione **Adicionar subscrições**.

2. Selecione a subscrição que pretende adquirir no catálogo (neste caso, uma das opções acima), introduza o número de licenças e, em seguida, **selecione Enviar por isso**. 

O seu cliente deve agora ter subscrições antigas e novas, a antiga subscrição do Skype para o Plano Online 1 e a nova subscrição 'target', por exemplo, Opção 1 - Office 365 Enterprise F1.

3. Para reatribuir as licenças dos utilizadores do cliente, a partir do menu **Partner Center,** selecione **Clientes,** selecione o cliente que está a mover e, em seguida, selecione **Utilizadores e licenças**. A página de Utilizadores e Licenças do cliente abre.

4. Para reatribuir a licença de utilizador, selecione o utilizador para reatribuir e, em seguida, **selecione Gerir licenças.**

5. Na página **'Gerir licenças',** limpe a caixa de verificação da licença Skype for Business Online Plan 1 e selecione um novo plano de serviço para a subscrição para a qual o cliente está a mover-se.

6. Selecione **Submeter**. Uma página de confirmação lista as novas atribuições de licença. Continue este mesmo processo para outros utilizadores que necessitem de atribuição de licenças.

Depois de transferir a licença do utilizador para o novo serviço, pode cancelar com segurança a subscrição aposentada a nível do cliente.

7. A partir do menu **Partner Center,** selecione **Clientes.** Selecione o cliente cuja subscrição está a cancelar.

8. Na página de detalhes da subscrição, desa estale a subscrição **de Suspended**.

9. **Selecione Enviar.**

A subscrição antiga está suspensa e a nova subscrição está ativa. A subscrição suspensa será desavisionada automaticamente após 120 dias. O cliente não incorre em custos adicionais para a subscrição antiga.

## <a name="next-steps"></a>Passos seguintes

- [Assessoria: Criar e enviar um convite experimental para os clientes experimentarem o Office 365](advisors-create-a-trial-invitation.md)
- [Assessoria: Construa a sua base de clientes com convites de experimentação do Office 365 e ofertas de compra](advisors-build-your-business.md)
- [Assessores: Criar uma oferta de compra](advisor-create-a-purchase-offer.md)
