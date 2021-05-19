---
title: Consolidação de inquilinos de autorização regional da CSP
ms.topic: how-to
ms.date: 07/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Utilize estas instruções para consolidar inquilinos para diferentes países/regiões. Isto inclui passos para migrar contas de clientes e subscrições de clientes.
author: billLinzbach
ms.author: billLi
ms.localizationpriority: medium
robots: noindex,nofollow
ms.custom: SEOMAY.20
ms.openlocfilehash: d2168dcd60b8675a21960918dab49b778025fa51
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147586"
---
# <a name="instructions-for-csp-regional-authorization-tenant-consolidation"></a>Instruções para consolidação de inquilinos de autorização regional de CSP

**Aplica-se a**: Partner Center | Centro de Parceiros para Microsoft Cloud para governo dos EUA

**Funções adequadas**: Administração global | Agente administrativo

\[Algumas informações dizem respeito a um produto pré-lançado que pode ser substancialmente modificado antes de ser lançado comercialmente. A Microsoft não faz garantias, de forma expressa ou implícita, em relação à informação aqui apresentada.\]

Pode consolidar inquilinos para o seu negócio. Utilize estas instruções para consolidar inquilinos para diferentes países/regiões.

>[!NOTE]  
>Deve estar ciente de todas as assinaturas e contagens de licença para cada um dos seus clientes na conta de que está em transição. Irá re-a provisionar essas mesmas assinaturas exatas com as mesmas contagens de licença ao abrigo da nova conta central da CSP como parte do processo de migração. Utilize a funcionalidade de lista de exportação para ajudar a criar uma lista de clientes para passar para o inquilino centralizado.  Uma vez que a consolidação esteja completa, não pode voltar ao estado inquilino anterior. A ação do cliente também pode ser necessária.

## <a name="prepare-for-migration"></a>Prepare para a migração

- Inscreva-se no **Partner Center**  utilizando a conta de Transição (a que irá **transitar** para a nova conta), e reveja todos os clientes e todos os serviços prestados a esses clientes.

- Assine fora desta conta.

## <a name="migrate-customer-accounts"></a>Migrar contas de clientes

1. Inscreva-se no **Partner Center**  com a conta **de transição** (nova) (aquela em que está a transitar clientes).

2. Selecione **Clientes**.

3. Selecione **Solicite uma relação de revendedor**. É-lhe apresentada uma mensagem de correio eletrónico padrão para enviar aos seus clientes. Esta mensagem contém um URL com o iD org exclusivo da sua nova conta Partner Center.

4. **Ação do Cliente:** Certifique-se de que cada um dos clientes ativos que pretende migrar visita este URL. Ao abrir o URL, o cliente é solicitado a iniciar sedução no portal do Office 365. O cliente assina na utilização do mesmo ID Org que utiliza para aceder aos portais de administração Azure e Office 365.

5. Após a sua assinatura, o Administrador Global para a conta do **cliente** é solicitado a apresentar um acordo que dê privilégios de administração delegados à nova conta CSP. Se concordarem, o cliente seleciona a caixa de verificação e concorda em autorizar a relação.

Os clientes aparecerão na lista de clientes do parceiro depois de terem apresentado o contrato, um a um.

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a>Subscrições baseadas em uso do Gabinete Migratório 365 e não-Azure

1. Uma vez que o seu cliente tenha assinado o contrato, pode recriar as suas subscrições sob o seu Inquilino Centralizado.

2. A partir do **Partner Center,** selecione **Clientes.**

3. Abra o nome da empresa para o cliente que pretende migrar.

4. Selecione **Adicionar subscrição**.

5. Adicione as assinaturas corretas e as contagens de licença do catálogo. Verifique com as informações fornecidas nas contas **de parceiros.**

   :::image type="content" source="images/regionalcustomer2.png" alt-text="lista de clientes":::

6. **Selecione Enviar.**

   Os serviços são agora prestados ao cliente a partir da conta **de transição para** parceiro.

7. Repita estes passos para migrar subscrições para todos os clientes adicionais.

Antes de avançar para a secção seguinte, certifique-se de que todas as subscrições de clientes existentes no âmbito das contas **de** parceiros são realoadas na conta **de transição para** parceiro.

> [!NOTE]
> Os parceiros devem suspender as subscrições na conta **de "Transição de** Inquilinos Parceiros" no Centro de Parceiros no mesmo dia em que essas assinaturas são transitadas e criadas ao abrigo da conta **de "Transição para** Inquilino Parceiro" no Centro de Parceiros para garantir que a faturação dupla não ocorre. Os pedidos de apoio serão negados para créditos devido a qualquer sobreposição na faturação que ocorra de não desativar corretamente as subscrições **de Transição** de Assinaturas.

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a>Desativação das 365 assinaturas do Office no âmbito da conta de transição de parceiros

A desativação da subscrição do CSP ao abrigo das contas de parceiros em **transição** impede qualquer faturação futura. Não é preciso desativar manualmente as subscrições do Azure, porque as subscrições do Azure são automaticamente desativadas durante o processo de migração.

1. Inscreva-se no **Centro de Parceiros** com a conta **de transição da** CSP e navegue para a lista de clientes.

2. Abra o cliente com subscrições para desativar e, em seguida, selecione a primeira oferta para desativar.

3. Desafie a subscrição para **suspender** e, em seguida, selecione **submeter**.

   >[!Note]
   >A suspensão da subscrição garante que não ocorra uma faturação dupla.

   A subscrição mostra **suspensa** na lista de assinaturas.

4. Repita estes passos para todas as subscrições sob o cliente. Verifique todos os **espetáculos suspensos.**

5. Selecione o próximo cliente da lista e repita o processo de desativação de todas as subscrições.

## <a name="migrating-azure-usage-based-subscriptions"></a>Subscrições baseadas em uso do Azure migratório

Ao contrário das assinaturas CSP do Office 365, a Azure, as assinaturas CSP baseadas na utilização não precisam de ser migradas manualmente. O Microsoft Azure Support migrará as subscrições do Azure e todos os serviços ou recursos implantados da **conta de revendedor de** CSP para a conta de revendedor de **transição para** CSP. Não haverá interrupção do serviço ao cliente durante esta transição.

1. Certifique-se de que as contas de clientes que terão as assinaturas Azure migradas aceitaram o acordo para ser associado à nova conta **de Transição para** CSP.

2. Irá notificar a Microsoft de quais as contas de clientes prontas a migrar e fornecer os nomes da empresa desses clientes.

3. A Microsoft migra as subscrições baseadas em uso do Azure e notifica-o quando a migração estiver completa.

4. Tem de confirmar que a subscrição do Azure no âmbito da conta de **revendedor de transição de** CSP está agora marcada **suspensa** no Partner Center sob a secção de subscrições de clientes.

5. Confirme que a subscrição do Azure ao abrigo da conta de **revendedor de transição para** CSP mostra agora um estado ativo no Partner Center sob a secção de subscrições do cliente. 

   >[!Note]
   > A desativação das subscrições ao abrigo do cliente não altera o aparecimento do cliente na lista de Clientes. Atualmente não existe opção de retirar clientes da lista. Os parceiros devem evitar adicionar subscrições a estes clientes da sua conta **de Transição de A partir** do futuro.

6. Repita estes passos para todas as subscrições sob todos os seus clientes para parar os encargos futuros na conta **(s) de Transição.** O parceiro receberá uma fatura final com crédito pelo número de dias não reutilizados entre o dia de cancelamento e o último dia do período de faturação. Nenhuma fatura futura gerará após o período final de faturação.

### <a name="additional-information"></a>Informações adicionais

- A desativação da subscrição da conta **de transição da** CSP não afeta o serviço do cliente final desde que o serviço tenha sido prestado a partir da conta **de transição para** CSP antes de desativar a subscrição.

- As subscrições não podem ser utilizadas pelo cliente e não geram encargos quando suspensas ou canceladas.

- De momento não existe forma de remover completamente um cliente da lista de **Clientes.**
- 
    >[!Note]
    > Os parceiros devem suspender as subscrições na conta **de** inquilinos parceiros no Centro de Parceiros no mesmo dia em que essas subscrições são transitadas e criadas ao abrigo da conta **Transição Para** garantir que a faturação dupla não ocorre. A Microsoft não apoiará pedidos de créditos devido a qualquer sobreposição na faturação que ocorra de não definir corretamente as subscrições **de Transição** de subscrições para suspensas.

### <a name="simplify-migration-using-export"></a>Simplificar a migração usando exportação

Utilizando a **Função Exportação,** pode capturar as subscrições que necessita de utilizar na sua nova estrutura consolidada:

1. Selecione **Clientes** no Partner Center para ver a lista de clientes. 

2. Abra o nome do cliente desejado.

3. Na página **de Subscrições,** selecione **Subscrições de Exportação** para exportar detalhes de subscrições para um ficheiro Excel.

4. Utilize esta lista para recriar as subscrições no seu novo inquilino consolidado.

### <a name="api-registration"></a>Registo da API

Para obter mais informações sobre o registo da API, consulte [configurar o acesso a API no Partner Center.](/partner-center/develop/set-up-api-access-in-partner-center)

## <a name="next-steps"></a>Passos seguintes

- [Cloud Solution Provider programa mercados regionais e moedas onde pode vender ofertas de CSP](regional-authorization-overview.md)
