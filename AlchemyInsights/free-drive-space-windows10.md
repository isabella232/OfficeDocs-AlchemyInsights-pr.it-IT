---
title: Liberare spazio di archiviazione in Windows 10
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 03/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9771"
- "9774"
- "9005390"
- "9005403"
ms.openlocfilehash: 2313636307bfddce2810c2d4c4ce9e3b407a7bdf
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505360"
---
# <a name="free-up-drive-space-in-windows-10"></a>Liberare spazio di archiviazione in Windows 10

Ci sono due modi per liberare spazio di archiviazione in Windows:

- Liberare spazio di archiviazione in Windows 10.
- Liberare spazio per gli aggiornamenti di Windows 10 con unità di archiviazione esterne. 

Se lo spazio di archiviazione è ancora insufficiente dopo la pulizia del disco, è probabile che la cartella Temp sia riempita rapidamente dai file delle applicazioni (.appx) usati da Microsoft Store. Per risolvere il problema, ripristinare Microsoft Store, svuotare la cache dello Store, quindi eseguire lo strumento di risoluzione dei problemi di Windows Update. Assicurare che Microsoft Store sia chiuso prima di procedere con questi passaggi.

**Passaggio 1: ripristinare Microsoft Store**

**Nota:** questa operazione elimina definitivamente i dati delle app sul dispositivo, incluso le preferenze e i dettagli di autenticazione.

1. Seleziona **Start** > **Impostazioni** > **App** > **App e funzionalità**.

1. Nell'elenco delle app, individua e seleziona Microsoft Store.

1. Seleziona **Opzioni avanzate**.

1. Scorri in basso e seleziona **Reimposta**, quindi **Conferma reimpostazione**.

**Passaggio 2: svuotare la cache di Microsoft Store**

1. Premi il tasto WINDOWS + R per aprire la finestra di dialogo Esegui.

1. Digita wsreset.exe e seleziona **OK**.

1. Si aprirà una finestra del prompt dei comandi vuota. Dopo circa 10 secondi, la finestra si chiude e lo Store si apre automaticamente.

**Passaggio 3: ripristinare Windows Update**

1. Seleziona **Start** > **Impostazioni** > **Aggiornamento e sicurezza** > **Risoluzione dei problemi**.

1. Scorri in basso e seleziona **Windows Update** dall'elenco, e seleziona **Avvia lo strumento di risoluzione dei problemi**.

1. Riavvia il computer e verificare se il problema persiste.

