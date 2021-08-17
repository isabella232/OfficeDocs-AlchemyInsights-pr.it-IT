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
ms.openlocfilehash: b6a8b2a1174f04a1e0ed0fdee9a954bb3bf108038f0804353d84755e490f5f47
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105356"
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