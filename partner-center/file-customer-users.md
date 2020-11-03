---
title: Campos para ficheiro .csv para importar vários utilizadores para uma conta de cliente
ms.topic: article
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Para adicionar vários utilizadores a uma conta de cliente, crie um ficheiro de valor separado em vírgula (.csv) com campos apropriados.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 07a28e5310716f3df11caa36e51339e877e65627
ms.sourcegitcommit: 7e19c211b1d5f2db2a4c56a743b14c8485decd99
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/03/2020
ms.locfileid: "92529432"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a><span data-ttu-id="ec464-103">Adicione vários utilizadores a uma conta de cliente criando um ficheiro .csv</span><span class="sxs-lookup"><span data-stu-id="ec464-103">Add multiple users to a customer account by creating a .csv file</span></span>

<span data-ttu-id="ec464-104">**Aplica-se a**</span><span class="sxs-lookup"><span data-stu-id="ec464-104">**Applies to**</span></span>

- <span data-ttu-id="ec464-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="ec464-105">Partner Center</span></span>

<span data-ttu-id="ec464-106">**Funções adequadas**</span><span class="sxs-lookup"><span data-stu-id="ec464-106">**Appropriate roles**</span></span>

- <span data-ttu-id="ec464-107">Administrador global</span><span class="sxs-lookup"><span data-stu-id="ec464-107">Global admin</span></span>

<span data-ttu-id="ec464-108">Adicione vários utilizadores à conta de um cliente de uma só vez, enviando um ficheiro de dados no formato de ficheiro de valor separado em vírgula (.csv) para o Centro de Parceiros.</span><span class="sxs-lookup"><span data-stu-id="ec464-108">Add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="ec464-109">Pode descarregar um ficheiro de dados de amostra do Centro de Parceiros e depois editá-lo para a sua utilização, ou pode criar um novo ficheiro de dados utilizando o modelo de dados definido abaixo.</span><span class="sxs-lookup"><span data-stu-id="ec464-109">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="ec464-110">Requisitos de ficheiros de dados</span><span class="sxs-lookup"><span data-stu-id="ec464-110">Data file requirements</span></span>

<span data-ttu-id="ec464-111">Para adicionar vários utilizadores à conta de um cliente utilizando o processo de upload em massa, terá de cumprir os seguintes requisitos:</span><span class="sxs-lookup"><span data-stu-id="ec464-111">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

- <span data-ttu-id="ec464-112">Tem de ter permissões globais de administrador na conta do cliente;</span><span class="sxs-lookup"><span data-stu-id="ec464-112">You must have global administrator permissions to the customer account;</span></span>
- <span data-ttu-id="ec464-113">Cada utilizador deve ter um endereço de e-mail único, anexado ao domínio de e-mail do cliente;</span><span class="sxs-lookup"><span data-stu-id="ec464-113">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
- <span data-ttu-id="ec464-114">Pode carregar até 100 discos de cada vez.</span><span class="sxs-lookup"><span data-stu-id="ec464-114">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="ec464-115">Se precisar de adicionar mais de 100 utilizadores, crie e carre faça upload de ficheiros de dados adicionais.</span><span class="sxs-lookup"><span data-stu-id="ec464-115">If you need to add more than 100 users, create and upload additional data files.</span></span>
- <span data-ttu-id="ec464-116">Todos os utilizadores devem estar na mesma **Localização** Geográfica.</span><span class="sxs-lookup"><span data-stu-id="ec464-116">All users must be in the same geographic **Location** .</span></span>
- <span data-ttu-id="ec464-117">Introduza apenas os dados descritos abaixo.</span><span class="sxs-lookup"><span data-stu-id="ec464-117">Enter only the data described below.</span></span> <span data-ttu-id="ec464-118">Dados extraéssis farão com que o upload falhe.</span><span class="sxs-lookup"><span data-stu-id="ec464-118">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="ec464-119">Introduza os seguintes dados no ficheiro de dados:</span><span class="sxs-lookup"><span data-stu-id="ec464-119">Enter the following data in the data file:</span></span>

| <span data-ttu-id="ec464-120">**Nome da coluna**</span><span class="sxs-lookup"><span data-stu-id="ec464-120">**Column name**</span></span> | <span data-ttu-id="ec464-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ec464-121">**Description**</span></span>  | <span data-ttu-id="ec464-122">**Limitação**</span><span class="sxs-lookup"><span data-stu-id="ec464-122">**Limitation**</span></span>  |
|:-------- |:------  |:----- |
| <span data-ttu-id="ec464-123">Nome próprio</span><span class="sxs-lookup"><span data-stu-id="ec464-123">First name</span></span>  | <span data-ttu-id="ec464-124">Primeiro nome do utilizador (campo opcional)</span><span class="sxs-lookup"><span data-stu-id="ec464-124">User's first name (optional field)</span></span>  | <span data-ttu-id="ec464-125">Limite de 50 caracteres</span><span class="sxs-lookup"><span data-stu-id="ec464-125">50-character limit</span></span>  |
| <span data-ttu-id="ec464-126">Apelido</span><span class="sxs-lookup"><span data-stu-id="ec464-126">Last name</span></span>  | <span data-ttu-id="ec464-127">Apelido do utilizador (campo opcional)</span><span class="sxs-lookup"><span data-stu-id="ec464-127">User's last name (optional field)</span></span>  | <span data-ttu-id="ec464-128">Limite de 50 caracteres</span><span class="sxs-lookup"><span data-stu-id="ec464-128">50-character limit</span></span>  |
| <span data-ttu-id="ec464-129">Nome a apresentar</span><span class="sxs-lookup"><span data-stu-id="ec464-129">Display name</span></span>    | <span data-ttu-id="ec464-130">Nome exibido no Centro de Parceiros (campo obrigatório)</span><span class="sxs-lookup"><span data-stu-id="ec464-130">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="ec464-131">Limite de 50 caracteres</span><span class="sxs-lookup"><span data-stu-id="ec464-131">50-character limit</span></span>                         |
| <span data-ttu-id="ec464-132">E-mail</span><span class="sxs-lookup"><span data-stu-id="ec464-132">Email</span></span>   | <span data-ttu-id="ec464-133">Endereço de e-mail de negócios do utilizador na empresa de clientes (campo obrigatório)</span><span class="sxs-lookup"><span data-stu-id="ec464-133">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="ec464-134">Cada utilizador deve ter um endereço de e-mail único</span><span class="sxs-lookup"><span data-stu-id="ec464-134">Each user must have a unique email address</span></span> |
| <span data-ttu-id="ec464-135">Atualização de estado</span><span class="sxs-lookup"><span data-stu-id="ec464-135">Status update</span></span>   | <span data-ttu-id="ec464-136">Usado para indicar se o novo registo de utilizadores foi criado com sucesso</span><span class="sxs-lookup"><span data-stu-id="ec464-136">Used to indicate whether or not the new user record was successfully created</span></span> | <span data-ttu-id="ec464-137">\*\*Deixe vazio\*\*</span><span class="sxs-lookup"><span data-stu-id="ec464-137">\*\*Leave empty\*\*</span></span>                        |

## <a name="next-steps"></a><span data-ttu-id="ec464-138">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="ec464-138">Next steps</span></span>

- [<span data-ttu-id="ec464-139">Como adicionar vários utilizadores para um cliente</span><span class="sxs-lookup"><span data-stu-id="ec464-139">How to add multiple users for a customer</span></span>](adding-multiple-users-to-a-customer-account.md)