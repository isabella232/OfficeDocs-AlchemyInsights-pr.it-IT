---
title: Messaggi di posta elettronica mancanti in quarantena
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 43f9a1f03084bf9adab706b3f77eff1d1db888ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831738"
---
# <a name="missing-emails-in-quarantine"></a>Messaggi di posta elettronica mancanti in quarantena"

Gli amministratori [possono visualizzare, rilasciare o eliminare questi messaggi.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

Per aprire il Centro sicurezza & conformità, passare a [https://protection.office.com](https://protection.office.com/) . Per aprire direttamente la pagina Quarantena, passare a [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

È possibile cercare in base ai seguenti valori:  

- **ID messaggio**: identificatore univoco globale del messaggio. Se si seleziona un messaggio nell'elenco, il valore  **ID**  messaggio verrà visualizzato  **nel**  riquadro a comparsa Dettagli visualizzato. Gli amministratori possono usare [Traccia messaggio](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) per trovare i messaggi e i valori ID messaggio corrispondenti.
- **Indirizzo di posta elettronica del mittente**: indirizzo di posta elettronica di un singolo mittente.
- **Indirizzo di posta elettronica del destinatario**: indirizzo di posta elettronica di un singolo destinatario.
- **Oggetto**: utilizzare l'intero oggetto del messaggio. Per la ricerca non viene fatta distinzione tra maiuscole e minuscole.

Dopo aver immesso i criteri di ricerca, fare clic sul ![ pulsante Aggiorna ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Aggiorna** per filtrare i risultati.  

I cmdlet utilizzati per visualizzare e gestire i messaggi e i file in quarantena sono:
- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage:](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage)si noti che questo cmdlet è solo per i messaggi, non per i file di malware da ATP per SharePoint Online, OneDrive for Business o Teams.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)