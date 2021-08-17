---
title: Gli utenti hanno ricevuto messaggi pericolosi
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002907"
- "5594"
- "3100017"
- "2578"
ms.openlocfilehash: 608e2226c055f58ecf4f62e3c913106a6d319190ed6b317508e41514c12ba5d0
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/11/2021
ms.locfileid: "57893407"
---
# <a name="did-your-users-receive-malicious-email"></a>Gli utenti hanno ricevuto messaggi pericolosi?

È ora possibile segnalare un'e-mail dannosa a Microsoft usando gli [invii nel portale di Microsoft 365 Defender](https://sip.security.microsoft.com/reportsubmission?viewid=admin).

I messaggi segnalati negli [invii degli amministratori](https://security.microsoft.com/reportsubmission?viewid=admin) vengono analizzati e nel riquadro a comparsa dei dettagli vengono visualizzati i risultati seguenti:

- Se si è verificato un errore nell'autenticazione della posta elettronica del mittente al momento del recapito.
- Informazioni su eventuali riscontri dei criteri che potrebbero aver influenzato o sostituito il verdetto di un messaggio.
- Risultati della detonazione correnti per verificare se gli URL o i file contenuti nel messaggio erano dannosi o meno.
- Feedback da parte di valutatori

Se è stata trovata un override, la nuova analisi dovrebbe essere completata dopo alcuni minuti. Se non si è verificato un problema nell'autenticazione della posta elettronica o il recapito non è stato influenzato da una sostituzione, per il feedback da parte dei valutatori potrebbe essere necessario fino a un giorno.

Se non si è d'accordo con il risultato finale su un messaggio, un URL o un file (bloccato o non bloccato), inviare di nuovo il messaggio dopo un giorno per ripetere l'analisi. È molto probabile che il verdetto cambi dopo aver inviato di nuovo il messaggio.

Nel frattempo, è possibile rimuovere il messaggio di posta elettronica dannoso dalla casella di Posta in arrivo dell'utente seguendo le istruzioni in [questo articolo](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).

- I clienti che hanno Microsoft Defender per Office 365 possono:
  - Usare [Esplora minacce per trovare ed eliminare i messaggi sospetti](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)
  - [Usare i collegamenti sicuri per bloccare l'accesso](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-links) a un URL dannoso
  - Tenere traccia degli utenti che hanno fatto clic ed eseguito l'accesso a URL dannosi: [Visualizzare l'URL di phishing e fare clic sui dati del verdetto](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-Url Track](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)
  - [Avviare manualmente una indagine automatizzata](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)

Ci si può proteggere da file e URL dannosi anche seguendo le istruzioni fornite in [Protezione da URL e file dannosi](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).
