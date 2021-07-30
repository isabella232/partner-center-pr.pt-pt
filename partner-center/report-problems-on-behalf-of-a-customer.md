---
title: Reportar problemas em nome de um cliente
ms.topic: how-to
ms.date: 02/26/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: Saiba quando escalar um problema de atendimento ao cliente para a Microsoft e como arquivar um bilhete de suporte para diferentes tipos de serviços Microsoft.
author: Kim-Davis
ms.author: kimnich
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4d4c82149638ad117d54ea9b518a68ec9ae19b2b
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/29/2021
ms.locfileid: "114841152"
---
# <a name="report-a-service-problem-on-behalf-of-a-customer---including-when-and-how-to-do-so"></a>Relatar um problema de serviço em nome de um cliente - incluindo quando e como fazê-lo

**Aplica-se a**: Partner Center | Centro de Parceiros para Microsoft Cloud for US Government

**Funções apropriadas**: Administração global

Se o seu cliente estiver a ter um problema de serviço que não pode resolver, e que satisfaça os [critérios descritos em problemas de Escalate para a Microsoft,](escalate-problems-to-microsoft.md)o seu fornecedor indireto pode apresentar um bilhete de suporte para eles. Este processo também é útil para escalar questões de faturação ou litígios, e para preocupações com fraudes.

## <a name="submit-a-service-request-for-a-customer"></a>Submeter um pedido de serviço para um cliente

1. No menu Centro de Parceiros, em CSP, selecione **Clientes**

2. Na página Clientes, selecione ou procure o cliente que deseja
    
3. No menu Cliente, selecione **Pedidos de serviço**

4. A partir do menu **dropdown de novos pedidos,** selecione **Azure** ou **Office 365, Dynamics 365, Enterprise Mobility Suite**. Será redirecionado para o portal Microsoft Azure ou para o centro de administração Office 365.

>[!NOTE]
>Os parceiros de Operações de Apoio que transacionam a Dynamics 365 em CSP são obrigados a manter um acordo de apoio do plano de Apoio Avançado para Parceiros (ASfP) ou superior. Este acordo de apoio é necessário para submeter a Dynamics 365 incidentes em nome de um cliente da CSP. [Saiba mais](https://partner.microsoft.com/support/partnersupport) sobre as opções do acordo de apoio.

### <a name="microsoft-azure"></a>Microsoft Azure

> [!IMPORTANT]
> Quando necessitar de criar um pedido de serviço para o seu cliente em Azure, esteja ciente do seguinte:
>
>- Para que, como revendedor indireto, crie pedidos de serviço para o seu cliente em Azure, o seu fornecedor indireto deve conceder-lhe acesso à conta Azure do cliente. Isto é diferente de administrar em nome dos clientes para Office 365.
>
>- Embora o administrador helpdesk no Partner Center não possa criar pedidos de serviço no portal de serviços Azure, o que eles podem fazer é criar um grupo de suporte no portal de serviço Azure e dar a esse grupo permissões para registar pedidos de suporte.

1. Selecione **Novo pedido de suporte**.

2. Preencha o pedido de apoio com as informações apropriadas e, em seguida, **selecione Criar**:

   - Na secção **Básico** do pedido de apoio, certifique-se de selecionar **Fornecedor de Soluções em Nuvem** no campo **do plano de suporte.**

   - Na secção de informações de **contacto** do pedido de suporte, insira as suas informações e não as informações do seu cliente.

3. Posteriormente, reveja os pedidos de serviço do seu cliente dentro do portal Microsoft Azure selecionando pedidos de **suporte de gestão**.

Poderá ter de criar um pedido de apoio para um cliente quando não tiver permissões de administrador para esse cliente. Isto pode acontecer num de dois cenários:

- Não pediste privilégios ao administrador quando estabeleceste a relação.
- Gere apenas as assinaturas Azure de um cliente, para que não tenha permissões administrativas.
 
Em qualquer um destes casos, pode utilizar o seguinte procedimento para criar um pedido de apoio. 

1. Copie o nome de domínio do cliente na sua página de conta no Partner Center.

2. Vá ao https://portal.azure.com/ [nome de domínio do cliente]. 

3. Selecione a subscrição Azure que requer suporte.

4. Selecione **Novo pedido de suporte** e, em seguida, siga as instruções para criar o pedido. 

 
### <a name="office-365-microsoft-dynamics-crm-online-enterprise-mobility-suite"></a>Office 365, Microsoft Dynamics CRM Online, Suíte de Mobilidade Empresarial

1. Na secção Criar uma secção **de pedido de serviço,** escolha a categoria de suporte adequada. Pode ser necessário selecionar **Mais...** para ver artigos adicionais.

2. Preencha o formulário de pedido de serviço e **selecione Enviar por isso.**

   > [!TIP]
   > Certifique-se de incluir os seus dados de contacto, não os do seu cliente.

3. Mais tarde, reveja os pedidos de atendimento do seu cliente indo ao centro de administração Office 365 e selecionando **Ver todos os bilhetes de apoio.**

### <a name="support-for-commercial-marketplace-products"></a>Apoio a produtos de mercado comercial

A Microsoft não fornece suporte a produtos para produtos comerciais de marketplace. Terá de contactar o Fornecedor Independente de Software (ISV) que publicou o produto para obter suporte.

Para encontrar as informações de contacto do ISV:

1.  Na página **Marketplace,** selecione o produto com o quais necessita de ajuda.

2.  Na página do produto, encontrará informações de contacto de suporte. Esta pode ser uma ou mais das seguintes opções:

    - Um link para um ponto de entrada de suporte no site do ISV
    - Um e-mail de apoio
    - Um número de telefone de contato de suporte

## <a name="faq"></a>FAQ

Consulte as seguintes perguntas frequentes sobre pedidos de serviço que pode submeter em nome de um cliente. 

### <a name="what-is-included-as-part-of-the-support-entitlement"></a>O que está incluído como parte do Direito de Apoio?

Os pedidos de serviço devem ser apresentados através do Partner Center. Estão disponíveis para Azure, Microsoft Office 365, Microsoft Dynamics CRM Online e Suíte de Mobilidade Empresarial. Como parceiro que participa no programa Fornecedor de Soluções em Nuvem, pode esperar tempo de resposta prioritária aos seus principais problemas.

O apoio ao seu próprio inquilino não está incluído como parte do benefício de apoio da CSP. No entanto, Office 365, Microsoft Dynamics CRM Online e o Enterprise Mobility Suite não cobram uma taxa de subscrição de suporte separada para parceiros ou clientes. O Azure cobra uma taxa, mas se tiver direito a Signature Cloud Support ou a outros benefícios da Microsoft Partner Network (MPN), poderá utilizar estes benefícios para pagar essa taxa.

Este benefício aplica-se a todos os parceiros que participam no programa Fornecedor de Soluções em Nuvem, seja pago ou em período experimental. O suporte à gestão de faturação e subscrição também está incluído como uma componente gratuita deste pacote.

### <a name="how-quickly-will-i-get-an-initial-response"></a>Com que rapidez vou ter uma resposta inicial?

Os nossos tempos de resposta iniciais dependem da gravidade do incidente apresentado. A gravidade de um problema é determinada pela sua indicação de impacto comercial quando submete um pedido de serviço.

Tempos iniciais de resposta para **incidentes técnicos de correção:**

- Impacto Crítico (gravidade A): Duas horas (Perda significativa ou degradação dos serviços. Serviços de produção em baixa.)
- Impacto Moderado (gravidade B): Quatro horas (Perda moderada ou degradação dos serviços. Serviços de produção parcialmente afetados.)
- Impacto Mínimo (gravidade C): Oito horas (Perda mínima ou degradação dos serviços. Serviços ainda disponíveis ou serviços não produtivos afetados.)

Os tempos iniciais de resposta são apenas para apoio de língua inglesa. O suporte linguístico local é prestado durante o horário comercial.
Para incidentes que se enquadram nos limites do direito ao apoio, mas que não são considerados incidentes de rutura, o tempo de resposta inicial pode ser de até um dia útil.

### <a name="can-i-submit-a-service-request-by-phone"></a>Posso enviar um pedido de serviço por telefone?

Não, o suporte telefónico não é oferecido para este programa.

### <a name="what-happens-if-i-sign-into-the-azure-portal-and-bypass-partner-center"></a>O que acontece se eu assinar no portal Azure e contornar o Partner Center?

Se você assinar diretamente no portal Microsoft Azure, você está vendo o centro no seu próprio contexto, não no contexto de um cliente. É por isso que só deve assinar diretamente no portal Microsoft Azure ao criar um pedido de serviço para as suas próprias subscrições.

O seu direito de suporte ao programa CSP não fornece suporte na subscrição do seu próprio Parceiro. Por isso, precisa de fornecer o seu direito válido ao criar um pedido de serviço que diga respeito à subscrição do seu próprio Parceiro. Exemplos incluem MPN contract ID, Premier, ou um plano de apoio Azure. Para mais informações, consulte as [FAQ de Suporte Azure.](https://go.microsoft.com/fwlink/?LinkId=717532)

### <a name="what-happens-if-i-sign-into-the-office-365-admin-center-portal-and-bypass-partner-center"></a>O que acontece se eu assinar no portal do centro de administração Office 365 e contornar o Centro de Parceiros?

Se você assinar diretamente no centro de administração Office 365, você está vendo o centro no seu próprio contexto, não no contexto de um cliente. É por isso que só deve assinar diretamente no centro de administração Office 365 ao criar um pedido de serviço para as suas próprias subscrições.

### <a name="how-do-i-get-additional-dynamics-365-support"></a>Como consigo apoio adicional da Dynamics 365?

Se estiver a passar por questões relacionadas com: Subscrições de planos dinâmicos 365, licenciamento, faturação, operações de & financeira, licenças de produtos Dynamics 365 ou necessitar de apoio técnico adicional:
 
[Suporte à Dinâmica de Contato](/dynamics365/customer-engagement/admin/contact-technical-support)

## <a name="next-steps"></a>Passos seguintes

- [Fornecer suporte aos seus clientes](customer-support.md)
- [Verificar o estado de funcionamento dos serviços](check-service-health.md)
