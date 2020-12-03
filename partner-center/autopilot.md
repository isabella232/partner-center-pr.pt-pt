---
title: Personalize a experiência fora da caixa de um dispositivo
ms.topic: how-to
ms.date: 04/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Antes de entregar o novo dispositivo de um cliente, pode utilizar perfis do Windows Autopilot para personalizar ou configurar previamente a experiência fora de caixa do dispositivo (OOBE).
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: 12057d50e4456dd2450ff497e00c89a9afa5dc4d
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534999"
---
# <a name="use-windows-autopilot-profiles-on-new-devices-to-customize-a-customers-out-of-box-experience"></a>Utilizar perfis do Windows Autopilot em novos dispositivos para personalizar a experiência inicial de um cliente

**Funções adequadas**

- Agente administrativo
- Administrador global
- Agente comercial
- Administração de gestão de utilizadores

Se gerir os dispositivos do cliente, poderá ter de personalizar a experiência fora da caixa (OOBE) para os utilizadores do cliente. Pode configurar novos dispositivos com perfis Do Windows Autopilot antes de entregar os dispositivos aos clientes e aplicar novos perfis aos dispositivos que os clientes já adquiriram. 

Note que os OEMs começaram a incluir uma etiqueta de envio no exterior da caixa do dispositivo Autopilot que mostra o ID da chave de produto do dispositivo **(PKID)**.  Este código de barras lídimensional e legível proporciona aos parceiros a jusante uma forma de registar dispositivos para o Autopilot sem ter de desboxar o(s) dispositivo(s) e recolher o ID do dispositivo por meios alternativos.

Este artigo explica como criar e aplicar perfis de piloto automático em dispositivos no Partner Center.

Se ainda não está familiarizado com o Autopilot, reveja as informações nestes artigos:

- [Descrição geral do Windows Autopilot](/windows/deployment/windows-10-auto-pilot)
- [Guia de referência de implantação de piloto automático](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a>Descrição geral

Com a funcionalidade Piloto Automático do Windows no Partner Center, pode criar perfis personalizados para aplicar aos dispositivos do cliente. As seguintes definições de perfil estavam disponíveis no momento da publicação deste artigo:

- Ignore as definições de privacidade. Esta definição opcional de perfil autopiloto permite que as organizações não perguntem sobre as definições de privacidade durante o processo OOBE.

- Desative a criação de conta de administração local no dispositivo. As organizações podem decidir se o utilizador que configura o dispositivo deve ter acesso ao administrador uma vez que o processo esteja concluído.

- Configurar automaticamente o dispositivo para o trabalho ou para a escola. Todos os dispositivos registados no Autopilot serão automaticamente considerados trabalho ou dispositivos escolares, pelo que esta questão não será feita durante o processo OOBE.

- Skip Cortana, OneDrive e páginas de configuração de registo OEM. Todos os dispositivos registados no Autopilot saltarão automaticamente estas páginas durante o processo de experiência fora de caixa (OOBE).

- Ignore o Contrato de Licença de Utilizador Final (EULA). A partir da versão 1709 do Windows 10, as organizações podem decidir saltar a página EULA apresentada durante o processo OOBE. Consulte o [despedimento do Windows Autopilot EULA](#windows-autopilot-eula-dismissal) abaixo para obter informações importantes a considerar sobre saltar a página EULA durante a configuração do Windows.

Aplicam-se as seguintes permissões e limitações de gestão de perfis e dispositivos:

- Os parceiros CSP podem continuar a gerir os perfis do Autopilot de clientes existentes com os quais têm relações de revendedores, mesmo que os clientes tenham removido os privilégios de administração delegada dos parceiros.

- Pode gerir dispositivos existentes dos clientes que adicionou.

- Não pode gerir dispositivos que o seu cliente carregou para a Microsoft Store para Empresas ou para o Portal do Microsoft Intune.

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a>Criar e gerir perfis de piloto automático no Partner Center

No Partner Center, pode criar perfis de implementação do Windows Autopilot e aplicá-los em dispositivos.

>[!NOTE]
>Só os agentes administrativos podem criar e aplicar perfis.

### <a name="create-a-new-autopilot-profile"></a>Criar um novo perfil de piloto automático

1. Selecione **clientes** do menu Partner Center e, em seguida, selecione o cliente para o qual está a criar o perfil Autopilot.

2. Na página de pormenor do cliente, selecione **Dispositivos**.

3. Nos **perfis do Windows Autopilot** selecione Adicionar novo **perfil**.

4. Introduza o nome e a descrição do perfil e, em seguida, configufique as definições OOBE. Escolha entre:  

   - Salte as definições de privacidade na configuração

   - Desativar a conta de administração local na configuração
  
   - Salte automaticamente as páginas na configuração<br>
        (Inclui *configuração automaticamente selecionada para o trabalho ou escola* e as páginas de *configuração de registo Skip Cortana, OneDrive e OEM)*
  
   - Ignorar o contrato de licença de utilizador final (EULA)<br> 
       >[!IMPORTANT] 
       >Consulte o [despedimento do Windows Autopilot EULA](#windows-autopilot-eula-dismissal) abaixo para obter informações importantes a considerar sobre saltar a página EULA durante a configuração do Windows.

5. **Selecione Enviar por terminada.**

### <a name="apply-an-autopilot-profile-to-customer-devices"></a>Aplicar um perfil autopiloto nos dispositivos do cliente

>[!NOTE]
>As instruções abaixo assumem que já adicionou os dispositivos do cliente ao Partner Center e que pode aceder à sua lista de dispositivos. Se ainda não adicionou os dispositivos do cliente, siga as instruções dos [dispositivos Add para a conta de um cliente](#add-devices-to-a-customers-account) e siga os passos abaixo.

Depois de criar um perfil autopiloto para um cliente, pode aplicá-lo aos dispositivos do cliente.

1. Selecione **clientes** do menu Partner Center e, em seguida, selecione o cliente para o quais criou o perfil Autopilot.

2. Na página de pormenor do cliente, selecione **Dispositivos**.

3. Em **Aplicar perfis a dispositivos** selecione os dispositivos ou grupos de dispositivos a que pretende adicionar perfis e, em seguida, selecione Aplicar o **perfil**. O perfil que acabou de aplicar aparece na coluna **Profile.**

4. Siga os passos abaixo para verificar se o perfil será aplicado com sucesso no dispositivo.

    a.  Ligue um dispositivo à rede e ligue-o.

    b.  Verifique se aparecem os ecrãs OOBE apropriados (se houver).

    c.  Quando o processo OOBE parar, reinicie o dispositivo nas definições predefinidos da sua fábrica para o preparar para um novo utilizador.

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a>Remova um perfil de piloto automático do dispositivo de um cliente

1. Selecione **clientes** do menu Partner Center e, em seguida, selecione o cliente para o quais criou o perfil Autopilot.

2. Na página de pormenor do cliente, selecione **Dispositivos**.

3. Em **Aplicar perfis a dispositivos** selecione os dispositivos de onde pretende remover o perfil e, em seguida, selecione Remover o **perfil**.

   >[!NOTE]
   >Remover um perfil de um dispositivo não elimina o perfil da sua lista. Se pretender eliminar um perfil, siga as instruções em [Atualizar ou elimine um perfil de Piloto Automático](#update-or-delete-an-autopilot-profile).

### <a name="update-or-delete-an-autopilot-profile"></a>Atualizar ou eliminar um perfil de piloto automático

Se um cliente quiser alterar a experiência fora da caixa depois de ter enviado os dispositivos para eles, pode alterar o perfil no Partner Center.

Quando o dispositivo do cliente se ligar à internet, irá descarregar a versão de perfil mais recente durante o processo OOBE. Além disso, sempre que um cliente restaurar um dispositivo nas suas definições padrão de fábrica, o dispositivo irá novamente descarregar a versão de perfil mais recente durante o processo OOBE.

1. Selecione **clientes** do menu Partner Center e, em seguida, selecione o cliente que quer que você mude um perfil de Piloto Automático.

2. Na página de pormenor do cliente, selecione **Dispositivos**.

3. Nos **perfis do Windows Autopilot** selecione o perfil necessário para atualizar. Faça as alterações necessárias e, em seguida, **selecione Enviar por isso.**

Para eliminar este perfil, **selecione Eliminar** o perfil do canto superior direito da página.

### <a name="add-devices-to-a-customers-account"></a>Adicionar dispositivos à conta de um cliente

>[!NOTE]
>Os agentes de vendas e os agentes administrativos podem adicionar dispositivos à conta de um cliente.

Antes de poder aplicar perfis autopilotos personalizados aos dispositivos do cliente, tem de conseguir aceder à lista de dispositivos do cliente.

Se pretender utilizar o nome OEM, número de série e combinação de modelos, esteja ciente destas limitações:

- Este tuple funciona apenas para dispositivos mais recentes (hashes 4k, por exemplo) e não é suportado para hashes de 128b (RS2 e dispositivos anteriores).

- O registo de tuple é sensível a casos, pelo que os dados do ficheiro devem coincidir com os nomes do modelo e do fabricante **_exatamente_* _ como fornecido pelo fornecedor OEM (fornecedor de hardware).

Siga as instruções abaixo para adicionar dispositivos à conta de um cliente no Partner Center.

1. Selecione _ *Clientes** do menu Partner Center e, em seguida, selecione o cliente cujos dispositivos pretende gerir.

2. Na página de pormenor do cliente, selecione **Dispositivos**.

3. Em **Aplicar perfis a dispositivos** selecione Adicionar **dispositivos**.

4. Introduza um nome para a lista de **dispositivos** e, em seguida, selecione Procurar para carregar a lista do cliente (em .csv formato de ficheiro) para o Partner Center.

    >[!NOTE]
    >Deveria ter recebido este ficheiro .csv com a compra do seu dispositivo. Se não recebeu um ficheiro .csv, pode criar um, seguindo os passos na [adição de dispositivos ao Windows Autopilot](/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).  

5. Faça o upload do ficheiro .csv e, em seguida, **selecione Save**.

Se receber uma mensagem de erro ao tentar carregar o ficheiro .csv, verifique o formato do ficheiro. Pode utilizar apenas o hash de hardware ou o nome do OEM, o número de série e o modelo (nessa ordem das colunas) ou o ID do Produto do Windows. Também pode utilizar a amostra .csv ficheiro fornecido a partir do link ao lado dos dispositivos Add para criar uma lista de **dispositivos.**

O seu ficheiro .csv deve ser parecido com isto:

> **Número de série do dispositivo,ID do produto do Windows,Hash de Hardware,Nome do fabricante,Modelo de dispositivo**

> **{serialNumber},,,Microsoft Corporation,Surface Laptop**

>[!NOTE]
> "Nome do fabricante" e "Modelo do Dispositivo" são sensíveis a maiôs.

Se não souber qual o valor a colocar para o nome do Fabricante e modelo de dispositivo, pode executá-lo no dispositivo para recolher os valores corretos:

<pre><code>md c:\\HWID

Set-Location c:\\HWID

Set-ExecutionPolicy -Scope Process -ExecutionPolicy Unrestricted

Install-Script -Name Get-WindowsAutoPilotInfo

Get-WindowsAutoPilotInfo.ps1 -OutputFile AutoPilotHWID.csv -Partner -Force
</code></pre>

## <a name="windows-autopilot-eula-dismissal"></a>Despedimento do Windows Autopilot EULA

### <a name="important-information"></a>INFORMAÇÃO IMPORTANTE

O Windows Autopilot permite-lhe configurar instalações personalizadas do Windows em dispositivos que gere para os seus clientes. Se for autorizado a fazê-lo pelo cliente, pode suprimir ou ocultar certos ecrãs de configuração que normalmente são apresentados aos utilizadores ao configurar o Windows, incluindo o ecrã de aceitação do EULA (End User License Agreement).

Ao utilizar esta função, concorda que suprimir ou ocultar quaisquer ecrãs concebidos para fornecer aos utilizadores um aviso ou aceitação de termos significa que obteve consentimento e autorização suficientes do seu cliente para ocultar termos, e que, em nome do seu cliente (seja uma organização ou um utilizador individual como o caso pode ser), consentir com quaisquer avisos e aceitar quaisquer termos aplicáveis ao seu cliente. Isto inclui o acordo com os termos e condições da licença ou aviso que seriam apresentados ao utilizador se não a suprimir ou esconder usando esta ferramenta. O seu cliente não poderá utilizar o software Windows nesses dispositivos se o cliente não tiver adquirido validamente uma licença para o software da Microsoft ou dos seus distribuidores licenciados.