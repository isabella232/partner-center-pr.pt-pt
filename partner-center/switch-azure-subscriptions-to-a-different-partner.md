---
title: Transferência da subscrição da Azure para outro parceiro
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como alterar o parceiro do programa Cloud Solution Provider associado às subscrições Azure de um cliente.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: dhirajgandhi
ms.author: dhgandhi
ms.date: 07/29/2020
ms.openlocfilehash: 992dd7f9901efd0176395fb626e4048d5229e82b
ms.sourcegitcommit: e10d2a19dea7e317d227d7fbdcf1bbc3dc4f6257
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/13/2020
ms.locfileid: "92530236"
---
# <a name="learn-how-to-transfer-a-customers-azure-subscriptions-to-another-partner"></a>Saiba como transferir as subscrições do Azure de um cliente para outro parceiro

**Aplica-se a**

- Centro de Parceiros para Microsoft Cloud para governo dos EUA
- Centro de Parceiros para Microsoft Global Cloud
- Parceiros no programa Cloud Solution Provider (CSP)

Este artigo descreve como um cliente pode mudar os seus serviços Microsoft Azure de um Cloud Solution Provider (CSP) para outro.

Para mudar os serviços ou subscrições do Azure de um cliente para um parceiro diferente, siga estes passos manuais. Tanto o parceiro como o cliente precisam de completar os passos.

>[!Note]  
>Atualmente, apenas os Fornecedores Diretos ou Indiretos podem transferir subscrições.
>Não é possível alterar parceiros para subscrições do Cloud Solution Provider associadas ao plano Azure, Office 365, Enterprise Mobility Suite ou Microsoft Dynamics CRM.

## <a name="switch-partners-for-azure-subscriptions"></a>Parceiros da Switch para subscrições Azure

1. Para transferir uma subscrição da Azure para um novo parceiro, o cliente deve iniciar o processo e contactar o seu atual parceiro de registo por escrito.

   >[!Note]
   > É da responsabilidade do atual parceiro criar o bilhete de serviço que inicia o processo de transferência. A Microsoft não pode intervir em nome do cliente ou do novo parceiro. O cliente deve planear trabalhar em estreita colaboração com o parceiro atual para que a transição corra bem.

2. O parceiro para a subscrição precisa de fazer as seguintes tarefas:

   Crie um bilhete de serviço Azure do Partner Center para solicitar uma transferência de assinatura:

   1. A partir do menu Partner Center, selecione **Clientes,** selecione o seu cliente da lista e, em seguida, selecione **a gestão do Serviço** . 

   2. Na secção **de bilhetes De Suporte,** selecione o novo dropdown de **bilhetes** e escolha **o Microsoft Azure** .
   
   3. A partir do [portal Azure,](https://portal.azure.com)selecione **Novo pedido de suporte** .
   
   4. No Passo 1, escolha a **gestão de Subscrição** como o tipo de problema, especifique o ID de subscrição que pretende ser transferido e escolha o **Cloud Solution Provider** como o plano de suporte.
   
   5. No passo 2, selecione **o impacto C-Minimal** e escolha **Outras Perguntas Gerais** como o tipo de problema.
   
   6. Descarregue o [formulário de Transferência de Assinatura CSP](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4ATIA).

3. O parceiro para a subscrição: Preencha o [formulário de Transferência de Assinatura CSP,](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4ATIA)assine-o e, em seguida, envie-o ao cliente. 

   Para preencher o formulário, necessitará das seguintes informações:

   - As informações de contacto do parceiro atual e a identificação da Microsoft. No menu Partner Center, selecione perfil de **Organização de Definições de Contas** e utilize o &gt; **Organization profile** **ID** da **Microsoft,** nome da Organização e **Endereço** listados lá.

   - O iD da Microsoft do cliente. No menu Partner Center, selecione **Clientes** e, em seguida, expanda a listagem do cliente para ver o seu **ID Microsoft** .

   - O ID de assinatura para transferir. Na listagem de clientes expandida, selecione **Ver Subscrições,** em seguida, expandir a subscrição escolhida para ver o **ID de subscrição** .

   >[!Note]
   >A transferência de uma subscrição resulta em dois IDs de subscrição que verá na página de Subscrição de **Edição** da subscrição transferida: **1** - O ID de subscrição do Partner Center é utilizado para efeitos de faturação. **2** - O ID de subscrição original do Azure é mantido e aparecerá no Partner Center, bem como no portal Azure Management. Esta identificação aparecerá no seu ficheiro de reconhecimento.  **Ao registar bilhetes de suporte, você precisa usar ambos os IDs.**

4. O cliente e novo parceiro para a subscrição:

   Reveja o formulário, preencha informações sobre o novo parceiro e assine-o. Confirme que o novo cliente tem um contrato em vigor. Envie o formulário de volta para o atual parceiro de registo.

   *Importante* : Se o novo Parceiro CSP não tiver uma relação de revendedor com o cliente, deve estabelecer uma antes da transferência da subscrição. [Pode encontrar informações sobre como fazê-lo aqui.](request-a-relationship-with-a-customer.md)

   >[!Note]
   >O novo sócio da CSP e o inquilino do cliente devem estar no mesmo país. 

5. Parceiro atual:

   Certifique-se de que o formulário inclui informações de contacto para ambos os administradores do parceiro. O Microsoft Support entrará em contacto com ambos os administradores para verificar a transferência. Certifique-se de ter as três assinaturas. Em seguida, utilize a opção **'Upload' de ficheiros** para anexar o formulário preenchido ao pedido de serviço existente. Um engenheiro de suporte da Microsoft entrará em conta num prazo de oito horas úteis para validar o recibo e a conclusão.

6. Novo parceiro:

   Atualize as definições de subscrição do Azure para remover o antigo parceiro da conta. Para ver quais as atribuições de funções a provisionadas, executar dois Comandos PowerShell.

   - Adicione o novo parceiro como revendedor na conta:

     ```powershell
     Connect-AzAccount -Tenant 'xxxx-xxxx-xxxx-xxxx'
     ```

     >[!NOTE]
     > O **ID** do inquilino do cliente aparece no Partner Center como o **ID** microsoft do cliente. Para encontrar o ID da Microsoft (ID do inquilino) para um cliente específico, inscreva-se no [painel](https://partner.microsoft.com/dashboard)do Partner Center . Em seguida, selecione **Clientes** do menu. Localize o cliente na lista. Selecione a seta para baixo para expandir a listagem do cliente. Verá informações sobre o *nome* de Domínio do cliente e o **ID** microsoft do cliente. Utilize o **ID microsoft** de 16 dígitos no comando PowerShell.

   - Ver funções na conta, incluindo parceiros csp anteriores:

     ```powershell
     Get-AzRoleAssignment
     ```

7. Remover permissões de acesso desatualizadas

   - No menu Partner Center, selecione **Clientes.**
   - Localize o cliente na lista. Selecione (clique duplo) o nome da empresa. Isto abre a página **de Assinaturas** do cliente.
   - No menu de detalhes do cliente, selecione **Gestão de Serviço.**
   - No **Microsoft Azure,** clique no link para ir ao **Microsoft Azure Management Portal** .

## <a name="next-steps"></a>Passos seguintes

- Descarregue o [formulário de Transferência de Assinatura CSP](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4ATIA).

- Saiba mais sobre [o suporte a vários parceiros.](multipartner.md)

- [suporte multi-parceiro.](multipartner.md)
- [suporte multicanal](multichannel.md).
- [Transfer Azure subscriptions](/azure/cost-management-billing/manage/transfer-subscriptions-subscribers-csp) (Transferir subscrições do Azure)