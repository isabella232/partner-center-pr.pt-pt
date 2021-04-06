---
title: Obtenha privilégios administrativos de um cliente
ms.topic: how-to
ms.date: 12/02/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtenha as permissões necessárias para gerir o serviço ou subscrição de um cliente em seu nome. Saiba como as permissões são concedidas, revogadas e geridas.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: high
ms.openlocfilehash: 624b66c7912af1f0109b6aadeffb67c5d4e9ea4b
ms.sourcegitcommit: 3d7d5064c5e021079ed7e6f93f03869cbf425a32
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/06/2021
ms.locfileid: "106502502"
---
# <a name="obtain-permissions-to-manage-a-customers-service-or-subscription"></a>Obter permissões para gerir o serviço ou subscrição de um cliente

**Funções adequadas**

- Agente administrativo
- Agente comercial

Para gerir o serviço ou subscrição de um cliente em seu nome, o cliente deve conceder-lhe permissões de administrador para esse serviço. Para obter permissões de administrador de um cliente, envie-lhes um pedido de relacionamento revendedor. Depois de o cliente aprovar o seu pedido, poderá inscrever-se no portal de administração do serviço e gerir o serviço em nome do cliente. 

## <a name="invite-a-customer-to-establish-a-reseller-relationship-with-you"></a>Convide um cliente a estabelecer uma relação de revendedor consigo

1.  Selecione **Clientes** e, em seguida, **selecione Solicite uma relação de revendedor**.

2.  Na página seguinte, analise a mensagem de e-mail de rascunho. Pode abrir a mensagem de rascunho na aplicação de e-mail predefinida ou pode copiar a mensagem para a área de transferência e colar num e-mail. 

    >[!IMPORTANT]
    >Pode editar o texto no e-mail, mas confirme que inclui a ligação, pois está personalizada para ligar o cliente diretamente à conta. 
    
3.  Selecione **Feito** quando tiver concluído este passo.

4.  Envie o e-mail para o seu cliente.

5.  Depois de o cliente aceitar o seu convite, eles aparecerão na sua página **de Clientes,** e poderá providenciar e gerir o serviço para o cliente a partir daí.

6.  Para gerir a conta, serviços, utilizadores e licenças do cliente, expanda o registo do cliente selecionando a seta para baixo perto do seu nome e, em seguida, selecione o portal de administração para o serviço que pretende gerir.

>[!IMPORTANT]  
>Os clientes podem reatribuir ou remover permissões de administrador no portal de administração de um serviço. No entanto, precisa de informar o cliente de que remover as permissões do administrador significa que deixará de poder abrir um pedido de serviço à Microsoft em seu nome. Não poderá abrir este tipo de pedidos de serviço em nome do cliente até renegociar o seu acordo com o cliente.

Os seus clientes podem descobrir qual dos seus parceiros tem privilégios administrativos para o seu inquilino dentro do portal de administração do Office 365. Para efetuar este procedimento:

1. O cliente precisa de se inscrever no portal de administração do Office 365 como administrador global.

2. Selecione **Definições**  >  **Relacionamentos de parceiros**.

3. Na página de **relações com** parceiros, o cliente verá uma lista dos parceiros com quem trabalham e daqueles a quem foi concedido privilégios de administração delegados ao seu inquilino.

## <a name="customers-can-manage-a-partners-delegated-admin-privileges"></a>Os clientes podem gerir os privilégios de administração delegados de um parceiro 

O seu cliente pode decidir remover os seus privilégios de administração delegados do seu inquilino, mas manter a relação consigo para efeitos de subscrição e renovação de licença. Os clientes gerem direitos e permissões nas suas contas office 365 na página de **relações de Parceiro** no Centro de Administração do Office 365. Nesta página, os clientes podem:

- Veja com que parceiros têm uma relação e com que parceiros delegaram privilégios de administração

- Remova os privilégios de administração delegados de um parceiro do inquilino

Para remover os privilégios de administração delegados de um parceiro:

1. Na página **de relações do Parceiro,** selecione o parceiro de interesse.
2. No painel de detalhes, **selecione Remover** administrador delegado .
3. No painel de confirmação, selecione **Remover**.

>[!IMPORTANT]  
>As atribuições de papel da AD Azure ao parceiro estão implícitas. Se tentar listar os membros das funções AD Azure utilizando o Portal AD/PowerShell/Graph do Azure, o parceiro não será devolvido. Para saber se os parceiros são atribuídos às funções de Azure AD, deve consultar a página de relações de Parceiro no Portal de Administração do Office 365 para saber se o privilégio de administração delegado foi ou não concedido ao parceiro.

## <a name="delegated-admin-privileges-in-azure-ad"></a>Privilégios de administração delegados em Azure AD 

Existem dois grupos de segurança, agentes administrativos e agentes da Helpdesk, no inquilino AZure AD do parceiro que são usados para administração delegada. Quando um cliente concede privilégios de administração delegados a um parceiro:

- O grupo de agente administrativo é designado para o papel de Administrador Global no inquilino AZure AD do cliente.

- O grupo helpdesk Agent é atribuído ao papel de Administrador helpdesk no inquilino AZure AD do cliente.

Com base nas funções de diretório atribuídas, os membros de ambos os grupos podem inscrever-se no inquilino AZure AD do cliente e nos serviços O365 utilizando as credenciais de parceiro e administrador em nome do cliente.

Se o seu cliente remover privilégios de administração delegados, as atribuições de funções AD Azure são removidas, e você não será mais capaz de gerir o inquilino AZure AD do cliente.

### <a name="azure-subscriptions-and-resource-management"></a>Assinaturas Azure e gestão de recursos

Cada subscrição da Azure tem o seu próprio conjunto de funções de gestão de recursos. Antes de um parceiro CSP poder gerir a subscrição Azure de um cliente, o parceiro deve ser atribuído a uma ou mais funções sob a assinatura Azure. Especificamente:

- Quando um cliente aceita um convite de revenda e concede privilégio de administração delegado a um parceiro, o parceiro não tem automaticamente acesso às assinaturas Azure existentes sob o inquilino do cliente.

- Quando o parceiro CSP prevê uma nova subscrição Azure para o cliente, o grupo de Agentes Admin sob o inquilino parceiro CSP é automaticamente atribuído Papel de Proprietário sob a subscrição. Com base nesta atribuição de funções, os membros do grupo podem aceder e gerir recursos sob a subscrição.

- Quando um cliente remove os privilégios de administração delegados de um parceiro que utiliza o Portal do Office 365, o parceiro ainda pode gerir a subscrição Azure do cliente, desde que o parceiro ainda esteja atribuído a uma ou mais funções sob a subscrição. Para impedir que o parceiro gere a subscrição do Azure, o cliente deve remover a atribuição de funções.

## <a name="windows-autopilot"></a>Windows Autopilot

A partir do Partner Center, os parceiros da CSP podem gerir perfis autopilotos para os seus clientes sem privilégios de administração delegados nestas circunstâncias: 

- Se um cliente remover privilégios de administração delegados mas mantiver uma relação de revendedor consigo, pode continuar a gerir perfis de Autopilot para eles.

- Pode gerir os dispositivos de cliente que você ou outro parceiro adicionou. 

- Não é possível gerir dispositivos que o seu cliente adicionou através da Microsoft Store for Business, Microsoft Store for Education ou Microsoft Intune Portal.

Para obter mais informações sobre o Autopilot, consulte [a configuração do dispositivo Simplificar com o Windows Autopilot](autopilot.md).

>[!IMPORTANT]  
>A atual experiência de gestão do Autopilot no Partner Center pode continuar a mudar. No momento da publicação deste artigo, estão a ser consideradas as seguintes alterações:

- O parceiro deve ter privilégio de administração delegado pelo cliente antes que o parceiro possa adicionar/atualizar/remover perfis e aplicar/remover o perfil de qualquer dispositivo no cliente.

- O parceiro deve ter o privilégio de administração delegado pelo cliente antes que o parceiro possa remover os dispositivos adicionados por outros parceiros ou pelo cliente no cliente inquilino. Caso contrário, o parceiro só pode remover dispositivos adicionados anteriormente pelo mesmo parceiro.
