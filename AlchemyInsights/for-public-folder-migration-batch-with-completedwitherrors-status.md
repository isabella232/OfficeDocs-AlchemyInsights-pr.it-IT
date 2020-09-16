---
title: Per il batch di migrazione delle cartelle pubbliche con stato CompletedWithErrors
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
- "3500007"
- "3532"
ms.openlocfilehash: cbf5237fdb5c660057465e67702e35f68e545ddb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744117"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a><span data-ttu-id="8cf8f-102">Per il batch di migrazione delle cartelle pubbliche con stato CompletedWithErrors</span><span class="sxs-lookup"><span data-stu-id="8cf8f-102">For Public folder migration batch with CompletedWithErrors status</span></span>

<span data-ttu-id="8cf8f-103">Utilizzare la procedura seguente per completare il batch, ignorando gli elementi di grandi dimensioni/negativi:</span><span class="sxs-lookup"><span data-stu-id="8cf8f-103">Use the following steps to complete the batch, skipping the large/bad items:</span></span> 
1. <span data-ttu-id="8cf8f-104">Approvare gli elementi ignorati nel batch di migrazione:</span><span class="sxs-lookup"><span data-stu-id="8cf8f-104">Approve the skipped items on migration batch:</span></span>

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. <span data-ttu-id="8cf8f-105">Utilizzare il seguente comando per approvare gli elementi ignorati nelle richieste di migrazione "sincronizzati" ma non completati:</span><span class="sxs-lookup"><span data-stu-id="8cf8f-105">Use the following command to approve the skipped items on migration requests that are “Synced” but not completed:</span></span>

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. <span data-ttu-id="8cf8f-106">Il batch di migrazione e le richieste devono essere riavviate e completate in pochi minuti.</span><span class="sxs-lookup"><span data-stu-id="8cf8f-106">The migration batch and requests should resume and complete in a few minutes.</span></span>

