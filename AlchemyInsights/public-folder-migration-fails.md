---
title: Migrazione della cartella pubblica non riuscita al 95%
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/25/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "639"
- "3500007"
ms.openlocfilehash: fc8da45d91d5c32be52e48770e469cf25eb068f5
ms.sourcegitcommit: d4fc2a03af69e28e96075812d040fdd34d2e23f0
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/26/2020
ms.locfileid: "46903578"
---
# <a name="public-folder-migration-fails-at-95"></a><span data-ttu-id="e0b27-102">Migrazione della cartella pubblica non riuscita al 95%</span><span class="sxs-lookup"><span data-stu-id="e0b27-102">Public folder migration fails at 95%</span></span>

<span data-ttu-id="e0b27-103">Per le migrazioni delle cartelle pubbliche non riuscite al 95%, con errore FailedToMailEnablePublicFoldersException:</span><span class="sxs-lookup"><span data-stu-id="e0b27-103">For public folder migrations failing at 95%, with error FailedToMailEnablePublicFoldersException:</span></span>

1. <span data-ttu-id="e0b27-104">Scaricare ed eseguire lo script [ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF) sul proprio server Exchange locale.</span><span class="sxs-lookup"><span data-stu-id="e0b27-104">Download and run the [ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF) script at your Exchange On-Premises server.</span></span>

2. <span data-ttu-id="e0b27-105">Eseguire le azioni correttive suggerite dallo script.</span><span class="sxs-lookup"><span data-stu-id="e0b27-105">Perform the corrective actions suggested by the script.</span></span>

3. <span data-ttu-id="e0b27-106">Eseguire Sync-MailPublicFolders (per Exchange 2010) o Sync-ModernMailPublicFolders (per Exchange 2013 e versioni successive).</span><span class="sxs-lookup"><span data-stu-id="e0b27-106">Run the Sync-MailPublicFolders (for Exchange 2010) or Sync-ModernMailPublicFolders (for Exchange 2013 and later).</span></span>

4. <span data-ttu-id="e0b27-107">Riavviare la migrazione delle cartelle pubbliche.</span><span class="sxs-lookup"><span data-stu-id="e0b27-107">Resume public folder migration.</span></span>
