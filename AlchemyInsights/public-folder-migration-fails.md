---
title: Migrazione della cartella pubblica non riuscita al 95%
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
ms.openlocfilehash: b22dce778b4507e0a3337a59a55531ce248b59c4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662423"
---
# <a name="public-folder-migration-fails-at-95"></a>Migrazione della cartella pubblica non riuscita al 95%

È possibile che sia stato avviato il completamento di un batch di migrazione e lo stato del batch di migrazione continui a essere indicato come **Sincronizzato** per molto tempo. Si tratta di un comportamento previsto.

È normale che lo stato di un batch di migrazione resti su **Sincronizzato** per alcune ore prima di passare a **Completamento in corso**. Per le migrazioni che interessano un numero elevato di cassette postali di destinazione, è normale che lo stato resti indicato come "sincronizzato" per più di 24 ore, a condizione che nessuna delle richieste di migrazione per le cartelle pubbliche non sia andata a buon fine o sia in quarantena. Attendere per 24-48 ore che il batch di migrazione completi l'operazione.

Per le migrazioni delle cartelle pubbliche non riuscite al 95%, con errore FailedToMailEnablePublicFoldersException:

1. Scaricare ed eseguire lo script [ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF) sul proprio server Exchange locale.

2. Eseguire le azioni correttive suggerite dallo script.

3. Eseguire Sync-MailPublicFolders (per Exchange 2010) o Sync-ModernMailPublicFolders (per Exchange 2013 e versioni successive).

4. Riavviare la migrazione delle cartelle pubbliche.
