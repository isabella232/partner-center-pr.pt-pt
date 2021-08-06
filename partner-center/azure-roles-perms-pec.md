---
title: Funções, permissões para parceiro ganhou crédito
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Conheça as funções e permissões para que os parceiros possam ganhar créditos (PEC) de parceiros. Estes diferem de funções para trabalhar no Partner Center.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 373346311924059c9d3a6c54019fe1d3a03a1db71f7602769cfaf6712c345707
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/06/2021
ms.locfileid: "115680656"
---
# <a name="roles-and-permissions-required-to-earn-partner-earned-credit"></a>Funções e permissões necessárias para ganhar o crédito do parceiro

As seguintes funções mapeiam para níveis de permissões que determinam se um parceiro é elegível para parceiro ganhou créditos.

>[!Important]
>Estas funções e permissões não são as mesmas que as funções e permissões que um utilizador precisa para trabalhar no Partner Center.

|**Role**   |**Descrição**   |**PEC elegível**   |
|-----------------|:------------------|:--------------|
|Proprietário  |Gere tudo, incluindo o acesso aos recursos.|Yes|
|Contribuinte |Gere tudo, exceto conceder acesso aos recursos.|Yes|
|Leitor|Pode ver tudo, mas não fazer alterações|No|
|ACRDelete|acr eliminar|Yes|
|ACRImageSigner|acr sinaleiro de imagem|Yes|
|ACRPull|acr puxar|Yes|
|AcrPush|impulso acr|Yes|
|AcrQuarantineReader|leitor de dados de quarentena acr|No|
|Escritor de AcrQuarantineWriter| acr escritor de dados de quarentena|Yes|
|Colaborador do Serviço de Gestão da API|Pode gerir o serviço e as APIs|Yes|
|Função do operador de serviço de gestão da API|Pode gerir o serviço, mas não as APIs|Yes|
|Função de leitor de serviço de gestão da API|Acesso apenas de leitura ao serviço e APIs|No|
|Contribuinte Informações Componente de Aplicação|Gere componentes de Informações de aplicação|Yes|
|Aplicação Informações Snapshot Debugger|Dá permissão ao utilizador para visualizar e descarregar instantâneos de depurg recolhidos com a Aplicação Informações Snapshot Debugger. Note que estas permissões não estão incluídas nas funções Proprietário ou Contribuinte.|Yes|
Operador de emprego de automação | Criar e Gerir Empregos utilizando livros de automação. | Yes | 
Operador de Automatização | Operadores de automação podem iniciar, parar, suspender e retomar postos de trabalho | Yes | 
Operador de runbook de automação | Leia as propriedades do Runbook - para ser capaz de criar Jobs of the runbook. | Yes | 
Contribuidor Avere | Pode criar e gerir um cluster Avere vFXT. | Yes | 
Operador avere | Usado pelo cluster Avere vFXT para gerir o cluster | Yes | 
Proprietário de dados Azure Event Hubs | Permite o acesso total aos recursos do Azure Event Hubs. | Yes | 
Recetor de dados Azure Event Hubs | Permite ter acesso aos recursos do Azure Event Hubs. | Yes | 
Ender de dados do Azure Event Hubs | Permite enviar acesso aos recursos do Azure Event Hubs. | Yes | 
Azure Kubernetes Service Cluster Função de Administrador | Lista de ação de credencial de administrador de agrupamento. | Yes | 
Papel de utilizador do cluster de serviço Azure Kubernetes | Listar ação credencial do utilizador do cluster. | Yes | 
Azure Mapas Data Reader (Pré-visualização) | Concede acesso a ler dados relacionados com mapas a partir de uma conta de mapas Azure. | No | 
Proprietário de dados Azure Service Bus | Permite o acesso total aos recursos Service Bus Azure. | Yes | 
Recetor de dados Azure Service Bus | Permite o acesso aos recursos Service Bus Azure. | Yes | 
Remetente de dados Azure Service Bus | Permite o acesso ao Azure Service Bus recursos. | Yes | 
Proprietário de registo de pilha de Azure | Permite-lhe gerir as inscrições do Azure Stack. | Yes | 
Colaborador de backup | Permite-lhe gerir o serviço de backup, mas não pode criar cofres e dar acesso a outros | Yes | 
Operador de Cópia de Segurança | Permite-lhe gerir serviços de backup, exceto remoção de backup, criação de cofre e dar acesso a outros | Yes | 
Leitor de reserva | Pode ver serviços de backup, mas não pode fazer alterações | No | 
Leitor de Faturação | Permite ler acesso a dados de faturação | No | 
Colaborador bizTalk | Permite-lhe gerir os serviços BizTalk, mas não ter acesso aos mesmos. | Yes | 
Acesso ao nó do membro blockchain (visualização) | Permite o acesso aos nóns do Membro Blockchain | Yes | 
Contribuidor de Projeto | Pode gerir definições de planta, mas não atribuí-las. | Yes | 
Operador de blueprint | Pode atribuir plantas publicadas existentes, mas não pode criar novas plantas. NOTA: isto só funciona se a atribuição for feita com uma identidade gerida atribuída pelo utilizador. | Yes | 
CDN Contribuinte de ponto final | Pode gerir CDN pontos finais, mas não pode dar acesso a outros utilizadores. | Yes | 
CDN Leitor de Ponto Final | Pode ver CDN pontos finais, mas não pode fazer alterações. | No | 
CDN Colaborador de Perfil | Pode gerir CDN perfis e seus pontos finais, mas não pode dar acesso a outros utilizadores. | Yes | 
CDN Leitor de Perfil | Pode ver CDN perfis e seus pontos finais, mas não pode fazer alterações. | No | 
Contribuidor de Rede Clássica | Permite-lhe gerir redes clássicas, mas não acesso a elas. | Yes | 
Colaborador clássico da conta de Armazenamento | Permite-lhe gerir contas de armazenamento clássicas, mas não acesso a elas. | Yes | 
Função clássica do serviço do operador chave da conta de Armazenamento | Os operadores clássicos de Armazenamento conta são autorizados a listar e regenerar chaves em Contas de Armazenamento Clássicas | Yes | 
Colaborador clássico da máquina virtual | Permite-lhe gerir máquinas virtuais clássicas, mas não acesso a elas, e não à rede virtual ou à conta de armazenamento a que estão ligadas. | Yes | 
Colaborador dos Serviços Cognitivos | Permite criar, ler, atualizar, eliminar e gerir chaves dos Serviços Cognitivos. | Yes | 
Leitor de dados de serviços cognitivos (pré-visualização) | Permite-lhe ler os dados dos Serviços Cognitivos. | No | 
Utilizador de Serviços Cognitivos | Permite-lhe ler e listar as chaves dos Serviços Cognitivos. | No | 
Papel do leitor de conta de cosm de Cosmos DB | Pode ler os dados da conta DB da Azure Cosmos. Consulte o Contribuinte de Conta DocumentDB para gerir as contas DB da Azure Cosmos. | No | 
Operador de DB cosmos | Permite-lhe gerir as contas DB da Azure Cosmos, mas não aceder aos dados nelas. Impede o acesso às chaves da conta e às cordas de ligação. | Yes | 
CosmosBackupOperator | Pode submeter pedido de restauro para uma base de dados Cosmos DB ou um recipiente para uma conta | Yes | 
Contribuidor do Cost Management | Pode ver os custos e gerir a configuração dos custos (por exemplo, orçamentos, exportações) | Yes | 
Leitor de Gestão de Custos | Pode ver dados de custos e configuração (por exemplo, orçamentos, exportações) | No | 
Contribuinte da Caixa de Dados | Permite-lhe gerir tudo no âmbito do Serviço de Caixa de Dados, exceto dar acesso a outros. | Yes | 
Leitor de caixa de dados | Permite-lhe gerir o Serviço de Caixa de Dados, exceto criar detalhes de encomenda ou edição e dar acesso a outros. | No | 
Contribuinte da Fábrica de Dados | Criar e gerir fábricas de dados, bem como recursos infantis dentro delas. | Yes | 
Desenvolvedor de Análise de Lago de Dados | Permite submeter, monitorizar e gerir os seus próprios trabalhos, mas não criar ou apagar contas data lake analytics. | Yes | 
Purgador de dados | Pode purgar dados de análise | Yes | 
Utilizador de Laboratórios DevTest | Permite ligar, iniciar, reiniciar e desligar as máquinas virtuais no Azure DevTest Labs. | Yes | 
Colaborador da Zona DNS | Permite gerir zonas DNS e recordes em Azure DNS, mas não permite controlar quem tem acesso a elas. | Yes | 
Colaborador de Conta DocumentDB | Pode gerir as contas de DB da Azure Cosmos. Azure Cosmos DB é anteriormente conhecido como DocumentDB. | Yes | 
Colaborador de EventosGrid EventSubscription | Permite-lhe gerir as operações de subscrição de eventos EventGrid. | Yes | 
Leitor de subscrição de eventos Com EventosGrid | Permite-lhe ler subscrições de eventosGrid. | No | 
Operador de cluster HDInsight | Permite-lhe ler e modificar configurações de cluster HDInsight. | Yes | 
HdInsight Domain Services Colaborador | Pode ler, criar, modificar e eliminar as operações relacionadas com os serviços de domínio necessárias para o pacote de segurança da empresa HDInsight | Yes | 
Contribuinte de Conta de Sistemas Inteligentes | Permite-lhe gerir contas de Sistemas Inteligentes, mas não acesso a elas. | Yes | 
Contribuidor do Cofre Chave | Permite-lhe gerir cofres chave, mas não acesso a eles. | Yes | 
Criador de Laboratório | Permite criar, gerir, eliminar os seus laboratórios geridos sob as suas contas do Azure Lab. | Yes | 
Contribuidor do Log Analytics | Log Analytics Contributor pode ler todos os dados de monitorização e editar as definições de monitorização. As definições de monitorização de edição incluem a adição da extensão VM aos VM; leitura das chaves da conta de armazenamento para poder configurar a recolha de registos da Azure Armazenamento; criar e configurar contas de automação; adição de soluções; e configurar diagnósticos Azure em todos os recursos da Azure. | Yes | 
Leitor do Log Analytics | O Log Analytics Reader pode visualizar e pesquisar todos os dados de monitorização, bem como visualizar as definições de monitorização, incluindo visualizar a configuração dos diagnósticos Azure em todos os recursos do Azure. | No | 
Contribuidor de Aplicativos Lógicos | Permite-lhe gerir aplicações lógicas, mas não alterar o acesso às suas. | Yes | 
Operador de aplicativos lógica | Permite-lhe ler, ativar e desativar aplicações lógicas, mas não editá-las ou atualizá-las. | Yes | 
Papel do operador de aplicação gerido | Permite-lhe ler e executar ações sobre recursos de aplicação gerida | Yes | 
Leitor de Aplicações Geridas | Permite-lhe ler recursos numa aplicação gerida e solicitar acesso ao JIT. | No | 
Colaborador de Identidade Gerido | Criar, Ler, Atualizar e Eliminar Identidade Atribuída ao Utilizador | Yes | 
Operador de identidade gerido | Ler e atribuir identidade atribuída ao utilizador | Yes | 
Colaborador do Grupo de Gestão | Função contributiva do Grupo de Gestão | Yes | 
Leitor de Grupo de Gestão | Função de leitor de grupo de gestão | No | 
Colaborador de monitorização | Pode ler todos os dados de monitorização e editar as definições de monitorização. Ver também Começar com papéis, permissões e segurança com o Azure Monitor. | Yes | 
Métricas de Monitorização Publisher | Permite publicar métricas contra recursos Azure | Yes | 
Leitor de Monitorização | Pode ler todos os dados de monitorização (métricas, registos, etc.). Ver também Começar com papéis, permissões e segurança com o Azure Monitor. | No | 
Contribuidor de Rede | Permite-lhe gerir as redes, mas não ter acesso a elas. | Yes | 
Novo contribuinte da conta APM da relíquia | Permite-lhe gerir as contas e aplicações de Gestão de Desempenho de Aplicações Novas Relíquias, mas não o acesso às contas. | Yes | 
Leitor e Acesso a Dados | Permite-lhe ver tudo, mas não permitirá que elimine ou crie uma conta de armazenamento ou recurso contido. Também permitirá o acesso de leitura/escrita a todos os dados contidos numa conta de armazenamento através do acesso às chaves da conta de armazenamento. | Yes | 
Contribuidor redis cache | Permite-te gerir caches Redis, mas não acesso a eles. | Yes | 
Contribuidor de Política de Recursos (Pré-visualização) | (Pré-visualização) Os utilizadores reenchitados da EA, com direitos de criar/modificar a política de recursos, criar bilhete de apoio e ler recursos/hierarquia. | Yes | 
Colaborador de Coleções de Trabalho do Programador | Permite-lhe gerir as coleções de emprego do Scheduler, mas não ter acesso a elas. | Yes | 
Colaborador do Serviço de Pesquisa | Permite-lhe gerir os serviços de Pesquisa, mas não o acesso aos mesmos. | Yes | 
Administrador de Segurança | Apenas no Centro de Segurança: Pode ver políticas de segurança, ver estados de segurança, editar políticas de segurança, ver alertas e recomendações, rejeitar alertas e recomendações | Yes | 
Gestor de Segurança (Legado) | Este é um papel antigo. Por favor, use o administrador de segurança em vez | Yes | 
Leitor de Segurança | Apenas no Centro de Segurança: Pode ver recomendações e alertas, ver políticas de segurança, ver estados de segurança, mas não pode fazer alterações | No | 
Contribuidor do Site Recovery | Permite-lhe gerir o serviço de Recuperação de Sítios, exceto a criação de abóbada e atribuição de funções | Yes | 
Operador do Site Recovery | Permite-lhe falhar e falhar, mas não realizar outras operações de gestão de Recuperação de Sítios | Yes | 
Leitor do Site Recovery | Permite-lhe ver o estado de Recuperação do Site, mas não realizar outras operações de gestão | No | 
Contribuinte da Conta De Âncoras Espaciais | Permite-lhe gerir âncoras espaciais na sua conta, mas não apagá-las | Yes | 
Proprietário de conta de âncoras espaciais | Permite-lhe gerir âncoras espaciais na sua conta, incluindo apagá-las | Yes | 
Leitor de conta de âncoras espaciais | Permite localizar e ler propriedades de âncoras espaciais na sua conta | No | 
SQL Contribuinte DB | Permite-lhe gerir SQL bases de dados, mas não acesso a elas. Além disso, não é possível gerir as suas políticas relacionadas com a segurança ou os seus pais SQL servidores. | Yes | 
SQL Colaborador de instância gerida | Permite-lhe gerir SQL Casos Geridos e configuração de rede necessária, mas não pode dar acesso a outros. | Yes | 
Gestor de Segurança SQL | Permite-lhe gerir as políticas relacionadas com a segurança de SQL servidores e bases de dados, mas não o acesso aos mesmos. | Yes | 
SQL Server Contribuinte | Permite-lhe gerir SQL servidores e bases de dados, mas não acesso aos mesmos, e não às suas políticas relacionadas com a segurança. | Yes | 
Contribuidor de Conta de Armazenamento | Permite a gestão das contas de armazenamento. Fornece acesso à chave da conta, que pode ser usada para aceder a dados através da autorização da Chave Partilhada. | Yes | 
Armazenamento Função de serviço do operador chave de conta | Permite a listagem e regeneração das chaves de acesso à conta de armazenamento. | Yes | 
Contribuinte de Dados do Armazenamento de Blobs | Leia, escreva e elimine o Azure Armazenamento recipientes e bolhas. Para saber quais as ações necessárias para uma determinada operação de dados, consulte permissões para chamadas de operações de dados de blob e fila. | Yes | 
Proprietário dos Dados do Armazenamento de Blobs | Fornece acesso total a Azure Armazenamento recipientes e dados blob, incluindo a atribuição do controlo de acesso POSIX. Para saber quais as ações necessárias para uma determinada operação de dados, consulte permissões para chamadas de operações de dados de blob e fila. | Yes | 
Leitor de Dados do Armazenamento de Blobs | Leia e enuncie Azure Armazenamento recipientes e bolhas. Para saber quais as ações necessárias para uma determinada operação de dados, consulte permissões para chamadas de operações de dados de blob e fila. | No | 
Armazenamento Delegado blob | Obtenha uma chave de delegação de utilizador, que pode ser usada para criar uma assinatura de acesso partilhado para um recipiente ou bolha que é assinado com credenciais AZure AD. Para mais informações, consulte Criar uma delegação de utilizador SAS. | Yes | 
Contribuinte de Partilhas SMB de Dados de Ficheiros de Armazenamento | Permite ler, escrever e apagar o acesso no Azure Armazenamento ações de ficheiros sobre a SMB | Yes | 
Contribuinte Elevado de Partilhas SMB de Dados de Ficheiros de Armazenamento | Permite ler, escrever, eliminar e modificar o acesso à permissão NTFS no Azure Armazenamento ações de ficheiros sobre a SMB | Yes | 
Leitor de Partilhas SMB de Dados de Ficheiros de Armazenamento | Permite a leitura do acesso ao Azure File Share over SMB | No | 
Armazenamento Contribuinte de Dados de Fila | Leia, escreva e elimine o Azure Armazenamento filas e mensagens de fila. Para saber quais as ações necessárias para uma determinada operação de dados, consulte permissões para chamadas de operações de dados de blob e fila. | Yes | 
Armazenamento Processador de mensagens de dados de fila | Espreite, recupere e elimine uma mensagem de uma fila de Armazenamento Azure. Para saber quais as ações necessárias para uma determinada operação de dados, consulte permissões para chamadas de operações de dados de blob e fila. | Yes | 
Armazenamento Remetente de mensagem de dados de fila | Adicione mensagens a uma fila de Armazenamento Azure. Para saber quais as ações necessárias para uma determinada operação de dados, consulte permissões para chamadas de operações de dados de blob e fila. | Yes | 
Armazenamento Leitor de dados de fila | Leia e enuse Armazenamento filas e mensagens de fila do Azure. Para saber quais as ações necessárias para uma determinada operação de dados, consulte permissões para chamadas de operações de dados de blob e fila. | No | 
Colaborador de Pedido de Apoio | Permite criar e gerir pedidos de Suporte | Yes | 
Gestor de Tráfego Contribuinte | Permite-lhe gerir Gestor de Tráfego perfis, mas não permite que controle quem tem acesso a eles. | Yes | 
Administrador de Acesso dos Utilizadores | Permite-lhe gerir o acesso do utilizador aos recursos Azure. | Yes | 
Login de administrador de máquina virtual | Ver Máquinas Virtuais no portal e iniciar sessão como administrador | Yes | 
Contribuidor de Máquina Virtual | Permite-lhe gerir máquinas virtuais, mas não acesso a elas, e não à rede virtual ou à conta de armazenamento a que estão ligadas. | Yes | 
Início de sessão do utilizador de máquina virtual | Ver Máquinas Virtuais no portal e iniciar sessão como um utilizador regular. | Yes | 
Colaborador do Plano Web | Permite-lhe gerir os planos web para sites, mas não acesso aos mesmos. | Yes | 
Colaborador do Site | Permite-lhe gerir websites (não planos web), mas não acesso a eles | Sim |

## <a name="next-steps"></a>Próximos passos

- [Partner earned credit - uma visão geral de como funciona na nova experiência de comércio na CSP](partner-earned-credit.md)
