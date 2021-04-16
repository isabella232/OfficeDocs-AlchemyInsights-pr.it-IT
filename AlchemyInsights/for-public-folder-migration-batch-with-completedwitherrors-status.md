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
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Per il batch di migrazione delle cartelle pubbliche con stato CompletedWithErrors

Utilizzare la procedura seguente per completare il batch, ignorando gli elementi di grandi dimensioni/non necessari: 
1. Approvare gli elementi ignorati nel batch di migrazione:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. Utilizzare il comando seguente per approvare gli elementi ignorati nelle richieste di migrazione "Sincronizzate" ma non completate:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. Il batch di migrazione e le richieste devono riprendere e completare in pochi minuti.

