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
ms.openlocfilehash: 152daadde25a9325937797f7a3daa90dfb59a9b4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150986"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a><span data-ttu-id="e9598-103">Adicionar vários utilizadores a uma conta de cliente criando um ficheiro .csv</span><span class="sxs-lookup"><span data-stu-id="e9598-103">Add multiple users to a customer account by creating a .csv file</span></span>

<span data-ttu-id="e9598-104">**Funções apropriadas**: Administração global</span><span class="sxs-lookup"><span data-stu-id="e9598-104">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="e9598-105">Adicione vários utilizadores à conta de um cliente de uma só vez, enviando um ficheiro de dados no formato de ficheiro de valor separado em vírgula (.csv) para o Centro de Parceiros.</span><span class="sxs-lookup"><span data-stu-id="e9598-105">Add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="e9598-106">Pode descarregar um ficheiro de dados de amostra do Centro de Parceiros e depois editá-lo para a sua utilização, ou pode criar um novo ficheiro de dados utilizando o modelo de dados definido abaixo.</span><span class="sxs-lookup"><span data-stu-id="e9598-106">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="e9598-107">Requisitos de ficheiros de dados</span><span class="sxs-lookup"><span data-stu-id="e9598-107">Data file requirements</span></span>

<span data-ttu-id="e9598-108">Para adicionar vários utilizadores à conta de um cliente utilizando o processo de upload em massa, terá de cumprir os seguintes requisitos:</span><span class="sxs-lookup"><span data-stu-id="e9598-108">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

- <span data-ttu-id="e9598-109">Tem de ter permissões globais de administrador na conta do cliente;</span><span class="sxs-lookup"><span data-stu-id="e9598-109">You must have global administrator permissions to the customer account;</span></span>
- <span data-ttu-id="e9598-110">Cada utilizador deve ter um endereço de e-mail único, anexado ao domínio de e-mail do cliente;</span><span class="sxs-lookup"><span data-stu-id="e9598-110">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
- <span data-ttu-id="e9598-111">Pode carregar até 100 discos de cada vez.</span><span class="sxs-lookup"><span data-stu-id="e9598-111">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="e9598-112">Se precisar de adicionar mais de 100 utilizadores, crie e carre faça upload de ficheiros de dados adicionais.</span><span class="sxs-lookup"><span data-stu-id="e9598-112">If you need to add more than 100 users, create and upload additional data files.</span></span>
- <span data-ttu-id="e9598-113">Todos os utilizadores devem estar na mesma **Localização** Geográfica.</span><span class="sxs-lookup"><span data-stu-id="e9598-113">All users must be in the same geographic **Location**.</span></span>
- <span data-ttu-id="e9598-114">Introduza apenas os dados descritos abaixo.</span><span class="sxs-lookup"><span data-stu-id="e9598-114">Enter only the data described below.</span></span> <span data-ttu-id="e9598-115">Dados extraéssis farão com que o upload falhe.</span><span class="sxs-lookup"><span data-stu-id="e9598-115">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="e9598-116">Introduza os seguintes dados no ficheiro de dados:</span><span class="sxs-lookup"><span data-stu-id="e9598-116">Enter the following data in the data file:</span></span>

| <span data-ttu-id="e9598-117">**Nome da coluna**</span><span class="sxs-lookup"><span data-stu-id="e9598-117">**Column name**</span></span> | <span data-ttu-id="e9598-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e9598-118">**Description**</span></span>  | <span data-ttu-id="e9598-119">**Limitação**</span><span class="sxs-lookup"><span data-stu-id="e9598-119">**Limitation**</span></span>  |
|:-------- |:------  |:----- |
| <span data-ttu-id="e9598-120">Nome próprio</span><span class="sxs-lookup"><span data-stu-id="e9598-120">First name</span></span>  | <span data-ttu-id="e9598-121">Primeiro nome do utilizador (campo opcional)</span><span class="sxs-lookup"><span data-stu-id="e9598-121">User's first name (optional field)</span></span>  | <span data-ttu-id="e9598-122">Limite de 50 caracteres</span><span class="sxs-lookup"><span data-stu-id="e9598-122">50-character limit</span></span>  |
| <span data-ttu-id="e9598-123">Apelido</span><span class="sxs-lookup"><span data-stu-id="e9598-123">Last name</span></span>  | <span data-ttu-id="e9598-124">Apelido do utilizador (campo opcional)</span><span class="sxs-lookup"><span data-stu-id="e9598-124">User's last name (optional field)</span></span>  | <span data-ttu-id="e9598-125">Limite de 50 caracteres</span><span class="sxs-lookup"><span data-stu-id="e9598-125">50-character limit</span></span>  |
| <span data-ttu-id="e9598-126">Nome a apresentar</span><span class="sxs-lookup"><span data-stu-id="e9598-126">Display name</span></span>    | <span data-ttu-id="e9598-127">Nome exibido no Centro de Parceiros (campo obrigatório)</span><span class="sxs-lookup"><span data-stu-id="e9598-127">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="e9598-128">Limite de 50 caracteres</span><span class="sxs-lookup"><span data-stu-id="e9598-128">50-character limit</span></span>                         |
| <span data-ttu-id="e9598-129">E-mail</span><span class="sxs-lookup"><span data-stu-id="e9598-129">Email</span></span>   | <span data-ttu-id="e9598-130">Endereço de e-mail de negócios do utilizador na empresa de clientes (campo obrigatório)</span><span class="sxs-lookup"><span data-stu-id="e9598-130">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="e9598-131">Cada utilizador deve ter um endereço de e-mail único</span><span class="sxs-lookup"><span data-stu-id="e9598-131">Each user must have a unique email address</span></span> |
| <span data-ttu-id="e9598-132">Atualização de estado</span><span class="sxs-lookup"><span data-stu-id="e9598-132">Status update</span></span>   | <span data-ttu-id="e9598-133">Usado para indicar se o novo registo de utilizadores foi criado com sucesso</span><span class="sxs-lookup"><span data-stu-id="e9598-133">Used to indicate whether the new user record was successfully created</span></span> | <span data-ttu-id="e9598-134">\*\*Deixe vazio\*\*</span><span class="sxs-lookup"><span data-stu-id="e9598-134">\*\*Leave empty\*\*</span></span>                        |

## <a name="next-steps"></a><span data-ttu-id="e9598-135">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="e9598-135">Next steps</span></span>

- [<span data-ttu-id="e9598-136">Como adicionar vários utilizadores para um cliente</span><span class="sxs-lookup"><span data-stu-id="e9598-136">How to add multiple users for a customer</span></span>](adding-multiple-users-to-a-customer-account.md)