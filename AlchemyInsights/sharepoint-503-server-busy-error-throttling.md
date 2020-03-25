---
title: Limitazione di SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 59104ef96c95de4e4bc7744825245bdafba97d7c
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931230"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="d6865-102">Limitazione di SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="d6865-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="d6865-103">**Importante**: molti clienti di SharePoint Online e OneDrive eseguono applicazioni aziendali critiche rispetto al servizio in esecuzione in background.</span><span class="sxs-lookup"><span data-stu-id="d6865-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="d6865-104">Tali applicazioni includono soluzioni per la migrazione del contenuto, di Prevenzione della perdita dei dati e per il backup.</span><span class="sxs-lookup"><span data-stu-id="d6865-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="d6865-105">In questi tempi straordinari, stiamo adottando misure per garantire che i servizi di SharePoint Online e OneDrive rimangano altamente disponibili e affidabili per gli utenti che dipendono ancor più dal servizio negli scenari di lavoro remoto.</span><span class="sxs-lookup"><span data-stu-id="d6865-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="d6865-106">A sostegno di questo obiettivo, abbiamo implementato limitazioni più rigide sulle app in background (migrazione, prevenzione della perdita dei dati e soluzioni di backup) durante il giorni nei giorni feriali.</span><span class="sxs-lookup"><span data-stu-id="d6865-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="d6865-107">In questo periodo sarà possibile notare una riduzione della velocità effettiva in queste app.</span><span class="sxs-lookup"><span data-stu-id="d6865-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="d6865-108">Tuttavia, nelle ore serali e durante il fine settimana nell'area il servizio sarà predisposto per elaborare una quantità notevolmente superiore di richieste delle app in background.</span><span class="sxs-lookup"><span data-stu-id="d6865-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="d6865-109">**503 Server is busy error**</span><span class="sxs-lookup"><span data-stu-id="d6865-109">**503 server is busy error**</span></span>

<span data-ttu-id="d6865-110">Gli utenti possono ricevere un server 503 è un errore durante il tentativo di accedere a siti di SharePoint o OneDrive.</span><span class="sxs-lookup"><span data-stu-id="d6865-110">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="d6865-111">Questo errore può essere causato dalla limitazione all'interno del servizio di SharePoint.</span><span class="sxs-lookup"><span data-stu-id="d6865-111">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="d6865-112">SharePoint Online utilizza la limitazione per mantenere le prestazioni ottimali e l'affidabilità del servizio SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="d6865-112">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="d6865-113">La limitazione limita il numero di azioni utente o di chiamate simultanee (tramite script o codice) per impedire un utilizzo eccessivo delle risorse.</span><span class="sxs-lookup"><span data-stu-id="d6865-113">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="d6865-114">Per ulteriori informazioni sulla limitazione, vedere [impedire la limitazione o il blocco in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="d6865-114">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="d6865-115">Se si ritiene che questo errore non sia correlato alla limitazione, è possibile controllare se è presente una manutenzione attiva sul tenant passando al [centro messaggi](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="d6865-115">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="d6865-116">Infine, verificare di aver visitato la pagina di [integrità del servizio](https://portal.office.com/adminportal/home#/servicehealth) per controllare eventuali avvisi/incidenti che potrebbero verificarsi.</span><span class="sxs-lookup"><span data-stu-id="d6865-116">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

