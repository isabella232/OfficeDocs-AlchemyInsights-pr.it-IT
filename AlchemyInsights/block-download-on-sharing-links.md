---
title: Bloccare il download sui collegamenti di condivisione
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000213"
- "5715"
ms.openlocfilehash: 5837013a71648d5d53cd215c3e3489f3de5528d5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685746"
---
# <a name="block-download-on-sharing-links"></a><span data-ttu-id="08d02-102">Bloccare il download sui collegamenti di condivisione</span><span class="sxs-lookup"><span data-stu-id="08d02-102">Block download on sharing links</span></span>

<span data-ttu-id="08d02-103">**Blocca il download** è disponibile per **collegamenti di sola visualizzazione** ai documenti di Office.</span><span class="sxs-lookup"><span data-stu-id="08d02-103">**Block download** is available for **view-only links** to Office documents.</span></span> <span data-ttu-id="08d02-104">Se si seleziona questa opzione, le persone che accedono al file tramite il collegamento creato non vedranno le opzioni per il download, la stampa o la copia del file.</span><span class="sxs-lookup"><span data-stu-id="08d02-104">When you select this option, people who gain access to the file via the link you created will not see options to download, print, or copy the file.</span></span>

<span data-ttu-id="08d02-105">Gli amministratori possono controllare se l'impostazione "blocca il download" è presente solo per i file di Office o meno modificando `BlockDownloadLinksFileType`l'impostazione nei cmdlets di Windows PowerShell [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/set-spotenant?view=sharepoint-ps) o [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps).</span><span class="sxs-lookup"><span data-stu-id="08d02-105">Administrators can control whether the "block download" setting appears only for Office files or not by changing the `BlockDownloadLinksFileType` setting in the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/set-spotenant?view=sharepoint-ps) or [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) PowerShell cmdlets.</span></span>
