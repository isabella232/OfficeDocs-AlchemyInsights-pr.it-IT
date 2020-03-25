---
title: Eseguire la migrazione delle opzioni a SharePoint Online
ms.author: pebaum
author: v-miegge
manager: v-cojank
ms.date: 11/04/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: c8c339c9-2e50-4daa-aa91-3eb5053e2bc6
ms.openlocfilehash: 830b39c51658cbc02f4be81acdfdf3b164a8df70
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932734"
---
# <a name="migrate-options-to-sharepoint-online"></a><span data-ttu-id="c16fc-102">Eseguire la migrazione delle opzioni a SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="c16fc-102">Migrate options to SharePoint Online</span></span>

<span data-ttu-id="c16fc-103">**Importante**: molti clienti di SharePoint Online e OneDrive eseguono applicazioni aziendali critiche rispetto al servizio in esecuzione in background.</span><span class="sxs-lookup"><span data-stu-id="c16fc-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="c16fc-104">Tali applicazioni includono soluzioni per la migrazione del contenuto, di Prevenzione della perdita dei dati e per il backup.</span><span class="sxs-lookup"><span data-stu-id="c16fc-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="c16fc-105">In questi tempi straordinari, stiamo adottando misure per garantire che i servizi di SharePoint Online e OneDrive rimangano altamente disponibili e affidabili per gli utenti che dipendono ancor più dal servizio negli scenari di lavoro remoto.</span><span class="sxs-lookup"><span data-stu-id="c16fc-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="c16fc-106">A sostegno di questo obiettivo, abbiamo implementato limitazioni più rigide sulle app in background (migrazione, prevenzione della perdita dei dati e soluzioni di backup) durante il giorni nei giorni feriali.</span><span class="sxs-lookup"><span data-stu-id="c16fc-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="c16fc-107">In questo periodo sarà possibile notare una riduzione della velocità effettiva in queste app.</span><span class="sxs-lookup"><span data-stu-id="c16fc-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="c16fc-108">Tuttavia, nelle ore serali e durante il fine settimana nell'area il servizio sarà predisposto per elaborare una quantità notevolmente superiore di richieste delle app in background.</span><span class="sxs-lookup"><span data-stu-id="c16fc-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="c16fc-109">**Opzioni di migrazione**</span><span class="sxs-lookup"><span data-stu-id="c16fc-109">**Migration options**</span></span>

<span data-ttu-id="c16fc-110">Sono disponibili diverse opzioni per la migrazione del contenuto a SharePoint Online, in base alle dimensioni e alla quantità di file che è necessario spostare, vedere un elenco di opzioni che si [trovano qui](https://docs.microsoft.com/sharepointmigration/migrate-to-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="c16fc-110">There are different options available to migrate content to SharePoint Online, depending on the size and quantity of files you need to move, please see a list of options [located here](https://docs.microsoft.com/sharepointmigration/migrate-to-sharepoint-online).</span></span>

<span data-ttu-id="c16fc-111">Per ulteriori informazioni sulla migrazione del contenuto, visitare i collegamenti riportati di seguito.</span><span class="sxs-lookup"><span data-stu-id="c16fc-111">For more information on content migration, please visit the links below.</span></span>

- [<span data-ttu-id="c16fc-112">Strumento di migrazione di SharePoint</span><span class="sxs-lookup"><span data-stu-id="c16fc-112">Sharepoint Migration Tool</span></span>](https://docs.microsoft.com/sharepointmigration/introducing-the-sharepoint-migration-tool)

- [<span data-ttu-id="c16fc-113">Introduzione a Gestione migrazione</span><span class="sxs-lookup"><span data-stu-id="c16fc-113">Get started with the Migration Manager</span></span>](https://docs.microsoft.com/sharepointmigration/mm-get-started)

- [<span data-ttu-id="c16fc-114">Velocità di migrazione di SharePoint Online e ODB</span><span class="sxs-lookup"><span data-stu-id="c16fc-114">Sharepoint Online and ODB Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

- [<span data-ttu-id="c16fc-115">Evitare la limitazione o il blocco in SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="c16fc-115">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [<span data-ttu-id="c16fc-116">Strumento di valutazione della migrazione di SharePoint (SMAT)</span><span class="sxs-lookup"><span data-stu-id="c16fc-116">SharePoint Migration Assessment Tool (SMAT)</span></span>](https://www.microsoft.com/download/details.aspx?id=53598&amp;751be11f-ede8-5a0c-058c-2ee190a24fa6=True)

<span data-ttu-id="c16fc-117">**Nota**: attualmente lo strumento di migrazione di SharePoint supporta solo le migrazioni da SharePoint 2010 e 2013.</span><span class="sxs-lookup"><span data-stu-id="c16fc-117">**Note**: Currently the SharePoint Migration tool only support migrations from SharePoint 2010  and 2013.</span></span> <span data-ttu-id="c16fc-118">La versione 2016 o 2019 non è supportata in questo momento.</span><span class="sxs-lookup"><span data-stu-id="c16fc-118">Version 2016 or 2019 are not supported at this time.</span></span>
