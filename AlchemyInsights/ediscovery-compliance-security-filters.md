---
title: Nessun risultato restituito durante la ricerca di contenuto/esportazione
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7463"
ms.openlocfilehash: db025cd1278471a3c54d55409d9a9418095778a7
ms.sourcegitcommit: 9c64886a9e1a9b0ff356b28a5c1482ecc148d7ef
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/14/2020
ms.locfileid: "49666651"
---
# <a name="no-results-returned-during-content-searchexport"></a><span data-ttu-id="699fc-102">Nessun risultato restituito durante la ricerca di contenuto/esportazione</span><span class="sxs-lookup"><span data-stu-id="699fc-102">No results returned during Content Search/Export</span></span>

<span data-ttu-id="699fc-103">Se si verificano problemi con gli scenari di eDiscovery seguenti:</span><span class="sxs-lookup"><span data-stu-id="699fc-103">If you are experiencing issues with the following eDiscovery scenarios:</span></span>

- <span data-ttu-id="699fc-104">Ricerca contenuto/Esporta non restituisce dati o dati imprevisti</span><span class="sxs-lookup"><span data-stu-id="699fc-104">Content Search/Export returns no data or unexpected data</span></span>
- <span data-ttu-id="699fc-105">errore di ricerca o esportazione di eDiscovery</span><span class="sxs-lookup"><span data-stu-id="699fc-105">eDiscovery Search or Export fails</span></span>

<span data-ttu-id="699fc-106">Questo può essere dovuto a determinati filtri di sicurezza di conformità che sono stati impostati da un amministratore specifico e non sono stati comunicati a tutti gli amministratori.</span><span class="sxs-lookup"><span data-stu-id="699fc-106">This may be caused due to certain Compliance Security Filters that were setup by a specific Admin and not been communicated to all Admins.</span></span>

<span data-ttu-id="699fc-107">Per risolvere il problema, controllare se sono presenti filtri di sicurezza per la conformità che potrebbero causare questi problemi:</span><span class="sxs-lookup"><span data-stu-id="699fc-107">To resolve this, check if there are any Compliance Security Filters that may be causing these issues:</span></span>

1. <span data-ttu-id="699fc-108">Connettersi a PowerShell per Centro sicurezza e conformità</span><span class="sxs-lookup"><span data-stu-id="699fc-108">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="699fc-109">Eseguire le seguenti commandlets:</span><span class="sxs-lookup"><span data-stu-id="699fc-109">Run the following commandlets:</span></span>

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

<span data-ttu-id="699fc-110">Per ulteriori informazioni sui filtri di sicurezza di conformità, vedere [filtro delle autorizzazioni per la ricerca di contenuto](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span><span class="sxs-lookup"><span data-stu-id="699fc-110">For additional information on Compliance Security Filters, see [Permissions Filtering for Content Search](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span></span>
