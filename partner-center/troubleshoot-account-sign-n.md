---
title: Resolução de problemas configurando a sua conta Partner Center ou problemas de renovação mpn
ms.topic: how-to
ms.date: 09/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-enroll
description: Problemas de resolução de problemas ao tentar matricular-se no Partner Center. Respostas abordam desafios com métodos de pagamento, esquecendo palavras-passe, e muito mais.
author: ParthP
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d57cec763db2c22b08ec7cc5ae1b6f39c697811f
ms.sourcegitcommit: e1da62b36420d78bf44e3962358d0af65ebc3402
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/27/2021
ms.locfileid: "129088523"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a>Resolver problemas de configuração da conta ou de renovação do MPN

**Funções adequadas**: Administração global | Administrador sócio da MPN

Aqui ficam algumas sugestões para resolver problemas comuns que surgem ao configurar a sua conta Partner Center.

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a>O que acontece se você estiver migrando do Centro de Membros parceiros e você não pode editar quaisquer campos de informação da empresa

Nos casos em que a sua empresa já tenha presença no Partner Center (por exemplo, uma conta Fornecedor de Soluções em Nuvem (CSP) – será mostrado um ecrã apenas de leitura. Este ecrã apresentará todas as informações sobre a sua empresa tal como existe no Partner Center.

Não podes alterar os detalhes deste ecrã. Isto é por design e não por um erro.

Para prosseguir, **selecione Aceitar** e, em seguida, selecione **Continue**.

### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a>Se o departamento de TI tiver desligado **inscreva-se no Partner Center**

Você vê esta mensagem porque os utilizadores virais são desativado, ou porque a Inscrição Viral é desativada no inquilino Azure Ative Directory (AD). O administrador Global para a sua conta Azure AD pode permitir as funcionalidades necessárias executando o seguinte comando PowerShell:

**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**

Para mais informações, leia [o Self-service inscreva-se.](/azure/active-directory/users-groups-roles/directory-self-service-signup)

## <a name="you-forgot-your-password"></a>Esqueceu-se da sua senha.

Se esqueceu a sua palavra-passe, na página de iniciar scontabilidade, selecione **Não pode aceder à sua conta?** Esta opção permite-lhe redefinir a sua palavra-passe ou pedir ao seu administrador Global para lhe atribuir novas credenciais.

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a>No ecrã "Fale-nos da sua empresa", recebe um erro de "Algo correu mal"

Esta mensagem de erro geralmente aparece se utilizar inadvertidamente caracteres, espaços ou código de país no número de telefone da sua empresa. O valor introduzido no campo Telefone Número só pode conter um máximo de 10 caracteres.

### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a>A compra do seu cartão de crédito está a receber uma mensagem de erro afirmando que "a sua encomenda foi recusada. Por favor, verifique as suas informações"

Utilize sempre o endereço correspondente ao seu cartão de crédito e não à sua entidade legal. Além disso, certifique-se de que o código postal está correto e corresponde ao endereço que utiliza.

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a>Pretende mudar de pagamento offline para método de pagamento online

Terá de cancelar a encomenda original e recomprar utilizando o método de pagamento preferido.

Para cancelar uma encomenda:

> [!NOTE]
> Para saber mais sobre a interface de espaços de trabalho, consulte [o Centro de Parceiros.](get-around-partner-center.md#turn-workspaces-on-and-off)

#### <a name="workspaces-view"></a>[Vista de espaços de trabalho](#tab/workspaces-view)

1. No [painel partner Center](https://partner.microsoft.com/dashboard), selecione o azulejo **de adesão.**

2. **Selecione ofertas de adesão** e, em seguida, **cancele a encomenda**.

3. Aparecerá uma janela de confirmação e deverá confirmar-se para cancelar a encomenda inicial.

#### <a name="current-view"></a>[Vista atual](#tab/current-view)

1. No [painel partner Center,](https://partner.microsoft.com/dashboard)selecione o **separador Ofertas de Adesão.**

2. Selecione **cancelar a encomenda**.

3. Aparecerá uma janela de confirmação e deverá confirmar-se para cancelar a encomenda inicial.

* * *

## <a name="next-steps"></a>Passos seguintes

- [Manage your Partner Center account](partner-center-account-setup.md) (Gerir a conta do Partner Center)
- [Como ler a sua conta e arquivo de reconhecimento](read-your-bill.md)
