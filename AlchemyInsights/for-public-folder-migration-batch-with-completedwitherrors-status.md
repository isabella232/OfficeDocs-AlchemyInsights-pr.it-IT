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
ms.openlocfilehash: 739e9d91f90e4c0374814d199e4372eb5625553a
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158614"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Per il batch di migrazione delle cartelle pubbliche con stato CompletedWithErrors

Utilizzare la procedura seguente per completare il batch, ignorando gli elementi di grandi dimensioni/negativi: 
1. Approvare gli elementi ignorati nel batch di migrazione:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. Utilizzare il seguente comando per approvare gli elementi ignorati nelle richieste di migrazione "sincronizzati" ma non completati:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. Il batch di migrazione e le richieste devono essere riavviate e completate in pochi minuti.

