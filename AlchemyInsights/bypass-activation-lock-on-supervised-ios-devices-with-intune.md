---
title: Ignorare blocco di attivazione nei dispositivi iOS supervisionati con Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1277"
- "6700008"
ms.openlocfilehash: 16be4e0cd2e47fe5d5888cbbe1380774f859e4d6
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 07/24/2020
ms.locfileid: "45397733"
---
# <a name="bypass-activation-lock-on-supervised-ios-devices-with-intune"></a>Ignorare blocco di attivazione nei dispositivi iOS supervisionati con Intune

La possibilità di ignorare il blocco di attivazione su dispositivi iOS semplifica il ripristino in scenari in cui un utente abilita il blocco di attivazione su un dispositivo aziendale e poi lascia l'azienda.

I prerequisiti per ignorare un blocco di attivazione includono:

- Il dispositivo è “supervisionato”.
- Il blocco di attivazione viene abilitato con i criteri di restrizione dei dispositivi iOS in Intune.

Inoltre, quando si ignora un blocco di attivazione, è necessario:

- Essere in possesso materiale del dispositivo che si eliminerà.
- Copiare il codice prima di eseguire la cancellazione.

**Nota:** il codice cancellazione non fa distinzione tra maiuscole e minuscole, quindi i caratteri “-” non sono necessari.

Per informazioni dettagliate, vedere [Ignorare il blocco di attivazione nei dispositivi iOS supervisionati con Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).

**Domande frequenti**

D: **Ho eseguito un'azione da remoto per rimuovere i dati aziendali da un dispositivo, che ora è bloccato e il suo stato è in sospeso.**

R: Per completare correttamente un'azione da remoto, il dispositivo di destinazione deve essere online e integro. Nelle situazioni seguenti, l'azione da remoto resta in sospeso per 30 giorni o finché il dispositivo non riconosce il comando quando il dispositivo:

- Non ha connettività.
- Perde lo stato di gestione con Intune.

Se ritieni che un dispositivo non sia più connesso e non rimuova i dati aziendali, selezionare Elimina. L'eliminazione rimuove il registro del dispositivo in modo che non venga più visualizzato nell'elenco Intune dei dispositivi. Per riattivare il dispositivo, è necessario che l'utente lo registri nuovamente.

D: **Perché alcune azioni remote non sono disponibili?**

R: Non tutte le piattaforme supportano tutte le azioni del dispositivo remoto. Le azioni da remoto riportate di seguito sono specifiche per ciascuna piattaforma.

- Ignora blocco attivazione (solo per iOS)
- Fresh Start (solo per Windows)
- Modalità smarrito (solo per iOS)
- Individuare il dispositivo (solo per iOS)
- Riavviare (solo per Windows)

Per altre informazioni su ogni azione, vedere [Azioni del dispositivo disponibili](https://docs.microsoft.com/intune/device-management#available-device-actions).