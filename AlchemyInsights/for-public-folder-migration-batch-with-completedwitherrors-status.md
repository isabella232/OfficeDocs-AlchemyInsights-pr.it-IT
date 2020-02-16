---
title: Per il batch di migrazione delle cartelle pubbliche con stato CompletedWithErrors
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3532"
ms.openlocfilehash: 4243cdf0170fed1eadac6560d2a04e1a861c63e5
ms.sourcegitcommit: 9aaa61d717e0fd475d2e9f0507c42aa40d073b5f
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 02/15/2020
ms.locfileid: "42043597"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a><span data-ttu-id="35c0d-102">Per il batch di migrazione delle cartelle pubbliche con stato CompletedWithErrors</span><span class="sxs-lookup"><span data-stu-id="35c0d-102">For Public folder migration batch with CompletedWithErrors status</span></span>

<span data-ttu-id="35c0d-103">Utilizzare la procedura seguente per completare il batch, ignorando gli elementi di grandi dimensioni/negativi:</span><span class="sxs-lookup"><span data-stu-id="35c0d-103">Use the following steps to complete the batch, skipping the large/bad items:</span></span> 
1. <span data-ttu-id="35c0d-104">Approvare gli elementi ignorati nel batch di migrazione:</span><span class="sxs-lookup"><span data-stu-id="35c0d-104">Approve the skipped items on migration batch:</span></span>

    <span data-ttu-id="35c0d-105">Set-MigrationBatch \<batchname>-ApproveSkippedItems</span><span class="sxs-lookup"><span data-stu-id="35c0d-105">Set-MigrationBatch \<batchname> -ApproveSkippedItems</span></span> 
2. <span data-ttu-id="35c0d-106">Utilizzare il seguente comando per approvare gli elementi ignorati nelle richieste di migrazione "sincronizzati" ma non completati:</span><span class="sxs-lookup"><span data-stu-id="35c0d-106">Use the following command to approve the skipped items on migration requests that are “Synced” but not completed:</span></span>

    <span data-ttu-id="35c0d-107">$pf = Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics-IncludeReport; ForEach ($i in $pf) {if ($i. LargeItemsEncountered-gt 0-oppure $i. BadItemsEncountered-gt 0) {set-PublicFolderMailboxMigrationRequest $i. Identity. IdentifyingGuid-SkippedItemApprovalTime $ ([DateTime]:: UtcNow)}}</span><span class="sxs-lookup"><span data-stu-id="35c0d-107">$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}</span></span>
3. <span data-ttu-id="35c0d-108">Il batch di migrazione e le richieste devono essere riavviate e completate in pochi minuti.</span><span class="sxs-lookup"><span data-stu-id="35c0d-108">The migration batch and requests should resume and complete in a few minutes.</span></span>

