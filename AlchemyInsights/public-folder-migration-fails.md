---
title: Migrazione della cartella pubblica non riuscita al 95%
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/25/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "639"
- "3500007"
ms.openlocfilehash: b22dce778b4507e0a3337a59a55531ce248b59c4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662423"
---
# <a name="public-folder-migration-fails-at-95"></a><span data-ttu-id="f2439-102">Migrazione della cartella pubblica non riuscita al 95%</span><span class="sxs-lookup"><span data-stu-id="f2439-102">Public folder migration fails at 95%</span></span>

<span data-ttu-id="f2439-103">È possibile che sia stato avviato il completamento di un batch di migrazione e lo stato del batch di migrazione continui a essere indicato come **Sincronizzato** per molto tempo.</span><span class="sxs-lookup"><span data-stu-id="f2439-103">You might have initiated completion of a migration batch, and the status of the migration batch continues showing **Synced** for a very long time.</span></span> <span data-ttu-id="f2439-104">Si tratta di un comportamento previsto.</span><span class="sxs-lookup"><span data-stu-id="f2439-104">This is expected behavior.</span></span>

<span data-ttu-id="f2439-105">È normale che lo stato di un batch di migrazione resti su **Sincronizzato** per alcune ore prima di passare a **Completamento in corso**.</span><span class="sxs-lookup"><span data-stu-id="f2439-105">It's common for the status of a migration batch to remain on **Synced** for a few hours before it switches to **Completing**.</span></span> <span data-ttu-id="f2439-106">Per le migrazioni che interessano un numero elevato di cassette postali di destinazione, è normale che lo stato resti indicato come "sincronizzato" per più di 24 ore, a condizione che nessuna delle richieste di migrazione per le cartelle pubbliche non sia andata a buon fine o sia in quarantena.</span><span class="sxs-lookup"><span data-stu-id="f2439-106">For migrations involving a large number of target mailboxes, it's normal to see the status remain in the synced state for more than 24 hours, provided none of the underlying public folder migration requests have failed or were quarantined.</span></span> <span data-ttu-id="f2439-107">Attendere per 24-48 ore che il batch di migrazione completi l'operazione.</span><span class="sxs-lookup"><span data-stu-id="f2439-107">Please allow 24-48 hours for the migration batch to complete the tasks.</span></span>

<span data-ttu-id="f2439-108">Per le migrazioni delle cartelle pubbliche non riuscite al 95%, con errore FailedToMailEnablePublicFoldersException:</span><span class="sxs-lookup"><span data-stu-id="f2439-108">For public folder migrations failing at 95%, with error FailedToMailEnablePublicFoldersException:</span></span>

1. <span data-ttu-id="f2439-109">Scaricare ed eseguire lo script [ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF) sul proprio server Exchange locale.</span><span class="sxs-lookup"><span data-stu-id="f2439-109">Download and run the [ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF) script at your Exchange On-Premises server.</span></span>

2. <span data-ttu-id="f2439-110">Eseguire le azioni correttive suggerite dallo script.</span><span class="sxs-lookup"><span data-stu-id="f2439-110">Perform the corrective actions suggested by the script.</span></span>

3. <span data-ttu-id="f2439-111">Eseguire Sync-MailPublicFolders (per Exchange 2010) o Sync-ModernMailPublicFolders (per Exchange 2013 e versioni successive).</span><span class="sxs-lookup"><span data-stu-id="f2439-111">Run the Sync-MailPublicFolders (for Exchange 2010) or Sync-ModernMailPublicFolders (for Exchange 2013 and later).</span></span>

4. <span data-ttu-id="f2439-112">Riavviare la migrazione delle cartelle pubbliche.</span><span class="sxs-lookup"><span data-stu-id="f2439-112">Resume public folder migration.</span></span>
