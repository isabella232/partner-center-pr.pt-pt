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
ms.openlocfilehash: ca9cd1b09c840531c3652f71afbd9c66f657f877
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/29/2021
ms.locfileid: "114840387"
---
# <a name="roles-and-permissions-required-to-earn-partner-earned-credit"></a>Funções e permissões necessárias para ganhar o crédito do parceiro

As seguintes funções mapeiam para níveis de permissões que determinam se um parceiro é elegível para parceiro ganhou créditos.

>[!Important]
>Estas funções e permissões não são as mesmas que as funções e permissões que um utilizador precisa para trabalhar no Partner Center.

|**Role**   |**Descrição**   |**PEC elegível**   |
|-----------------|:------------------|:--------------|
|Proprietário  |Gere tudo, incluindo o acesso aos recursos.|Sim|
|Contribuinte |Gere tudo, exceto conceder acesso aos recursos.|Sim|
|Leitor|Pode ver tudo, mas não fazer alterações|Não|
|ACRDelete|acr eliminar|Sim|
|ACRImageSigner|acr sinaleiro de imagem|Sim|
|ACRPull|acr puxar|Sim|
|AcrPush|impulso acr|Sim|
|AcrQuarantineReader|leitor de dados de quarentena acr|Não|
|Escritor de AcrQuarantineWriter| acr escritor de dados de quarentena|Sim|
|Colaborador do Serviço de Gestão da API|Pode gerir o serviço e as APIs|Sim|
|Função do operador de serviço de gestão da API|Pode gerir o serviço, mas não as APIs|Sim|
|Função de leitor de serviço de gestão da API|Acesso apenas de leitura ao serviço e APIs|Não|
|Contribuinte Informações Componente de Aplicação|Gere componentes de Informações de aplicação|Sim|
|Aplicação Informações Snapshot Debugger|Dá permissão ao utilizador para visualizar e descarregar instantâneos de depurg recolhidos com a Aplicação Informações Snapshot Debugger. Note que estas permissões não estão incluídas nas funções Proprietário ou Contribuinte.|Sim|
Operador de emprego de automação | Criar e Gerir Empregos utilizando livros de automação. | Sim | 
Operador de Automatização | Operadores de automação podem iniciar, parar, suspender e retomar postos de trabalho | Sim | 
Operador de runbook de automação | Leia as propriedades do Runbook - para ser capaz de criar Jobs of the runbook. | Sim | 
Contribuidor Avere | Pode criar e gerir um cluster Avere vFXT. | Sim | 
Operador avere | Usado pelo cluster Avere vFXT para gerir o cluster | Sim | 
Proprietário de dados Azure Event Hubs | Permite o acesso total aos recursos do Azure Event Hubs. | Sim | 
Recetor de dados Azure Event Hubs | Permite ter acesso aos recursos do Azure Event Hubs. | Sim | 
Ender de dados do Azure Event Hubs | Permite enviar acesso aos recursos do Azure Event Hubs. | Sim | 
Azure Kubernetes Service Cluster Função de Administrador | Lista de ação de credencial de administrador de agrupamento. | Sim | 
Papel de utilizador do cluster de serviço Azure Kubernetes | Listar ação credencial do utilizador do cluster. | Sim | 
Azure Mapas Data Reader (Pré-visualização) | Concede acesso a ler dados relacionados com mapas a partir de uma conta de mapas Azure. | Não | 
Proprietário de dados Azure Service Bus | Permite o acesso total aos recursos Service Bus Azure. | Sim | 
Recetor de dados Azure Service Bus | Permite o acesso aos recursos Service Bus Azure. | Sim | 
Remetente de dados Azure Service Bus | Permite o acesso ao Azure Service Bus recursos. | Sim | 
Proprietário de registo de pilha de Azure | Permite-lhe gerir as inscrições do Azure Stack. | Sim | 
Colaborador de backup | Permite-lhe gerir o serviço de backup, mas não pode criar cofres e dar acesso a outros | Sim | 
Operador de Cópia de Segurança | Permite-lhe gerir serviços de backup, exceto remoção de backup, criação de cofre e dar acesso a outros | Sim | 
Leitor de reserva | Pode ver serviços de backup, mas não pode fazer alterações | Não | 
Leitor de Faturação | Permite ler acesso a dados de faturação | Não | 
Colaborador bizTalk | Permite-lhe gerir os serviços BizTalk, mas não ter acesso aos mesmos. | Sim | 
Acesso ao nó do membro blockchain (visualização) | Permite o acesso aos nóns do Membro Blockchain | Sim | 
Contribuidor de Projeto | Pode gerir definições de planta, mas não atribuí-las. | Sim | 
Operador de blueprint | Pode atribuir plantas publicadas existentes, mas não pode criar novas plantas. NOTA: isto só funciona se a atribuição for feita com uma identidade gerida atribuída pelo utilizador. | Sim | 
CDN Contribuinte de ponto final | Pode gerir CDN pontos finais, mas não pode dar acesso a outros utilizadores. | Sim | 
CDN Leitor de Ponto Final | Pode ver CDN pontos finais, mas não pode fazer alterações. | Não | 
CDN Colaborador de Perfil | Pode gerir CDN perfis e seus pontos finais, mas não pode dar acesso a outros utilizadores. | Sim | 
CDN Leitor de Perfil | Pode ver CDN perfis e seus pontos finais, mas não pode fazer alterações. | Não | 
Contribuidor de Rede Clássica | Permite-lhe gerir redes clássicas, mas não acesso a elas. | Sim | 
Colaborador clássico da conta de Armazenamento | Permite-lhe gerir contas de armazenamento clássicas, mas não acesso a elas. | Sim | 
Função clássica do serviço do operador chave da conta de Armazenamento | Os operadores clássicos de Armazenamento conta são autorizados a listar e regenerar chaves em Contas de Armazenamento Clássicas | Sim | 
Colaborador clássico da máquina virtual | Permite-lhe gerir máquinas virtuais clássicas, mas não acesso a elas, e não à rede virtual ou à conta de armazenamento a que estão ligadas. | Sim | 
Colaborador dos Serviços Cognitivos | Permite criar, ler, atualizar, eliminar e gerir chaves dos Serviços Cognitivos. | Sim | 
Leitor de dados de serviços cognitivos (pré-visualização) | Permite-lhe ler os dados dos Serviços Cognitivos. | Não | 
Utilizador de Serviços Cognitivos | Permite-lhe ler e listar as chaves dos Serviços Cognitivos. | Não | 
Papel do leitor de conta de cosm de Cosmos DB | Pode ler os dados da conta DB da Azure Cosmos. Consulte o Contribuinte de Conta DocumentDB para gerir as contas DB da Azure Cosmos. | Não | 
Operador de DB cosmos | Permite-lhe gerir as contas DB da Azure Cosmos, mas não aceder aos dados nelas. Impede o acesso às chaves da conta e às cordas de ligação. | Sim | 
CosmosBackupOperator | Pode submeter pedido de restauro para uma base de dados Cosmos DB ou um recipiente para uma conta | Sim | 
Contribuidor do Cost Management | Pode ver os custos e gerir a configuração dos custos (por exemplo, orçamentos, exportações) | Sim | 
Leitor de Gestão de Custos | Pode ver dados de custos e configuração (por exemplo, orçamentos, exportações) | Não | 
Contribuinte da Caixa de Dados | Permite-lhe gerir tudo no âmbito do Serviço de Caixa de Dados, exceto dar acesso a outros. | Sim | 
Leitor de caixa de dados | Permite-lhe gerir o Serviço de Caixa de Dados, exceto criar detalhes de encomenda ou edição e dar acesso a outros. | Não | 
Contribuinte da Fábrica de Dados | Criar e gerir fábricas de dados, bem como recursos infantis dentro delas. | Sim | 
Desenvolvedor de Análise de Lago de Dados | Permite submeter, monitorizar e gerir os seus próprios trabalhos, mas não criar ou apagar contas data lake analytics. | Sim | 
Purgador de dados | Pode purgar dados de análise | Sim | 
Utilizador de Laboratórios DevTest | Permite ligar, iniciar, reiniciar e desligar as máquinas virtuais no Azure DevTest Labs. | Sim | 
Colaborador da Zona DNS | Permite gerir zonas DNS e recordes em Azure DNS, mas não permite controlar quem tem acesso a elas. | Sim | 
Colaborador de Conta DocumentDB | Pode gerir as contas de DB da Azure Cosmos. Azure Cosmos DB é anteriormente conhecido como DocumentDB. | Sim | 
Colaborador de EventosGrid EventSubscription | Permite-lhe gerir as operações de subscrição de eventos EventGrid. | Sim | 
Leitor de subscrição de eventos Com EventosGrid | Permite-lhe ler subscrições de eventosGrid. | Não | 
Operador de cluster HDInsight | Permite-lhe ler e modificar configurações de cluster HDInsight. | Sim | 
HdInsight Domain Services Colaborador | Pode ler, criar, modificar e eliminar as operações relacionadas com os serviços de domínio necessárias para o pacote de segurança da empresa HDInsight | Sim | 
Contribuinte de Conta de Sistemas Inteligentes | Permite-lhe gerir contas de Sistemas Inteligentes, mas não acesso a elas. | Sim | 
Contribuidor do Cofre Chave | Permite-lhe gerir cofres chave, mas não acesso a eles. | Sim | 
Criador de Laboratório | Permite criar, gerir, eliminar os seus laboratórios geridos sob as suas contas do Azure Lab. | Sim | 
Contribuidor do Log Analytics | Log Analytics Contributor pode ler todos os dados de monitorização e editar as definições de monitorização. As definições de monitorização de edição incluem a adição da extensão VM aos VM; leitura das chaves da conta de armazenamento para poder configurar a recolha de registos da Azure Armazenamento; criar e configurar contas de automação; adição de soluções; e configurar diagnósticos Azure em todos os recursos da Azure. | Sim | 
Leitor do Log Analytics | O Log Analytics Reader pode visualizar e pesquisar todos os dados de monitorização, bem como visualizar as definições de monitorização, incluindo visualizar a configuração dos diagnósticos Azure em todos os recursos do Azure. | Não | 
Contribuidor de Aplicativos Lógicos | Permite-lhe gerir aplicações lógicas, mas não alterar o acesso às suas. | Sim | 
Operador de aplicativos lógica | Permite-lhe ler, ativar e desativar aplicações lógicas, mas não editá-las ou atualizá-las. | Sim | 
Papel do operador de aplicação gerido | Permite-lhe ler e executar ações sobre recursos de aplicação gerida | Sim | 
Leitor de Aplicações Geridas | Permite-lhe ler recursos numa aplicação gerida e solicitar acesso ao JIT. | Não | 
Colaborador de Identidade Gerido | Criar, Ler, Atualizar e Eliminar Identidade Atribuída ao Utilizador | Sim | 
Operador de identidade gerido | Ler e atribuir identidade atribuída ao utilizador | Sim | 
Colaborador do Grupo de Gestão | Função contributiva do Grupo de Gestão | Sim | 
Leitor de Grupo de Gestão | Função de leitor de grupo de gestão | Não | 
Colaborador de monitorização | Pode ler todos os dados de monitorização e editar as definições de monitorização. Ver também Começar com papéis, permissões e segurança com o Azure Monitor. | Sim | 
Métricas de Monitorização Publisher | Permite publicar métricas contra recursos Azure | Sim | 
Leitor de Monitorização | Pode ler todos os dados de monitorização (métricas, registos, etc.). Ver também Começar com papéis, permissões e segurança com o Azure Monitor. | Não | 
Contribuidor de Rede | Permite-lhe gerir as redes, mas não ter acesso a elas. | Sim | 
Novo contribuinte da conta APM da relíquia | Permite-lhe gerir as contas e aplicações de Gestão de Desempenho de Aplicações Novas Relíquias, mas não o acesso às contas. | Sim | 
Leitor e Acesso a Dados | Permite-lhe ver tudo, mas não permitirá que elimine ou crie uma conta de armazenamento ou recurso contido. Também permitirá o acesso de leitura/escrita a todos os dados contidos numa conta de armazenamento através do acesso às chaves da conta de armazenamento. | Sim | 
Contribuidor redis cache | Permite-te gerir caches Redis, mas não acesso a eles. | Sim | 
Contribuidor de Política de Recursos (Pré-visualização) | (Pré-visualização) Os utilizadores reenchitados da EA, com direitos de criar/modificar a política de recursos, criar bilhete de apoio e ler recursos/hierarquia. | Sim | 
Colaborador de Coleções de Trabalho do Programador | Permite-lhe gerir as coleções de emprego do Scheduler, mas não ter acesso a elas. | Sim | 
Colaborador do Serviço de Pesquisa | Permite-lhe gerir os serviços de Pesquisa, mas não o acesso aos mesmos. | Sim | 
Administrador de Segurança | Apenas no Centro de Segurança: Pode ver políticas de segurança, ver estados de segurança, editar políticas de segurança, ver alertas e recomendações, rejeitar alertas e recomendações | Sim | 
Gestor de Segurança (Legado) | Este é um papel antigo. Por favor, use o administrador de segurança em vez | Sim | 
Leitor de Segurança | Apenas no Centro de Segurança: Pode ver recomendações e alertas, ver políticas de segurança, ver estados de segurança, mas não pode fazer alterações | Não | 
Contribuidor do Site Recovery | Permite-lhe gerir o serviço de Recuperação de Sítios, exceto a criação de abóbada e atribuição de funções | Sim | 
Operador do Site Recovery | Permite-lhe falhar e falhar, mas não realizar outras operações de gestão de Recuperação de Sítios | Sim | 
Leitor do Site Recovery | Permite-lhe ver o estado de Recuperação do Site, mas não realizar outras operações de gestão | Não | 
Contribuinte da Conta De Âncoras Espaciais | Permite-lhe gerir âncoras espaciais na sua conta, mas não apagá-las | Sim | 
Proprietário de conta de âncoras espaciais | Permite-lhe gerir âncoras espaciais na sua conta, incluindo apagá-las | Sim | 
Leitor de conta de âncoras espaciais | Permite localizar e ler propriedades de âncoras espaciais na sua conta | Não | 
SQL Contribuinte DB | Permite-lhe gerir SQL bases de dados, mas não acesso a elas. Além disso, não é possível gerir as suas políticas relacionadas com a segurança ou os seus pais SQL servidores. | Sim | 
SQL Colaborador de instância gerida | Permite-lhe gerir SQL Casos Geridos e configuração de rede necessária, mas não pode dar acesso a outros. | Sim | 
Gestor de Segurança SQL | Permite-lhe gerir as políticas relacionadas com a segurança de SQL servidores e bases de dados, mas não o acesso aos mesmos. | Sim | 
SQL Server Contribuinte | Permite-lhe gerir SQL servidores e bases de dados, mas não acesso aos mesmos, e não às suas políticas relacionadas com a segurança. | Sim | 
Contribuidor de Conta de Armazenamento | Permite a gestão das contas de armazenamento. Fornece acesso à chave da conta, que pode ser usada para aceder a dados através da autorização da Chave Partilhada. | Sim | 
Armazenamento Função de serviço do operador chave de conta | Permite a listagem e regeneração das chaves de acesso à conta de armazenamento. | Sim | 
Contribuinte de Dados do Armazenamento de Blobs | Leia, escreva e elimine o Azure Armazenamento recipientes e bolhas. Para saber quais as ações necessárias para uma determinada operação de dados, consulte permissões para chamadas de operações de dados de blob e fila. | Sim | 
Proprietário dos Dados do Armazenamento de Blobs | Fornece acesso total a Azure Armazenamento recipientes e dados blob, incluindo a atribuição do controlo de acesso POSIX. Para saber quais as ações necessárias para uma determinada operação de dados, consulte permissões para chamadas de operações de dados de blob e fila. | Sim | 
Leitor de Dados do Armazenamento de Blobs | Leia e enuncie Azure Armazenamento recipientes e bolhas. Para saber quais as ações necessárias para uma determinada operação de dados, consulte permissões para chamadas de operações de dados de blob e fila. | Não | 
Armazenamento Delegado blob | Obtenha uma chave de delegação de utilizador, que pode ser usada para criar uma assinatura de acesso partilhado para um recipiente ou bolha que é assinado com credenciais AZure AD. Para mais informações, consulte Criar uma delegação de utilizador SAS. | Sim | 
Contribuinte de Partilhas SMB de Dados de Ficheiros de Armazenamento | Permite ler, escrever e apagar o acesso no Azure Armazenamento ações de ficheiros sobre a SMB | Sim | 
Contribuinte Elevado de Partilhas SMB de Dados de Ficheiros de Armazenamento | Permite ler, escrever, eliminar e modificar o acesso à permissão NTFS no Azure Armazenamento ações de ficheiros sobre a SMB | Sim | 
Leitor de Partilhas SMB de Dados de Ficheiros de Armazenamento | Permite a leitura do acesso ao Azure File Share over SMB | Não | 
Armazenamento Contribuinte de Dados de Fila | Leia, escreva e elimine o Azure Armazenamento filas e mensagens de fila. Para saber quais as ações necessárias para uma determinada operação de dados, consulte permissões para chamadas de operações de dados de blob e fila. | Sim | 
Armazenamento Processador de mensagens de dados de fila | Espreite, recupere e elimine uma mensagem de uma fila de Armazenamento Azure. Para saber quais as ações necessárias para uma determinada operação de dados, consulte permissões para chamadas de operações de dados de blob e fila. | Sim | 
Armazenamento Remetente de mensagem de dados de fila | Adicione mensagens a uma fila de Armazenamento Azure. Para saber quais as ações necessárias para uma determinada operação de dados, consulte permissões para chamadas de operações de dados de blob e fila. | Sim | 
Armazenamento Leitor de dados de fila | Leia e enuse Armazenamento filas e mensagens de fila do Azure. Para saber quais as ações necessárias para uma determinada operação de dados, consulte permissões para chamadas de operações de dados de blob e fila. | Não | 
Colaborador de Pedido de Apoio | Permite criar e gerir pedidos de Suporte | Sim | 
Gestor de Tráfego Contribuinte | Permite-lhe gerir Gestor de Tráfego perfis, mas não permite que controle quem tem acesso a eles. | Sim | 
Administrador de Acesso dos Utilizadores | Permite-lhe gerir o acesso do utilizador aos recursos Azure. | Sim | 
Login de administrador de máquina virtual | Ver Máquinas Virtuais no portal e iniciar sessão como administrador | Sim | 
Contribuidor de Máquina Virtual | Permite-lhe gerir máquinas virtuais, mas não acesso a elas, e não à rede virtual ou à conta de armazenamento a que estão ligadas. | Sim | 
Início de sessão do utilizador de máquina virtual | Ver Máquinas Virtuais no portal e iniciar sessão como um utilizador regular. | Sim | 
Colaborador do Plano Web | Permite-lhe gerir os planos web para sites, mas não acesso aos mesmos. | Sim | 
Colaborador do Site | Permite-lhe gerir websites (não planos web), mas não acesso a eles | Sim |

## <a name="next-steps"></a>Próximos passos

- [Partner earned credit - uma visão geral de como funciona na nova experiência de comércio na CSP](partner-earned-credit.md)
