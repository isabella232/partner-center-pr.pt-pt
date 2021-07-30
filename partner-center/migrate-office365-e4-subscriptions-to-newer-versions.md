---
title: Migrar Office 365 assinaturas E4
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Microsoft Office 365 A edição enterprise E4 é aposentada a partir de 7 de abril de 2017. Saiba como migrar as subscrições dos seus clientes para versões mais recentes de Office 365.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a1b47860f0af3427342d89945528e9118ecfc0aa
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/29/2021
ms.locfileid: "114843328"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a>Migrate Office 365 E4 subscriptions to newer Office 365 versions (Migrar subscrições do Office 365 E4 para versões mais recentes do Office 365)

**Funções adequadas**: Administração global | Administração de administração de utilizadores | Agente administrativo | Agente comercial

O plano Office 365 Enterprise E4 está reformado, a partir de 7 de abril de 2017. As subscrições E4 existentes já não podem adquirir novas Office 365 e as subscrições E4 não serão renovadas automaticamente quando expirarem.

Quando as assinaturas E4 terminarem, serão canceladas. Para garantir a continuidade dos clientes, deve transitar os clientes com assinaturas E4 expiradas para uma opção SKU suportada, listada abaixo. Recomendamos que os clientes mudem os clientes para novas subscrições antes da data de fim anual da subscrição para evitar eventuais interrupções de serviço para os clientes. 

> [!NOTE]  
> Tanto Office 365 Enterprise E4 SKUs comerciais e governamentais estão reformados.
 
Na página de pormenor da subscrição, o estado de subscrição E4 mudou para "Expira na [data]" de "Renovações automáticas em [data]". 

Se utilizar a API (CREST ou Partner Center), pode descobrir subscrições caducadas avaliando a data final da subscrição juntamente com a renovação automática = Propriedade falsa. 

As subscrições E4 serão definidas para renovação automática=Falsa em 7 de abril de 2017. Pode mover os clientes para um novo plano a qualquer momento. 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a>Planos de substituição da edição Office 365 Enterprise E4

Pode optar por manter a mesma funcionalidade com o E4 ou fazer com que os seus clientes aproveitem as funcionalidades e funcionalidades mais recentes em Office 365 e Skype para Empresas Online. Os detalhes dos preços encontram-se na lista de preços e a matriz da lista de ofertas no Partner Center. A Secure Product Enterprise E3 ou Secure Productive Enterprise E5 pode ser substituída nas seguintes opções para Office 365 Enterprise E3 ou Office 365 Enterprise E5, respectivamente.

- Opção 1: Office 365 Enterprise E5

- Opção 2: Office 365 Enterprise E3 + Skype para Empresas Cloud PBX

- Opção 3: Office 365 Enterprise E3 + Skype para Empresas Plus CAL (paridade de preço e funcionalidade com E4)

- Opção 4: Office 365 Enterprise E3


| Funcionalidade | Opção 1 | Opção 2 | Opção 3 | Opção 4 |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| Obter todos os recursos incluídos em Office 365 Enterprise E4? | Sim | Sim | Sim | Não |
| Telefone números geridos em Office 365? | Sim | Sim | Não | Não |
| Telefone números geridos tanto no local como em Office 365 (implantação híbrida)? | Sim | Sim | Não | Não |
| Opção de adicionar um plano de chamada de voz PSTN? | Sim | Sim | Não | Não |
| Conferência PSTN? | Sim | Não | Não | Não |
| Ferramentas avançadas para colaboração, análise e segurança? | Sim | Não | Não | Não |
| Relatórios interativos, dashboards e visualizações de dados? | Sim | Não | Não | Não | 
| Mais controlo sobre a segurança dos dados e o cumprimento da privacidade incorporada, transparência e controlos refinados dos utilizadores? | Sim | Não | Não | Não | 

## <a name="transition-customers-to-new-product-plans"></a>Transição de clientes para novos planos de produtos

A Microsoft oferece continuamente novos produtos e serviços aos nossos parceiros. Nestes casos, poderá ter de atualizar os clientes para novos serviços ou migrar as suas subscrições de SKUs que acabarão por ser encerradas. Os clientes migradores de SKUs reformados para os mais recentes requerem os seguintes passos:

-   Comprar a nova subscrição
-   Reatribuir licenças de utilizador atuais
-   Cancelar a assinatura antiga

Siga estes passos para migrar a subscrição de Office 365 Enterprise E4 de um cliente para uma das opções na tabela acima.

### <a name="step-1---purchase-the-new-subscription"></a>Passo 1 - Comprar a nova subscrição

1. A partir do menu **Partner Center,** selecione **Clientes,** selecione o cliente que deseja mover e, em seguida, selecione **Adicionar subscrições**.

2. Selecione a subscrição que pretende adquirir no catálogo (neste caso, uma das opções acima), introduza o número de licenças e, em seguida, **selecione Enviar por isso**.

   O seu cliente deve agora ter subscrições antigas e novas, a subscrição antiga Office 365 Enterprise E4 e a nova subscrição 'target', por exemplo, Opção 1 - Office 365 Enterprise E5.

### <a name="step-2---reassign-the-customers-users-licenses"></a>Passo 2 - Reatribuir as licenças dos utilizadores do cliente

1. A partir do menu **Partner Center,** selecione **Clientes,** selecione o cliente que deseja mover e, em seguida, selecione **Utilizadores e licenças**. A página de Utilizadores e Licenças do cliente abre.

2. Para reatribuir licenças de utilizador, selecione o utilizador para reatribuir e, em seguida, **selecione Gerir licenças**.

3. Na página **'Gerir licenças',** limpe a caixa de verificação **de licenças Office 365 Enterprise E4** e selecione um novo plano de serviço para a subscrição para a qual o cliente está a mover-se.

4. Selecione **Submeter**. Uma página de confirmação lista as novas atribuições de licença.

5. Continue os mesmos passos com qualquer outro cliente que necessite de reatribuição de licença.

Depois de transferir as licenças do utilizador para o novo serviço, pode cancelar com segurança a subscrição aposentada ao nível superior do Cliente.

### <a name="step-3---cancel-the-old-subscription"></a>Passo 3 - Cancelar a assinatura antiga

1. A partir do menu **Partner Center,** selecione **Clientes.** Selecione o cliente que pretende mover e selecione a subscrição que pretende cancelar.

2. Na página de detalhes da subscrição, desa estale o estado de subscrição **de Suspenso**.

3. Selecione **Submeter**.

A subscrição antiga está suspensa e a nova subscrição está ativa. A subscrição suspensa será desavisionada automaticamente após 120 dias. O cliente não incorre em custos adicionais para a subscrição antiga.



 



