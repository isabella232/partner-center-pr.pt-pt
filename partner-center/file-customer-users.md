---
title: Campos para .csv ficheiro para importar vários utilizadores para uma conta de cliente
ms.topic: article
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Para adicionar vários utilizadores a uma conta de cliente, crie um ficheiro de valor separado em vírgula (.csv) com campos apropriados.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8ba08d97f1d360eae5af1941ed36753addd24939
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441426"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a><span data-ttu-id="445a1-103">Adicionar vários utilizadores a uma conta de cliente criando um ficheiro .csv</span><span class="sxs-lookup"><span data-stu-id="445a1-103">Add multiple users to a customer account by creating a .csv file</span></span>

<span data-ttu-id="445a1-104">**Funções adequadas**</span><span class="sxs-lookup"><span data-stu-id="445a1-104">**Appropriate roles**</span></span>

- <span data-ttu-id="445a1-105">Administrador global</span><span class="sxs-lookup"><span data-stu-id="445a1-105">Global admin</span></span>

<span data-ttu-id="445a1-106">Adicione vários utilizadores à conta de um cliente de uma só vez, enviando um ficheiro de dados no formato de ficheiro de valor separado em vírgula (.csv) para o Centro de Parceiros.</span><span class="sxs-lookup"><span data-stu-id="445a1-106">Add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="445a1-107">Pode descarregar um ficheiro de dados de amostra do Centro de Parceiros e depois editá-lo para a sua utilização, ou pode criar um novo ficheiro de dados utilizando o modelo de dados definido abaixo.</span><span class="sxs-lookup"><span data-stu-id="445a1-107">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="445a1-108">Requisitos de ficheiros de dados</span><span class="sxs-lookup"><span data-stu-id="445a1-108">Data file requirements</span></span>

<span data-ttu-id="445a1-109">Para adicionar vários utilizadores à conta de um cliente utilizando o processo de upload em massa, terá de cumprir os seguintes requisitos:</span><span class="sxs-lookup"><span data-stu-id="445a1-109">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

- <span data-ttu-id="445a1-110">Tem de ter permissões globais de administrador na conta do cliente;</span><span class="sxs-lookup"><span data-stu-id="445a1-110">You must have global administrator permissions to the customer account;</span></span>
- <span data-ttu-id="445a1-111">Cada utilizador deve ter um endereço de e-mail único, anexado ao domínio de e-mail do cliente;</span><span class="sxs-lookup"><span data-stu-id="445a1-111">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
- <span data-ttu-id="445a1-112">Pode carregar até 100 discos de cada vez.</span><span class="sxs-lookup"><span data-stu-id="445a1-112">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="445a1-113">Se precisar de adicionar mais de 100 utilizadores, crie e carre faça upload de ficheiros de dados adicionais.</span><span class="sxs-lookup"><span data-stu-id="445a1-113">If you need to add more than 100 users, create and upload additional data files.</span></span>
- <span data-ttu-id="445a1-114">Todos os utilizadores devem estar na mesma **Localização** Geográfica.</span><span class="sxs-lookup"><span data-stu-id="445a1-114">All users must be in the same geographic **Location**.</span></span>
- <span data-ttu-id="445a1-115">Introduza apenas os dados descritos abaixo.</span><span class="sxs-lookup"><span data-stu-id="445a1-115">Enter only the data described below.</span></span> <span data-ttu-id="445a1-116">Dados extraéssis farão com que o upload falhe.</span><span class="sxs-lookup"><span data-stu-id="445a1-116">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="445a1-117">Introduza os seguintes dados no ficheiro de dados:</span><span class="sxs-lookup"><span data-stu-id="445a1-117">Enter the following data in the data file:</span></span>

| <span data-ttu-id="445a1-118">**Nome da coluna**</span><span class="sxs-lookup"><span data-stu-id="445a1-118">**Column name**</span></span> | <span data-ttu-id="445a1-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="445a1-119">**Description**</span></span>  | <span data-ttu-id="445a1-120">**Limitação**</span><span class="sxs-lookup"><span data-stu-id="445a1-120">**Limitation**</span></span>  |
|:-------- |:------  |:----- |
| <span data-ttu-id="445a1-121">Nome próprio</span><span class="sxs-lookup"><span data-stu-id="445a1-121">First name</span></span>  | <span data-ttu-id="445a1-122">Primeiro nome do utilizador (campo opcional)</span><span class="sxs-lookup"><span data-stu-id="445a1-122">User's first name (optional field)</span></span>  | <span data-ttu-id="445a1-123">Limite de 50 caracteres</span><span class="sxs-lookup"><span data-stu-id="445a1-123">50-character limit</span></span>  |
| <span data-ttu-id="445a1-124">Apelido</span><span class="sxs-lookup"><span data-stu-id="445a1-124">Last name</span></span>  | <span data-ttu-id="445a1-125">Apelido do utilizador (campo opcional)</span><span class="sxs-lookup"><span data-stu-id="445a1-125">User's last name (optional field)</span></span>  | <span data-ttu-id="445a1-126">Limite de 50 caracteres</span><span class="sxs-lookup"><span data-stu-id="445a1-126">50-character limit</span></span>  |
| <span data-ttu-id="445a1-127">Nome a apresentar</span><span class="sxs-lookup"><span data-stu-id="445a1-127">Display name</span></span>    | <span data-ttu-id="445a1-128">Nome exibido no Centro de Parceiros (campo obrigatório)</span><span class="sxs-lookup"><span data-stu-id="445a1-128">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="445a1-129">Limite de 50 caracteres</span><span class="sxs-lookup"><span data-stu-id="445a1-129">50-character limit</span></span>                         |
| <span data-ttu-id="445a1-130">E-mail</span><span class="sxs-lookup"><span data-stu-id="445a1-130">Email</span></span>   | <span data-ttu-id="445a1-131">Endereço de e-mail de negócios do utilizador na empresa de clientes (campo obrigatório)</span><span class="sxs-lookup"><span data-stu-id="445a1-131">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="445a1-132">Cada utilizador deve ter um endereço de e-mail único</span><span class="sxs-lookup"><span data-stu-id="445a1-132">Each user must have a unique email address</span></span> |
| <span data-ttu-id="445a1-133">Atualização de estado</span><span class="sxs-lookup"><span data-stu-id="445a1-133">Status update</span></span>   | <span data-ttu-id="445a1-134">Usado para indicar se o novo registo de utilizadores foi criado com sucesso</span><span class="sxs-lookup"><span data-stu-id="445a1-134">Used to indicate whether the new user record was successfully created</span></span> | <span data-ttu-id="445a1-135">\*\*Deixe vazio\*\*</span><span class="sxs-lookup"><span data-stu-id="445a1-135">\*\*Leave empty\*\*</span></span>                        |

## <a name="next-steps"></a><span data-ttu-id="445a1-136">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="445a1-136">Next steps</span></span>

- [<span data-ttu-id="445a1-137">Como adicionar vários utilizadores para um cliente</span><span class="sxs-lookup"><span data-stu-id="445a1-137">How to add multiple users for a customer</span></span>](adding-multiple-users-to-a-customer-account.md)