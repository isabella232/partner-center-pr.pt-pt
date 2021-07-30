---
title: Migrar subscrições do Kaizala Pro para o Microsoft 365
description: Saiba como migrar Kaizala Pro subscrições para versões Microsoft 365 ou Office 365. Leia este artigo para mais detalhes sobre a transição dos seus clientes.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
ms.author: sukumart
author: sukumart
ms.date: 06/01/2020
localization_priority: Normal
ms.openlocfilehash: e248657b9b4d4cf50cb7d38b2a0593ae6445bd28
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/29/2021
ms.locfileid: "114843141"
---
# <a name="migrate-kaizala-pro-standalone-subscriptions-to-microsoft-365-or-office-365-versions"></a>Migrar Kaizala Pro subscrições autónomas para versões Microsoft 365 ou Office 365

**Funções adequadas**: Agente de vendas

A partir de 1 de julho de 2020, a Microsoft está a terminar as vendas do serviço Kaizala Pro autónomo. Os clientes deixarão de poder adquirir novas subscrições Kaizala Pro após esta data, e as subscrições Kaizala Pro existentes não serão renovadas automaticamente quando expirarem.

Para garantir a continuidade dos clientes, deve transitar os clientes com subscrições autónomas Kaizala Pro expiradas para uma opção SKU suportada, listada abaixo. Recomendamos que os clientes mudem os clientes para novas subscrições antes da data de fim anual da subscrição para evitar eventuais interrupções de serviço para os clientes.

Se utilizar a API (CREST ou Partner Center), pode descobrir subscrições caducadas avaliando a data final da subscrição juntamente com a propriedade de renovação automática definida como falsa: `auto renew = False` .

As assinaturas E4 serão marcadas para `auto renew=False` 1 de julho de 2020. Pode mover os clientes para um novo plano a qualquer momento.

## <a name="kaizala-pro-standalone-replacement-plans"></a>Kaizala Pro Planos de substituição autónomos

Com os novos planos, os seus clientes podem tirar partido das funcionalidades e funcionalidades mais recentes em Microsoft 365. Os detalhes dos preços encontram-se na lista de preços e a matriz da lista de ofertas no Partner Center.

- [**Microsoft 365 para negócios,**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2)incluindo:  
   - Microsoft 365 Empresas Basic
   - Microsoft 365 Empresas
   - Microsoft 365 Empresas Premium
    
- [**Microsoft 365 para a Linha da Frente,**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab)incluindo:
   - Microsoft 365 F3 (anteriormente Microsoft 365 F1) e Office 365 F3
    
- [**Microsoft 365 para a Enterprise,**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans)incluindo: 
   - Office 365 E1
   - Microsoft 365 E3 e Office 365 E3
   - Microsoft 365 E5 e Office 365 E5

- [**Microsoft 365 para a Educação,**](https://www.microsoft.com/education/buy-license/microsoft365)incluindo: 
    - Microsoft 365 A1 e Office 365 A1
    - Microsoft 365 A3 e Office 365 A3
    - Microsoft 365 A5 e Office 365 A5

## <a name="transition-customers-to-new-product-plans"></a>Transição de clientes para novos planos de produtos

A Microsoft oferece continuamente novos produtos e serviços aos nossos parceiros. Nestes casos, poderá ter de atualizar os clientes para novos serviços ou migrar as suas subscrições de SKUs que acabarão por ser encerradas. Os clientes migradores de SKUs reformados para os mais recentes requerem os seguintes passos:

A. Comprar a nova subscrição

B. Reatribuir licenças de utilizador atuais

C. Cancelar subscrição antiga


## <a name="migrate-your-customers-to-new-plans"></a>Migrar os seus clientes para novos planos

### <a name="a-purchase-the-new-subscription"></a>A. Comprar a nova subscrição

1. Para adquirir a nova subscrição, a partir do menu **Partner Center,** selecione **Clientes,** selecione o cliente que pretende mover e, em seguida, selecione **Adicionar subscrições**.

2. Selecione a subscrição que pretende adquirir no catálogo (neste caso, uma das opções acima), introduza o número de licenças e, em seguida, **selecione Enviar por isso**.

O seu cliente deve agora ter subscrições antigas e novas, a subscrição antiga Kaizala Pro Autónoma e a nova subscrição 'target', por exemplo, Opção 1 - Office 365 Enterprise F1.

### <a name="b-reassign-current-user-licenses"></a>B. Reatribuir licenças de utilizador atuais

1. Para reatribuir as licenças dos utilizadores do cliente, a partir do menu **Partner Center,** selecione **Clientes,** selecione o cliente que está a mover e, em seguida, selecione **Utilizadores e licenças**. A página de Utilizadores e Licenças do cliente abre.

2. Para reatribuir a licença de utilizador, selecione o utilizador para reatribuir e, em seguida, **selecione Gerir licenças**.

3. Na página **'Gerir licenças',** limpe a caixa de verificação de licenças Kaizala Pro Autónoma e selecione um novo plano de serviço para a subscrição para a qual o cliente está a mover-se.

4.  Selecione **Submeter**. Uma página de confirmação lista as novas atribuições de licença. Continue este mesmo processo para outros utilizadores que necessitem de atribuição de licenças.

### <a name="c-cancel-old-subscription"></a>C. Cancelar subscrição antiga

Depois de transferir a licença do utilizador para o novo serviço, pode cancelar com segurança a subscrição aposentada a nível do cliente.

1.  A partir do menu **Partner Center,** selecione **Clientes.** Selecione o cliente cuja subscrição está a cancelar.

2.  Na página de detalhes da subscrição, desa estale a subscrição **de Suspended**.

3.  Selecione **Submeter**.

A subscrição antiga está suspensa e a nova subscrição está ativa. A subscrição suspensa será desavisionada automaticamente após 120 dias. O cliente não incorre em custos adicionais para a subscrição antiga.
