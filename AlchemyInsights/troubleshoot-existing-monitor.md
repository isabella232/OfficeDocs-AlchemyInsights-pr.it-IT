---
title: Risoluzione dei problemi del monitor esistente
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
- "3454"
- "9001450"
ms.openlocfilehash: c4d2bb64b6b5ea79d4cd585e2be85c3c17e0f76f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824583"
---
# <a name="troubleshoot-an-existing-monitor"></a>Risolvere i problemi di un monitor esistente

Provare queste soluzioni per risolvere i problemi relativi a un monitor. 

**Aggiornare lo schermo del monitor:**

Premere contemporaneamente i tasti seguenti: Tasto Windows + CTRL + MAIUSC + B. In questo modo verrà aggiornata la comunicazione con il driver di grafica. I monitor lampeggiano momentaneamente e tornano dopo alcuni secondi.

**Risolvere i problemi relativi all'hardware di monitoraggio:**

1. Scollegare e ricollegare il cavo che collega il PC al monitor.
2. Disconnettere i dispositivi non essenziali dal PC (ad esempio adattatori o dock).

**Se hai installato di recente un aggiornamento nel PC, puoi eseguire il rollback del driver video:**

1. Seleziona **Start,** digita **Gestione dispositivi** e seleziona Gestione **dispositivi** dai risultati.
2. Espandere la **sezione Schede di visualizzazione,** fare clic con il pulsante destro del mouse sulla scheda di visualizzazione e scegliere **Proprietà.**
3. Passare alla scheda **Driver** e selezionare **Roll Back Driver**. <br>
Nota: se questa opzione non è disponibile o è disattivata, selezionare **No** nelle opzioni seguenti per passare al passaggio successivo.
4. Potrebbe essere necessario riavviare il PC prima che queste modifiche si apportare.

**Disinstallare e reinstallare il driver video:**

1. Seleziona **Start,** digita **Gestione dispositivi** e seleziona Gestione **dispositivi** dai risultati.
2. Espandi la **sezione Schede di visualizzazione,** fai clic con il pulsante destro del mouse sulla scheda video e scegli **Disinstalla dispositivo.** 
3. Seleziona la casella accanto a **Elimina il software driver per questo dispositivo** e seleziona **Disinstalla.**<br>
Nota: potrebbe essere richiesto di riavviare il computer in questa fase. Prima di riavviare, assicurati di scrivere le istruzioni rimanenti.
4. Aprire di nuovo Gestione dispositivi.
5. Espandi la **sezione Schede video,** fai clic con il pulsante destro del mouse sulla scheda video e scegli **Aggiorna driver.**
6. Selezionare **Cerca automaticamente il software del driver di** aggiornamento e seguire le istruzioni di installazione.