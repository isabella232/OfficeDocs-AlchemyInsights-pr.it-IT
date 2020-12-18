---
title: Errori di sincronizzazione della registrazione automatica del dispositivo Apple
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: d7a9398046a1073e30fdbe2950f750bb55d4fa2f
ms.sourcegitcommit: 87c8d0a1e6668211b9dd5427f98984ccdcadb02d
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/17/2020
ms.locfileid: "49707893"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Errori di sincronizzazione della registrazione automatica del dispositivo Apple

"È stato rilevato che si dispone di uno o più token di ADE/DEP che si trovano in uno stato di errore. Fino a quando non viene risolto lo stato di errore per ogni token coinvolto, la funzionalità ADE non funzionerà per lo stesso ".

Questo errore potrebbe manifestarsi in vari modi, tra cui:

1. I dispositivi potrebbero non essere sincronizzati da ABM/ASM a Intune
2. Le assegnazioni dei profili di registrazione potrebbero non riuscire
3. I dispositivi potrebbero non eseguire correttamente la registrazione ADE

Controllare l'errore di sincronizzazione riportato nella console di Intune in **dispositivi > registrare i dispositivi > registrazione Apple > i token del programma** di registrazione e consultare la documentazione seguente per visualizzare eventuali correzioni possibili:

[Errori di sincronizzazione ABM/ASM per i token di registrazione dei dispositivi automatizzati iOS/iPados e macOS](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
