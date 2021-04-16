---
title: Per il batch di migrazione delle cartelle pubbliche con stato CompletedWithErrors
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
- "3500007"
- "3532"
ms.openlocfilehash: 9ed21bfb9069b56a4fc59b201bb3ad94c6bb6712
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812468"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a><span data-ttu-id="7d7ea-102">Per il batch di migrazione delle cartelle pubbliche con stato CompletedWithErrors</span><span class="sxs-lookup"><span data-stu-id="7d7ea-102">For Public folder migration batch with CompletedWithErrors status</span></span>

<span data-ttu-id="7d7ea-103">Utilizzare la procedura seguente per completare il batch, ignorando gli elementi di grandi dimensioni/non necessari:</span><span class="sxs-lookup"><span data-stu-id="7d7ea-103">Use the following steps to complete the batch, skipping the large/bad items:</span></span> 
1. <span data-ttu-id="7d7ea-104">Approvare gli elementi ignorati nel batch di migrazione:</span><span class="sxs-lookup"><span data-stu-id="7d7ea-104">Approve the skipped items on migration batch:</span></span>

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. <span data-ttu-id="7d7ea-105">Utilizzare il comando seguente per approvare gli elementi ignorati nelle richieste di migrazione "Sincronizzate" ma non completate:</span><span class="sxs-lookup"><span data-stu-id="7d7ea-105">Use the following command to approve the skipped items on migration requests that are “Synced” but not completed:</span></span>

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. <span data-ttu-id="7d7ea-106">Il batch di migrazione e le richieste devono riprendere e completare in pochi minuti.</span><span class="sxs-lookup"><span data-stu-id="7d7ea-106">The migration batch and requests should resume and complete in a few minutes.</span></span>

