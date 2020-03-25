---
title: Indicazioni generali sulle prestazioni della migrazione
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
- "3179"
ms.openlocfilehash: 10a0069c41d2e5128b2592425d815364a83b730f
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932483"
---
# <a name="general-migration-performance-guidance"></a><span data-ttu-id="ba80a-102">Indicazioni generali sulle prestazioni della migrazione</span><span class="sxs-lookup"><span data-stu-id="ba80a-102">General migration performance guidance</span></span>

<span data-ttu-id="ba80a-103">**Importante**: molti clienti di SharePoint Online e OneDrive eseguono con il servizio applicazioni business critical eseguite in background.</span><span class="sxs-lookup"><span data-stu-id="ba80a-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="ba80a-104">Tali applicazioni includono soluzioni per la migrazione del contenuto, di Prevenzione della perdita dei dati e per il backup.</span><span class="sxs-lookup"><span data-stu-id="ba80a-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="ba80a-105">In questi tempi straordinari, stiamo adottando misure per garantire che i servizi di SharePoint Online e OneDrive rimangano altamente disponibili e affidabili per gli utenti che dipendono ancor più dal servizio negli scenari di lavoro remoto.</span><span class="sxs-lookup"><span data-stu-id="ba80a-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="ba80a-106">A sostegno di questo obiettivo, abbiamo implementato limitazioni più rigide sulle app in background (migrazione, prevenzione della perdita dei dati e soluzioni di backup) durante il giorni nei giorni feriali.</span><span class="sxs-lookup"><span data-stu-id="ba80a-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="ba80a-107">In questo periodo sarà possibile notare una riduzione della velocità effettiva in queste app.</span><span class="sxs-lookup"><span data-stu-id="ba80a-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="ba80a-108">Tuttavia, nelle ore serali e durante il fine settimana nell'area il servizio sarà predisposto per elaborare una quantità notevolmente superiore di richieste delle app in background.</span><span class="sxs-lookup"><span data-stu-id="ba80a-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="ba80a-109">**Indicazioni sulle prestazioni della migrazione**</span><span class="sxs-lookup"><span data-stu-id="ba80a-109">**Migration performance guidance**</span></span>

<span data-ttu-id="ba80a-p103">Le prestazioni della migrazione possono essere influenzate dall'infrastruttura di rete, dalle dimensioni del file, dalla durata della migrazione e dalla limitazione. Queste informazioni saranno utili per pianificare e aumentare l'efficienza della migrazione.</span><span class="sxs-lookup"><span data-stu-id="ba80a-p103">Migration performance can be impacted by network infrastructure, file size, migration time, and throttling. Understanding these will help you plan and maximize the efficiency of your migration.</span></span>

- [<span data-ttu-id="ba80a-112">Indicazioni generali sulle prestazioni della migrazione</span><span class="sxs-lookup"><span data-stu-id="ba80a-112">General migration performance guidance</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)
