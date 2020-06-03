---
title: Risoluzione dei problemi relativi agli eventi da posta elettronica
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: e27589b7f6730036040b948b6275cef072fd8235
ms.sourcegitcommit: dc149ab45fbc2c974b54fb81156d2bc1b07017bb
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44515990"
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