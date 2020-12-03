---
title: Recuperare un elemento che non è più presente nella cartella Posta eliminata
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/2/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1800008"
- "7320"
ms.openlocfilehash: b6ac084ead88b090d6caab1405d5d96f24890ea7
ms.sourcegitcommit: 62a83a1c6bd9779a1a11b749490bd11670d4b063
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/02/2020
ms.locfileid: "49560712"
---
# <a name="recover-an-item-thats-no-longer-in-your-deleted-items-folder"></a>Recuperare un elemento che non è più presente nella cartella Posta eliminata

Se non è possibile trovare un elemento nella cartella Posta eliminata, la posizione successiva è la cartella elementi ripristinabili. Si tratta di una cartella nascosta in cui gli elementi vengono spostati quando:
- Sono stati eliminati dalla cartella Posta eliminata.
- La cartella Posta eliminata viene svuotata da un utente o da un criterio impostato dall'amministratore IT.
- Per eliminare un elemento, selezionarlo e premere **MAIUSC + CANC**.

Per visualizzare e recuperare gli elementi spostati nella cartella elementi ripristinabili:
1. In un Web browser accedere a Outlook Web App con l'URL fornito dalla persona che gestisce la posta elettronica per l'organizzazione. Immettere il nome utente e la password, quindi selezionare **Accedi**.
1. Nell'elenco delle cartelle di posta elettronica fare clic con il pulsante destro del mouse su **elementi eliminati** e quindi scegliere **Recupera elementi eliminati.**
1. Se necessario, utilizzare la casella di ricerca per individuare l'elemento che si desidera ripristinare.
1. Quando si trova l'elemento, selezionarlo e fare clic su **Ripristina**.
   Gli elementi recuperati vengono spostati nel percorso predefinito per ogni tipo di elemento.
    - I messaggi passano alla posta in arrivo.
    - Gli elementi del calendario passano al calendario.
    - I contatti passano alla cartella contatti.
    - Le attività passano alla cartella attività.

**Suggerimenti per il ripristino degli elementi nella cartella elementi ripristinabili**

- La data di eliminazione per un elemento nella cartella elementi ripristinabili è quella in cui l'elemento è stato spostato nella cartella Posta eliminata. Non è la data in cui l'elemento è stato spostato nella cartella elementi ripristinabili.
- Gli elementi nella cartella elementi ripristinabili non dispongono di icone, in modo che siano tutti molto simili.
    - Se stai cercando un contatto, Cerca un elemento con il nome della persona, ma non la riga dell'oggetto.
    - Se stai cercando un appuntamento del calendario, Cerca un elemento che non ha il nome di una persona o una riga dell'oggetto.
    - Se stai cercando un contatto, un appuntamento del calendario o un'attività Cerca il testo di quell'elemento.
- Per recuperare più elementi, posizionare il puntatore del mouse su ogni elemento e selezionare la casella di controllo accanto a essa, fare clic su **Ripristina**. È inoltre possibile recuperare più elementi adiacenti selezionando la casella di controllo per il primo elemento, tenendo premuto il tasto **MAIUSC** e quindi selezionando la casella di controllo relativa all'ultimo elemento. Quando tutti gli elementi sono selezionati, selezionare **Ripristina**.
- È possibile eliminare gli elementi dall'elenco **Recupera elementi eliminati** . Seleziona l'elemento e quindi seleziona **Elimina**. Se si elimina un elemento, non sarà possibile utilizzare recuperare gli elementi eliminati per recuperarli. L'eliminazione di un messaggio non viene rimossa da qualsiasi backup eseguito prima di eliminarlo.
- È possibile che l'organizzazione abbia specificato la durata della disponibilità degli elementi nella cartella elementi ripristinabili per il ripristino. Ad esempio, potrebbe essere presente un criterio che elimina tutto ciò che è stato nella cartella Posta eliminata per 30 giorni e un altro criterio che consente di ripristinare gli elementi nella cartella elementi ripristinabili per un massimo di 14 giorni.
