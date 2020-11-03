---
title: Reservas Azure & subscrições de servidores
ms.topic: article
ms.date: 08/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Conheça as oportunidades do Cloud Solution Provider para adquirir, providenciar e gerir reservas e subscrições do Azure para os clientes.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3c08e897a8f5d7c11b36627b0c24ad2da3f92329
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/22/2020
ms.locfileid: "92529909"
---
# <a name="acquire-provision--manage-azure-reserved-vm-instances-ri--server-subscriptions-for-customers"></a><span data-ttu-id="6fedb-103">Adquirir, provisão, & gerir Azure reservou vm instâncias (RI) + subscrições de servidores para clientes</span><span class="sxs-lookup"><span data-stu-id="6fedb-103">Acquire, provision, & manage Azure reserved VM instances (RI) + server subscriptions for customers</span></span>

<span data-ttu-id="6fedb-104">Aplica-se a:</span><span class="sxs-lookup"><span data-stu-id="6fedb-104">Applies to:</span></span>

- <span data-ttu-id="6fedb-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="6fedb-105">Partner Center</span></span>

<span data-ttu-id="6fedb-106">**Funções adequadas**</span><span class="sxs-lookup"><span data-stu-id="6fedb-106">**Appropriate roles**</span></span>

- <span data-ttu-id="6fedb-107">Agente administrativo</span><span class="sxs-lookup"><span data-stu-id="6fedb-107">Admin agent</span></span>
- <span data-ttu-id="6fedb-108">Administrador global</span><span class="sxs-lookup"><span data-stu-id="6fedb-108">Global admin</span></span>
- <span data-ttu-id="6fedb-109">Agente helpdesk</span><span class="sxs-lookup"><span data-stu-id="6fedb-109">Helpdesk agent</span></span>
- <span data-ttu-id="6fedb-110">Agente comercial</span><span class="sxs-lookup"><span data-stu-id="6fedb-110">Sales agent</span></span>
- <span data-ttu-id="6fedb-111">Administração de gestão de utilizadores</span><span class="sxs-lookup"><span data-stu-id="6fedb-111">User management admin</span></span>

> [!NOTE]
> <span data-ttu-id="6fedb-112">Este artigo aplica-se apenas aos parceiros do programa Cloud Solution Provider (CSP).</span><span class="sxs-lookup"><span data-stu-id="6fedb-112">This article applies only to partners in the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="6fedb-113">Os clientes que utilizem outros tipos de subscrições (tais como, pay-as-you-go, individual, Microsoft Customer Agreement ou Enterprise Agreement) devem, em vez disso, ler [esta documentação de reservas Azure](/azure/cost-management-billing/reservations).</span><span class="sxs-lookup"><span data-stu-id="6fedb-113">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>


## <a name="what-are-azure-reservations"></a><span data-ttu-id="6fedb-114">O que é o Azure Reservations?</span><span class="sxs-lookup"><span data-stu-id="6fedb-114">What are Azure Reservations?</span></span>

<span data-ttu-id="6fedb-115">As Reservas Azure ajudam-no a economizar dinheiro pré-pagando por um ano ou três anos de máquina virtual, capacidade de computação SQL Database, produção de DB Azure Cosmos ou outros recursos Azure.</span><span class="sxs-lookup"><span data-stu-id="6fedb-115">Azure Reservations help you save money by pre-paying for one-year or three-years of virtual machine, SQL Database compute capacity, Azure Cosmos DB throughput, or other Azure resources.</span></span> <span data-ttu-id="6fedb-116">O pré-pagamento permite-lhe obter um desconto nos recursos que utiliza.</span><span class="sxs-lookup"><span data-stu-id="6fedb-116">Pre-paying allows you to get a discount on the resources you use.</span></span> <span data-ttu-id="6fedb-117">As reservas podem reduzir significativamente a sua máquina virtual, o cálculo da base de dados SQL, o Azure Cosmos DB e outros custos de recursos até 72% em comparação com os preços de pay-as-you-go.</span><span class="sxs-lookup"><span data-stu-id="6fedb-117">Reservations can significantly reduce your virtual machine, SQL database compute, Azure Cosmos DB, and other resource costs up to 72% compared to pay-as-you-go prices.</span></span> <span data-ttu-id="6fedb-118">O Reservations oferece um desconto de faturação e não afeta o estado de atividade dos seus recursos.</span><span class="sxs-lookup"><span data-stu-id="6fedb-118">Reservations provide a billing discount and don't affect the runtime state of your resources.</span></span> <span data-ttu-id="6fedb-119">Para mais informações consulte [o que são Reservas Azure?](/azure/billing/billing-save-compute-costs-reservations)</span><span class="sxs-lookup"><span data-stu-id="6fedb-119">For more information see [What are Azure Reservations?](/azure/billing/billing-save-compute-costs-reservations)</span></span>

## <a name="why-should-customers-buy-a-reservation"></a><span data-ttu-id="6fedb-120">Por que os clientes devem comprar uma reserva?</span><span class="sxs-lookup"><span data-stu-id="6fedb-120">Why should customers buy a reservation?</span></span>

<span data-ttu-id="6fedb-121">Se os clientes tiverem máquinas virtuais, as bases de dados Azure Cosmos DB ou SQL que funcionam por longos períodos de tempo, a compra de uma reserva dá-lhes a opção mais rentável.</span><span class="sxs-lookup"><span data-stu-id="6fedb-121">If customers have virtual machines, Azure Cosmos DB or SQL databases that run for long periods of time, purchasing a reservation gives them the most cost-effective option.</span></span> <span data-ttu-id="6fedb-122">Por exemplo, se um cliente executa continuamente quatro instâncias de um serviço sem reserva, eles são cobrados a taxas de pagamento como você-go.</span><span class="sxs-lookup"><span data-stu-id="6fedb-122">For example, if a customer continuously runs four instances of a service without a reservation, they are charged at pay-as-you-go rates.</span></span> <span data-ttu-id="6fedb-123">Se comprarem uma reserva para esses recursos, recebem imediatamente o desconto de reserva.</span><span class="sxs-lookup"><span data-stu-id="6fedb-123">If they purchase a reservation for those resources, they immediately get the reservation discount.</span></span> <span data-ttu-id="6fedb-124">Deixarão de ser aplicadas taxas pay as you go aos recursos.</span><span class="sxs-lookup"><span data-stu-id="6fedb-124">The resources are no longer charged at the pay-as-you-go rates.</span></span>

### <a name="compelling-new-azure-offer-in-csp"></a><span data-ttu-id="6fedb-125">Oferta convincente do Novo Azure na CSP</span><span class="sxs-lookup"><span data-stu-id="6fedb-125">Compelling New Azure offer in CSP</span></span>

<span data-ttu-id="6fedb-126">Ao trazer reservas e subscrições de servidores do Azure para o seu programa CSP, a Microsoft está a permitir que os seus parceiros abordem a procura rápida de clientes por soluções mais económicas para suportar cargas de trabalho de nuvem altamente previsíveis e persistentes.</span><span class="sxs-lookup"><span data-stu-id="6fedb-126">By bringing Azure Reservations and Server Subscriptions to its CSP program, Microsoft is better enabling its partners to address fast-growing customer demand for more cost-effective solutions to support highly predictable, persistent cloud workloads.</span></span> <span data-ttu-id="6fedb-127">O programa CSP permite que os parceiros adquiram, provisões e gerem subscrições de Reservas e Servidores Azure em nome de clientes comerciais através do Microsoft Partner Center e do portal Azure.</span><span class="sxs-lookup"><span data-stu-id="6fedb-127">The CSP program enables partners to acquire, provision and manage Azure Reservations and Server Subscriptions on behalf of commercial customers via Microsoft Partner Center and Azure portal.</span></span>

<span data-ttu-id="6fedb-128">Até damos aos parceiros do nosso programa CSP escolhas sobre como as reservas do Azure podem ser compradas.</span><span class="sxs-lookup"><span data-stu-id="6fedb-128">We even give partners in our CSP program choices about how Azure reservations can be purchased.</span></span> <span data-ttu-id="6fedb-129">Os parceiros da CSP podem [comprar reservas Azure em nome de um cliente](azure-reservations-buying.md) ou podem permitir que o cliente compre as suas [próprias reservas a](give-customers-permission.md) partir de uma subscrição anterior da Azure que o parceiro adquiriu para eles.</span><span class="sxs-lookup"><span data-stu-id="6fedb-129">CSP partners can [buy Azure reservations on behalf of a customer](azure-reservations-buying.md) or they can [allow the customer to buy their own reservations](give-customers-permission.md) from a prior Azure subscription the partner has purchased for them.</span></span>

<span data-ttu-id="6fedb-130">As Reservas Azure conferem aos clientes a flexibilidade da virtualização para uma vasta gama de soluções de computação, incluindo desenvolvimento e testes, execução de aplicações e alargamento do centro de dados.</span><span class="sxs-lookup"><span data-stu-id="6fedb-130">Azure Reservations give customers the flexibility of virtualization for a wide range of computing solutions, including development and testing, running applications and extending the data center.</span></span>

<span data-ttu-id="6fedb-131">Com [a Azure Reserved VM Instances,](https://azure.microsoft.com/pricing/reserved-vm-instances/) por exemplo, os clientes comerciais podem agora economizar até 72% em relação ao preço de VM pay-as-you-go simplesmente comprando - ou "reservando" - a máquina virtual por um período de 1 ou 3 anos.</span><span class="sxs-lookup"><span data-stu-id="6fedb-131">With [Azure Reserved VM Instances](https://azure.microsoft.com/pricing/reserved-vm-instances/) for example, commercial customers can now save up to 72% versus pay-as-you-go Azure VM pricing simply by purchasing - or "reserving" - the virtual machine for a 1- or 3-year period.</span></span> <span data-ttu-id="6fedb-132">Os clientes do Windows Server com Benefício Híbrido Azure, incluídos na Software Assurance, poderão economizar até 80% em relação aos preços de pay-as-you-go.</span><span class="sxs-lookup"><span data-stu-id="6fedb-132">Windows Server customers with Azure Hybrid Benefit, included with Software Assurance, will be able to save up to 80% versus pay-as-you-go pricing.</span></span>

<span data-ttu-id="6fedb-133">Com uma combinação incomparável de preços convincentes e flexibilidade de implementação incomparável, os clientes verão o melhor valor global quando escolherem reservas Azure:</span><span class="sxs-lookup"><span data-stu-id="6fedb-133">With an unmatched combination of compelling pricing and unmatched deployment flexibility, customers will see the best overall value when they choose Azure Reservations:</span></span>

#### <a name="azure-reservations"></a><span data-ttu-id="6fedb-134">Reservas do Azure</span><span class="sxs-lookup"><span data-stu-id="6fedb-134">Azure reservations</span></span>

- <span data-ttu-id="6fedb-135">Azure Reservado VM Instances</span><span class="sxs-lookup"><span data-stu-id="6fedb-135">Azure Reserved VM Instances</span></span>
- <span data-ttu-id="6fedb-136">Reservas SQL DB</span><span class="sxs-lookup"><span data-stu-id="6fedb-136">SQL DB Reservations</span></span>
- <span data-ttu-id="6fedb-137">Instância Gerida do SQL</span><span class="sxs-lookup"><span data-stu-id="6fedb-137">SQL Managed Instance</span></span>
- <span data-ttu-id="6fedb-138">Azure Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="6fedb-138">Azure Cosmos DB</span></span>
- <span data-ttu-id="6fedb-139">Azure SQL Data Warehouse</span><span class="sxs-lookup"><span data-stu-id="6fedb-139">Azure SQL Data Warehouse</span></span>
- <span data-ttu-id="6fedb-140">Serviços Aplicacionais</span><span class="sxs-lookup"><span data-stu-id="6fedb-140">App Services</span></span>
- <span data-ttu-id="6fedb-141">Reservas da unidade Azure Databricks</span><span class="sxs-lookup"><span data-stu-id="6fedb-141">Azure Databricks unit reservations</span></span>
- <span data-ttu-id="6fedb-142">Disco Gerido</span><span class="sxs-lookup"><span data-stu-id="6fedb-142">Managed Disk</span></span>
- <span data-ttu-id="6fedb-143">Blob de blocos</span><span class="sxs-lookup"><span data-stu-id="6fedb-143">Block blob</span></span>
- <span data-ttu-id="6fedb-144">MySQL</span><span class="sxs-lookup"><span data-stu-id="6fedb-144">MySQL</span></span>
- <span data-ttu-id="6fedb-145">Explorador de dados Azure</span><span class="sxs-lookup"><span data-stu-id="6fedb-145">Azure Data explorer</span></span>
- <span data-ttu-id="6fedb-146">MariaDB</span><span class="sxs-lookup"><span data-stu-id="6fedb-146">MariaDB</span></span>
- <span data-ttu-id="6fedb-147">PostgreSQL</span><span class="sxs-lookup"><span data-stu-id="6fedb-147">PostgreSQL</span></span>

#### <a name="server-subscriptions"></a><span data-ttu-id="6fedb-148">Assinaturas de servidor</span><span class="sxs-lookup"><span data-stu-id="6fedb-148">Server subscriptions</span></span>

- <span data-ttu-id="6fedb-149">Windows Server</span><span class="sxs-lookup"><span data-stu-id="6fedb-149">Windows Server</span></span>
- <span data-ttu-id="6fedb-150">CaLs de Serviços remotos de Desktop (RDS)</span><span class="sxs-lookup"><span data-stu-id="6fedb-150">Remote Desktop Services (RDS) CALs</span></span>
- <span data-ttu-id="6fedb-151">SQL Server</span><span class="sxs-lookup"><span data-stu-id="6fedb-151">SQL Server</span></span>

#### <a name="linux-isv-annual-subscriptions"></a><span data-ttu-id="6fedb-152">Assinaturas anuais do Linux ISV</span><span class="sxs-lookup"><span data-stu-id="6fedb-152">Linux ISV annual subscriptions</span></span>

- <span data-ttu-id="6fedb-153">SUSE Linux</span><span class="sxs-lookup"><span data-stu-id="6fedb-153">SUSE Linux</span></span>
- <span data-ttu-id="6fedb-154">Red Hat Enterprise Linux</span><span class="sxs-lookup"><span data-stu-id="6fedb-154">Red Hat Enterprise Linux</span></span>
- <span data-ttu-id="6fedb-155">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="6fedb-155">Azure Red Hat OpenShift</span></span>

#### <a name="isv-annual-subscriptions"></a><span data-ttu-id="6fedb-156">Assinaturas anuais do ISV</span><span class="sxs-lookup"><span data-stu-id="6fedb-156">ISV annual subscriptions</span></span>

- <span data-ttu-id="6fedb-157">Azure VMware Solution by CloudSimple</span><span class="sxs-lookup"><span data-stu-id="6fedb-157">Azure VMware Solution by CloudSimple</span></span>

## <a name="getting-started"></a><span data-ttu-id="6fedb-158">Introdução</span><span class="sxs-lookup"><span data-stu-id="6fedb-158">Getting started</span></span>

<span data-ttu-id="6fedb-159">Para entender como pode posicionar reservas do Azure com os seus clientes e levantar-se e funcionar operacionalmente o mais rapidamente possível, recomendamos a seguinte abordagem para rever os materiais de prontidão:</span><span class="sxs-lookup"><span data-stu-id="6fedb-159">To understand how you can position Azure Reservations with your customers and get up and running operationally as quickly as possible, we recommend the following approach to review the readiness materials:</span></span>

1. <span data-ttu-id="6fedb-160">Reveja as apresentações de visão geral e webinars associados para a proposta de valor do cliente e posicionamento</span><span class="sxs-lookup"><span data-stu-id="6fedb-160">Review the Overview Presentations and associated webinars for the customer value proposition and positioning</span></span>
2. <span data-ttu-id="6fedb-161">Reveja e compreenda o Guia Operacional do Comércio Moderno</span><span class="sxs-lookup"><span data-stu-id="6fedb-161">Review and understand the Modern Commerce Operating Guide</span></span>
3. <span data-ttu-id="6fedb-162">Reveja as subscrições do Azure RI e do Servidor FAQ</span><span class="sxs-lookup"><span data-stu-id="6fedb-162">Review the Azure RI and Server Subscriptions FAQ</span></span>
4. <span data-ttu-id="6fedb-163">Compreender atualizações para Reservas Azure e Subscrições de Servidor na API do [Centro Parceiro (API/SDK)](/partner-center/develop/purchase-azure-reserved-vm-instances)</span><span class="sxs-lookup"><span data-stu-id="6fedb-163">Understand updates for Azure Reservations and Server Subscriptions in the [Partner Center API (API/SDK)](/partner-center/develop/purchase-azure-reserved-vm-instances)</span></span>

## <a name="resources"></a><span data-ttu-id="6fedb-164">Recursos</span><span class="sxs-lookup"><span data-stu-id="6fedb-164">Resources</span></span>

<span data-ttu-id="6fedb-165">Abaixo está uma lista completa de recursos para ajudá-lo a bordo rapidamente para transar Reservas Azure através do Partner Center:</span><span class="sxs-lookup"><span data-stu-id="6fedb-165">Below is a comprehensive list of resources to help you onboard quickly to transacting Azure Reservations through Partner Center:</span></span>

### <a name="sales-readiness"></a><span data-ttu-id="6fedb-166">Prontidão de vendas</span><span class="sxs-lookup"><span data-stu-id="6fedb-166">Sales readiness</span></span>

- [<span data-ttu-id="6fedb-167">Reservas Azure e Subscrições de servidor com visão geral do benefício híbrido Azure</span><span class="sxs-lookup"><span data-stu-id="6fedb-167">Azure Reservations and Server Subscriptions with Azure Hybrid Benefit Overview</span></span>](https://assetsprod.microsoft.com/Azure-reservations-and-server-subscriptions-with-azure-hybrid-benefit.pptx)
- [<span data-ttu-id="6fedb-168">Folha de Vendas</span><span class="sxs-lookup"><span data-stu-id="6fedb-168">Sales Sheet</span></span>](https://assetsprod.microsoft.com/mpn/Azure-RI-Sales-Sheet-CSP.pdf)
- [<span data-ttu-id="6fedb-169">FaQ parceiro para reservas Azure</span><span class="sxs-lookup"><span data-stu-id="6fedb-169">Partner FAQ for Azure Reservations</span></span>](https://assetsprod.microsoft.com/Partner-faq-for-azure-reservations.docx)
- [<span data-ttu-id="6fedb-170">FaQ parceiro para reservas Azure e SQL DB</span><span class="sxs-lookup"><span data-stu-id="6fedb-170">Partner FAQ for Azure Reservations and SQL DB</span></span>](https://assetsprod.microsoft.com/Partner-faq-for-azure-reservations-sql-db.docx)
- [<span data-ttu-id="6fedb-171">Licença de Acesso ao Cliente (RDS) (anúncio)</span><span class="sxs-lookup"><span data-stu-id="6fedb-171">Remote Desktop Services (RDS) Client Access License (CAL) (announcement)</span></span>](https://cloudblogs.microsoft.com/windowsserver/2018/10/03/remote-desktop-services-2019-generally-available-with-windows-server-2019/)
- [<span data-ttu-id="6fedb-172">Azure Reservado VM Instances (portal Azure)</span><span class="sxs-lookup"><span data-stu-id="6fedb-172">Azure Reserved VM Instances (Azure portal)</span></span>](/azure/virtual-machines/windows/prepay-reserved-vm-instances)
- [<span data-ttu-id="6fedb-173">Subscrições de servidores</span><span class="sxs-lookup"><span data-stu-id="6fedb-173">Server Subscriptions</span></span>](csp-software-subscriptions.md)
- [<span data-ttu-id="6fedb-174">SQL DB em Visão Geral do Azure</span><span class="sxs-lookup"><span data-stu-id="6fedb-174">SQL DB in Azure Overview</span></span>](https://assetsprod.microsoft.com/Sql-db-in-azure-overview.pptx)
- [<span data-ttu-id="6fedb-175">Reservas DE DB SQL (portal Azure)</span><span class="sxs-lookup"><span data-stu-id="6fedb-175">SQL DB Reservations (Azure portal)</span></span>](/azure/sql-database/sql-database-reserved-capacity)
- [<span data-ttu-id="6fedb-176">Azure Cosmos DB (portal Azure)</span><span class="sxs-lookup"><span data-stu-id="6fedb-176">Azure Cosmos DB (Azure portal)</span></span>](/azure/cosmos-db/cosmos-db-reserved-capacity)
- [<span data-ttu-id="6fedb-177">SQL Managed Instance (portal Azure)</span><span class="sxs-lookup"><span data-stu-id="6fedb-177">SQL Managed Instance (Azure portal)</span></span>](/azure/sql-database/sql-database-managed-instance)
- [<span data-ttu-id="6fedb-178">SUSE e Red Hat Enterprise Linux (portal Azure)</span><span class="sxs-lookup"><span data-stu-id="6fedb-178">SUSE and Red Hat Enterprise Linux (Azure portal)</span></span>](/azure/virtual-machines/linux/prepay-suse-software-charges)
- [<span data-ttu-id="6fedb-179">Chapéu Vermelho Linux em Azure</span><span class="sxs-lookup"><span data-stu-id="6fedb-179">Red Hat Linux on Azure</span></span>](https://azure.com/redhat)
- [<span data-ttu-id="6fedb-180">SUSE Linux em Azure</span><span class="sxs-lookup"><span data-stu-id="6fedb-180">SUSE Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/suse/)
- [<span data-ttu-id="6fedb-181">Linux no Azure</span><span class="sxs-lookup"><span data-stu-id="6fedb-181">Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/)
- [<span data-ttu-id="6fedb-182">Visão geral dos preços do Azure</span><span class="sxs-lookup"><span data-stu-id="6fedb-182">Azure Pricing Overview</span></span>](https://azure.microsoft.com/pricing/)
- [<span data-ttu-id="6fedb-183">Calculadora de Preços de Azure</span><span class="sxs-lookup"><span data-stu-id="6fedb-183">Azure Pricing Calculator</span></span>](https://azure.microsoft.com/pricing/calculator)
- [<span data-ttu-id="6fedb-184">Reservas da unidade Azure Databricks</span><span class="sxs-lookup"><span data-stu-id="6fedb-184">Azure Databricks unit reservations</span></span>](/azure/billing/billing-prepay-databricks-reserved-capacity)
- <span data-ttu-id="6fedb-185">Listas de preços da CSP: As listas de preços **das assinaturas de** subscrições de software estão ambas **localizadas** na página de preços do Centro de [Parceiros & Ofertas.](https://partner.microsoft.com/pcv/sales)</span><span class="sxs-lookup"><span data-stu-id="6fedb-185">CSP Price lists:  The **Microsoft Azure Reserved Instances** and **Software Subscriptions** price lists are both located on the Partner Center [Pricing & Offers](https://partner.microsoft.com/pcv/sales) page.</span></span>

### <a name="training"></a><span data-ttu-id="6fedb-186">Formação</span><span class="sxs-lookup"><span data-stu-id="6fedb-186">Training</span></span>

<span data-ttu-id="6fedb-187">Registe-se para ver [webinars](https://commercial-licensing.eventbuilder.com/FY2019_ALL) de prontidão de licenciamento comercial e eventos a pedido.</span><span class="sxs-lookup"><span data-stu-id="6fedb-187">Register to view [Commercial Licensing Readiness webinars](https://commercial-licensing.eventbuilder.com/FY2019_ALL) and on-demand events.</span></span>

<span data-ttu-id="6fedb-188">Os eventos de prontidão de licenciamento a pedido incluem tópicos como:</span><span class="sxs-lookup"><span data-stu-id="6fedb-188">Licensing Readiness on-demand events include topics like:</span></span>

- <span data-ttu-id="6fedb-189">CSP Online Services, CSP Azure e atualizações gerais de licenciamento, incluindo Azure (novembro de 2018)</span><span class="sxs-lookup"><span data-stu-id="6fedb-189">CSP Online Services, CSP Azure, and general licensing updates, including Azure (November 2018)</span></span>
- <span data-ttu-id="6fedb-190">SQL DB Capacidade Reservada & Flexibilidade do Tamanho da Instância (agosto de 2018)</span><span class="sxs-lookup"><span data-stu-id="6fedb-190">SQL DB Reserved Capacity & Instance Size Flexibility (August 2018)</span></span>
- <span data-ttu-id="6fedb-191">Subscrições de servidores em CSP (julho de 2018)</span><span class="sxs-lookup"><span data-stu-id="6fedb-191">Server Subscriptions in CSP (July 2018)</span></span>
- <span data-ttu-id="6fedb-192">Visão geral das reservas do Azure em CSP (maio de 2018)</span><span class="sxs-lookup"><span data-stu-id="6fedb-192">Azure Reservations Overview in CSP (May 2018)</span></span>

<span data-ttu-id="6fedb-193">Outra formação útil inclui o [Módulo de Licenciamento Azure na Universidade Parceira.](https://aka.ms/azure_partner_licensing)</span><span class="sxs-lookup"><span data-stu-id="6fedb-193">Other useful training includes the [Azure Licensing Module on Partner University](https://aka.ms/azure_partner_licensing).</span></span>

### <a name="operations"></a><span data-ttu-id="6fedb-194">Operações</span><span class="sxs-lookup"><span data-stu-id="6fedb-194">Operations</span></span>

- <span data-ttu-id="6fedb-195">[Guia de Operações de Comércio Moderno](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx) (atualizado): Um guia abrangente que abrange a política chave e aspetos operacionais tais como acordos, encomenda através do Partner Center, fatura, detalhes da lista de preços, incentivos, ficheiro de reconciliação, API/SDK, Sandbox e Azure Partner Shared Services.</span><span class="sxs-lookup"><span data-stu-id="6fedb-195">[Modern Commerce Operations Guide](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx) (updated):  A comprehensive guide covering key policy and operational aspects such as agreements, ordering through Partner Center, invoice, price list details, incentives, reconciliation file, API/SDK, Sandbox, and Azure Partner Shared Services.</span></span>
- [<span data-ttu-id="6fedb-196">Ofertas Modernas Disponibilidade de País e Matriz de Moeda do Cliente</span><span class="sxs-lookup"><span data-stu-id="6fedb-196">Modern Offers Country Availability and Customer Currency Matrix</span></span>](https://assetsprod.microsoft.com/modern-offers-country-currency-availability.xlsx)
- [<span data-ttu-id="6fedb-197">Vender Instâncias Reservadas microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="6fedb-197">Sell Microsoft Azure Reserved Instances</span></span>](azure-reservations.md)
- [<span data-ttu-id="6fedb-198">Compre reservas da Microsoft Azure em nome dos seus clientes</span><span class="sxs-lookup"><span data-stu-id="6fedb-198">Buy Microsoft Azure reservations on behalf of your customers</span></span>](azure-reservations-buying.md)
- [<span data-ttu-id="6fedb-199">Gerir reservas da Azure em nome dos seus clientes</span><span class="sxs-lookup"><span data-stu-id="6fedb-199">Manage Azure reservations on behalf of your customers</span></span>](azure-reservations-manage.md)
- [<span data-ttu-id="6fedb-200">Faturação para reservas de Azure</span><span class="sxs-lookup"><span data-stu-id="6fedb-200">Billing for Azure reservations</span></span>](azure-plan-billing.md)
- [<span data-ttu-id="6fedb-201">Tamanho VM para utilização máxima da reserva</span><span class="sxs-lookup"><span data-stu-id="6fedb-201">VM sizing for maximum reservation usage</span></span>](azure-usage.md)
- [<span data-ttu-id="6fedb-202">Parceiro Centro API (API/SDK)</span><span class="sxs-lookup"><span data-stu-id="6fedb-202">Partner Center API (API/SDK)</span></span>](/partner-center/develop/purchase-azure-reserved-vm-instances)
- [<span data-ttu-id="6fedb-203">Serviços de Ambiente de Trabalho Remoto</span><span class="sxs-lookup"><span data-stu-id="6fedb-203">Remote Desktop Services</span></span>](/windows-server/remote/remote-desktop-services/welcome-to-rds)

## <a name="azure-hybrid-benefit"></a><span data-ttu-id="6fedb-204">Benefício Híbrido do Azure</span><span class="sxs-lookup"><span data-stu-id="6fedb-204">Azure Hybrid Benefit</span></span>

<span data-ttu-id="6fedb-205">O [Azure Hybrid Benefit](https://azure.microsoft.com/pricing/hybrid-benefit) ajuda-o a obter mais valor das suas licenças do Windows Server e a economizar até \*47% em máquinas virtuais.</span><span class="sxs-lookup"><span data-stu-id="6fedb-205">The [Azure Hybrid Benefit](https://azure.microsoft.com/pricing/hybrid-benefit) helps you get more value from your Windows Server licenses and save up to \*47 percent on virtual machines.</span></span> <span data-ttu-id="6fedb-206">Pode utilizar o benefício com licenças de datacenter do Windows Server e standard edition cobertas com a Software Assurance.</span><span class="sxs-lookup"><span data-stu-id="6fedb-206">You can use the benefit with Windows Server Datacenter and Standard edition licenses covered with Software Assurance.</span></span> <span data-ttu-id="6fedb-207">Dependendo da edição, pode converter ou reutilizar as suas licenças para executar máquinas virtuais do Windows Server em Azure e pagar uma taxa de computação base mais baixa (taxas de máquina virtual Linux).</span><span class="sxs-lookup"><span data-stu-id="6fedb-207">Depending on the edition, you can convert or reuse your licenses to run Windows Server virtual machines in Azure and pay a lower base compute rate (Linux virtual machine rates).</span></span>

<span data-ttu-id="6fedb-208">Ver também [Azure Hybrid Benefit FAQ](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)</span><span class="sxs-lookup"><span data-stu-id="6fedb-208">See also [Azure Hybrid Benefit FAQ](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)</span></span>

<span data-ttu-id="6fedb-209">\*As poupanças reais podem variar em função da região, do tipo de instância ou da utilização.</span><span class="sxs-lookup"><span data-stu-id="6fedb-209">\*Actual savings may vary based on region, instance type, or usage.</span></span>
