---
title: Problemi relativi alle prestazioni-SharePoint o OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: aecbf4043c6456ece73f7deed6b068040f0691a2
ms.sourcegitcommit: 0fb89d8106fe409ab1b78e50f5357ffc2252f7c7
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/17/2019
ms.locfileid: "40068410"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="02897-102">SharePoint o OneDrive lento, inaccessibile o non disponibile per più utenti</span><span class="sxs-lookup"><span data-stu-id="02897-102">SharePoint or OneDrive slow, inaccessible, or unavailable for multiple users</span></span>

<span data-ttu-id="02897-103">SharePoint o OneDrive possono essere lenti, inaccessibili o non disponibili o possono visualizzare i servizi non disponibili o 503 errori, per diversi motivi:</span><span class="sxs-lookup"><span data-stu-id="02897-103">SharePoint or OneDrive may be slow, inaccessible, or unavailable, or may display service unavailable or 503 errors, for several reasons:</span></span>
  
- <span data-ttu-id="02897-104">Se il sito di SharePoint o OneDrive è lento o ritardato per più utenti, potrebbe verificarsi un problema di servizio temporaneo in cui gli utenti avvertono ritardi intermittenti o errori di spostamento quando si accede a siti di SharePoint o di contenuto di OneDrive.</span><span class="sxs-lookup"><span data-stu-id="02897-104">If your SharePoint or OneDrive site is slow or delayed for multiple users, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="02897-105">Controllare il [Dashboard dell'integrità del servizio](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) per verificare se l'organizzazione ha un impatto.</span><span class="sxs-lookup"><span data-stu-id="02897-105">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>
  
- <span data-ttu-id="02897-106">Gli utenti possono ricevere un *server 503 è* un errore durante il tentativo di accedere a siti di SharePoint o OneDrive.</span><span class="sxs-lookup"><span data-stu-id="02897-106">Users may receive a *503 server is busy* error when attempting to navigate to SharePoint or OneDrive sites.</span></span> <span data-ttu-id="02897-107">Questo errore può essere causato dalla limitazione all'interno del servizio di SharePoint.</span><span class="sxs-lookup"><span data-stu-id="02897-107">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="02897-108">SharePoint Online utilizza la limitazione per mantenere le prestazioni ottimali e l'affidabilità del servizio SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="02897-108">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="02897-109">La limitazione limita il numero di azioni utente o di chiamate simultanee (tramite script o codice) per impedire un utilizzo eccessivo delle risorse.</span><span class="sxs-lookup"><span data-stu-id="02897-109">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="02897-110">Per ulteriori informazioni sulla limitazione, vedere [impedire la limitazione o il blocco in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="02897-110">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

- <span data-ttu-id="02897-111">Se si verifica un rallentamento delle prestazioni con un sito o una pagina di SharePoint **classica** o **moderna** , utilizzare lo [strumento di diagnostica della pagina](https://aka.ms/perftool) per analizzare le pagine.</span><span class="sxs-lookup"><span data-stu-id="02897-111">If you experience slow performance with a **classic** or **modern** SharePoint site or page, utilize the [Page Diagnostic tool](https://aka.ms/perftool) to analyze the pages.</span></span>
  
- <span data-ttu-id="02897-112">Se si verificano ancora prestazioni generali lente, vedere le risorse nella parte inferiore di questo articolo: [Introduzione all'ottimizzazione delle prestazioni per SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span><span class="sxs-lookup"><span data-stu-id="02897-112">If you still experience general slow performance, please review the resources at the bottom of this article: [Introduction to performance tuning for SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span></span>
  