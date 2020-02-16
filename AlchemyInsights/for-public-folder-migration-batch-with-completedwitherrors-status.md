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
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Per il batch di migrazione delle cartelle pubbliche con stato CompletedWithErrors

Utilizzare la procedura seguente per completare il batch, ignorando gli elementi di grandi dimensioni/negativi: 
1. Approvare gli elementi ignorati nel batch di migrazione:

    Set-MigrationBatch \<batchname>-ApproveSkippedItems 
2. Utilizzare il seguente comando per approvare gli elementi ignorati nelle richieste di migrazione "sincronizzati" ma non completati:

    $pf = Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics-IncludeReport; ForEach ($i in $pf) {if ($i. LargeItemsEncountered-gt 0-oppure $i. BadItemsEncountered-gt 0) {set-PublicFolderMailboxMigrationRequest $i. Identity. IdentifyingGuid-SkippedItemApprovalTime $ ([DateTime]:: UtcNow)}}
3. Il batch di migrazione e le richieste devono essere riavviate e completate in pochi minuti.

