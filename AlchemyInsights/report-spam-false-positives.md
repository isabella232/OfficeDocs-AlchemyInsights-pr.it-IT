---
title: Si desidera segnalare un falso positivo alla posta indesiderata a Microsoft?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "975"
- "666"
- "3100019"
ms.openlocfilehash: d3897f24ce9a967b08a3fd15a2fdedbb3fe2a22d
ms.sourcegitcommit: f05d4caa0e657ee74d6b6e9abc88488f17d740fe
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/19/2021
ms.locfileid: "58396619"
---
# <a name="do-you-have-legitimate-messages-being-marked-as-spam"></a>Sono presenti messaggi legittimi contrassegnati come posta indesiderata?

È frustrante quando un messaggio di posta elettronica legittimo finisce nella cartella Posta indesiderata o in quarantena. Considerare i motivi più comuni per i falsi positivi:

**Sostituzioni del tenant (più comuni)** Questo è completamente all'interno del controllo da correggere.

Inviare il messaggio sul Microsoft 365 Defender per l'analisi dei criteri e delle regole che influiscono; i dettagli della nuova analisi sono disponibili in pochi minuti.
Rivedere o modificare i criteri o le regole in base alle condizioni applicabili. 

**Sostituzioni dell'utente finale (comuni)** Questo è completamente all'interno del controllo da correggere. 

Inviare il messaggio sul Microsoft 365 Defender per l'analisi dei criteri e delle regole che influiscono; i dettagli della nuova analisi sono disponibili in pochi minuti. 

Se un messaggio è stato bloccato perché è stato inviato da un indirizzo nell'elenco Mittenti bloccati di un utente, le intestazioni includono il verdetto filtro posta indesiderata "SFV:BLK".

**Autenticazione di posta elettronica dei mittenti** Questo è parzialmente all'interno del controllo da correggere.

Inviare il messaggio per analizzare gli errori nell'autenticazione della posta elettronica del mittente al momento del recapito; i risultati sono disponibili entro un giorno. 

Se si è proprietari dell'infrastruttura di invio, vedere come allinearla a SPF, DKIM e DMARC per assicurarsi che i sistemi di posta elettronica di destinazione ritienino attendibili i messaggi inviati dal dominio. In alternativa, contattare i mittenti per risolvere le configurazioni DNS.

**Verdetti di filtro Microsoft** Questo è parzialmente all'interno del controllo da correggere.

Inviare il messaggio e segnalare il messaggio come sicuro; i risultati dell'analisi sono disponibili entro un giorno. Utilizzare l'elenco tenant consentiti/bloccati quando non si è d'accordo con il filtro dei verdetti in situazioni particolari. Tuttavia, non è consigliabile ignorare i verdetti del filtro Microsoft in modo permanente. 

Per altre informazioni, vedere:

- Consentire agli utenti finali di inviare messaggi a Microsoft. Microsoft usa questi invii per migliorare l'efficacia delle tecnologie di protezione della posta elettronica e vengono visualizzati nei report di invio che possono essere utilizzati come indicazione per aggiornare i criteri. 

- Per guardare un breve video sull'invio dei messaggi per l'analisi, vedere [Submitting messages for analysis](https://go.microsoft.com/fwlink/?linkid=2166435).

- [Usare l'Invio dell'amministratore per inviare posta indesiderata sospetta, phishing, URL e file a Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/admin-submission)

- [Gestire l'elenco di tenant consentiti/bloccati](https://docs.microsoft.com/microsoft-365/security/office-365-security/tenant-allow-block-list)

- [Intestazioni dei messaggi della protezione da posta indesiderata in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)

- [Protezione da posta indesiderata in uscita in EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/outbound-spam-controls)