---
title: Criar e gerir regras de encaminhamento de oportunidades de entrada
ms.topic: article
ms.date: 08/20/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: A sua empresa pode criar regras para decidir como é que uma oportunidade de co-venda recebida dos vendedores da Microsoft é encaminhada.
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: efb76953b05bfb10a18657155349e267ee84f456
ms.sourcegitcommit: 42238e2ce36725631f542887c9112593d701ca9c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/20/2021
ms.locfileid: "122621707"
---
# <a name="create-and-manage-inbound-opportunities-routing-rules"></a>Criar e gerir regras de encaminhamento de oportunidades de entrada

**Funções adequadas**: Administração de referências | Utilizador de referências

> [!IMPORTANT]
> **A criação de regras de encaminhamento é opcional.** É recomendado apenas para grandes empresas com presença em todo o mundo ou se a sua empresa tem uma hierarquia complexa de MPN onde a gestão de referência deve ser feita a um nível específico de localização com base nos mercados de clientes e soluções.

## <a name="introduction"></a>Introdução

A funcionalidade descrita neste documento ajudará a sua empresa a configurar regras, o que pode ajudar a encaminhar as oportunidades de Co-venda enviadas pelos vendedores da Microsoft para as localizações MPN à sua escolha. Por padrão, as referências do vendedor da Microsoft serão enviadas para a localização MPN associada à solução de Co-venda incluída na oportunidade. As regras de encaminhamento se forem criadas ajudarão a sua empresa a anular o encaminhamento predefinido. Apenas [**a administração de encaminhamento**](permissions-overview.md#manage-referrals) com todo o âmbito da organização pode criar e editar regras de encaminhamento. Os parceiros com papel [**de utilizador de encaminhamento**](permissions-overview.md#manage-referrals) só podem ver as regras de encaminhamento para entender como as referências estão a ser encaminhadas dentro da sua empresa.

As regras não serão aplicadas retrospetivamente. Quaisquer referências criadas no passado ou com uma configuração mais antiga da regra de encaminhamento não serão atualizadas. Quaisquer alterações feitas às regras são aplicáveis instantaneamente.

Há três pivôs principais para qualquer regra.

- **Mercado de clientes** - O mercado onde está localizada a empresa cliente

- **Solução** - soluções publicadas pela sua empresa quer através do portal OCP GTM quer do mercado comercial

- **Localização MPN** - a localização MPN para a qual a referência deve ser encaminhada

Cada regra pode ser lida como - **Para as referências enviadas pelos vendedores da Microsoft com a solução(s) da minha empresa, encaminhe-as para esta localização MPN**

> [!Note]
> As regras de encaminhamento de entrada são aplicáveis apenas para oportunidades de co-venda enviadas pelos vendedores da Microsoft para a sua empresa.

## <a name="navigation"></a>Navegação

Pode criar regras de encaminhamento no **separador Referências** na página **de definições de Conta.** Para navegar na página, selecione o ícone de definições ao lado do ícone do utilizador no canto superior direito e, em seguida, selecione o **separador Referências** no painel de navegação esquerdo.

## <a name="initial-setup"></a>Configuração inicial

**As regras de configuração do encaminhamento não são obrigatórias**. Se a sua empresa decidir utilizar as regras de encaminhamento para tirar partido da lógica de encaminhamento, pode começar por importar as regras padrão que o sistema de gestão de referência utiliza para encaminhar as referências. A lógica atual utiliza o ID MPN associado à solução para encaminhar todas as referências de entrada dos vendedores da Microsoft, independentemente do país do cliente. Estão disponíveis para a sua referência e **podem ser importados com um clique** como regras de encaminhamento. Uma vez concluída a ação de importação, as regras serão aplicadas para todas as novas referências enviadas pelos vendedores da Microsoft. A sua empresa pode editar ou eliminar as regras existentes e criar novas regras, se necessário. Só [**a administração de referência**](permissions-overview.md#manage-referrals) com o âmbito global pode importar as regras. A mesma permissão é necessária para quaisquer alterações subsequentes às regras de encaminhamento.

> [!IMPORTANT]
> **Existem alterações na lógica de notificação de email.** Assim que as regras tiverem sido importadas, os e-mails que foram anteriormente enviados para contactos de **solução carregados** no separador Co-venda no mercado comercial não serão mais enviados. Apenas serão notificados os administradores de **[encaminhamento](permissions-overview.md#manage-referrals)** do local da MPN para o qual a oportunidade de co-venda é enviada.

## <a name="override-rules"></a>Regras de substituição

Pode anular dois tipos de regras e anular uma condição específica da regra padrão. Na regra por defeito, só pode alterar o local de MPN para o qual as referências devem ser encaminhadas. Os outros dois tipos de regras que pode sobrepor-se são os que têm **todas as soluções** e todos os **mercados** como condições nas regras.

**Todos os mercados se sobrepõem** - Assumindo que criou uma regra que diz, para todos os mercados de clientes e uma determinada solução A, encaminhar as referências para a localização MPN M1. Pode anular tal regra com um mercado específico e a mesma combinação de soluções. O exemplo pode ser "para as referências que contêm clientes do mercado Reino Unido e solução A, encaminhá-lo para a localização M2 da MPN.

**Todas as soluções se sobrepõem** - Assumindo que criou uma regra que diz, para todas as soluções e um determinado mercado MKT1, encaminhar as referências para a localização M1 da MPN. Pode anular tal regra com uma solução específica e a mesma combinação de mercado. O exemplo pode ser "para as referências que contêm clientes do mercado MKT1 e solução B, encaminhá-lo para a localização MPN M2.

Abaixo da tabela mostra o resumo de tipos de soluções que pode sobrepor

| **Tipo** | **Pode anular?** |
|-------|-------|
|Predefinição| No |
|Todos os mercados| Sim|
|Todas as soluções| Sim|
|Uma solução específica e uma combinação específica do mercado| No|

> [!Note]
> Pode alterar a localização mpn para a regra por defeito, mesmo que não possa alterar mais nada nessa regra.

## <a name="rules-evaluation"></a>Avaliação de regras

Se a sua empresa tiver várias regras que podem ser aplicadas a um cenário, abaixo dos critérios de avaliação utilizados.

- O primeiro controlo será para uma regra com a solução específica e a combinação de mercado, que estão na oportunidade de entrada. Uma correspondência direta com tal regra terá precedência sobre todas as outras regras.
- Se o primeiro controlo falhar, verificamos se existem alguma regra que contenha a solução mencionada no encaminhamento com condição de mercado definida como todos os mercados.
- Se o segundo controlo falhar, verificamos se existem regras em que todas as soluções são mencionadas como critérios de solução para um mercado específico.
- Se a terceira verificação também falhar, utilizamos a regra Predefinido.

> [!Note]
> Não é possível criar uma regra que entra em conflito com outras regras num determinado nível de localização e solução. A UI lançará um erro com o nome da regra que está em conflito com a sua configuração se estiver a tentar criar uma regra conflituosa.

## <a name="example"></a>Exemplo

As regras de encaminhamento de entrada serão explicadas com a ajuda das regras de encaminhamento criadas para a Contoso Corporation. Antes de compreender como as regras serão aplicadas, entendamos a hierarquia da MPN e a configuração do utilizador na Contoso Corporation.

#### <a name="mpn-hierarchy-of-contoso-corporation"></a>Hierarquia da MPN da Corporação Contoso

| **ID do MPN** | **Tipo** | **Endereço** |
|-------|-------|-------|
|999999| Global| Um caminho de Contoso, **Redmond, Estados Unidos da América**|
|555555| Localização| One Contoso way, **Londres, Reino Unido**|
|666666| Localização| Um caminho de Contoso, **Singapura, Singapura**|
|777777| Localização| Um caminho de Contoso, **Bengaluru, Índia**|

#### <a name="sellers-from-contoso-corporation"></a>Vendedores da Corporação Contoso

Abaixo estão os vendedores com as respetivas funções de referência e âmbito na Contoso Corporation.

| **Nome** | **Role** | **Âmbito** |
|-------|-------|-------|
|Vendedor Um|Administrador de encaminhamento|Organização Inteira|
|Vendedor Dois|Administrador de encaminhamento|Bengaluru|
|Vendedor Três|Utilizador de encaminhamento|Londres|
|Vendedor Quatro|Utilizador de encaminhamento|Singapura|

#### <a name="inbound-routing-rules-for-contoso-corporation"></a>Regras de encaminhamento de entrada para a Contoso Corporation

Assuma que o conjunto de regras abaixo foi criado pelo Vendedor 1 para a Contoso Corporation. Apenas **o Vendedor Um** pode criar estas regras, uma vez que a [administração de encaminhamento](permissions-overview.md#manage-referrals) em todo o âmbito da organização é necessária para criar e editar regras.

| **Mercados** | **Soluções** | **Localização MPN** | **Nome da regra de encaminhamento** |
|-------|-------|-------|-------|
|Todos os mercados|Todas as soluções|Redmond|Predefinição|
|Reino Unido|Todas as soluções|Londres|Reino Unido todas as soluções|
|Todos os mercados|Sol-ABC|Singapura|Sol-ABC em todos os mercados|
|Índia|Sol-PQR|Bengaluru|Índia-Sol-PQR|

#### <a name="summary-of-routing-for-various-scenarios-based-on-the-rules-for-contoso-corporation"></a>Resumo do encaminhamento para vários cenários baseado nas regras da Contoso Corporation

| **Não** | **Cenário** | **Mercado de Clientes** | **Soluções incluídas** |**Regra de encaminhamento aplicada** |**Atribuição mpn** |**Acesso a referências** |
|-----|----------|-------|-------|-------|-------|-----------|
| 1|Nenhuma solução específica e jogo de regras de mercado|Reino Unido|SOL-PQR|Global|999999| Seller One, Seller Two, Seller Three (se adicionado à equipa), Seller Four (se adicionado à equipa)|
| 2|Todas as soluções e uma regra de mercado específica combinam|Reino Unido|SOL-PQR|Reino Unido todas as soluções|555555| Vendedor Um, Vendedor Três (se adicionado à equipa) |
| 3|Solução específica e todas as regras de mercados combinam|Nigéria|SOL-ABC|SOL-ABC em todos os mercados|666666| Vendedor Um, Vendedor Quatro (se adicionado à equipa) |
| 4|Solução específica e jogo de regras de mercado|Índia|SOL-PQR|Índia-Sol-PQR|777777| Vendedor Um, Vendedor Dois|
| 5|Encaminhamento de entrada com uma solução não detida pela sua empresa|Estados Unidos da América|SOL-XYZ|Global|999999| Seller One, Seller Two, Seller Three (se adicionado à equipa), Seller Four (se adicionado à equipa)|

## <a name="next-steps"></a>Passos seguintes

- [Gerir Oportunidades de Co-venda](manage-co-sell-opportunities.md)

- [Obtenha o conector co-venda para Dynamics 365 CRM](connector-dynamics.md)

- [Obtenha o conector co-venda para Salesforce CRM](connector-salesforce.md)
