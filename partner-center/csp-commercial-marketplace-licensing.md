---
title: Gerir licenciamento em ofertas de marketplace
ms.topic: how-to
ms.date: 04/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como configurar e gerir o licenciamento para as suas ofertas de mercado comercial ISV.
author: petand123
ms.author: v-petand
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3b2281696a2fe69253cd033eb2a7eef7fb3046f3
ms.sourcegitcommit: 1899307642f057070b1bdd647594fc46ba61fb08
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/30/2021
ms.locfileid: "108284892"
---
# <a name="manage-licensing-in-marketplace-offers"></a>Gerir licenciamento em ofertas de marketplace

**Funções adequadas**

- Administrador global
- Administrador de conta

Este artigo acompanha-o através do processo de criação de uma oferta no Partner Center, disponibilizando-a no Microsoft AppSource e, em seguida, gerindo licenças para essa oferta.  

>[!IMPORTANT]
>As capacidades deste artigo estão atualmente em Visualização Pública.

## <a name="before-you-begin"></a>Antes de começar

Antes de iniciar este processo, deve familiarizar-se com as informações abaixo.

### <a name="review-the-azure-marketplace-documentation"></a>Reveja a documentação do Azure Marketplace

Os artigos abaixo contêm informações que deve saber antes de continuar. 

- [Criar uma oferta do Dynamics 365 for Customer Engagement e do PowerApps](https://docs.microsoft.com/azure/marketplace/dynamics-365-customer-engage-offer-setup)
- [Criar uma conta de mercado comercial no Partner Center](https://docs.microsoft.com/azure/marketplace/create-account)

### <a name="create-your-offer-id"></a>Crie o seu ID de oferta

Nos procedimentos abaixo, você será solicitado para introduzir um ID de oferta. Dedem um pouco para chegar a um ID de oferta adequado, tendo em conta os seguintes pontos:

- Este ID é visível para os clientes no endereço web para a oferta de mercado e modelos de Gestor de Recursos Azure, se aplicável.
- O ID da oferta combinado com o ID da Editora deve ter menos de 40 caracteres de comprimento.
- Utilize apenas letras minúsculas e números. O ID da Oferta pode incluir hífens e sublinhados, mas sem espaços. Por exemplo, se o seu ID editor for testpublisherid e introduzir test-offer-1, o endereço web da oferta será https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1 .
- Este ID não pode ser alterado depois de selecionar **Criar**.

### <a name="create-your-offer-alias"></a>Crie o seu pseudónimo Oferta

O pseudónimo Offer é o nome usado para a oferta no Partner Center. Você também precisará de um pseudónimo de Oferta apropriado que siga as diretrizes abaixo:

- Este nome não é usado no mercado e é diferente do nome da oferta e outros valores mostrados aos clientes.
- Este nome não pode ser alterado depois de selecionar Criar.

## <a name="create-your-offer"></a>Crie a sua oferta

O primeiro passo no processo de licenciamento é criar a sua oferta de mercado comercial. 

1. Inicie sessão no [dashboard do Centro de Parceiros](https://partner.microsoft.com/dashboard/).
2. No menu de navegação à esquerda, selecione **Commercial Marketplace/Overview**.
3. No topo da página 'Overview', selecione **Nova oferta** e, em seguida, selecione **Dynamics 365 para Customer Engagement & PowerApps**.
4. Insira o **ID da Oferta** e **ofereça o pseudónimo** que criou anteriormente.
5. Selecione **Criar** para gerar a oferta e continuar.
6. Escolha as suas opções de licenciamento.

    - Para ativar a gestão da licença para a sua oferta, selecione **Ative a gestão da licença de aplicações através da Microsoft.** Este é um cenário único, e não pode mudá-lo uma vez que a sua oferta é publicada.

    - Também pode permitir que os clientes executem a funcionalidade base da sua aplicação sem licença e executem funcionalidades premium uma vez que tenham adquirido uma licença. Para isso, selecione **Permitir que os clientes instalem a minha aplicação mesmo que as licenças não sejam atribuídas.**

    - Se não quiser que a sua oferta tenha a gestão da licença ativada, selecione **Get it now (Free)**, **Free trial**, ou **Contacte-me**.

## <a name="create-your-plan"></a>Criar o plano

Nestes passos definirá o plano ou planos que deseja ativar para a sua oferta.

1. No menu de navegação à esquerda, selecione **Plan overview** e, em seguida, selecione **Criar novo plano**.
2. Introduza o nome **de identificação** e **plano do** plano e, em seguida, selecione **Criar**.
3. Na página de listagem do **Plano,** insira a **descrição do seu Plano.**
4. Para guardar a descrição e terminar mais tarde, **selecione Guardar o rascunho**.

5. Quando terminar, selecione **'Rever' e publicar.** A informação do plano será agora exibida no appsource.microsoft.com em lista de ofertas (secção de planos).

6. Depois de ter criado todos os planos para esta oferta, terá de copiar o ID de serviço de cada plano. Selecione **a visão geral** do plano no topo da página de listagem do Plano. Copie o ID de serviço para cada plano para um local seguro.

## <a name="add-service-ids-to-your-solution"></a>Adicione IDs de serviço à sua solução

O próximo passo é atualizar a sua solução adicionando os IDs de serviço para cada plano que acabou de copiar. Para obter orientações sobre este ponto, consulte [Criar um Pacote AppSource para a sua solução.](https://docs.microsoft.com/powerapps/developer/data-platform/create-package-app-appsource)

## <a name="upload-your-package-and-publish-your-offer"></a>Faça upload do seu pacote e publique a sua oferta

1. No painel de navegação à esquerda, selecione **Mercado Comercial** e, em seguida, selecione **configuração técnica**.
2. Sob **o Modelo base de licença,** selecione **Utilizador.**
3. No **pacote CRM,** insira o URL da sua localização do pacote.
4. Utilize os outros separadores no painel de navegação esquerdo para introduzir qualquer outra informação necessária. Quando terminar, selecione **'Rever' e publicar**.

Depois de publicar a oferta, vamos rever e verificar as suas informações. Se houver algum problema com este processo, vamos notificá-lo. Quando todos os problemas tiverem sido resolvidos, receberá uma notificação de que a sua oferta está disponível no AppSource. Nessa altura, podes fazê-lo viver.

## <a name="make-your-offer-live-in-partner-center"></a>Faça a sua oferta ao vivo no Partner Center

O procedimento abaixo acompanha-o através do processo de fazer a sua oferta ao vivo no AppSource. Para saber mais sobre este processo, consulte [Introdução às opções de listagem.](https://docs.microsoft.com/azure/marketplace/determine-your-listing-type)

>[!NOTE]
>Uma vez publicada a sua oferta, levará 4 a 6 horas para ir ao vivo.

1. Inicie sessão no [dashboard do Centro de Parceiros](https://partner.microsoft.com/dashboard/).
2. No menu de navegação à esquerda, selecione **Commercial Marketplace/Overview**.
3. Na página **geral,** encontre a oferta que procura. As ofertas prontas a serem publicadas terão um estatuto de **Pré-visualização**. Selecione a oferta.
4. Na página geral da **Oferta,** selecione **Go live**.
A oferta será ao vivo em 4-6 horas.
5. Para ver a sua lista de ofertas no AppSource, selecione o link **AppSource** na parte inferior da página geral da **Oferta.**

    - **Para ofertas habilitados a licença :** Se a sua oferta necessitar de uma verificação de licença, os utilizadores só poderão introduzir uma pista clicando **em Contato comigo**, para que possa comunicar com eles.

    - **Para ofertas habilitados a licenças com opção de instalação gratuita**: Se a sua oferta não necessitar de uma verificação de licença, os utilizadores administrativos verão um botão **Get It Now** para além do Contact **Me**. Os utilizadores que pretendam experimentar a sua opção de instalação gratuita devem clicar em **Get It Now**, o que os levará a instalar a oferta no Power Platform Admin Center. Os utilizadores ainda podem utilizar **o Contato Me** se tiverem alguma dúvida, ou se quiserem fazer upgrade para um plano pago.

## <a name="register-isv-connect-deal-in-dealreg"></a>Registar negócio ISV Connect no DealReg

O próximo passo é registar o seu acordo. Para isso, consulte [registar as suas ofertas.](https://docs.microsoft.com/partner-center/register-deals)

## <a name="invite-the-customer"></a>Convide o cliente

Utilize o seguinte procedimento para convidar o cliente a participar neste negócio.  

1. Inicie sessão no [dashboard do Centro de Parceiros](https://partner.microsoft.com/dashboard/).
2. No menu de navegação à esquerda, selecione **Commercial Marketplace/Overview**.
3. Filtrar para **ofertas submetidas,** selecione o separador **Em Progresso** e, em seguida, selecione o negócio que deseja.
4. Na página geral para este negócio, selecione **Gerir licenças**.
5. Na janela **de licenças 'Gerir',** selecione o cliente da lista de dados do **Cliente.** Se a relação com o cliente ainda não existir, selecione **+Convide um novo cliente a consentir.**
6. Copie o link que é apresentado.
7. Envie este link por e-mail para a administração de faturação ou administração global do seu cliente, e faça-os usar este link para aceder a admin.microsoft.com e aceitar e autorizar a relação que está a estabelecer.

    >[!NOTE]
    >A relação não será estabelecida até que o cliente realize este passo.

## <a name="activate-manage-and-remove-your-licenses"></a>Ativar, gerir e remover as suas licenças

Uma vez estabelecido o seu cliente, pode começar a adicionar planos da sua oferta e atribuir licenças a cada plano.

1. Na janela de licenças Manage para este negócio, selecione **+Adicione um plano**.
2. Preencha os **Planos para esta solução** e número de campos **de licenças** e, em seguida, selecione **licenças de Atualização**. As licenças estarão disponíveis em admin.microsoft.com para os clientes gerirem e atribuíram aos colaboradores.

    - Para alterar o número de licenças para um plano existente, insira o novo número no campo **Número de licenças** e, em seguida, selecione **Licenças de Atualização**.

    - Para desativar ou remover licenças para uma oferta, selecione o ícone do caixote do lixo no campo Ações e, em seguida, selecione **'Update licenses'** **(Atualização).**