---
title: Creare e gestire i tag dei dispositivi
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11446"
- "9003537"
ms.openlocfilehash: 3a7d53beaaf830055904f0634f09a3e9e447006e
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 06/02/2021
ms.locfileid: "52721730"
---
# <a name="create-and-manage-device-tags-or-groups"></a>Creare e gestire i tag dei dispositivi

Aggiungere tag nei dispositivi per creare un'affiliazione a un gruppo logico. I tag del dispositivo supportano la mappatura corretta della rete, consentendo di collegare tag diversi per acquisire il contesto e consentire la creazione di elenchi dinamici come parte di un incidente. I tag possono essere usati come filtro nella visualizzazione Elenco dispositivi o per raggruppare i dispositivi. Per altre informazioni sul raggruppamento dei dispositivi, vedere [Creare e gestire i tag dei dispositivi](/microsoft-365/security/defender-endpoint/machine-tags).

È possibile aggiungere tag nei dispositivi:

- Usando il portale

- Impostando un valore della chiave del Registro di sistema
 
**Nota:** potrebbe esserci latenza tra il momento in cui un tag viene aggiunto a un dispositivo e la sua disponibilità nell'elenco dei dispositivi e nella pagina del dispositivo.

Per aggiungere tag del dispositivo usando l'API, vedere [Aggiungere o rimuovere l'API dei tag del dispositivo](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags).

## <a name="add-and-manage-device-tags-using-the-portal"></a>Aggiungere e gestire i tag per i dispositivi tramite il portale

1. Selezionare il dispositivo in cui gestire i tag. È possibile selezionare o cercare un dispositivo in una delle seguenti visualizzazioni:

    - **Dashboard delle operazioni di sicurezza**: selezionare il nome del dispositivo dalla sezione Dispositivi principali con avvisi attivi.
    - **Coda degli avvisi**: selezionare il nome del dispositivo accanto all'icona del dispositivo dalla coda degli avvisi.
    - **Elenco dispositivi**: selezionare il nome del dispositivo nell'elenco dei dispositivi.
    - **Casella di ricerca**: selezionare Dispositivo dal menu a discesa e inserire il nome del dispositivo.

    È anche possibile accedere alla pagina di avviso tramite le visualizzazioni file e IP.

1. Selezionare **Gestisci tag** dalla riga Azioni di risposta.

1. Digitare per trovare o creare i tag.

I tag vengono aggiunti alla visualizzazione del dispositivo e si riflettono nella visualizzazione Elenco dispositivi. È quindi possibile usare il filtro dei tag per visualizzare l'elenco di dispositivi pertinente.

Per altre informazioni, vedere [Creare e gestire i tag dei dispositivi](/microsoft-365/security/defender-endpoint/machine-tags).