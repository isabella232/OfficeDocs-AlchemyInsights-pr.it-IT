---
title: Commenti in Microsoft Planner
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001717"
- "3810"
ms.openlocfilehash: 09385fd0235939d01e0baf141362cb8b76910682
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817644"
---
# <a name="comments-in-microsoft-planner"></a>Commenti in Microsoft Planner

I commenti relativi alle attività nell'ambito di un piano vengono archiviati nella cassetta postale di Exchange Online relativa al gruppo di Microsoft 365 associato al piano.  Quando si pubblica un commento su un'attività, viene inviata una notifica tramite posta elettronica alla cartella posta in arrivo del gruppo, che riceverà un messaggio di posta elettronica per ogni commento successivo.

Ecco alcune risposte ai problemi comuni relativi ai commenti:

- **Gli utenti non ricevono messaggi di posta elettronica**: i commenti vengono inviati alla posta in arrivo del gruppo a cui appartiene il piano. Perché un utente riceva i messaggi di posta elettronica di gruppo, il gruppo deve essere configurato per l'invio delle conversazioni di gruppo alle cartelle posta in arrivo dei membri.

- **I commenti non vengono salvati**: l'utente che aggiunge il commento non è autorizzato a inviare messaggi di posta elettronica al gruppo di Microsoft 365. Per altre informazioni su questo scenario, leggere l'articolo sul [funzionamento di Microsoft Planner](https://techcommunity.microsoft.com/t5/planner-blog/how-microsoft-planner-works/ba-p/1214736).

- Viene visualizzato il messaggio di errore **Non hai più accesso** oppure **gli utenti ospiti non riescono ad aggiungere commenti**: gli utenti ospiti che non possono inviare messaggi di posta elettronica alla cartella posta in arrivo del gruppo potrebbero visualizzare questo messaggio. Per risolvere il problema, verificare che l'utente ospite abbia un indirizzo di posta elettronica valido.

- **Gli utenti rimossi ricevono i messaggi di posta elettronica**: se un utente invia un commento a un'attività prima di essere rimosso dal piano, il thread di posta elettronica includerà l'utente per ogni commento aggiunto all'attività.

Per informazioni dettagliate sui commenti con Microsoft Planner, vedere l'articolo sul [funzionamento di Microsoft Planner](https://techcommunity.microsoft.com/t5/planner-blog/how-microsoft-planner-works/ba-p/1214736) e [Commentare le attività in Microsoft Planner](https://support.microsoft.com/office/fd4aedde-7785-4cd0-96ee-122fbc9140e1).
