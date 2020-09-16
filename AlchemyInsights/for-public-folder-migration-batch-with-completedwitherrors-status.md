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
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Per il batch di migrazione delle cartelle pubbliche con stato CompletedWithErrors

Utilizzare la procedura seguente per completare il batch, ignorando gli elementi di grandi dimensioni/negativi: 
1. Approvare gli elementi ignorati nel batch di migrazione:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. Utilizzare il seguente comando per approvare gli elementi ignorati nelle richieste di migrazione "sincronizzati" ma non completati:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. Il batch di migrazione e le richieste devono essere riavviate e completate in pochi minuti.

