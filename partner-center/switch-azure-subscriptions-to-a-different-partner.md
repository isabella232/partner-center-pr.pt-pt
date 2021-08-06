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
ms.openlocfilehash: cac2d1443fd47f45a70729bf034e65f33861e73698633938ae196e274f4a382b
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/06/2021
ms.locfileid: "115681387"
---
# <a name="learn-how-to-transfer-a-customers-azure-subscriptions-to-another-partner"></a>Saiba como transferir as subscrições do Azure de um cliente para outro parceiro

**Aplica-se a**: Partner Center | Centro de Parceiros para Microsoft Cloud for US Government

**Funções apropriadas**: Administração global

Este artigo descreve como um cliente pode mudar os seus serviços de Microsoft Azure de um Fornecedor de Soluções em Nuvem (CSP) para outro quando adquiriu a oferta anterior da Azure em CSP.

Após a Fase 1 das alterações que estamos a fazer à oferta anterior do [Azure em CSP,](https://go.microsoft.com/fwlink/p/?linkid=2164140)para todas as relações de revendedor existentes entre parceiros e clientes no programa CSP, o parceiro pode continuar a transacionar a oferta anterior da Azure (MS-AZR-0145p) se o cliente já o tiver adquirido. Para todas as relações de revendedor existentes entre parceiros e clientes, se o cliente não tiver comprado a oferta anterior da Azure antes, o parceiro só pode transacionar a nova oferta da Azure.

- **Se o parceiro atual e futuro tiver subscrições anteriores ativas da Azure com um cliente,** as transferências anteriores da Azure (MS-AZR-0145p) descritas neste documento entre o parceiro atual e futuro continuarão disponíveis após a Fase 1, desde que ambos os parceiros mantenham subscrições de oferta anteriores ativas. Esta capacidade de transferência terminaria quando um futuro parceiro deixasse de ter nenhuma subscrição de oferta anterior ativa ou quando a oferta anterior do Azure (MS-AZR-0145p) em CSP se reformasse permanentemente na Fase 3.

   > [!NOTE]
   > Não existe uma ferramenta automatizada disponível para este cenário e o processo abaixo deve ser alavancado.

- **Se apenas o atual parceiro tiver um cliente com uma subscrição ativa anterior da Azure (MS-AZR-0145p) e o futuro parceiro não** o fizer, a transferência da oferta anterior da Azure entre parceiros deixaria de ser possível após a Fase 1. Uma vez que o futuro parceiro não pode criar uma subscrição anterior da Azure (MS-AZR-0145p) para o cliente, esta transferência não seria ativada. Neste caso, esta ferramenta de transição pode ser usada para mover a subscrição Azure do cliente entre parceiros em CSP, ao mesmo tempo que a converte para uma nova subscrição de oferta Azure.

Para trocar os serviços ou subscrições do Azure de um cliente para um parceiro diferente com a oferta anterior da Azure (MS-AZR-0145p), siga estes passos manuais. Tanto o parceiro como o cliente precisam de completar os passos.

> [!NOTE]  
> Atualmente, apenas os Fornecedores Diretos ou Indiretos podem transferir subscrições.
> Não é possível mudar de parceiros para subscrições Fornecedor de Soluções em Nuvem associadas ao plano Azure, Office 365, Suíte de Mobilidade Empresarial ou Microsoft Dynamics CRM subscrições.

## <a name="transfer-azure-subscriptions-to-another-partner-with-the-previous-azure-offer"></a>Transferir subscrições da Azure para outro parceiro com a oferta anterior da Azure

1. Para transferir uma subscrição da Azure para um novo parceiro com a oferta anterior da Azure, o cliente deve iniciar o processo e contactar o seu atual parceiro de registo por escrito.

   > [!NOTE]
   > É da responsabilidade do atual parceiro criar o bilhete de serviço que inicia o processo de transferência. A Microsoft não pode intervir em nome do cliente ou do novo parceiro. O cliente deve planear trabalhar em estreita colaboração com o parceiro atual para que a transição corra bem.

2. O parceiro para a subscrição precisa de fazer as seguintes tarefas:

   Crie um bilhete de serviço Azure do Partner Center para solicitar uma transferência de assinatura:

   1. A partir do menu Partner Center, selecione **Clientes,** selecione o seu cliente da lista e, em seguida, selecione **a gestão do Serviço**.
   2. Na secção **de bilhetes De Apoio,** selecione a nova entrega de **bilhetes** e escolha **Microsoft Azure**.
   3. A partir do [portal Azure,](https://portal.azure.com)selecione **Novo pedido de suporte**.
   4. No Passo 1, escolha a **gestão da Subscrição** como o tipo de problema, especifique o ID de subscrição que deseja transferido e escolha **Fornecedor de Soluções em Nuvem** como plano de suporte.
   5. No passo 2, selecione **o impacto C-Minimal** e escolha **Outras Perguntas Gerais** como o tipo de problema.
   6. Descarregue o [formulário de Transferência de Assinatura CSP](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC).

3. O parceiro para a subscrição: Preencha o [formulário de Transferência de Assinatura CSP,](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC)assine-o e, em seguida, envie-o ao cliente. 

   Para completar o formulário, necessitará das seguintes informações:

   - As informações de contacto do parceiro atual e a identificação da Microsoft. No menu Partner Center, selecione perfil de **Organização de Definições de Contas** e utilize o &gt;  **ID** da **Microsoft,** nome da Organização e **Endereço** listados lá.
   - O iD da Microsoft do cliente. No menu Partner Center, selecione **Clientes** e, em seguida, expanda a listagem do cliente para ver o seu **ID Microsoft**.
   - O ID de assinatura para transferir. Na listagem de clientes expandida, selecione **Ver Subscrições,** em seguida, expandir a subscrição escolhida para ver o **ID de subscrição**.

   > [!NOTE]
   > A transferência de uma subscrição resulta em dois IDs de subscrição que verá na página de Subscrição de **Edição** da subscrição transferida: **1**- O ID de subscrição do Partner Center é utilizado para efeitos de faturação. **2**- O ID de subscrição original do Azure é mantido e aparecerá no Partner Center, bem como no portal Azure Management. Esta identificação aparecerá no seu ficheiro de reconhecimento.  **Ao registar bilhetes de suporte, você precisa usar ambos os IDs.**

4. O cliente e novo parceiro para a subscrição:

   Reveja o formulário, preencha informações sobre o novo parceiro e assine-o. Confirme que o novo cliente tem um contrato em vigor. Envie o formulário de volta para o atual parceiro de registo.

   *Importante*: Se o novo Parceiro CSP não tiver uma relação de revendedor com o cliente, deve estabelecer uma antes da transferência da subscrição. [Pode encontrar informações sobre como fazê-lo aqui.](request-a-relationship-with-a-customer.md)

   > [!NOTE]
   > O novo sócio da CSP e o inquilino do cliente devem estar no mesmo país. 

5. Parceiro atual:

   Certifique-se de que o formulário inclui informações de contacto para ambos os administradores do parceiro. O Microsoft Support entrará em contacto com ambos os administradores para verificar a transferência. Certifique-se de ter as três assinaturas. Em seguida, utilize a opção **'Upload' de ficheiros** para anexar o formulário preenchido ao pedido de serviço existente. Um engenheiro de suporte da Microsoft entrará em conta num prazo de oito horas úteis para validar o recibo e a conclusão.

6. Novo parceiro:

   Atualize as definições de subscrição do Azure para remover o antigo parceiro da conta. Para ver quais as atribuições de funções a provisionadas, executar dois Comandos PowerShell.

   - Adicione o novo parceiro como revendedor na conta:

     ```powershell
     Connect-AzAccount -Tenant 'xxxx-xxxx-xxxx-xxxx'
     ```

     > [!NOTE]
     > O **ID** do inquilino do cliente aparece no Partner Center como o **ID** microsoft do cliente. Para encontrar o ID da Microsoft (ID do inquilino) para um cliente específico, inscreva-se no [painel](https://partner.microsoft.com/dashboard)do Partner Center . Em seguida, selecione **Clientes** do menu. Localize o cliente na lista. Selecione a seta para baixo para expandir a listagem do cliente. Verá informações sobre o *nome* de Domínio do cliente e o **ID** microsoft do cliente. Utilize o **ID microsoft** de 16 dígitos no comando PowerShell.

   - Ver funções na conta, incluindo parceiros csp anteriores:

     ```powershell
     Get-AzRoleAssignment
     ```

7. Remover permissões de acesso desatualizadas:

   1. No menu Partner Center, selecione **Clientes.**
   1. Localize o cliente na lista. Selecione (clique duplo) o nome da empresa. Esta ação abre a página **de Assinaturas** do Cliente.
   1. No menu de detalhes do cliente, selecione **Gestão de Serviço.**
   1. Em **Microsoft Azure,** selecione o link **do Portal de Gestão de Microsoft Azure.**

## <a name="next-steps"></a>Passos seguintes

- [Transfer Azure subscriptions (Transferir subscrições do Azure)](/azure/cost-management-billing/manage/transfer-subscriptions-subscribers-csp)
- [Transferir assinaturas Azure ao abrigo de um plano Azure](transfer-azure-subscriptions-under-azure-plan.md)
- Descarregue o [formulário de Transferência de Assinatura CSP](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC)
- Saiba mais sobre [o suporte a vários parceiros](multipartner.md)
- Saiba mais sobre [suporte a vários canais](multichannel.md)
