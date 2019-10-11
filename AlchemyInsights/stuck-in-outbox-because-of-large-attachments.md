---
title: Bloccato in posta in uscita a causa di allegati di grandi dimensioni
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2713"
- "9000768"
ms.openlocfilehash: d5fb20fcc146be67c5a04de0640ed4efd625311a
ms.sourcegitcommit: 8004ee243b5c68ff9532224a2e6c69dda0abbd0b
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 10/10/2019
ms.locfileid: "37441310"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a>Risoluzione dei messaggi bloccati nella posta in uscita

Si consiglia di iniziare eseguendo lo scenario ["sono presenti problemi di invio, ricezione o individuazione dei messaggi di posta elettronica"](https://aka.ms/SaRA-OutlookSendReceive) dallo strumento [Assistente supporto e ripristino di Microsoft](https://diagnostics.office.com/#/) .

Quando un messaggio viene bloccato nella posta in uscita, le cause più probabili sono le seguenti:
- Allegati di grandi dimensioni.
- L'opzione **Invia immediatamente quando connesso** non è abilitata.

Per rimuovere allegati di grandi dimensioni: 

1. In Outlook selezionare **Invia/Ricevi** > **lavoro offline**. 
2. Nel riquadro di spostamento, selezionare **posta in uscita**. Da qui, è possibile: 
    - Eliminare il messaggio (selezionarlo e quindi fare clic su **Elimina**).
    - Trascinare il messaggio nella cartella bozze, fare doppio clic per aprirlo e rimuovere l'allegato selezionarlo e quindi scegliere **Elimina**.
3. Se viene visualizzato un messaggio di errore che indica che Outlook sta tentando di trasmetterlo, chiudere Outlook. Potrebbe essere necessario qualche minuto per uscire. Se Outlook non si chiude, premere CTRL + ALT + CANC e selezionare **Avvia Gestione attività**. In Task Manager selezionare la scheda **processi** , scorrere verso il basso fino a Outlook. exe e selezionare **Termina processo**.
4. Dopo la chiusura di Outlook, riavviarlo e ripetere i passaggi 2 e 3. 
5. Dopo aver rimosso l'allegato, fare clic su **Invia/Ricevi** > **lavoro offline** per riprendere a lavorare online. 

I messaggi vengono bloccati anche nella cartella posta in uscita quando si fa clic su **Invia**, ma non si è connessi. Fare clic su **Invia/Ricevi** e guardare il pulsante **lavora in modalità** non in linea. Se è blu, si è scollegati. Selezionarlo per la connessione (il pulsante diventa bianco) e fare clic su **Invia tutto**.
 
Per abilitare l' **invio immediato quando**si è connessi:
 
- Selezionare **** > **** opzioni >  file**Avanzate**.
Nella sezione **invio e ricezione** selezionare **Invia immediatamente quando**si è connessi e quindi fare clic su **OK**.
 
Per i dettagli completi, vedere:
- [Video: invio o eliminazione di un messaggio di posta elettronica bloccato](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [La posta elettronica rimane nella cartella posta in uscita fino a quando non viene avviata manualmente un'operazione di invio/ricezione in Outlook](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
