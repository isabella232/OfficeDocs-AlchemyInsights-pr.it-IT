---
title: Ricerca contenuto Nessun risultato
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 0267286ca5967ee891e65343d49adf776f0322a6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816852"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="450b6-102">Nessun risultato da Ricerca/Esportazioni contenuto</span><span class="sxs-lookup"><span data-stu-id="450b6-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="450b6-103">I problemi relativi alla ricerca/esportazione del contenuto che non restituiscono dati potrebbero essere dovuti a determinati filtri di sicurezza della conformità che sono stati impostati da un amministratore specifico e che non lo comunicano a tutti gli amministratori.</span><span class="sxs-lookup"><span data-stu-id="450b6-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="450b6-104">Per risolvere il problema, verificare se sono presenti filtri di sicurezza di conformità che potrebbero causare questo problema:</span><span class="sxs-lookup"><span data-stu-id="450b6-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="450b6-105">Connettersi a Powershell per Centro sicurezza e conformità</span><span class="sxs-lookup"><span data-stu-id="450b6-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="450b6-106">Eseguire i seguenti commandlet:</span><span class="sxs-lookup"><span data-stu-id="450b6-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="450b6-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="450b6-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="450b6-108">Get-ComplianceSecurityFilter -Organization $org</span><span class="sxs-lookup"><span data-stu-id="450b6-108">Get-ComplianceSecurityFilter -Organization $org</span></span>