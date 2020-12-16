---
title: 'Servizi di trasferimento: spostare tutti i servizi di RDFE in un altro abbonamento'
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004116"
- "7196"
ms.openlocfilehash: d6744484fe42f09f03de562a00fd56712607d418
ms.sourcegitcommit: ec88047d550006a1df4b6f10a3f513218113b9a5
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/15/2020
ms.locfileid: "49681477"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a><span data-ttu-id="87746-102">Servizi di trasferimento: spostare tutti i servizi di RDFE in un altro abbonamento</span><span class="sxs-lookup"><span data-stu-id="87746-102">Transfer Services - Move all RDFE services to another subscription</span></span>

<span data-ttu-id="87746-103">**Spostare risorse**</span><span class="sxs-lookup"><span data-stu-id="87746-103">**Move resources**</span></span>

<span data-ttu-id="87746-104">Le risorse di Azure possono essere spostate in un altro gruppo di risorse o in una sottoscrizione di Azure con la stessa sottoscrizione utilizzando Azure Portal, Azure PowerShell, Azure CLI o l'API REST per spostare le risorse.</span><span class="sxs-lookup"><span data-stu-id="87746-104">Azure resources can be moved to either another Azure subscription or resource group under the same subscription using Azure portal, Azure PowerShell, Azure CLI, or the REST API to move resources.</span></span>

<span data-ttu-id="87746-105">Prima di poter spostare le risorse, vedere:</span><span class="sxs-lookup"><span data-stu-id="87746-105">Before you can move resources, see:</span></span>

- [<span data-ttu-id="87746-106">Elenco di controllo prima di spostare le risorse</span><span class="sxs-lookup"><span data-stu-id="87746-106">Checklist before moving resources</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [<span data-ttu-id="87746-107">Servizi che possono essere spostati</span><span class="sxs-lookup"><span data-stu-id="87746-107">Services that can be moved</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="87746-108">Come convalidare lo spostamento</span><span class="sxs-lookup"><span data-stu-id="87746-108">How to validate the move</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [<span data-ttu-id="87746-109">Spostare le linee guida per i servizi</span><span class="sxs-lookup"><span data-stu-id="87746-109">Move guidance for services</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="87746-110">Per spostare le risorse esistenti in un altro gruppo di risorse o sottoscrizione, è possibile utilizzare:</span><span class="sxs-lookup"><span data-stu-id="87746-110">To move existing resources to another resource group or subscription, you can use:</span></span>

- [<span data-ttu-id="87746-111">Portale di Azure</span><span class="sxs-lookup"><span data-stu-id="87746-111">Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [<span data-ttu-id="87746-112">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="87746-112">Azure PowerShell</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [<span data-ttu-id="87746-113">CLI di Azure</span><span class="sxs-lookup"><span data-stu-id="87746-113">Azure CLI</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [<span data-ttu-id="87746-114">API REST</span><span class="sxs-lookup"><span data-stu-id="87746-114">REST API</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

<span data-ttu-id="87746-115">Esercitazione: [spostare le risorse di Azure in un altro gruppo di risorse o sottoscrizione](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span><span class="sxs-lookup"><span data-stu-id="87746-115">Tutorial: [Move Azure resources to another resource group or subscription](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span></span>

<span data-ttu-id="87746-116">**Risoluzione degli errori di Azure Resource Manager**</span><span class="sxs-lookup"><span data-stu-id="87746-116">**Troubleshoot errors with Azure Resource Manager**</span></span>

<span data-ttu-id="87746-117">Fare riferimento agli articoli riportati di seguito per informazioni sugli errori di distribuzione di Azure comuni e su come ottenere la risoluzione dei problemi.</span><span class="sxs-lookup"><span data-stu-id="87746-117">Refer to the articles below to learn about some common Azure deployment errors and receive information to resolve them.</span></span> <span data-ttu-id="87746-118">Se non è possibile trovare il codice di errore per l'errore di distribuzione, vedere [trovare il codice di errore](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).</span><span class="sxs-lookup"><span data-stu-id="87746-118">If you can't find the error code for your deployment error, see [Find error code](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).</span></span>

- [<span data-ttu-id="87746-119">Risoluzione dei problemi relativi agli errori di distribuzione</span><span class="sxs-lookup"><span data-stu-id="87746-119">Troubleshoot deployment errors</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [<span data-ttu-id="87746-120">Risoluzione dei problemi relativi allo spostamento delle risorse di Azure nel nuovo gruppo di risorse o sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="87746-120">Troubleshoot moving Azure resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

<span data-ttu-id="87746-121">Si noti che, se si desidera aggiornare la sottoscrizione di Azure, ad esempio il passaggio da libero a pay-as-you-go, sarà necessario convertire l'abbonamento.</span><span class="sxs-lookup"><span data-stu-id="87746-121">Note that if you would like to upgrade your Azure subscription, such as switching from free to pay-as-you-go, you will need to convert your subscription.</span></span>

- <span data-ttu-id="87746-122">Per eseguire l'aggiornamento di una versione di valutazione gratuita, vedere [Upgrade Your Free Trial or Microsoft Imagine Azure Subscription to pay-as-you-go](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).</span><span class="sxs-lookup"><span data-stu-id="87746-122">To upgrade a free trial, see [Upgrade your Free Trial or Microsoft Imagine Azure subscription to Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).</span></span>
- <span data-ttu-id="87746-123">Per modificare un account Pay-As-You-Go, vedere [Change Your Azure pay-as-you-go Subscription to an different offer](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).</span><span class="sxs-lookup"><span data-stu-id="87746-123">To change a pay-as-you-go account, see [Change your Azure Pay-As-You-Go subscription to a different offer](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).</span></span>

<span data-ttu-id="87746-124">**Per aggiungere o associare una sottoscrizione di Azure al tenant di Azure Active Directory:**</span><span class="sxs-lookup"><span data-stu-id="87746-124">**To add or associate an Azure subscription to your Azure Active Directory tenant:**</span></span>

1. <span data-ttu-id="87746-125">Accedere e selezionare l'abbonamento che si desidera utilizzare dalla [pagina abbonamenti nel portale di Azure](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).</span><span class="sxs-lookup"><span data-stu-id="87746-125">Sign in and select the subscription you want to use from the [Subscriptions page in Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).</span></span>
2. <span data-ttu-id="87746-126">Selezionare **Cambia directory**.</span><span class="sxs-lookup"><span data-stu-id="87746-126">Select **Change directory**.</span></span>
3. <span data-ttu-id="87746-127">Esaminare gli eventuali avvisi visualizzati e quindi selezionare **Cambia**.</span><span class="sxs-lookup"><span data-stu-id="87746-127">Review any warnings that appear, and then select **Change**.</span></span>
4. <span data-ttu-id="87746-128">La directory viene modificata per la sottoscrizione e verrà visualizzato un messaggio di esito positivo.</span><span class="sxs-lookup"><span data-stu-id="87746-128">The directory is changed for the subscription and you will get a success message.</span></span>
5. <span data-ttu-id="87746-129">Utilizzare la *directory* Switcher per passare alla nuova directory.</span><span class="sxs-lookup"><span data-stu-id="87746-129">Use the *Directory* switcher to go to your new directory.</span></span> <span data-ttu-id="87746-130">Potrebbe essere necessario fino a 10 minuti affinché tutto venga visualizzato correttamente.</span><span class="sxs-lookup"><span data-stu-id="87746-130">It may take up to 10 minutes for everything to show up properly.</span></span>

<span data-ttu-id="87746-131">**Documenti consigliati**</span><span class="sxs-lookup"><span data-stu-id="87746-131">**Recommended Documents**</span></span>

- [<span data-ttu-id="87746-132">Trasferimento della proprietà di una sottoscrizione di Azure</span><span class="sxs-lookup"><span data-stu-id="87746-132">Transferring ownership of an Azure subscription</span></span>](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [<span data-ttu-id="87746-133">Spostare risorse in un nuovo gruppo di risorse o in una sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="87746-133">Move resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [<span data-ttu-id="87746-134">Gestire le risorse mediante il portale di Azure</span><span class="sxs-lookup"><span data-stu-id="87746-134">Manage resources using Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
