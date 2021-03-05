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
ms.openlocfilehash: 912c9e56b4c468fb333769f15bd7c212594dc11a
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448926"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Errori di sincronizzazione di Registrazione automatica dispositivi Apple

"È stato rilevato che si dispone di uno o più token ADE/DEP in uno stato di errore. Finché lo stato di errore non viene risolto per ogni token interessato, la funzionalità ADE non funzionerà come previsto.".

Questo errore potrebbe manifestarsi in diversi modi, tra cui:

1. I dispositivi potrebbero non essere sincronizzati da ABM/ASM a Intune
2. Le assegnazioni del profilo di registrazione potrebbero non riuscire
3. I dispositivi potrebbero non completare correttamente la registrazione ADE

Controlla l'errore di sincronizzazione segnalato nella console di Intune in Dispositivi > Registrazione dispositivi > i token del programma di registrazione Apple > **registrazione.**

Una delle cause più comuni dell'errore di sincronizzazione è la scadenza del token corrente. In molti casi, il rinnovo del token interessato risolverà il problema.

Se uno o più token sono scaduti, vedere la documentazione seguente per rinnovarli in base alle esigenze:

[Rinnovare un token di registrazione automatica dei dispositivi](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

Inoltre, è possibile vedere la documentazione seguente per vedere possibili correzioni per altri errori che causano errori di sincronizzazione dei token:

[Errori di sincronizzazione ABM/ASM per i token di registrazione dispositivi automatizzati iOS/iPadOS e macOS](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[Errori di sincronizzazione ABM/ASM per i token di registrazione dispositivi automatizzati iOS/iPadOS e macOS](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
