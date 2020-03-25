---
title: Limitazione della migrazione di SharePoint con 503 errori
ms.author: pebaum
author: pebaum
ms.date: 8/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000136"
- "2541"
ms.openlocfilehash: 7e12c74d33e3cee7c626ad899a4e7f2f0a409bca
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931662"
---
# <a name="sharepoint-migration-throttling-with-503-errors"></a><span data-ttu-id="b7ea8-102">Limitazione della migrazione di SharePoint con 503 errori</span><span class="sxs-lookup"><span data-stu-id="b7ea8-102">SharePoint migration throttling with 503 errors</span></span>

<span data-ttu-id="b7ea8-103">**Importante**: molti clienti di SharePoint Online e OneDrive eseguono applicazioni aziendali critiche rispetto al servizio in esecuzione in background.</span><span class="sxs-lookup"><span data-stu-id="b7ea8-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="b7ea8-104">Tali applicazioni includono soluzioni per la migrazione del contenuto, di Prevenzione della perdita dei dati e per il backup.</span><span class="sxs-lookup"><span data-stu-id="b7ea8-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="b7ea8-105">In questi tempi straordinari, stiamo adottando misure per garantire che i servizi di SharePoint Online e OneDrive rimangano altamente disponibili e affidabili per gli utenti che dipendono ancor più dal servizio negli scenari di lavoro remoto.</span><span class="sxs-lookup"><span data-stu-id="b7ea8-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="b7ea8-106">A sostegno di questo obiettivo, abbiamo implementato limitazioni più rigide sulle app in background (migrazione, prevenzione della perdita dei dati e soluzioni di backup) durante il giorni nei giorni feriali.</span><span class="sxs-lookup"><span data-stu-id="b7ea8-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="b7ea8-107">In questo periodo sarà possibile notare una riduzione della velocità effettiva in queste app.</span><span class="sxs-lookup"><span data-stu-id="b7ea8-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="b7ea8-108">Tuttavia, nelle ore serali e durante il fine settimana nell'area il servizio sarà predisposto per elaborare una quantità notevolmente superiore di richieste delle app in background.</span><span class="sxs-lookup"><span data-stu-id="b7ea8-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="b7ea8-109">**503 errori durante la migrazione a SharePoint Online**</span><span class="sxs-lookup"><span data-stu-id="b7ea8-109">**503 errors when migrating to SharePoint Online**</span></span>

<span data-ttu-id="b7ea8-110">Viene visualizzato che si esegue la migrazione a SharePoint Online e si ricevono 503 errori.</span><span class="sxs-lookup"><span data-stu-id="b7ea8-110">It appears you are migrating to SharePoint Online and receiving 503 errors.</span></span> <span data-ttu-id="b7ea8-111">Seguire i passaggi riportati di seguito, in modo da potervi aiutare al più presto possibile.</span><span class="sxs-lookup"><span data-stu-id="b7ea8-111">Please follow the steps below so we may assist you as soon as possible.</span></span> 

1. <span data-ttu-id="b7ea8-112">Fare clic su supporto per i **contatti**e quindi su **nuova richiesta di servizio**.</span><span class="sxs-lookup"><span data-stu-id="b7ea8-112">Click **Contact Support**, and then **New Service Request**.</span></span>
2. <span data-ttu-id="b7ea8-113">Per il titolo e la descrizione, digitare **limitazione della migrazione di SharePoint con 503**.</span><span class="sxs-lookup"><span data-stu-id="b7ea8-113">For the title and description, type **SharePoint Migration Throttling with 503**.</span></span>
3. <span data-ttu-id="b7ea8-114">Dopo aver inviato il ticket, aggiornarlo con le seguenti informazioni:</span><span class="sxs-lookup"><span data-stu-id="b7ea8-114">Once the ticket has been submitted, please update it with the following information:</span></span>
    - <span data-ttu-id="b7ea8-115">La quantità di sinistra della migrazione (ad esempio, il numero di TBs?).</span><span class="sxs-lookup"><span data-stu-id="b7ea8-115">How much left of migration (for example, how many TBs?).</span></span>
    - <span data-ttu-id="b7ea8-116">Data di inizio e di fine della migrazione.</span><span class="sxs-lookup"><span data-stu-id="b7ea8-116">Migration start and end date.</span></span>
    - <span data-ttu-id="b7ea8-117">Descrivere la posizione in cui si esegue la migrazione del contenuto, ad esempio SharePoint Server, box, GDrive, condivisioni di file e così via.</span><span class="sxs-lookup"><span data-stu-id="b7ea8-117">Describe where you are migrating your content from, such as SharePoint Server, Box, GDrive, File shares, etc..</span></span>
    - <span data-ttu-id="b7ea8-118">Stimare il numero di errori di limitazione (ad esempio, x Throttle all'ora?) e quando è stata eseguita la limitazione.</span><span class="sxs-lookup"><span data-stu-id="b7ea8-118">Estimate the number of throttling errors (for example, x throttle per hour?) and when did the throttling happen.</span></span>
    - <span data-ttu-id="b7ea8-119">Strumento di migrazione in uso (ad esempio, SPMT o ShareGate).</span><span class="sxs-lookup"><span data-stu-id="b7ea8-119">Which migration tool you are using (for example, SPMT or ShareGate).</span></span>


