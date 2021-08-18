---
title: Rimozione dei dati e cancellazione dei dispositivi in Intune
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
- "1279"
- "6700008"
- "9004638"
- "8392"
ms.openlocfilehash: 92673c4a2a0e0faa98d3ade5ca1f6aa687d4c94a
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331045"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>Rimozione dei dati e cancellazione dei dispositivi in Intune

Le azioni remote Ritiro dispositivo e Cancellazione dispositivo possono essere utilizzate per rimuovere i dati aziendali gestiti da Intune o per eseguire il ripristino delle impostazioni predefinite e ripristinare il dispositivo alle impostazioni predefinite.

1. Accedere a Gestione dispositivi Microsoft 365 e passare a **Dispositivi** > **Tutti i dispositivi**.
2. Selezionare il dispositivo da cui cancellare i dati.
3. Selezionare il tipo di cancellazione remota da eseguire. Il ritiro elimina solo le informazioni dell'organizzazione, mentre la cancellazione completa ripristina il dispositivo alle impostazioni predefinite.
4. Selezionare **Sì** per confermare. Fino al completamento della cancellazione, lo stato azione del dispositivo sarà *Ritiro in sospeso*.
    Una volta completata l'azione, il dispositivo mobile non verrà più visualizzato nell'elenco dei dispositivi gestiti.

**Nota** Non è possibile rimuovere i dati aziendali dai dispositivi AGGIUNTI ad Azure AD. 

Per informazioni dettagliate sull'effetto delle azioni di ritiro e cancellazione, incluse le informazioni conservate ed eliminate, vedere la seguente documentazione:

- [Rimuovere i dispositivi con la cancellazione, la disattivazione o l'annullamento della registrazione manuale del dispositivo](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).
- [Come cancellare i dati aziendali solo dalle app gestite da Intune](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- [Cancellare tutti i dati da un dispositivo macOS](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).