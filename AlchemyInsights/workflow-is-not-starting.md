---
title: Flusso di lavoro non avviato
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: e69f3e529e4a2202f641cb62f42b1a20d774a398
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403747"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="8ac9c-102">Flusso di lavoro non avviato</span><span class="sxs-lookup"><span data-stu-id="8ac9c-102">Workflow is not starting</span></span>

- <span data-ttu-id="8ac9c-103">I flussi di lavoro di SharePoint 2010 e SharePoint 2013 non vengono avviati.</span><span class="sxs-lookup"><span data-stu-id="8ac9c-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="8ac9c-104">Se il flusso di lavoro non viene avviato, potrebbe verificarsi un problema temporaneo del servizio in cui gli utenti potrebbero subire ritardi intermittenti con l'avanzamento del flusso di lavoro.</span><span class="sxs-lookup"><span data-stu-id="8ac9c-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="8ac9c-105">Controllare il [dashboard di integrità del](https://admin.microsoft.com/AdminPortal/Home/servicehealth) servizio per verificare se l'organizzazione è influenzata.</span><span class="sxs-lookup"><span data-stu-id="8ac9c-105">Check the [Service Health Dashboard](https://admin.microsoft.com/AdminPortal/Home/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="8ac9c-106">Se sono trascorse più di 24 ore dalla prima volta che hai visto questo problema, registra un ticket di supporto.</span><span class="sxs-lookup"><span data-stu-id="8ac9c-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="8ac9c-107">In molti casi, stiamo già lavorando a una soluzione.</span><span class="sxs-lookup"><span data-stu-id="8ac9c-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="8ac9c-108">Fornire almeno 24 ore per completare una soluzione.</span><span class="sxs-lookup"><span data-stu-id="8ac9c-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="8ac9c-109">Flussi di lavoro di SharePoint 2010 ritardati all'avvio.</span><span class="sxs-lookup"><span data-stu-id="8ac9c-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="8ac9c-110">Ciò si verifica se il flusso di lavoro viene attivato in batch di grandi dimensioni.</span><span class="sxs-lookup"><span data-stu-id="8ac9c-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="8ac9c-111">(ad esempio, quando vengono aggiunti più elementi contemporaneamente).</span><span class="sxs-lookup"><span data-stu-id="8ac9c-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="8ac9c-112">I flussi di lavoro non sono progettati per l'esecuzione in tempo reale, quindi un ritardo è in base alla progettazione.</span><span class="sxs-lookup"><span data-stu-id="8ac9c-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="8ac9c-113">Se il flusso di lavoro è complesso XMOL (Extensible Object Markup Language), la compilazione può essere lenta.</span><span class="sxs-lookup"><span data-stu-id="8ac9c-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="8ac9c-114">Controlla [questo](https://support.microsoft.com//kb/3043697) articolo.</span><span class="sxs-lookup"><span data-stu-id="8ac9c-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="8ac9c-115">È consigliabile semplificare il flusso di lavoro o riprogettare il flusso di lavoro utilizzando il tipo di piattaforma flusso di lavoro di Microsoft SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="8ac9c-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="8ac9c-116">Se la cronologia del flusso di lavoro è aumentata, è possibile eliminare gli elementi o creare un nuovo elenco della cronologia.</span><span class="sxs-lookup"><span data-stu-id="8ac9c-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="8ac9c-117">Ulteriori informazioni : [Eliminazione della cronologia del flusso di lavoro](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="8ac9c-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="8ac9c-118">Argomenti correlati</span><span class="sxs-lookup"><span data-stu-id="8ac9c-118">Related topics</span></span>
<span data-ttu-id="8ac9c-119">Si desidera provare Microsoft Flow in SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="8ac9c-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="8ac9c-120">Create Flow</span><span class="sxs-lookup"><span data-stu-id="8ac9c-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="8ac9c-121">SharePoint e Flusso</span><span class="sxs-lookup"><span data-stu-id="8ac9c-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
