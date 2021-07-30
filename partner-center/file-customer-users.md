---
title: Campos para .csv ficheiro para importar vários utilizadores para uma conta de cliente
ms.topic: article
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: Para adicionar vários utilizadores a uma conta de cliente, crie um ficheiro de valor separado em vírgula (.csv) com campos apropriados.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 7d8cbeecf081dc82448625daeedc0ce21b31174e
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/29/2021
ms.locfileid: "114838347"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a>Adicionar vários utilizadores a uma conta de cliente criando um ficheiro .csv

**Funções apropriadas**: Administração global

Adicione vários utilizadores à conta de um cliente de uma só vez, enviando um ficheiro de dados no formato de ficheiro de valor separado em vírgula (.csv) para o Centro de Parceiros. Pode descarregar um ficheiro de dados de amostra do Centro de Parceiros e depois editá-lo para a sua utilização, ou pode criar um novo ficheiro de dados utilizando o modelo de dados definido abaixo.

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a>Requisitos de ficheiros de dados

Para adicionar vários utilizadores à conta de um cliente utilizando o processo de upload em massa, terá de cumprir os seguintes requisitos:

- Tem de ter permissões globais de administrador na conta do cliente;
- Cada utilizador deve ter um endereço de e-mail único, anexado ao domínio de e-mail do cliente;
- Pode carregar até 100 discos de cada vez. Se precisar de adicionar mais de 100 utilizadores, crie e carre faça upload de ficheiros de dados adicionais.
- Todos os utilizadores devem estar na mesma **Localização** Geográfica.
- Introduza apenas os dados descritos abaixo. Dados extraéssis farão com que o upload falhe.

Introduza os seguintes dados no ficheiro de dados:

| **Nome da coluna** | **Descrição**  | **Limitação**  |
|:-------- |:------  |:----- |
| Nome próprio  | Primeiro nome do utilizador (campo opcional)  | Limite de 50 caracteres  |
| Apelido  | Apelido do utilizador (campo opcional)  | Limite de 50 caracteres  |
| Nome a apresentar    | Nome exibido no Centro de Parceiros (campo obrigatório)                            | Limite de 50 caracteres                         |
| E-mail   | Endereço de e-mail de negócios do utilizador na empresa de clientes (campo obrigatório)           | Cada utilizador deve ter um endereço de e-mail único |
| Atualização de estado   | Usado para indicar se o novo registo de utilizadores foi criado com sucesso | \*\*Deixe vazio\*\*                        |

## <a name="next-steps"></a>Passos seguintes

- [Como adicionar vários utilizadores para um cliente](adding-multiple-users-to-a-customer-account.md)