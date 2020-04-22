---
title: Il flusso di lavoro non inizia
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: 941e6349c98278a1a8cdac77457ec1cc72cdef8b
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766101"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="4ffae-102">Il flusso di lavoro non inizia</span><span class="sxs-lookup"><span data-stu-id="4ffae-102">Workflow is not starting</span></span>

- <span data-ttu-id="4ffae-103">I flussi di lavoro di SharePoint 2010 e SharePoint 2013 non vengono avviati.</span><span class="sxs-lookup"><span data-stu-id="4ffae-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="4ffae-104">Se il flusso di lavoro non è avviato, potrebbe verificarsi un problema di servizio temporaneo in cui gli utenti potrebbero riscontrare ritardi intermittenti con lo stato del flusso di lavoro.</span><span class="sxs-lookup"><span data-stu-id="4ffae-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="4ffae-105">Controllare il [Dashboard dell'integrità del servizio](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) per verificare se l'organizzazione ha un impatto.</span><span class="sxs-lookup"><span data-stu-id="4ffae-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="4ffae-106">Se sono passate più di 24 ore da quando hai visto questo problema, registra un ticket di supporto.</span><span class="sxs-lookup"><span data-stu-id="4ffae-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="4ffae-107">In molti casi, stiamo già lavorando a una soluzione.</span><span class="sxs-lookup"><span data-stu-id="4ffae-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="4ffae-108">Per completare una soluzione, è possibile fornirci almeno 24 ore.</span><span class="sxs-lookup"><span data-stu-id="4ffae-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="4ffae-109">I flussi di lavoro di SharePoint 2010 sono stati posticipati all'inizio.</span><span class="sxs-lookup"><span data-stu-id="4ffae-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="4ffae-110">Questo problema si verifica se il flusso di lavoro viene attivato in batch di grandi dimensioni.</span><span class="sxs-lookup"><span data-stu-id="4ffae-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="4ffae-111">ad esempio, quando vengono aggiunti contemporaneamente più elementi.</span><span class="sxs-lookup"><span data-stu-id="4ffae-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="4ffae-112">I flussi di lavoro non sono stati creati per l'esecuzione in tempo reale, quindi un ritardo è in base alla progettazione.</span><span class="sxs-lookup"><span data-stu-id="4ffae-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="4ffae-113">Se il flusso di lavoro è XMOL (Extensible Object Markup Language) complesso, la compilazione può essere lenta.</span><span class="sxs-lookup"><span data-stu-id="4ffae-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="4ffae-114">Controllare [questo](https://support.microsoft.com//kb/3043697) articolo.</span><span class="sxs-lookup"><span data-stu-id="4ffae-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="4ffae-115">È consigliabile semplificare il flusso di lavoro o riprogettarlo utilizzando il tipo di piattaforma per flussi di lavoro di Microsoft SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="4ffae-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="4ffae-116">Se la cronologia del flusso di lavoro è cresciuta, potrebbe essere necessario eliminare gli elementi o creare un nuovo elenco di cronologia.</span><span class="sxs-lookup"><span data-stu-id="4ffae-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="4ffae-117">Ulteriori informazioni: [eliminare la cronologia dei flussi di lavoro](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="4ffae-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="4ffae-118">Argomenti correlati</span><span class="sxs-lookup"><span data-stu-id="4ffae-118">Related topics</span></span>
<span data-ttu-id="4ffae-119">Si desidera provare Microsoft Flow in SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="4ffae-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="4ffae-120">Crea flusso</span><span class="sxs-lookup"><span data-stu-id="4ffae-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="4ffae-121">SharePoint e flusso</span><span class="sxs-lookup"><span data-stu-id="4ffae-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


