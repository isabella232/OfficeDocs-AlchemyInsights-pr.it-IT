---
title: Prestazioni di migrazione di SharePoint
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "2700"
ms.openlocfilehash: 812444589d5a5bf766bbc6f466077d4ca829d79f
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932239"
---
# <a name="sharepoint-migration-performance"></a><span data-ttu-id="31f39-102">Prestazioni di migrazione di SharePoint</span><span class="sxs-lookup"><span data-stu-id="31f39-102">SharePoint migration performance</span></span>

<span data-ttu-id="31f39-103">**Importante**: molti clienti di SharePoint Online e OneDrive eseguono con il servizio applicazioni business critical eseguite in background.</span><span class="sxs-lookup"><span data-stu-id="31f39-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="31f39-104">Tali applicazioni includono soluzioni per la migrazione del contenuto, di Prevenzione della perdita dei dati e per il backup.</span><span class="sxs-lookup"><span data-stu-id="31f39-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="31f39-105">In questi tempi straordinari, stiamo adottando misure per garantire che i servizi di SharePoint Online e OneDrive rimangano altamente disponibili e affidabili per gli utenti che dipendono ancor più dal servizio negli scenari di lavoro remoto.</span><span class="sxs-lookup"><span data-stu-id="31f39-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="31f39-106">A sostegno di questo obiettivo, abbiamo implementato limitazioni più rigide sulle app in background (migrazione, prevenzione della perdita dei dati e soluzioni di backup) durante il giorni nei giorni feriali.</span><span class="sxs-lookup"><span data-stu-id="31f39-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="31f39-107">In questo periodo sarà possibile notare una riduzione della velocità effettiva in queste app.</span><span class="sxs-lookup"><span data-stu-id="31f39-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="31f39-108">Tuttavia, nelle ore serali e durante il fine settimana nell'area il servizio sarà predisposto per elaborare una quantità notevolmente superiore di richieste delle app in background.</span><span class="sxs-lookup"><span data-stu-id="31f39-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="31f39-109">**Prestazioni della migrazione**</span><span class="sxs-lookup"><span data-stu-id="31f39-109">**Migration performance**</span></span>

<span data-ttu-id="31f39-p103">Le prestazioni della migrazione possono essere influenzate dall'infrastruttura di rete, dalle dimensioni del file, dalla durata della migrazione e dalla limitazione. Queste informazioni saranno utili per pianificare e aumentare l'efficienza della migrazione.</span><span class="sxs-lookup"><span data-stu-id="31f39-p103">Migration performance can be impacted by network infrastructure, file size, migration time, and throttling. Understanding these will help you plan and maximize the efficiency of your migration.</span></span>

<span data-ttu-id="31f39-112">Per altre informazioni, visitare i collegamenti seguenti.</span><span class="sxs-lookup"><span data-stu-id="31f39-112">For more information, please visit the links below.</span></span>

- [<span data-ttu-id="31f39-113">Velocità di migrazione in SharePoint Online e OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="31f39-113">Sharepoint Online and ODB Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

- [<span data-ttu-id="31f39-114">Evitare la limitazione o il blocco in SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="31f39-114">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [<span data-ttu-id="31f39-115">Scaricare e installare lo Strumento di migrazione di SharePoint</span><span class="sxs-lookup"><span data-stu-id="31f39-115">Download and install the SharePoint Migration Tool</span></span>](https://docs.microsoft.com/sharepointmigration/introducing-the-sharepoint-migration-tool)
