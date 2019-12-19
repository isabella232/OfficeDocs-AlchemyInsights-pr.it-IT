---
title: Risoluzione dei problemi relativi al monitor esistente
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: d90baddd01bdf8508bd6289509c8399b8241887a
ms.sourcegitcommit: 42463e8d8869f36225a27388d83d37629c6b149e
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/18/2019
ms.locfileid: "40738573"
---
# <a name="troubleshoot-an-existing-monitor"></a>Risoluzione dei problemi di un monitor esistente

Provare queste soluzioni per la risoluzione dei problemi relativi a un monitor. 

**Aggiornare la visualizzazione del monitor:**

Premere contemporaneamente i tasti seguenti: tasto Windows + CTRL + MAIUSC + B. In questo modo verrà aggiornata la comunicazione con il driver di grafica. I monitor lampeggeranno momentaneamente e torneranno dopo alcuni secondi.

**Risoluzione dei problemi relativi all'hardware:**

1. Scollegare il cavo che collega il PC al monitor e ricollegarlo.
2. Scollegare tutti i dispositivi non essenziali dal PC (ad esempio, adattatori o dock).

**Se è stato installato di recente un aggiornamento sul PC, è possibile eseguire il rollback del driver dello schermo:**

1. Fare clic su **Start**, digitare **Gestione dispositivi**e selezionare **Gestione dispositivi** dai risultati.
2. Espandere la sezione **adattatori visualizzazione** , fare clic con il pulsante destro del mouse sulla scheda video, scegliere **Proprietà**.
3. Passare alla scheda **driver** e selezionare Ripristina **driver**. <br>
Nota: se questa opzione non è disponibile o è disabilitata, selezionare **No** dalle opzioni seguenti per passare al passaggio successivo.
4. Potrebbe essere necessario riavviare il PC prima che queste modifiche abbiano effetto.

**Disinstallare e reinstallare il driver di visualizzazione:**

1. Fare clic su **Start**, digitare **Gestione dispositivi**e selezionare **Gestione dispositivi** dai risultati.
2. Espandere la sezione **adattatori visualizzazione** , fare clic con il pulsante destro del mouse sulla scheda video e scegliere **Disinstalla dispositivo**. 
3. Selezionare la casella accanto a **Elimina il software del driver per il dispositivo** e selezionare **Disinstalla**.<br>
Nota: è possibile che venga richiesto di riavviare il computer in questa fase. Assicurarsi di annotare le istruzioni rimanenti prima del riavvio.
4. Aprire di nuovo gestione dispositivi.
5. Espandere la sezione **adattatori visualizzazione** , fare clic con il pulsante destro del mouse sulla scheda video e selezionare **Aggiorna driver**.
6. Selezionare **Cerca automaticamente per aggiornare il software del driver** e seguire le istruzioni per l'installazione.