---
title: Risoluzione dei problemi relativi agli eventi da posta elettronica
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
- "9000301"
- "5765"
ms.openlocfilehash: 2cea347f248a3b04873428946f1817657af04773
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834843"
---
# <a name="troubleshooting-events-from-email"></a>Risoluzione dei problemi relativi agli eventi da posta elettronica

1. Verificare che la funzionalità sia abilitata per la cassetta postale: **Get-EventsFromEmailConfiguration -Identity <mailbox>**

2. Osservare quindi i log "Eventi da posta elettronica" **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**

3. Nei log casella "Eventi da posta elettronica" trovare il valore InternetMessageId che corrisponde all'elemento nella cassetta postale.  

4. Il valore TrustScore determina se l'elemento viene aggiunto o meno. Gli eventi verranno aggiunti solo se TrustScore = "Trusted".

Il valore TrustScore è determinata dalle proprietà SPF, DKIM o DMARC, che si trovano nell'intestazione del messaggio.

Per visualizzare queste proprietà:

**Outlook desktop**

- Aprire l'elemento
- File -> Proprietà -> Intestazioni Internet

oppure

**MFCMapi**

- Passare all'elemento nella cartella di posta in arrivo
- Cercare PR_TRANSPORT_MESSAGE_HEADERS_W

Queste proprietà sono determinate e registrate durante il trasporto e il routing. Per altre informazioni sulla risoluzione dei problemi, potrebbe essere necessario continuare con il supporto del trasporto per i problemi in SPF, DKIM e DMARC.