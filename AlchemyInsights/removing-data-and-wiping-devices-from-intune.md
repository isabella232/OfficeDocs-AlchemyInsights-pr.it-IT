---
title: Rimozione dei dati e cancellazione dei dispositivi in Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
ms.openlocfilehash: efaf111f694ab57d0435b141a6d4baad58658ed2
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 07/28/2020
ms.locfileid: "45434604"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>Rimozione dei dati e cancellazione dei dispositivi in Intune

Le azioni remote Ritiro dispositivo e Cancellazione dispositivo possono essere utilizzate per rimuovere i dati aziendali gestiti da Intune o per eseguire il ripristino delle impostazioni predefinite e ripristinare il dispositivo alle impostazioni predefinite.

1. Accedere a Gestione dispositivi Microsoft 365 e passare a **Dispositivi** > **Tutti i dispositivi**.
2. Selezionare il dispositivo da cui cancellare i dati.
3. Selezionare il tipo di cancellazione remota da eseguire. Il ritiro elimina solo le informazioni dell'organizzazione, mentre la cancellazione completa ripristina il dispositivo alle impostazioni predefinite.
4. Selezionare **Sì** per confermare. Fino al completamento della cancellazione, lo stato azione del dispositivo sarà Ritiro in sospeso.</br>
    Una volta completata l'azione, il dispositivo mobile non verrà più visualizzato nell'elenco dei dispositivi gestiti.

**Nota** Non è possibile rimuovere i dati aziendali dai dispositivi AGGIUNTI ad Azure AD.

Per informazioni dettagliate sull'effetto delle azioni di ritiro e cancellazione, incluse le informazioni conservate ed eliminate, vedere [Rimuovere i dispositivi con cancellazione, ritiro o annullamento manuale della registrazione](https://docs.microsoft.com/intune/devices-wipe).

Per cancellare tutti i dati da un dispositivo macOS, vedere [Cancellare tutti i dati da un dispositivo macOS](https://docs.microsoft.com/intune/device-erase).