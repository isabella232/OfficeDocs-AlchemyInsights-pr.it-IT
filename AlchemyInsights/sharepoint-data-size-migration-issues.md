---
title: Problemi durante la migrazione dei dati in SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "1885"
ms.openlocfilehash: b53a98480bab48497274c7358f7e606caa477f5a
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931698"
---
# <a name="issues-while-migrating-data-to-sharepoint-online"></a><span data-ttu-id="f912a-102">Problemi durante la migrazione dei dati in SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="f912a-102">Issues while migrating data to SharePoint Online</span></span>

<span data-ttu-id="f912a-103">**Importante**: molti clienti di SharePoint Online e OneDrive eseguono applicazioni aziendali critiche rispetto al servizio in esecuzione in background.</span><span class="sxs-lookup"><span data-stu-id="f912a-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="f912a-104">Tali applicazioni includono soluzioni per la migrazione del contenuto, di Prevenzione della perdita dei dati e per il backup.</span><span class="sxs-lookup"><span data-stu-id="f912a-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="f912a-105">In questi tempi straordinari, stiamo adottando misure per garantire che i servizi di SharePoint Online e OneDrive rimangano altamente disponibili e affidabili per gli utenti che dipendono ancor più dal servizio negli scenari di lavoro remoto.</span><span class="sxs-lookup"><span data-stu-id="f912a-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="f912a-106">A sostegno di questo obiettivo, abbiamo implementato limitazioni più rigide sulle app in background (migrazione, prevenzione della perdita dei dati e soluzioni di backup) durante il giorni nei giorni feriali.</span><span class="sxs-lookup"><span data-stu-id="f912a-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="f912a-107">In questo periodo sarà possibile notare una riduzione della velocità effettiva in queste app.</span><span class="sxs-lookup"><span data-stu-id="f912a-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="f912a-108">Tuttavia, nelle ore serali e durante il fine settimana nell'area il servizio sarà predisposto per elaborare una quantità notevolmente superiore di richieste delle app in background.</span><span class="sxs-lookup"><span data-stu-id="f912a-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="f912a-109">**Migrazione su 100TB di dati**</span><span class="sxs-lookup"><span data-stu-id="f912a-109">**Migrating over 100TB of data**</span></span>

<span data-ttu-id="f912a-110">Viene visualizzato che si sta eseguendo la migrazione su 100TB di dati in SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="f912a-110">It appears you are migrating over 100TB of data to SharePoint Online.</span></span> <span data-ttu-id="f912a-111">Seguire i passaggi riportati di seguito, in modo da potervi aiutare al più presto possibile.</span><span class="sxs-lookup"><span data-stu-id="f912a-111">Please follow the steps below so we may assist you as soon as possible.</span></span> 

1. <span data-ttu-id="f912a-112">Selezionare una **nuova richiesta di servizio**e quindi una **nuova richiesta di servizio**.</span><span class="sxs-lookup"><span data-stu-id="f912a-112">Select **New Service Request**, and then **New Service Request**.</span></span> 
2. <span data-ttu-id="f912a-113">Lasciare il titolo e la descrizione come **migrazione di SharePoint su 100TB**.</span><span class="sxs-lookup"><span data-stu-id="f912a-113">Leave the title and description as **SharePoint migration over 100TB**.</span></span>
3. <span data-ttu-id="f912a-114">Dopo aver inviato il ticket, aggiornarlo con le seguenti informazioni:</span><span class="sxs-lookup"><span data-stu-id="f912a-114">Once the ticket has been submitted, please update it with the following information:</span></span> 

    - <span data-ttu-id="f912a-115">Dimensioni stimate della migrazione.</span><span class="sxs-lookup"><span data-stu-id="f912a-115">Estimated size of your migration.</span></span>
    - <span data-ttu-id="f912a-116">Stima del momento in cui si desidera avviare e completare la migrazione.</span><span class="sxs-lookup"><span data-stu-id="f912a-116">An estimate of when you would like to start and complete your migration.</span></span>
    - <span data-ttu-id="f912a-117">Descrivere la posizione in cui si esegue la migrazione del contenuto, ad esempio SharePoint Server, box, GDrive, condivisioni di file e così via.</span><span class="sxs-lookup"><span data-stu-id="f912a-117">Describe where you are migrating your content from, such as SharePoint Server, Box, GDrive, File shares, etc..</span></span>


  

