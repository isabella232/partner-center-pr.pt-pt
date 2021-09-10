---
title: Migrar Skype para Empresas subscrições
description: Saiba como e quando migrar determinados clientes com Skype para Empresas subscrições do Plano Online 1 para novas versões Office 365.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 06/03/2020
ms.openlocfilehash: 58908e966eb80d219afa0cbc8c043932f5aef1a1
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/09/2021
ms.locfileid: "123961523"
---
# <a name="migrate-skype-for-business-online-plan-1-subscriptions-to-newer-office-365-versions"></a>Migrate Skype for Business Online Plan 1 subscriptions to newer Office 365 version (Migrar as subscrições do Skype para Empresas Online Plano 1 para a versão mais recente do Office 365)

**Funções adequadas**: Agente de vendas

O Plano Skype para Empresas Online 1 será retirado, a partir de 1 de agosto de 2018. Após essa data, os clientes deixarão de poder adquirir novas subscrições do Plano 1 Skype para Empresas, e as subscrições existentes não renovarão automaticamente quando expirarem e não fornecerão uma opção de renovação. Na página de pormenor da subscrição, o Skype para Empresas Estado de subscrição do Plano Online 1 mudou para "Expira na [data]" de "Renovações automáticas em [data]".  

Para garantir a continuidade dos clientes, deve transitar os clientes com Skype para Empresas subscrições do Plano Online 1 para uma opção SKU suportada, listada abaixo. Recomendamos que os clientes mudem os clientes para novas subscrições antes da data de fim anual da subscrição para evitar eventuais interrupções de serviço para os clientes. 

>[!NOTE]
>Tanto Skype para Empresas o Plano Online 1 comerciais e o governo SKUs estão reformados.

Se utilizar a API (quer O Comércio REST (CREST) quer o Partner Center), encontre subscrições caducadas avaliando a data final da subscrição juntamente com a renovação automática = Propriedade falsa. As subscrições do Plano Skype para Empresas 1 serão definidas para renovação automática=Falsa no dia 1 de setembro de 2018. Pode mover os clientes para um novo plano a qualquer momento. 

## <a name="skype-for-business-online-plan-1-replacement-plans"></a>Skype para Empresas Plano Online 1 planos de substituição

Com os novos planos, os seus clientes podem tirar partido de funcionalidades e funcionalidades mais recentes em Office 365. Os detalhes dos preços encontram-se na lista de preços e a matriz da lista de ofertas no Partner Center. 

- Opção 1: Office 365 Enterprise F1
- Opção 2: Microsoft 365 Enterprise F1
- Opção 3: Outros planos de Office 365

|**Funcionalidade**    |**Opção 1**   |**Opção 2**   |**Opção 3**   |
|:-----------------|:-----------------|:-------------|:------------|
|Obtenha todas as funcionalidades incluídas no Skype para Empresas Plano Online 1|Yes   |Yes   |Yes   |
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

O seu cliente deve agora ter subscrições antigas e novas, a subscrição do antigo plano Skype para Empresas online 1 e a nova subscrição 'target', por exemplo, Opção 1 - Office 365 Enterprise F1.

3. Para reatribuir as licenças dos utilizadores do cliente, a partir do menu **Partner Center,** selecione **Clientes,** selecione o cliente que está a mover e, em seguida, selecione **Utilizadores e licenças**. A página de Utilizadores e Licenças do cliente abre.

4. Para reatribuir a licença de utilizador, selecione o utilizador para reatribuir e, em seguida, **selecione Gerir licenças.**

5. Na página **'Gerir licenças',** limpe a caixa de verificação de licenças Skype para Empresas Plano Online 1 e selecione um novo plano de serviço para a subscrição para a qual o cliente está a mover-se.

6. Selecione **Submeter**. Uma página de confirmação lista as novas atribuições de licença. Continue este mesmo processo para outros utilizadores que necessitem de atribuição de licenças.

Depois de transferir a licença do utilizador para o novo serviço, pode cancelar com segurança a subscrição aposentada a nível do cliente.

7. A partir do menu **Partner Center,** selecione **Clientes.** Selecione o cliente cuja subscrição está a cancelar.

8. Na página de detalhes da subscrição, desa estale a subscrição **de Suspended**.

9. **Selecione Enviar.**

A subscrição antiga está suspensa e a nova subscrição está ativa. A subscrição suspensa será desavisionada automaticamente após 120 dias. O cliente não incorre em custos adicionais para a subscrição antiga.

## <a name="next-steps"></a>Passos seguintes

- [Assessores: Criar e enviar um convite experimental para os clientes tentarem Office 365](advisors-create-a-trial-invitation.md)
- [Assistentes: Criar a base de clientes com ofertas de compra e convites para avaliação do Office 365](advisors-build-your-business.md)
- [Assessores: Criar uma oferta de compra](advisor-create-a-purchase-offer.md)
