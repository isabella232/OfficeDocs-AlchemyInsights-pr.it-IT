---
title: Migrazione della cartella pubblica non riuscita al 95%
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/25/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "639"
- "3500007"
ms.openlocfilehash: fc8da45d91d5c32be52e48770e469cf25eb068f5
ms.sourcegitcommit: d4fc2a03af69e28e96075812d040fdd34d2e23f0
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/26/2020
ms.locfileid: "46903578"
---
# <a name="public-folder-migration-fails-at-95"></a>Migrazione della cartella pubblica non riuscita al 95%

Per le migrazioni delle cartelle pubbliche non riuscite al 95%, con errore FailedToMailEnablePublicFoldersException:

1. Scaricare ed eseguire lo script [ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF) sul proprio server Exchange locale.

2. Eseguire le azioni correttive suggerite dallo script.

3. Eseguire Sync-MailPublicFolders (per Exchange 2010) o Sync-ModernMailPublicFolders (per Exchange 2013 e versioni successive).

4. Riavviare la migrazione delle cartelle pubbliche.
