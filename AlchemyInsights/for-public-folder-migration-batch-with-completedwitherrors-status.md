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
ms.openlocfilehash: 78ceac80626159e72af5f9ac963365c5c057a4ef0de2b3dc7e4cde5e5cc155e5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54068168"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Per il batch di migrazione delle cartelle pubbliche con stato CompletedWithErrors

Utilizzare la procedura seguente per completare il batch, ignorando gli elementi di grandi dimensioni/non necessari: 
1. Approvare gli elementi ignorati nel batch di migrazione:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. Utilizzare il comando seguente per approvare gli elementi ignorati nelle richieste di migrazione "Sincronizzate" ma non completate:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. Il batch di migrazione e le richieste devono riprendere e completare in pochi minuti.

