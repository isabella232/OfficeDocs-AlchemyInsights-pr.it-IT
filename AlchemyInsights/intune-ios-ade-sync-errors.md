---
title: Errori di sincronizzazione di Registrazione automatica dispositivi Apple
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: 1664a26b313c4a38c9c6d78cdb89997749ba175fd3dd72f278e99bbd50b0ee84
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013752"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Errori di sincronizzazione di Registrazione automatica dispositivi Apple

"È stato rilevato che si dispone di uno o più token ADE/DEP in uno stato di errore. Finché lo stato dell'errore non viene risolto per ogni token interessato, la funzionalità ADE non funzionerà come previsto.".

Questo errore potrebbe manifestarsi in diversi modi, tra cui:

1. I dispositivi potrebbero non essere sincronizzati da ABM/ASM a Intune
2. Le assegnazioni del profilo di registrazione potrebbero non riuscire
3. I dispositivi potrebbero non completare correttamente la registrazione ADE

Controlla l'errore di sincronizzazione riportato nella console di Intune in **Dispositivi > Registrare** dispositivi > registrazione Apple > token del programma di registrazione .

Una delle cause più comuni dell'errore di sincronizzazione è la scadenza del token corrente. In molti casi, il rinnovo del token interessato risolverà il problema.

Se uno o più token sono scaduti, vedere la documentazione seguente per rinnovarli in base alle esigenze:

[Rinnovare un token di registrazione automatica dei dispositivi](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

Inoltre, è possibile vedere la documentazione seguente per visualizzare potenziali correzioni per altri errori che causano errori di sincronizzazione dei token:

[Errori di sincronizzazione ABM/ASM per i token di registrazione dispositivi automatizzati iOS/iPadOS e macOS](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[Errori di sincronizzazione ABM/ASM per i token di registrazione dispositivi automatizzati iOS/iPadOS e macOS](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
