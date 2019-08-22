---
title: Ricerca contenuto nessun risultato
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 09cdbc3cb0465e0e0bc08872c49e283081ad3e92
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36516783"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="25a38-102">Nessun risultato dalla ricerca contenuto/esportazioni</span><span class="sxs-lookup"><span data-stu-id="25a38-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="25a38-103">Problemi relativi alla ricerca di contenuto/esportazioni la mancata restituzione di dati potrebbe essere dovuta a un determinato filtro di sicurezza di conformità che è stato configurato da un amministratore specifico e che non lo ha comunicato a tutti gli amministratori.</span><span class="sxs-lookup"><span data-stu-id="25a38-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="25a38-104">Per risolvere il problema, verificare se sono presenti filtri di sicurezza per la conformità che potrebbero causare questo problema:</span><span class="sxs-lookup"><span data-stu-id="25a38-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="25a38-105">Connettersi a PowerShell per Centro sicurezza e conformità</span><span class="sxs-lookup"><span data-stu-id="25a38-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="25a38-106">Eseguire le seguenti commandlets:</span><span class="sxs-lookup"><span data-stu-id="25a38-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="25a38-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="25a38-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="25a38-108">Get-ComplianceSecurityFilter-Organization $org</span><span class="sxs-lookup"><span data-stu-id="25a38-108">Get-ComplianceSecurityFilter -Organization $org</span></span>