---
title: Pulizia automatica di dispositivi non aggiornati in Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 905881f08ace7afae871ac48fa30ed1a0f15d13972cdff299a6694ca2eafc9cc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53997076"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a>Pulizia automatica di dispositivi non aggiornati in Intune

Intune consente all'amministratore di configurare un intervallo di tempo compreso tra 90 e 270 giorni, dopo il quale i dispositivi non aggiornati verranno rimossi dal servizio. Questa impostazione è estesa all'intera organizzazione e, una volta attivata, diventa effettiva immediatamente. Qualsiasi dispositivo non archiviato nel server di Intune per un periodo superiore a quello impostato verrà eliminato definitivamente.

**Nota** Solo gli oggetti dei dispositivi MDM sono idonei per questa azione di pulizia. Sono esclusi solo gli oggetti dei dispositivi EAS.

Per altre informazioni su quando un dispositivo diventa idoneo per l'eliminazione in base all'opzione di pulizia del dispositivo e al relativo "stato":

Impostazione: **Eliminare dispositivi dopo l'ultima data di archiviazione: Sì (un valore specifico (N) di giorni)**

- In base al valore (N) configurato nell'impostazione, il servizio Intune elimina il dispositivo dopo il numero di giorni specificato dall'ultima archiviazione.

Impostazioni: **Eliminare dispositivi dopo l'ultima data di archiviazione: No**

- 180 giorni dopo la scadenza del certificato del dispositivo e in mancanza del suo rinnovo, il dispositivo viene eliminato.

**Nota** In entrambi i casi, il dispositivo deve essere registrato correttamente in Intune. La registrazione si verifica durante la prima archiviazione del dispositivo con il servizio Intune.

Se un dispositivo viene iscritto correttamente con Intune ma è registrato in Intune, il dispositivo verrà eliminato 270 giorni dopo l'iscrizione. (90 giorni in cui è possibile selezionare il dispositivo come revocato e altri 180 giorni per eliminare il record.)

Attualmente non è presente alcun meccanismo nella console Intune per stabilire la data di scadenza della certificazione del dispositivo per qualsiasi dispositivo specifico.