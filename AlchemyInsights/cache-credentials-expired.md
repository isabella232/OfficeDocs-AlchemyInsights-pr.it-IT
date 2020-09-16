---
title: 'Errore: non è possibile caricare o scaricare le modifiche perché le credenziali memorizzate nella cache sono scadute'
ms.author: v-miegge
author: v-miegge
manager: v-cojank
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: ''
ms.custom:
- "3534"
- "9001489"
ms.openlocfilehash: 8105fa7b311bc932f95c8bff4d6b58ed9aabe74a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734483"
---
# <a name="error-we-cant-upload-or-download-your-changes-because-your-cached-credentials-have-expired"></a>Errore: non è possibile caricare o scaricare le modifiche perché le credenziali memorizzate nella cache sono scadute

Quando si salvano i file nell'app OneDrive, se viene visualizzato un messaggio di errore contenente la frase **"le credenziali memorizzate nella cache sono scadute"**, eseguire le operazioni seguenti:

1. Chiudere tutte le applicazioni di Office.
1. Aprire Credential Manager e digitare **Credential Manager** nella casella di ricerca sulla barra delle applicazioni, quindi selezionare il **Pannello di controllo di gestione credenziali**.
1. Selezionare **credenziali di Windows**.
1. Individuare qualsiasi voce che inizia con la parola **OneDrive**.
1. Selezionare la voce e quindi premere **Rimuovi**.
1. Chiudi Gestione credenziali, quindi fai clic con il pulsante destro del mouse sul cloud blu nel systray e seleziona **Chiudi OneDrive**.
1. Digitare **OneDrive** nella casella di ricerca sulla barra delle applicazioni e selezionare **OneDrive app** per avviare OneDrive.
1. Accedere a OneDrive, quindi provare a salvare il file in OneDrive.
