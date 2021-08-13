---
title: Ripristinare un elemento che non si trova più nella cartella Posta eliminata
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
ms.openlocfilehash: 81a7a2e9623c788743fad99e15c4d771bb12a6c1c81f35a9d2a6a0729ecf8db7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54062354"
---
# <a name="recover-an-item-thats-no-longer-in-your-deleted-items-folder"></a>Ripristinare un elemento non più presente nella cartella Posta eliminata

Se non è possibile trovare un elemento nella cartella Posta eliminata, la posizione successiva da cercare è la cartella Elementi ripristinabili. Si tratta di una cartella nascosta in cui vengono spostati gli elementi quando:
- Vengono eliminati dalla cartella Posta eliminata.
- La cartella Posta eliminata viene svuotata dall'utente o da un criterio impostato dall'amministratore IT.
- Per eliminare un elemento, selezionarlo e premere **MAIUSC+CANC.**

Per visualizzare e ripristinare gli elementi spostati nella cartella Elementi ripristinabili:
1. In un Web browser accedere a Outlook Web App con l'URL fornito dalla persona che gestisce la posta elettronica per l'organizzazione. Immettere il nome utente e la password, quindi selezionare **Accedi.**
1. Nell'elenco delle cartelle di posta elettronica fare clic con il pulsante destro del mouse su **Posta eliminata,** quindi selezionare **Recupera elementi eliminati...**.
1. Se necessario, utilizzare la casella di ricerca per trovare l'elemento che si desidera ripristinare.
1. Quando si trova l'elemento, selezionarlo e fare clic su **recupera**.
   Gli elementi recuperati vengono spostati nella posizione predefinita per ogni tipo di elemento.
    - I messaggi vengono inviati alla posta in arrivo.
    - Gli elementi del calendario vengono visualizzati nel calendario.
    - I contatti passano alla cartella Contatti.
    - Le attività passano alla cartella Attività.

**Suggerimenti per il ripristino degli elementi nella cartella Elementi ripristinabili**

- La data di eliminazione di un elemento nella cartella Elementi ripristinabili è quando l'elemento è stato spostato nella cartella Posta eliminata. Non è la data in cui l'elemento è stato spostato nella cartella Elementi ripristinabili.
- Gli elementi nella cartella Elementi ripristinabili non hanno icone, quindi hanno un aspetto molto simile.
    - Se si sta cercando un contatto, cercare un elemento con il nome della persona, ma senza oggetto.
    - Se si sta cercando un appuntamento del calendario, cercare un elemento che non abbia il nome di una persona o una riga dell'oggetto.
    - Se si sta cercando un contatto, un appuntamento del calendario o un'attività, cercare il testo di tale elemento.
- Per recuperare più elementi, posizionare il puntatore del mouse su ogni elemento e selezionare la casella di controllo accanto a esso, fare clic su **recupera**. È inoltre possibile recuperare più elementi adiacenti selezionando la  casella di controllo per il primo elemento, tenendo premuto MAIUSC e quindi selezionando la casella di controllo per l'ultimo elemento. Quando tutti gli elementi sono selezionati, selezionare **recupera**.
- È possibile eliminare gli elementi **dall'elenco Recupera elementi eliminati.** Basta selezionare l'elemento e quindi **selezionare Elimina**. Se si elimina un elemento, non sarà possibile utilizzare Recupera elementi eliminati per recuperarlo. L'eliminazione di un messaggio non lo rimuoverà dai backup evasi prima di essere eliminato.
- È possibile che l'organizzazione abbia specificato per quanto tempo gli elementi nella cartella Elementi ripristinabili sono disponibili per il ripristino. Ad esempio, potrebbe essere presente un criterio che elimina tutti gli elementi presenti nella cartella Posta eliminata per 30 giorni e un altro criterio che consente di ripristinare gli elementi nella cartella Elementi ripristinabili per un massimo di 14 giorni.
