---
title: Risoluzione dei problemi e degli errori dello strumento di migrazione di SharePoint
ms.author: v-miegge
author: v-miegge
manager: v-cojank
ms.date: 10/31/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "3178"
ms.assetid: ''
ms.openlocfilehash: f9f5694b1d88bccebdc5448d5629ea5120c52511
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931122"
---
# <a name="troubleshooting-sharepoint-migration-tool-issues-and-errors"></a><span data-ttu-id="54ae2-102">Risoluzione dei problemi e degli errori dello strumento di migrazione di SharePoint</span><span class="sxs-lookup"><span data-stu-id="54ae2-102">Troubleshooting SharePoint Migration Tool issues and errors</span></span>

<span data-ttu-id="54ae2-103">**Importante**: molti clienti di SharePoint Online e OneDrive eseguono applicazioni aziendali critiche rispetto al servizio in esecuzione in background.</span><span class="sxs-lookup"><span data-stu-id="54ae2-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="54ae2-104">Tali applicazioni includono soluzioni per la migrazione del contenuto, di Prevenzione della perdita dei dati e per il backup.</span><span class="sxs-lookup"><span data-stu-id="54ae2-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="54ae2-105">In questi tempi straordinari, stiamo adottando misure per garantire che i servizi di SharePoint Online e OneDrive rimangano altamente disponibili e affidabili per gli utenti che dipendono ancor più dal servizio negli scenari di lavoro remoto.</span><span class="sxs-lookup"><span data-stu-id="54ae2-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="54ae2-106">A sostegno di questo obiettivo, abbiamo implementato limitazioni più rigide sulle app in background (migrazione, prevenzione della perdita dei dati e soluzioni di backup) durante il giorni nei giorni feriali.</span><span class="sxs-lookup"><span data-stu-id="54ae2-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="54ae2-107">In questo periodo sarà possibile notare una riduzione della velocità effettiva in queste app.</span><span class="sxs-lookup"><span data-stu-id="54ae2-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="54ae2-108">Tuttavia, nelle ore serali e durante il fine settimana nell'area il servizio sarà predisposto per elaborare una quantità notevolmente superiore di richieste delle app in background.</span><span class="sxs-lookup"><span data-stu-id="54ae2-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="54ae2-109">**Problemi e errori comuni**</span><span class="sxs-lookup"><span data-stu-id="54ae2-109">**Common issues and errors**</span></span>

<span data-ttu-id="54ae2-110">Quando si utilizza lo strumento di migrazione di SharePoint (SPMT), è possibile che si verifichino problemi ed errori comuni.</span><span class="sxs-lookup"><span data-stu-id="54ae2-110">You may encounter some common issues and errors when using the SharePoint Migration Tool (SPMT).</span></span> <span data-ttu-id="54ae2-111">Per ulteriori informazioni, fare riferimento ai collegamenti riportati di seguito.</span><span class="sxs-lookup"><span data-stu-id="54ae2-111">Please reference the links below for more information.</span></span>

* [<span data-ttu-id="54ae2-112">Risoluzione dei problemi e degli errori comuni dello Strumento di migrazione di SharePoint</span><span class="sxs-lookup"><span data-stu-id="54ae2-112">Troubleshooting common SPMT issues and errors</span></span>](https://docs.microsoft.com/sharepointmigration/troubleshooting-common-spmt-issues)
* [<span data-ttu-id="54ae2-113">Risoluzione dei problemi di installazione di SPMT</span><span class="sxs-lookup"><span data-stu-id="54ae2-113">Troubleshooting SPMT install issues</span></span>](https://docs.microsoft.com/sharepointmigration/spmt-install-issues)