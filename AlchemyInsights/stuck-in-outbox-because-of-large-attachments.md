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
- "9002385"
- "4645"
ms.openlocfilehash: 4f69de167dc51961fa7cf71b4d73ca7ee3ed4d55
ms.sourcegitcommit: 57fb994ddd3854d06faa67680c971b003b06bf83
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/13/2020
ms.locfileid: "43241256"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a>Risoluzione dei messaggi bloccati nella posta in uscita

Si consiglia di iniziare eseguendo lo scenario ["sono presenti problemi di invio, ricezione o individuazione dei messaggi di posta elettronica"](https://aka.ms/SaRA-OutlookSendReceive) dallo strumento [Assistente supporto e ripristino di Microsoft](https://diagnostics.office.com/#/) .

Quando un messaggio viene bloccato nella posta in uscita, la causa più probabile è un allegato di grandi dimensioni o l'opzione "Invia immediatamente quando connesso" non è abilitata.

**Rimuovere l'allegato di grandi dimensioni**

1. In Outlook selezionare **Invia/Ricevi** > **lavoro offline**. 
2. Nel riquadro di spostamento, selezionare **posta in uscita**. Da qui, è possibile: 
    - Eliminare il messaggio (selezionarlo e quindi fare clic su **Elimina**).
    - Trascinare il messaggio nella cartella bozze, fare doppio clic per aprirlo e rimuovere l'allegato selezionarlo e quindi scegliere **Elimina**.
3. Se viene visualizzato un messaggio di errore che indica che Outlook sta tentando di trasmetterlo, chiudere Outlook. Potrebbe essere necessario qualche minuto per uscire. Se Outlook non si chiude, premere CTRL + ALT + CANC e selezionare **Avvia Gestione attività**. In Task Manager selezionare la scheda **processi** , scorrere verso il basso fino a Outlook. exe e selezionare **Termina processo**.
4. Dopo la chiusura di Outlook, riavviarlo e ripetere i passaggi 2 e 3. 
5. Dopo aver rimosso l'allegato, fare clic su **Invia/Ricevi** > **lavoro offline** per riprendere a lavorare online. 

I messaggi vengono bloccati anche nella cartella posta in uscita quando si fa clic su **Invia**, ma non si è connessi. Fare clic su **Invia/Ricevi** e guardare il pulsante **lavora in modalità** non in linea. Se è blu, si è scollegati. Fare clic su di esso per connettersi (il pulsante diventa bianco) e fare clic su **Invia tutto**.
 
**Abilita invio immediato quando si è connessi**
 
1. Nella scheda File fare clic su **Opzioni**.

2. Nella finestra di dialogo Opzioni di Outlook fare clic su **Avanzate**.

3. Nella sezione invio e ricezione fare clic per abilitare l' **invio immediato quando**si è connessi. Fare clic su **OK**.
 
Per informazioni complete, vedere:
- [Video: invio o eliminazione di un messaggio di posta elettronica bloccato](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [La posta elettronica rimane nella cartella posta in uscita fino a quando non viene avviata manualmente un'operazione di invio/ricezione in Outlook](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
