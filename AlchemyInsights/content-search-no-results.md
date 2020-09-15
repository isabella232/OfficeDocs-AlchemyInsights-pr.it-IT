---
title: Ricerca contenuto nessun risultato
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 1e90c403556a317ff810971ccfa4a91694fb1171
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680651"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="5492c-102">Nessun risultato dalla ricerca contenuto/esportazioni</span><span class="sxs-lookup"><span data-stu-id="5492c-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="5492c-103">Problemi relativi alla ricerca di contenuto/esportazioni la mancata restituzione di dati potrebbe essere dovuta a un determinato filtro di sicurezza di conformità che è stato configurato da un amministratore specifico e che non lo ha comunicato a tutti gli amministratori.</span><span class="sxs-lookup"><span data-stu-id="5492c-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="5492c-104">Per risolvere il problema, verificare se sono presenti filtri di sicurezza per la conformità che potrebbero causare questo problema:</span><span class="sxs-lookup"><span data-stu-id="5492c-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="5492c-105">Connettersi a PowerShell per Centro sicurezza e conformità</span><span class="sxs-lookup"><span data-stu-id="5492c-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="5492c-106">Eseguire le seguenti commandlets:</span><span class="sxs-lookup"><span data-stu-id="5492c-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="5492c-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="5492c-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="5492c-108">Get-ComplianceSecurityFilter-Organization $org</span><span class="sxs-lookup"><span data-stu-id="5492c-108">Get-ComplianceSecurityFilter -Organization $org</span></span>