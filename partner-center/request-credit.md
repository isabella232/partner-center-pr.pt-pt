---
title: Request an SLA credit from Microsoft (Pedir um crédito do SLA à Microsoft)
ms.topic: article
ms.date: 03/31/2021
description: Conheça os benefícios, restrições e procedimentos para solicitar um crédito de acordo de nível de serviço (SLA) da Microsoft se os seus clientes experimentarem uma falha de serviço.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: 100a3d2988c19d57f7426c7212b7464d8e96dc94
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110152958"
---
# <a name="how-and-when-to-request-a-service-level-agreement-sla-credit-from-microsoft"></a>Como e quando solicitar um crédito de nível de serviço (SLA) da Microsoft

**Funções adequadas**: Agente administrador | Administração global

Pode solicitar **créditos de acordo de nível de serviço (SLA)** da Microsoft se um serviço que está a prestar aos seus clientes tiver uma paragem.

## <a name="sla-credit-calculation"></a>Cálculo do crédito SLA

Os créditos SLA da Microsoft são determinados com base em quais os serviços foram impactados. Por exemplo, se o seu cliente tiver uma suite Office 365 mas apenas tiver uma paragem do SharePoint, o crédito SLA é aprovado apenas para o SharePoint e não para todo o plano do cliente.

*Os créditos são avaliados de forma pró-avaliação com base no serviço afetado e na duração da paralisação.* Para ver os tipos de cenários que se qualificam para créditos SLA, consulte o [documento SLA Consolidado de Serviços Online.](http://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=37) Esta informação aplica-se também aos serviços vendidos através do programa Cloud Solution Provider.


## <a name="request-an-sla-credit"></a>Solicite um crédito SLA

*O parceiro Cloud Solution Provider (CSP) deve apresentar a reclamação e todas as informações necessárias até ao final do mês civil seguinte ao mês em que ocorreu o incidente.* Por exemplo, se o incidente ocorreu no dia 15 de fevereiro, a Microsoft deve receber a reclamação e todas as informações necessárias até 31 de março. Clientes finais e revendedores indiretos não podem apresentar crédito sla; quer o prestador indireto quer o parceiro de conta direta devem apresentar reclamações em seu nome.

>[!NOTE]
>Incidentes consultivos[(Como verificar a saúde do serviço Microsoft 365](/microsoft-365/enterprise/view-service-health#incidents-and-advisories)) não são elegíveis para créditos SLA.

### <a name="required-information"></a>Informação necessária

O nome do cliente, o identificador de inquilinos, o bilhete de sócio#, e o carimbo de data/hora criado do bilhete não são suficientes para que uma reclamação seja processada.

Antes [de submeter um pedido de crédito SLA](#submit-sla-credit-request) à Microsoft, deve recolher **todas as** seguintes informações para incluir no seu bilhete de suporte:

- O cliente do inquilino GUID
- O [identificador do incidente de paragem?](#outage-incident-identifier)
- Prova de que o cliente foi impactado pela paralisação e solicitou um crédito SLA.
- As assinaturas impactadas foram adquiridas através da CSP? *(sim* ou *não)*

#### <a name="evidence-that-proves-customer-impact"></a>Evidência que comprova o impacto do cliente

- Informações sobre o tempo e duração do tempo de inatividade
- O número e localização dos utilizadores afetados (se aplicável)
- Descrições das suas tentativas de resolver o incidente no momento da ocorrência
- Um e-mail do cliente afetado solicitando apoio e, posteriormente, crédito
- O número de bilhete de suporte e detalhes do contacto com o cliente no que diz respeito à resolução do impacto do serviço


#### <a name="outage-incident-identifier"></a>Identificador de incidente de interrupção

Pode encontrar o identificador para o incidente de paragem na página **de Saúde** do Serviço no centro de administração microsoft 365. O **ID de incidente de interrupção** é um número precedido por uma abreviatura de duas letras que indica o serviço afetado (por exemplo, *EX25194* para uma paragem online de troca). A tabela seguinte descreve abreviaturas de serviço comuns:

| Abreviatura de duas letras | Serviço Microsoft |
| ----------------------- | ----------------- |
| EX | Exchange Online |
| FO | Troca de Proteção Online |
| SB | Skype para Business Online (anteriormente Lync Online) |
| SO | Assinatura de escritório |
| PB | Power BI para Office 365 |
| SP | SharePoint Online |
| YA | Empresa Yammer |
| MO | Erro do portal |

### <a name="submit-sla-credit-request"></a>Submeter pedido de crédito SLA

Para submeter o seu pedido de crédito SLA à Microsoft através do painel partner Center:

1. Inicie sessão no dashboard do Centro de Parceiros.
2. No menu à esquerda, escolha **pedidos** de Serviço e, em seguida, selecione **pedidos de suporte do Parceiro**.
3. Na página de pedido do **Parceiro,** escolha **Novo pedido.**
4. Na página **Iniciar o pedido,** encontre a secção **CSP - clientes, encomendas e subscrições**. Nesta secção, escolha **Selecionar um tipo de problema,** em seguida, selecione **pedidos de crédito de serviços ao cliente**.
5. Na página **de soluções Recomendadas,** em Que precisa de **mais ajuda?**
6. Na página **Detalhes,** preencha a secção **de detalhes do 'Emissão'.** Na caixa de texto **Details,** certifique-se de inserir as [informações necessárias](#required-information) que recolheu anteriormente.
7. Escolha **Enviar** para enviar o seu pedido de crédito SLA.

## <a name="next-steps"></a>Passos seguintes

- [Reportar problemas em nome do seu cliente](report-problems-on-behalf-of-a-customer.md)
