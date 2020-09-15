---
title: Individuazione di dispositivi iOS smarriti con Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1283"
- "6700008"
ms.openlocfilehash: 70f12328813a312631c67cd72cc75559ed2eca1b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47675169"
---
# <a name="locating-lost-ios-devices-with-intune"></a>Individuazione di dispositivi iOS smarriti con Intune

L'abilitazione della Modalità smarrito su un dispositivo iOS consente a un amministratore di avere un messaggio e un numero di telefono di contatto visualizzati nella schermata di blocco.

Dopo l'abilitazione della Modalità smarrito, l'amministratore può usare l'azione Individua dispositivo per identificare la posizione fisica del dispositivo.

L'azione Individua dispositivo in Intune funziona con i dispositivi iOS per mostrare la posizione di un dispositivo specifico su una mappa.

Con questa azione è necessario che il dispositivo iOS sia in:

- Modalità supervisione
- Modalità smarrito

Per altre informazioni, vedere [Abilitare la Modalità smarrito nei dispositivi iOS/iPadOS con Intune](https://docs.microsoft.com/intune/device-lost-mode) e [Individuare i dispositivi iOS/iPadOS smarriti o rubati con Intune](https://docs.microsoft.com/intune/device-locate).

**Domande frequenti**

D: Ho eseguito un'azione da remoto per rimuovere i dati aziendali da un dispositivo, che ora è bloccato e il suo stato è in sospeso.

R: Per completare correttamente un'azione da remoto, il dispositivo di destinazione deve essere online e integro. Nelle situazioni seguenti, l'azione da remoto resta in sospeso per 30 giorni o finché il dispositivo non riconosce il comando:

- Quando il dispositivo non ha connettività
- Quando il dispositivo perde lo stato di gestione con Intune

Se ritieni che un dispositivo non sia più connesso e non sia in grado di rimuovere i dati aziendali, selezionare Elimina. L'eliminazione rimuove il registro del dispositivo in modo che non venga più visualizzato nell'elenco Intune dei dispositivi. Se il dispositivo diventa nuovamente attivo, l'utente dovrà registrarlo di nuovo.

D: Perché alcune azioni remote non sono disponibili?

R: Non tutte le piattaforme supportano tutte le azioni del dispositivo remoto. Le azioni remote seguenti sono specifiche per determinate piattaforme, quindi sono disponibili solo per tali piattaforme.

- Ignora blocco attivazione (solo per iOS)
- Fresh Start (solo per Windows)
- Modalità smarrito (solo per iOS)
- Individuare il dispositivo (solo per iOS)
- Riavviare (solo per Windows)

Per altre informazioni su ogni azione, vedere [Azioni del dispositivo disponibili](https://docs.microsoft.com/intune/device-management#available-device-actions).