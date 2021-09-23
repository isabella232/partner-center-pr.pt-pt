---
title: Transferência da subscrição da Azure para outro parceiro
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: Saiba como alterar o Fornecedor de Soluções em Nuvem parceiro de programa associado às subscrições Azure de um cliente.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: dhirajgandhi
ms.author: dhgandhi
ms.date: 07/21/2021
ms.openlocfilehash: b9ce8fff5915d3d4bf42f699c5a0c9130e37814b
ms.sourcegitcommit: fceaca54b0ec695cf214209c09b4516e1b40866a
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/23/2021
ms.locfileid: "128322123"
---
# <a name="transfer-a-customers-azure-subscriptions-to-a-different-partner-without-converting-them-to-an-azure-plan"></a>Transfira as subscrições Azure de um cliente para um parceiro diferente sem as converter num plano Azure

**Aplica-se a**: Partner Center | Centro de Parceiros para Microsoft Cloud for US Government

**Funções apropriadas**: Administração global

Este artigo descreve como um cliente pode transferir uma subscrição Azure do seu Fornecedor de Soluções em Nuvem atual (CSP) para outro CSP.

A primeira secção, [transferindo uma subscrição do Azure para outro parceiro,](#transferring-azure-subscriptions-to-another-partner)descreve como um cliente pode transferir uma subscrição de Microsoft Azure de um Fornecedor de Soluções em Nuvem (CSP) para outro.

Na secção seguinte, [a Transferência de uma subscrição anterior da oferta Azure sem a converter para o plano Azure,](#transferring-a-previous-azure-offer-subscription-without-converting-it-to-the-azure-plan)descreve brevemente como o novo plano Azure está a ser introduzido. Em seguida, descreve um caso especial em que algumas subscrições da oferta anterior do Azure podem ser transferidas para outra CSP sem as converter para o novo plano Azure.

O cliente, o atual prestador de serviços e um novo prestador de serviços têm todas [responsabilidades na transferência de uma subscrição de um cliente para um novo prestador de serviços Azure.](#responsibilities-when-transferring-a-customer-subscription-to-a-new-azure-service-provider) Um cliente deve planear trabalhar em estreita colaboração com o parceiro atual para que a transição corra bem.

 Informações de alto nível para ajudar os assinantes do Azure a transferir subscrições de e para parceiros CSP podem ser encontradas em [subscrições de Transfer Azure entre assinantes e CSPs](/azure/cost-management-billing/manage/transfer-subscriptions-subscribers-csp).

Informações adicionais sobre como os clientes podem alterar as suas subscrições Azure de um parceiro para outro podem ser encontradas na [Transferência de subscrições Azure de um cliente para um CSP diferente (ao abrigo de um plano Azure)](./transfer-azure-subscriptions-under-azure-plan.md)

## <a name="prerequisites"></a>Pré-requisitos

- Um Parceiro CSP deve ter uma relação de revendedor com um cliente antes de uma subscrição poder ser transferida.  Para obter mais informações, consulte [Como solicitar uma relação de revendedor a um cliente no Partner Center.](./request-a-relationship-with-a-customer.md)
- Um parceiro deve ser um fornecedor direto ou um fornecedor indireto para transferir uma subscrição.
- As assinaturas associadas às seguintes ofertas não podem ser transferidas: Plano Azure, Office 365, Suite de Mobilidade Empresarial e Microsoft Dynamics CRM.
- Um cliente deve estar no mesmo país que um parceiro para transferir uma subscrição.
- Os parceiros que operam em Microsoft Cloud for US Government ou Microsoft Cloud Germany devem solicitar permissão para gerir o serviço ou subscrição de um cliente. Para mais informações, consulte [Obter permissões para gerir o serviço ou subscrição de um cliente.](./customers-revoke-admin-privileges.md)

## <a name="transferring-azure-subscriptions-to-another-partner"></a>Transferência de assinaturas Azure para outro parceiro

Transferir uma subscrição da Azure de um parceiro da CSP para outro é um processo multipasso que requer ações do cliente, do atual parceiro e do novo parceiro em várias fases. A tabela a seguir pretende ser um diagrama de sequência para ajudar a esclarecer quem faz o quê e quando.

### <a name="responsibilities-when-transferring-a-customer-subscription-to-a-new-azure-service-provider"></a>Responsabilidades na transferência de uma subscrição de cliente para um novo prestador de serviços Azure

|Passo  |Cliente  |Parceiro atual  |Novo parceiro  |
|---------|---------|---------|---------|
|1     |[Cliente notifica Microsoft e atual parceiro por escrito](#step-1-customer-contacts-current-partner-in-writing)         |         |         |
|2     |         |[Crie bilhete de apoio para solicitar transferência](#step-2-current-provider-creates-azure-support-ticket-to-request-a-transfer)        |         |
|3     |         |[Enviar formulário de transferência preenchido para o cliente](#step-3-current-partner-completes-transfer-form-and-sends-it-to-the-customer)|         |
|4     |         |[Alteração completa do formulário Fornecedor de Soluções em Nuvem](#step-3-current-partner-completes-transfer-form-and-sends-it-to-the-customer)       |         |
|5     |[Formulário de revisão, sinal, & de retorno](#step-5-the-customer-and-new-partner-review--return-the-form)       |         |[Formulário de revisão, sinal, & de retorno](#step-5-the-customer-and-new-partner-review--return-the-form)         |
|6     |         |[Rever formulário e anexar ao pedido de serviço](#step-6-current-partner-reviews-form-and-attaches-it-to-the-service-request)        |         |
|7     |         |         |[Remover antigo parceiro da conta](#step-7-new-partner-removes-old-partner-from-account)         |
|8     |         |         |[Remover permissões de acesso desatualizadas](#step-8-new-partner-removes-outdated-access-permissions)         |

### <a name="steps-for-transferring-a-customer-subscription-to-a-new-azure-service-provider"></a>Passos para transferir uma subscrição de cliente para um novo prestador de serviços Azure

#### <a name="step-1-customer-contacts-current-partner-in-writing"></a>Passo 1: Cliente contacta parceiro atual por escrito

O cliente inicia o processo de transferência notificando a Microsoft e o atual Parceiro CSP por escrito (isto é, não verbalmente) do seu pedido de transferência de uma subscrição.

#### <a name="step-2-current-provider-creates-azure-support-ticket-to-request-a-transfer"></a>Passo 2: Atual fornecedor cria bilhete de apoio Azure para solicitar transferência

O atual parceiro cria um bilhete de apoio Azure para solicitar uma transferência de assinatura.

> [!NOTE]
> É da responsabilidade do atual parceiro criar o bilhete de apoio que inicia o processo de transferência. A Microsoft não intervém em nome do cliente ou do novo parceiro.

**Para criar um bilhete de apoio para solicitar uma transferência:**

1. No menu Partner Center, selecione **Clientes,** selecione o cliente da lista e, em seguida, selecione **a gestão do Serviço**.
1. Na secção **de bilhetes De Apoio,** selecione **Novo bilhete** e, em seguida, **Microsoft Azure.**
1. No [portal Azure,](https://portal.azure.com/)selecione **Novo pedido de suporte**.
1. Na Etapa 1 do pedido de apoio, escolha a gestão da **Subscrição** como o tipo de emissão, especifique o ID de subscrição que deseja transferido e escolha **Fornecedor de Soluções em Nuvem** como plano de suporte.
1. No passo 2, selecione **o impacto C-Minimal** e escolha **Outras Perguntas Gerais** como o tipo de problema.

#### <a name="step-3-current-partner-completes-transfer-form-and-sends-it-to-the-customer"></a>Passo 3: O parceiro atual preenche o formulário de transferência e envia-o ao cliente

O parceiro atual descarrega e completa o [formulário Change of Fornecedor de Soluções em Nuvem,](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC)assina-o e depois envia-o para o cliente.

#### <a name="step-4-current-partner-completes-current-partner-fills-in-the-change-of-cloud-solution-provider-form"></a>Passo 4: Atual parceiro completa o atual parceiro preenche o formulário De Mudança de Fornecedor de Soluções em Nuvem

O atual parceiro completa o [formulário De Mudança de Fornecedor de Soluções em Nuvem,](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC)assina-o e envia-o ao cliente.

Entre as informações necessárias para completar a *alteração de Fornecedor de Soluções em Nuvem* formulário está:

- **As informações de contacto do parceiro atual e** o ID do Microsoft (que pode ser encontrado no menu Partner Center selecionando as **definições de Conta > perfil da Organização).**
- **O ID do Microsoft do cliente** (que pode ser encontrado no menu Partner Center selecionando **clientes** e expandindo a lista do cliente para revelar o seu ID microsoft).
- **ID de subscrição** para transferir (que pode ser encontrado no menu Partner Center selecionando **clientes** e, em seguida, expandindo a listagem do cliente, selecionando **Subscrições de Ver**, e, em seguida, expandindo a subscrição escolhida para revelar o ID de subscrição.

#### <a name="step-5-the-customer-and-new-partner-review--return-the-form"></a>Passo 5: O cliente e o novo parceiro analisam & devolver o formulário

Trabalhando em conjunto, o cliente e o novo parceiro:

1. Reveja o formulário, preencha informações sobre o novo parceiro e assine-o.
1. Confirme que o novo cliente tem um contrato em vigor.
1. Envie o formulário de volta para o parceiro atual.

#### <a name="step-6-current-partner-reviews-form-and-attaches-it-to-the-service-request"></a>Passo 6: Os atuais comentários de parceiros formam-no e anexam-no ao pedido de serviço

Quando o atual parceiro recebe o formulário, eles:

- Certifique-se de que o formulário inclui informações de contacto para ambos os administradores do parceiro. (O Microsoft Support contacta ambos os administradores para verificar a transferência.)
- Verifique se têm as três assinaturas e, em seguida, utilize a opção **De Upload de Ficheiros** para anexar o formulário preenchido ao pedido de serviço existente. (Um engenheiro de suporte da Microsoft contacta-os dentro de oito horas úteis para validar a receção e a conclusão.)

#### <a name="step-7-new-partner-removes-old-partner-from-account"></a>Passo 7: Novo parceiro retira antigo parceiro da conta

O novo parceiro atualiza as definições de subscrição do Azure no PowerShell para remover o antigo parceiro da conta.

> [!NOTE]
> O primeiro cmdlet PowerShell requer o ID do **cliente,** que aparece no Partner Center como o **ID** microsoft do cliente . O procedimento que se segue descreve como encontrar o Microsoft ID (ID do inquilino) do cliente para utilização no cmdlet.

**Para encontrar o Microsoft ID (ID do inquilino) de um cliente para utilização no *cmdlet powerShell Ligação-AzAccount:***

1. Inscreva-se no painel do Centro [de Parceiros.](https://partner.microsoft.com/dashboard)
1. Selecione **clientes** do menu.
1. Localize o cliente na lista que aparece.
1. Selecione a seta para baixo para expandir a listagem do cliente. Verá informações sobre o *nome* de Domínio do cliente e o **ID** microsoft do cliente.
1. Utilize o **ID microsoft** de 16 dígitos no cmdlet PowerShell que segue este procedimento.

O primeiro cmdlet PowerShell adiciona o novo parceiro como revendedor na conta:

```powershell
Connect-AzAccount -Tenant 'xxxx-xxxx-xxxx-xxxx'
```

O segundo cmdlet apresenta as funções na conta, incluindo os anteriores parceiros CSP:

```powershell
Get-AzRoleAssignment
```

#### <a name="step-8-new-partner-removes-outdated-access-permissions"></a>Passo 8: Novo parceiro remove permissões de acesso desatualizadas

   **Para remover permissões de acesso desatualizadas:**

   1. No menu Partner Center, selecione **Clientes.**
   1. Localize o cliente na lista de clientes.
   1. Clique duas vezes no nome da empresa do cliente. A página **de Assinaturas do** cliente aparece.
   1. No menu de detalhes do cliente, selecione **gestão de serviço.**
   1. Sob **Microsoft Azure**, selecione **Microsoft Azure Portal de Gestão**.

## <a name="transferring-a-previous-azure-offer-subscription-without-converting-it-to-the-azure-plan"></a>Transferir uma subscrição anterior da oferta do Azure sem convertê-la no plano Azure

Esta secção descreve brevemente como o novo plano Azure está a ser introduzido. Em seguida, descreve um caso especial em que algumas subscrições da oferta anterior do Azure podem ser transferidas para outra CSP sem as converter para o novo plano Azure.

> [!NOTE]
> Para transferir as subscrições Azure de um cliente que foram adquiridas ao abrigo da oferta anterior do Azure para um novo CSP *e convertê-las no plano Azure*, (que é a ação padrão), ver a secção anterior [*Transferir uma assinatura Azure para outro parceiro*](#transferring-azure-subscriptions-to-another-partner), e o artigo Transferir as [*subscrições Azure de um cliente para um CSP diferente (ao abrigo de um plano Azure)*](./transfer-azure-subscriptions-under-azure-plan.md).

### <a name="the-azure-plan-and-the-previous-azure-offer"></a>O plano Azure e a oferta anterior do Azure

A Microsoft introduziu uma nova experiência de comércio, o [plano Azure,](./azure-plan-lp.md)em julho de 2021. Para dar tempo aos parceiros para incorporarem novas funcionalidades com os seus serviços e clientes de transição da oferta anterior da Azure (MS-AZR-0145p) para o plano Azure, a oferta anterior da Azure continua disponível por tempo limitado.

A transição da oferta anterior do Azure para o plano Azure está em três fases:

**Fase 1**: Desde a introdução do plano Azure em julho de 2021, todos os novos clientes do programa Azure CSP foram colocados no plano Azure. Os parceiros podem continuar a negociar a oferta anterior da Azure com clientes que já a tenham comprado.

**Fase 2**: A 1 de fevereiro de 2022, os incentivos e a oportunidade de margem de parceiro serão retirados da oferta anterior do Azure.

**Fase 3**: Num momento ainda por determinar, a oferta anterior do Azure será retirada, e os clientes ainda na oferta anterior do Azure serão migrados para o plano Azure. (Os sócios serão notificados da data de reforma com seis meses de antecedência.)

### <a name="transferring-subscriptions-without-conversion"></a>Transferência de assinaturas sem conversão

Esta secção descreve o caso especial de transferência de uma subscrição adquirida ao abrigo da oferta anterior da Azure a um novo provedor de CSP, *sem a converter no plano Azure.*

A subscrição de um cliente à oferta anterior do Azure pode ser transferida para um novo parceiro CSP sem conversão para o plano Azure, utilizando os passos na secção anterior, [transferindo subscrições do Azure para outro parceiro,](#transferring-azure-subscriptions-to-another-partner)se:

- A oferta anterior da Azure ainda está disponível.
- Tanto o atual parceiro como o novo parceiro têm um cliente com uma subscrição da oferta anterior da Azure.

Se apenas o atual parceiro tiver um cliente com uma subscrição da oferta anterior do Azure, o atual parceiro pode utilizar a ferramenta de transição para mover a subscrição do cliente para o novo parceiro, convertendo-a simultaneamente no novo plano Azure.

> [!NOTE]
> Apenas os parceiros que tenham uma relação de faturação direta com a Microsoft podem aceder à ferramenta de transição. Os revendedores indiretos precisam de trabalhar com os seus fornecedores indiretos para utilizar a ferramenta de transição.

## <a name="next-steps"></a>Passos seguintes

- [Transfer Azure subscriptions (Transferir subscrições do Azure)](/azure/cost-management-billing/manage/transfer-subscriptions-subscribers-csp)
- [Transferir assinaturas Azure ao abrigo de um plano Azure](transfer-azure-subscriptions-under-azure-plan.md)
- Descarregue o [formulário de Transferência de Assinatura CSP](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC)
- Saiba mais sobre [o suporte a vários parceiros](multipartner.md)
- Saiba mais sobre [suporte a vários canais](multichannel.md)