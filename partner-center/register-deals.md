---
title: Registar as suas ofertas
ms.topic: article
ms.date: 06/29/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Quando registas um acordo que ganhaste no Partner Center, ajuda a Microsoft a proporcionar-te mais oportunidades no futuro.
author: rajap-ms
ms.author: rajap
ms.localizationpriority: medium
ms.openlocfilehash: eaa9bb6f8e57033669ef584e7c52c0d050a532e0
ms.sourcegitcommit: 8235c89e789cdb5115fc1c19151fa8e97c743fe5
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/30/2021
ms.locfileid: "113080670"
---
# <a name="register-deals-youve-won-in-partner-center"></a>Registar ofertas que ganhou no Partner Center

**Funções adequadas**: Administração de referências

Pode registar ofertas que ganhou no Partner Center, fornecendo informações adicionais sobre o contrato. Esta informação ajuda-nos a proporcionar-lhe mais oportunidades no futuro.

Há dois caminhos que levam ao registo de negócios:

- Criou um novo acordo na secção **de oportunidades de Co-venda,** e o seu negócio cumpre os critérios para o registo de negócios.
- Quer reportar um acordo fechado da ISV Connect, que não foi co-vendido com a Microsoft.

## <a name="register-a-deal-originating-from-a-co-sell-opportunity"></a>Registar um negócio originário de uma oportunidade de co-venda

Se pretender registar um negócio originário de uma oportunidade de co-venda, o seu negócio deve cumprir os seguintes requisitos de elegibilidade:

- O tipo de negócio é co-venda ou liderado por parceiros (você optou por permitir que os vendedores da Microsoft vejam esta oferta).
- Há pelo menos uma solução elegível para incentivos no negócio. Uma solução é elegível para incentivos se contiver pelo menos uma das seguintes etiquetas:
  - Co-venda Azure IP
  - Prémio de Aplicações Empresariais
  - Norma de Aplicações empresariais
- O estado do acordo é "Won".
- Se o tipo de negócio for co-vendido, a Microsoft deve ter aceitado o convite ou marcado o negócio como ganho. Pode ver o estado da Microsoft olhando para o cartão microsoft abaixo dos detalhes da sua oferta.

Se tiver cumprido os requisitos de elegibilidade, será automaticamente solicitado que registe o seu acordo com um botão **Register now** mostrado na barra de progresso do negócio:

:::image type="content" source="images/register-deals.png" alt-text="Screenshot mostrando a barra de progresso do negócio.":::

> [!NOTE]
> Se o item **de registo do Deal** não aparecer na barra de progresso do negócio para o seu negócio, então o negócio não satisfaz todos os requisitos para o registo de negócio.

Depois de clicar **em Registar agora,** será redirecionado para a página De Registo de Negócios e solicitado para preencher um formulário com o qual inclui informações pré-preenchidas para o seu cliente e solução. Preencha o formulário usando as instruções abaixo e clique em **Registar**.

Após o registo, serão criados um ou dois registos de registo de negócios dependendo da solução.

- Se a sua solução for elegível para o ISV Connect, será criado um registo de registo de negócio ISV Connect. Este registo de registo de negócio será usado para faturação.
- Se a sua solução for elegível para incentivos ip Co-sell, então será criado um registo de registo de negócio de co-venda IP. Este registo de contrato será revisto e aprovado ou rejeitado pela equipa de revisão do acordo de Co-venda.

## <a name="report-a-closed-isv-connect-deal"></a>Reportar um negócio fechado isv connect

Para reportar um negócio fechado do ISV Connect, vá ao **separador de registo do Negócio** e clique + **Reporte fechado isv Connect deal**. Preencha os campos necessários e clique em **Registar.** Este registo de registo de negócio será usado para faturação.

## <a name="fill-out-the-deal-registration-form"></a>Preencha o formulário de registo de negócio

> [!NOTE]
> Pode filtrar ofertas com o nome do cliente, estado e tipo de negócio. Para tal, clique no botão **Filtro** na parte superior da página 'Registar oferta'.

Quer tenha vindo a negociar o registo de uma oportunidade de co-venda, ou se está a reportar um negócio fechado do ISV Connect, que não foi co-vendido com a Microsoft, será solicitado que preencha os seguintes campos no formulário de registo de negócio.

- **Detalhes do cliente**: **Insira** o nome da Empresa para o seu cliente e selecione o seu **País/Região.** Em **seguida,** entre na sua Cidade e **Estado/Província.**
- **Solução**: Selecione a solução que será utilizada para o negócio. Se não vir a solução certa listada, contacte o suporte.
- **Tipo de contrato**: Especificar se este negócio é um **novo** contrato ou uma **renovação** de um contrato anterior.
- **Valor total do contrato**: O valor total esperado para o noivado. Este valor deve incluir todas as taxas de software e serviço, mas não custos de hardware. Certifique-se de selecionar a moeda apropriada.
- **Valor da solução**: O valor total da solução cloud que será usada para o negócio. Certifique-se de incluir todos os custos associados com taxas de software e manutenção, mas não inclua itens reembolsáveis, taxas de personalização não recorrentes ou taxas de licença CSP diretamente associadas pagas pela Microsoft.
- **A solução será implementada no Azure? Caso contrário, escolha Outros**: Selecione **Azure** ou **Outro**.
- **O consumo da solução será gerido pelo inquilino do parceiro ou inquilino do cliente?**  
- **Data de início do contrato**: A data em que o contrato começará. Para ofertas pay-as-you-go (PAYG), utilize a data da primeira fatura. Por design, o Partner Center não o deixará introduzir uma data de início mais cedo do que a data de assinatura do contrato. Isto pode ter impacto em algumas ofertas, tais como implementações IP que começam antes da data de sinalização. Para introduzir estas ofertas com sucesso, utilize a data de assinatura do contrato **para os** campos de data de assinatura e início da data quando estiver a enviar. (O contrato deve indicar explicitamente a duração do negócio para que a ACV possa ser devidamente calculada.)
- **Data final do contrato**: Se o contrato terminar numa data específica, selecione **Tem uma data de fim** e forneça essa data. Se o contrato não tiver uma data de final específica, selecione **Perpetual**. Para ofertas pay-as-you-go (PAYG), utilize a data da última ou mais recente fatura.
- **Contrato assinado data**: Data em que o contrato final foi assinado pela sua organização e pelo cliente. Para ofertas pay-as-you-go (PAYG), utilize a data da primeira fatura.
- **Contacto de registo**: **O nome próprio**, **apelido,** **número de telefone** e **e-mail** para uma pessoa da sua organização que possamos contactar se precisarmos de mais detalhes sobre qualquer informação fornecida aqui.

Quando tiver concluído todas as secções da página, clique em **Registar**.

- Se o negócio for um negócio ISV Connect, você vai notar que o estado do negócio é "Submetido, Concluído". Não são necessárias mais medidas neste registo de contrato. Este disco será usado para faturação.
- Se o negócio for um acordo de co-venda IP, você vai notar que o estado do negócio é "Submetido". A equipa de revisão de negócios da Microsoft Co-sell irá rever as informações que forneceu neste registo de registo de negócio. A equipa de revisão solicitará mais medidas consigo, se necessário, ou aprovará/rejeitará diretamente o negócio.
- Se está a registar um negócio originário de uma oportunidade de Co-venda, e vê que foram criados dois registos de registo de negócios, significa que a solução no seu negócio é elegível tanto para o ISV Connect como para a CO-venda IP. O registo ISV Connect será utilizado para faturação. O disco de co-venda IP será revisto pela equipa de validação de negócios de Co-venda.

