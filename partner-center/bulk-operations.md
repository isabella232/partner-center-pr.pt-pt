---
title: Operações a granel através de ficheiros excel em referências
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como descarregar, criar ou atualizar oportunidades de co-venda usando ficheiros excel
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 02/03/2021
ms.openlocfilehash: 831fbc294bfd82caef77489f74747bb32cf0b12c
ms.sourcegitcommit: 64b43ad8fb7bb56628450bea06b9cd2606c36b03
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/12/2021
ms.locfileid: "100334593"
---
# <a name="bulk-operations-for-co-sell-opportunities-using-comma-separated-valuecsv-files"></a>Operações a granel para co-venda de oportunidades utilizando ficheiros de valor separados por vírgula (CSV)

**Funções adequadas**

- Administração de referências
- Utilizador de referências

As operações a granel no Partner Center ajudarão a sua empresa a exportar e importar dados de oportunidades de co-venda. Navegue para a página de oportunidades de co-venda para encontrar as ligações de importação e exportação no topo direito do banner do título da página. Os utilizadores com ambas as **permissões de administração** e **referências As** permissões do utilizador podem utilizar esta funcionalidade.

> [!IMPORTANT]
> As ações de criação/atualização efetuadas através da importação a granel não são reversíveis. Tenha cuidado quando estiver a modificar ou a criar um grande número de registos. Apenas um subconjunto de campos pode ser modificado após a criação de um acordo. **Nenhuma ação será permitida uma vez que qualquer negócio atinja um estado terminal como Declined/Expirado/Won/Lost.**

## <a name="exporting-co-sell-opportunities"></a>Oportunidades de co-venda exportadoras

Abaixo estão os detalhes da funcionalidade de exportação

- Pode exportar um **máximo de 5000 registos** clicando no botão de exportação.
- As ofertas que são descarregadas serão baseadas nos seus níveis de acesso. Os administradores de encaminhamento e os utilizadores de encaminhamento podem obter resultados diferentes com base no seu âmbito e inclusão como membros da equipa nas ofertas. Saiba mais sobre [permissões de referências.](permissions-overview.md#manage-referrals)
- A função de exportação tem em conta o separador atual na página de oportunidades de co-venda e os filtros que foram aplicados.
- Será gerado um ficheiro CSV com todos os dados baseados nos filtros aplicados.
- Pode levar até um minuto para fazer o download dos registos.
- Não tens de esperar que a ação de descarregamento esteja concluída. Mesmo que navegue para outras páginas no Partner Center, o ficheiro será descarregado assim que a função de exportação estiver concluída.
- Pode reutilizar o ficheiro descarregado para modificar os detalhes do negócio e fazer upload para atualizar quaisquer registos.

## <a name="importing-co-sell-opportunities"></a>Importando oportunidades de co-venda

- Pode criar ou atualizar um **máximo de 1000 registos** utilizando a funcionalidade de importação.
- Pode construir o modelo de raiz descarregando o modelo a partir da página Import no Partner Center.
- Também pode utilizar a funcionalidade Exportação para descarregar os registos existentes e atualizá-los.
- Se o ficheiro tiver mais de 1000 registos, não pode ser processado.
- Após o processo do ficheiro, será apresentado um resumo com o número de referências criadas, atualizadas e não processadas no último cartão de ficheiro de processo.
- Pode descarregar os detalhes dos registos processados, corrigir quaisquer erros e carregar o mesmo ficheiro para criar ou atualizar os registos que falharam na execução anterior. **Remova todos os registos bem sucedidos do ficheiro antes de carregar os registos corrigidos que falharam na execução anterior.**
- Para adicionar mais soluções, adicione colunas extras ao lado da solução 1 e use o nome da coluna como Solução X, onde X representa o número da solução no negócio. Por exemplo, Solução 2, Solução 3.
- Pode adicionar até 50 soluções para um acordo.
- Para adicionar mais membros da equipa, adicione colunas extras ao lado do membro da Equipa 1 e use o nome da coluna como membro da equipa X, onde X representa o número do membro da equipa no negócio. Por exemplo, membro da equipa 2, membro da equipa 3.
- Pode somar 50 membros da equipa para um acordo.

> [!NOTE]
> Não tens de esperar que o processamento esteja concluído. Os detalhes do último ficheiro processado estarão disponíveis para download assim que o processamento estiver concluído. **Pode levar até 10 minutos se estiver a enviar ficheiros com 1000 registos.**

> [!IMPORTANT]
> Leia atentamente todas as instruções e verifique o formato de cada coluna a partir da tabela abaixo antes de criar ou atualizar ofertas utilizando ficheiros CSV no Partner Center.

|**Nome da coluna**|**É obrigatório?**|**Descrição**|**Valor da amostra**|
|-----|:-----|:---------|:---|
Erros|No|Erros relacionados com as operações de criação/atualização w.r.t às referências serão incluídos nesta coluna. Se houver vários erros, todos serão listados separados por um ponto e vírgula.|Solução de campo obrigatória 1 em falta|
ID de noivado|No|O ID de noivado é gerado pelo sistema de referências do centro parceiro da Microsoft. Não é necessário para a nova criação de referência. Pode utilizar a identificação de noivado existente se estiver a atualizar um registo.|f7eaae47-0b84-4ac4-b4ea-5b2587d42cee
ID de referência|No|O ID de referência é gerado pelo sistema de referências do centro de parceiros da Microsoft. Não é necessário para a nova criação de referência. Preencha-o com o ID de encaminhamento se estiver a atualizar um registo existente.|ebacdkdc-0b84-4ac4-b4ea-5b2587d42cee
Nome do negócio|Yes|O nome amigável para o negócio para a sua referência.|Acordo de primavera do Reino Unido
Nome do Cliente|Yes|Nome da empresa de clientes. Utilize o nome legal da organização para uma rápida correspondência do lado da Microsoft.|Corporação Contoso
Linha de Endereço do Cliente 1|Yes|Linha de endereço 1 da empresa cliente. |Um Caminho contoso
Linha de Endereço do Cliente 2|No|Linha de endereço 2 da empresa cliente.|Rua NE 148
Cidade do Cliente|Yes|Cidade onde está localizada a organização do cliente.|Redmond
Estado do Cliente|No|Estado onde está localizada a organização do cliente.|Viseu
Código Postal do Cliente|No|Código Postal da região onde se encontra a organização do cliente.|98052
País do Cliente|Yes|País/Região onde está localizada a organização de clientes. Utilize os códigos de três letras do país, tal como mencionado [aqui.]( https://en.wikipedia.org/wiki/List_of_ISO_3166_country_codes)|E.U.A.
ID do cliente D-U-N-S|No|Tente obter a identificação duns da organização do cliente. Isto ajudará a combinar mais rapidamente a organização do cliente do lado da Microsoft, o que ajuda a uma atribuição mais rápida do vendedor. Você pode obter DUNS ID gratuitamente a partir deste [site.](https://www.dnb.com/duns-number/lookup.html)|81466849
Contato com o cliente Primeiro Nome|Depende|O primeiro nome só é obrigatório se precisar da ajuda da Microsoft. O primeiro nome do contacto principal da organização de clientes que trabalha neste negócio.|John
Contato com o cliente Nome do Último Nome|Depende|O apelido só é obrigatório se precisar da ajuda da Microsoft. Último nome do contacto primário da organização de clientes que trabalha neste negócio.|Cliente
Número de telefone de contato com o cliente|Depende|O número de telefone só é obrigatório se precisar de ajuda da Microsoft. Número de telefone do contacto principal da organização de clientes que trabalha neste negócio.|9999999999
Endereço de e-mail de contato do cliente|Depende|O endereço de e-mail só é obrigatório se precisar de ajuda da Microsoft. Endereço de e-mail do contacto principal da organização de clientes que trabalha neste negócio.|john.customer@contoso.com
Estado de encaminhamento de parceiros|Yes|Indica o estado do negócio do ponto de vista da sua empresa. Necessário se estiver a tentar criar ou modificar uma referência. Usa **o New** se estiveres a tentar criar um novo acordo. Os valores aceites são documentados [aqui.](https://docs.microsoft.com/partner/develop/referral-resources#referralstatus)|Ativo
Substatus de referência de parceiros|Yes|Indica o estado exato do negócio. Use **Aceito** se estiver a tentar criar um novo acordo. Também é necessário se estiver a modificar uma referência existente. Os valores aceites são documentados [aqui.](https://docs.microsoft.com/partner/develop/referral-resources#referralsubstatus)|Aceite
Estado de referência da Microsoft|Depende|Indica o estado do pedido de co-venda que enviou à Microsoft à procura de ajuda. Este é um campo só de leitura. Qualquer alteração feita a este campo enquanto importa os dados será ignorada.| Pendente
Razão recusada/perdida|Depende| Só é obrigado a fornecer estas informações se estiver a alterar o sub estado do seu campo para Declinado ou Perdido. Pode ignorar esta coluna de outra forma. <br/> **Introduza um número com base nas opções abaixo** <br/><br/> **1**- O orçamento do projeto não é adequado  <br/> **2**- O cliente não respondeu  <br/> **3**- O cliente escolheu outro fornecedor  <br/> **4** - Requisito do cliente não cumprido  <br/> **5** - Não um cliente <br/> **6**- A linha do tempo proposta era demasiado curta <br/> **7** - Reportar como abuso, spam ou phishing <br/> **8** - Outros |6|
Fase de Vendas|No|Este é o campo para indicar a fase de venda detalhada da referência. Leia mais sobre as fases de vendas [aqui](https://aka.ms/salesStages)|40
Valor estimado da oferta|Yes|"O valor do negócio com base nas conversas iniciais com o cliente. Isto pode ser alterado até que o negócio chegue a um dos estados terminais| ganhou ou perdeu.|12563
Moeda|Yes|A moeda em que o valor do negócio é inscrito. Pode encontrar os códigos de moeda [aqui.](https://en.wikipedia.org/wiki/ISO_4217)|USD
Data de fecho estimada|Yes|A data de fecho estimada do negócio com base nas conversas iniciais com o cliente no formato MM/DD/YYYYY. <br/> **A data deve estar no intervalo da UTC. Todas as datas exibidas na UI partner center são baseadas em azonos temporizados localizados. Pode haver uma diferença de +/- um dia na UI do Partner Center se estiver a analisar a referência para a qual forneceu a data no timezone UTC.**|1/30/2020
CRM ID|No|Identificador desta referência específica no seu sistema crm, se houver. Este é um campo de entrada de texto gratuito.|34234324-sdfsdf-345345-sfd
ID de campanha de marketing|No|Este campo indica a campanha de marketing, que resultou nesta referência específica. Tipicamente usado para o cálculo roi|BingSummer2020
Notas|No|Notas detalhadas que indicam as atualizações relacionadas com a referenciação|Esta é uma nota de amostra
Ajuda da Microsoft necessária?|Yes|Isto é para indicar se você quer que a Microsoft o ajude a fazer este pedido de co-venda|Yes
Que ajuda específica da Microsoft?|Depende|Uma das seis maneiras diferentes que a Microsoft pode ajudá-lo. Isto só é aplicável se escolher Não para a pergunta "A ajuda da Microsoft necessária? " <br/> **Introduza um número com base nas opções abaixo** <br/><br/> **1**- Carga de trabalho - proposta de valor específico  <br/> **2**- Arquitetura técnica do cliente  <br/> **3**- Prova de conceito /Demonstração  <br/> **4**- Orçamentos e Licenciamento  <br/> **5**- Pós - sucesso do cliente de vendas  <br/> **6**- Geral ou outro|1|
Partilhe com a equipa de vendas da Microsoft|Yes|Isto indica se quer partilhar ou não os detalhes do negócio com a equipa de vendas da Microsoft. Isto só é aplicável se escolher Não para a pergunta "A ajuda da Microsoft necessária? "|Yes
Notas para a Microsoft|No|Quaisquer notas específicas para a Microsoft se precisar de ajuda da Microsoft|Precisa de ajuda com um POC para cliente Contoso
Consentimento para partilhar contacto Cliente/Parceiro|Yes|Consentimento para partilhar os dados de contacto do cliente e os dados de contato dos seus colaboradores da empresa que estão a trabalhar no negócio. **As ofertas não serão criadas ou atualizadas se escolher o Nº para esta coluna.** |Yes
Solução 1|Yes|ID de solução (Obrigatório), A moeda (Opcional) na qual o valor da oferta é introduzido. Pode encontrar os códigos de moeda [aqui,](https://en.wikipedia.org/wiki/ISO_4217)Preço do SKU (Opcional) e Quantidade do SKU (Opcional)  |SOL-1234-PQRS, USD, 10,100
Membro da equipa 1|Yes|Primeiro nome, apelido, número de telemóvel e identificação de e-mail do respetivo membro da equipa.| Bob, Partner, 999999, Bob.partner@Contoso.com
