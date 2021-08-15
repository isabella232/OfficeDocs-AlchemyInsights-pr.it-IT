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
ms.openlocfilehash: 900d5f250846e9a7046f72156c150f4970d91d5ad94cb7fc054952228f4bf257
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54026226"
---
# <a name="missing-emails-in-quarantine"></a>Messaggi di posta elettronica mancanti in quarantena"

Gli amministratori [possono visualizzare, rilasciare o eliminare questi messaggi.](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

Per aprire il Centro sicurezza & conformità, passare a [https://protection.office.com](https://protection.office.com/) . Per aprire direttamente la pagina Quarantena, passare a [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

È possibile cercare in base ai seguenti valori:  

- **ID messaggio**: identificatore univoco globale del messaggio. Se si seleziona un messaggio nell'elenco, il valore  **ID**  messaggio verrà visualizzato  **nel**  riquadro a comparsa Dettagli visualizzato. Gli amministratori possono usare [Traccia messaggio](/microsoft-365/security/office-365-security/message-trace-scc) per trovare i messaggi e i valori ID messaggio corrispondenti.
- **Indirizzo di posta elettronica del mittente**: indirizzo di posta elettronica di un singolo mittente.
- **Indirizzo di posta elettronica del destinatario**: indirizzo di posta elettronica di un singolo destinatario.
- **Oggetto**: utilizzare l'intero oggetto del messaggio. Per la ricerca non viene fatta distinzione tra maiuscole e minuscole.

Dopo avere immesso i criteri di ricerca, fare clic sul ![pulsante Aggiorna](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Aggiorna** per filtrare i risultati.

I cmdlet utilizzati per visualizzare e gestire i messaggi e i file in quarantena sono:
- [Delete-QuarantineMessage](/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage](/powershell/module/exchange/preview-quarantinemessage): questo cmdlet è valido solo per i messaggi e non per i file di malware di Microsoft Defender per Office 365 per SharePoint Online, OneDrive for Business o Teams.
- [Release-QuarantineMessage](/powershell/module/exchange/release-quarantinemessage)