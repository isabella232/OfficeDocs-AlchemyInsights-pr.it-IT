---
title: Batch di migrazione della cartella pubblica non completato, mostrato come sincronizzato
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
ms.openlocfilehash: 33302110249b02aef87639792ebfd9cafd6638c0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771488"
---
# <a name="public-folder-migration-batch-not-completing-shows-synced"></a><span data-ttu-id="5b6d2-102">Batch di migrazione della cartella pubblica non completato, mostrato come sincronizzato</span><span class="sxs-lookup"><span data-stu-id="5b6d2-102">Public folder migration batch not completing, shows synced</span></span>

<span data-ttu-id="5b6d2-103">È possibile che sia stato avviato il completamento di un batch di migrazione, e lo stato del batch di migrazione continui a essere indicato come "Sincronizzato" per molto tempo.</span><span class="sxs-lookup"><span data-stu-id="5b6d2-103">You may have initiated completion of migration batch and status of the migration batch continues showing "Synced" for very long time.</span></span> <span data-ttu-id="5b6d2-104">Si tratta di un comportamento previsto.</span><span class="sxs-lookup"><span data-stu-id="5b6d2-104">This is expected behavior.</span></span>

<span data-ttu-id="5b6d2-105">È normale che lo stato di un batch di migrazione resti su Sincronizzato per alcune ore prima di passare a Completamento in corso.</span><span class="sxs-lookup"><span data-stu-id="5b6d2-105">It's common for the status of migration batch to remain on Synced for a few hours before it switches to Completing.</span></span> <span data-ttu-id="5b6d2-106">Per le migrazioni che interessano un numero elevato di cassette postali di destinazione, è normale che lo stato resti indicato come "Sincronizzato" per più di 24 ore, a condizione che nessuna delle richieste di migrazione per le cartelle pubbliche non sia andata a buon fine o sia in quarantena.</span><span class="sxs-lookup"><span data-stu-id="5b6d2-106">For migrations involving a large number of target mailboxes, it's normal to see the status remain in the Synced state for more than 24 hours, provided none of the underlying public folder migration requests have failed or were quarantined.</span></span> <span data-ttu-id="5b6d2-107">Attendere per 24-48 ore che il batch di migrazione completi l'operazione.</span><span class="sxs-lookup"><span data-stu-id="5b6d2-107">Please allow 24-48 hours for the migration batch to complete the tasks.</span></span>
