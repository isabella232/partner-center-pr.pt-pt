---
title: Vender software no local através da CSP
ms.topic: how-to
ms.date: 03/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: Saiba como os parceiros do programa CSP podem comprar, gerir, vender e cancelar subscrições de software no local em nome dos clientes no Partner Center.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f58f120d376b98f9fa054f0bec87f324874ce0bb
ms.sourcegitcommit: b78e85a0bc62e3536b067417cb3db7899cda4f97
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/06/2021
ms.locfileid: "129584903"
---
# <a name="sell-on-premises-software-through-the-cloud-solution-provider-csp-program"></a>Venda de software no local através do programa Fornecedor de Soluções em Nuvem (CSP)

**Funções adequadas**: Agente administrador | Administrador global

O software no local em CSP suporta uma transição suave para a nuvem, introduzindo software no local num programa focado na nuvem. Esta nova oferta ajuda a trazer o parceiro de valor acrescentado para cada cenário de compra, uma vez que fornece uma única plataforma para transacionar todos os produtos da Microsoft. Como CSP, pode agora vender software no local através do Partner Center, além de Open, EA e outros programas atualmente em uso.  
 
Ao mesmo tempo que garantimos o melhor valor geral do cliente com opções de licenciamento de software no local, também tornamos o modelo de negócio o mais amigável possível. O licenciamento simples de software no local em CSP significa previsibilidade de custos e um processo de venda simplificado para si. Este novo modelo de negócio facilita a aquisição, gestão e preço no local do software para os seus clientes, permitindo-lhe focar-se em negócios vencedores com um portfólio alargado de soluções de valor acrescentado de gestão de TI.

## <a name="buy-software-subscriptions-on-behalf-of-customers"></a>Comprar subscrições de software em nome dos clientes

Para comprar subscrições de software em nome de um cliente, vá à página de detalhes do cliente, selecione Produtos Add e, em seguida, siga as instruções no ecrã para criar e pagar a sua encomenda.

> [!NOTE]
> Para mais informações, consulte este [guia para encomendar e realizar através do Partner Center.](https://partner.microsoft.com/resources/detail/guide-to-ordering-and-fulfillment-through-partner-center-pdf)

## <a name="activate-and-manage-software-subscriptions"></a>Activate and manage software subscriptions (Ativar e gerir subscrições de software)

Depois de ter adquirido o seu software, você ou os seus clientes precisam descarregá-lo (parceiros usando Partner Center; clientes que usam o Centro de Administração Microsoft 365). Utilize o seguinte procedimento para o fazer. É importante compreender os riscos associados à cópia de links e ao descarregamento de software. Para obter mais informações, consulte **o Use Partner Center para obter transferências de software de clientes e chaves de licença** no Guia de Operações do Centro [Parceiro.](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf)

> [!NOTE]
> Você deve ser um agente de administração no Partner Center para obter o link para chaves e downloads.

1. Aceda à página de detalhes do seu cliente e, em seguida, selecione **Software**. Verá uma lista de todo o software que comprou em nome do cliente.

2. Escolha **a versão do** produto, **idioma,** **bit**, e selecione Obter chaves **e downloads**. 

3. Escolha **a Chave Get** que irá exibir o produto de 32 dígitos num diálogo pop-up que pode copiar e enviar ao cliente. 

4. Escolha **baixar** para baixar as partes. 

5. Escolha **Copy Link** se quiser enviar ao cliente o link para o download de bits. 

6. Também pode **cancelar** a encomenda de software e receber 100% de crédito (se for feito dentro do período de 60 dias de política de cancelamento).

> [!NOTE]
> Apenas os clientes têm acesso para ver as chaves do produto e descarregar informações no Administração Microsoft 365 Center (função global de administração necessária). Os parceiros devem usar o Partner Center para ver esta informação.

> [!NOTE]
> As compras de CSP são ativadas através de uma chave de ativação múltipla (MAK). Serviço de Gestão de Chaves chaves (KMS) não são permitidas, mesmo mediante pedido. 

## <a name="move-a-customers-on-premises-license-from-vl-to-csp-with-no-downtime"></a>Mover a licença de um cliente no local de VL para CSP sem tempo de inatividade

Apesar de KMS chaves não estiverem disponíveis em CSP, ainda pode mover as licenças do seu cliente no local de VL para CSP e evitar tempo de inatividade devido ao interruptor do canal de compra. KMS distribui as licenças aos clientes, e geralmente permanecem ativas durante 180 dias antes de o dispositivo tentar renovar essa ativação. Isto significa que o dispositivo já será ativado e funcionará durante algum tempo antes de surgirem quaisquer problemas. 

Se o cliente implementar o novo MAK durante este tempo, manualmente ou de forma escrita (utilização), `slmgr.vbs` não ocorrerá tempo de inatividade. Se o cliente não implementar o novo MAK durante este tempo e tentar renovar a licença mais tarde, o dispositivo poderá ficar limitado ou bloqueado em algumas funcionalidades até ser reativado. 

Para obter mais informações, aceda aos [clientes Ativados que executam Windows 10 (Windows 10) - Windows Implantação](/windows/deployment/volume-activation/activate-windows-10-clients-vamt#key-management-service-activation-renewal). Para assistência com este tipo de implantação, pode submeter um pedido [de Pré-Venda Técnica e Serviços de Implantação.](/partner-center/technical-benefits#submit-a-technical-presales-and-deployment-services-request)

## <a name="cancel-a-purchase"></a>Cancelar uma compra

Utilize o seguinte procedimento para cancelar uma compra. Uma vez que o cancelamento esteja concluído, a chave de software será revogada.

> [!NOTE]
> Deve ser um agente administrativo para cancelar uma compra. 

1.  Antes de iniciar o processo, certifique-se de que tem o seguinte: 
    - O cliente inquilino GUID ou nome de domínio
    - ID de encomenda ou ID de subscrição
    - Motivo de reembolso
    - Montante solicitado

2.  Na página de detalhes do cliente, selecione **Software**. Verá uma lista de todo o software que comprou. 

3.  Localize o software que pretende cancelar e **selecione Cancelar**. O Relatório abre um problema com a página **do Partner Center.** 

4.  Em **Detalhes**, na lista **de tipos de problemas,** selecione **CSP Purchase/Refund em nome dos clientes**.

5.  Preencha os campos **de Impacto** e **Título.** 

6.  No campo **Descrição,** forneça o seguinte: 
    -   O cliente inquilino GUID ou nome de domínio
    -   ID de encomenda ou ID de subscrição
    -   Motivo de reembolso
    -   Montante solicitado

7.  No campo **Contacto,** insira o seu nome, endereço de e-mail e número de telefone. 

8.  Se precisar de anexar um ficheiro por qualquer motivo, **selecione Adicionar ficheiros**. Este passo é opcional. 

9.  Quando terminar, **selecione Submeter.**
