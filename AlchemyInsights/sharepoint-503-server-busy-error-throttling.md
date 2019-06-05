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
ms.openlocfilehash: 620a1094c1926b2c095c057a1791aaed8383afb3
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/04/2019
ms.locfileid: "34716931"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="c9e59-102">Limitazione di SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="c9e59-102">SharePoint Online Throttling</span></span>

<p><span data-ttu-id="c9e59-103"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Gli utenti possono ricevere un server 503 è un errore durante il tentativo di accedere a siti di SharePoint o OneDrive.</span></span><span class="sxs-lookup"><span data-stu-id="c9e59-103"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Users may receive a 503 server is busy error when attempting to navigate to Sharepoint or OneDrive sites. </span></span></span></p> <p><span data-ttu-id="c9e59-104"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Questo errore può essere causato dalla limitazione all'interno del servizio di SharePoint. SharePoint Online utilizza la limitazione per mantenere le prestazioni ottimali e l'affidabilità del servizio SharePoint Online. La limitazione limita il numero di azioni utente o di chiamate simultanee (tramite script o codice) per impedire un utilizzo eccessivo delle risorse. Se si ottiene la limitazione, il 99% del tempo è a causa del codice personalizzato.</span></span><span class="sxs-lookup"><span data-stu-id="c9e59-104"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">This error can be caused by throttling within the Sharepoint service. SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service. Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources. If you do get throttled, 99% of the time it is because of custom code.</span></span></span></p> <p><span data-ttu-id="c9e59-105"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Per ulteriori informazioni sulla limitazione, vedere <a href="https://docs.microsoft.com/en-us/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online">impedire la limitazione o il blocco in SharePoint Online</a>.</span></span><span class="sxs-lookup"><span data-stu-id="c9e59-105"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">For more information on throttling see, <a href="https://docs.microsoft.com/en-us/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online">Avoid getting throttled or blocked in SharePoint Online</a>.</span></span></span></p> <p><span data-ttu-id="c9e59-106"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Se si ritiene che questo errore non sia correlato alla limitazione, è possibile controllare se è presente una manutenzione attiva sul tenant passando al <a href="https://portal.office.com/adminportal/home#/MessageCenter">centro messaggi</a>. Infine, verificare di aver visitato la pagina di <a href="https://portal.office.com/adminportal/home#/servicehealth">integrità del servizio</a> per controllare eventuali avvisi/incidenti che potrebbero verificarsi.</span></span><span class="sxs-lookup"><span data-stu-id="c9e59-106"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the <a href="https://portal.office.com/adminportal/home#/MessageCenter">Message center</a>. Finally , ensure you visit the <a href="https://portal.office.com/adminportal/home#/servicehealth">Service Health</a> page to check for any advisories/incidents that may be occurring.</span></span></span></p> <p>&nbsp;</p>


