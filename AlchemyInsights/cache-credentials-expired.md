---
title: 'Errore: non è possibile caricare o scaricare le modifiche perché le credenziali memorizzate nella cache sono scadute'
ms.author: v-miegge
author: v-miegge
manager: v-cojank
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: ''
ms.custom:
- "3534"
- "9001489"
ms.openlocfilehash: 14c9a4599072b0b0d3af50338fdb0a7cf0d474c9
ms.sourcegitcommit: 1e66f4850b0f06db1d1be82dc97f849abca80d38
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 02/07/2020
ms.locfileid: "41855784"
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
