---
title: Limitazione di SharePoint Online
ms.author: kirks
author: Techwriter40
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: c7881c0c7331e0aa74fcc439f52157bb75a56160
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36559845"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="82a7e-102">Limitazione di SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="82a7e-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="82a7e-103">Gli utenti possono ricevere un server 503 è un errore durante il tentativo di accedere a siti di SharePoint o OneDrive.</span><span class="sxs-lookup"><span data-stu-id="82a7e-103">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="82a7e-104">Questo errore può essere causato dalla limitazione all'interno del servizio di SharePoint.</span><span class="sxs-lookup"><span data-stu-id="82a7e-104">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="82a7e-105">SharePoint Online utilizza la limitazione per mantenere le prestazioni ottimali e l'affidabilità del servizio SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="82a7e-105">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="82a7e-106">La limitazione limita il numero di azioni utente o di chiamate simultanee (tramite script o codice) per impedire un utilizzo eccessivo delle risorse.</span><span class="sxs-lookup"><span data-stu-id="82a7e-106">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="82a7e-107">Se si ottiene la limitazione, il 99% del tempo è a causa del codice personalizzato.</span><span class="sxs-lookup"><span data-stu-id="82a7e-107">If you do get throttled, 99% of the time it is because of custom code.</span></span>

<span data-ttu-id="82a7e-108">Per ulteriori informazioni sulla limitazione, vedere [impedire la limitazione o il blocco in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="82a7e-108">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="82a7e-109">Se si ritiene che questo errore non sia correlato alla limitazione, è possibile controllare se è presente una manutenzione attiva sul tenant passando al [centro messaggi](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="82a7e-109">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="82a7e-110">Infine, verificare di aver visitato la pagina di [integrità del servizio](https://portal.office.com/adminportal/home#/servicehealth) per controllare eventuali avvisi/incidenti che potrebbero verificarsi.</span><span class="sxs-lookup"><span data-stu-id="82a7e-110">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

