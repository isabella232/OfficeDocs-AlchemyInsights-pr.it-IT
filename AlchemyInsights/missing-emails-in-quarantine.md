---
title: Messaggi di posta elettronica mancanti in quarantena
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 55ed9a92675939c05477fbf6d12bbedd6eb931d6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673718"
---
# <a name="missing-emails-in-quarantine"></a>Messaggi di posta elettronica mancanti in quarantena "

Gli amministratori possono [visualizzare, rilasciare o eliminare questi messaggi.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

Per aprire il Centro sicurezza & conformità, accedere a [https://protection.office.com](https://protection.office.com/) . Per aprire direttamente la pagina di quarantena, andare a [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

È possibile cercare in base ai seguenti valori:  

- **ID messaggio**: identificatore univoco globale del messaggio. Se si seleziona un messaggio nell'elenco, il valore  **ID messaggio**  verrà visualizzato nel riquadro a comparsa  **Dettagli**  visualizzato. Gli amministratori possono usare [Traccia messaggio](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) per trovare i messaggi e i valori ID messaggio corrispondenti.
- **Indirizzo di posta elettronica del mittente**: indirizzo di posta elettronica di un singolo mittente.
- **Indirizzo di posta elettronica del destinatario**: indirizzo di posta elettronica di un singolo destinatario.
- **Oggetto**: utilizzare l'intero oggetto del messaggio. Per la ricerca non viene fatta distinzione tra maiuscole e minuscole.

Dopo aver immesso i criteri di ricerca, fare clic su Aggiorna ![ pulsante ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Refresh** di aggiornamento per filtrare i risultati.  

I cmdlet utilizzati per visualizzare e gestire i messaggi e i file in quarantena sono i seguenti:
- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): si noti che questo cmdlet è solo per i messaggi, non per i file malware da ATP per SharePoint Online, OneDrive for business o teams.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)