---
title: Contrassegnare un dominio o un mittente di posta elettronica come attendibile
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
- "9002921"
- "5673"
ms.openlocfilehash: 57d1e2d696a8be42b5f868f021d829bf019349bf
ms.sourcegitcommit: 3994cece80410371330b39f7b79b1b1c1bfcf648
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 05/08/2021
ms.locfileid: "52286684"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Contrassegnare un dominio o un mittente di posta elettronica come attendibile

- L'uso degli **elenchi di mittenti attendibili non è consigliabile** poiché espone la propria organizzazione alla posta indesiderata, al phishing e agli attacchi di spoofing.
- Tuttavia, se è presente un requisito aziendale, **è consigliabile** usare le **[Regole dei flussi di posta](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** a tale scopo. La nostra guida garantisce l'autenticazione del mittente: verifica che il dominio di invio non venga contraffatto. **Nota**: non è consigliabile gestire i falsi positivi tramite gli elenchi di mittenti attendibili, perché le eccezioni al filtro della posta indesiderata possono esporre l'organizzazione agli attacchi di sicurezza. Se gli utenti ricevono messaggi non contrassegnati correttamente come posta indesiderata **[segnalare i messaggi e i file a Microsoft](https://protection.office.com/reportsubmission)**.
- I mittenti attendibili in Outlook, l'elenco dei mittenti consentiti o l'elenco dei domini consentiti nei criteri antispam **devono essere evitati** perché i mittenti ignorano tutte le protezioni per la posta indesiderata, lo spoofing, il phishing e l'autenticazione del mittente (SPF, DKIM, DMARC). Questo metodo è usato solo per i test temporanei.
- Per convalidare se un determinato messaggio di posta elettronica ha ignorato la valutazione antispam è possibile controllare l'intestazione del messaggio "X-Forefront-Antispam-Report" (SFV: SFE, SFV: SKA, SFV: SKN), vedere **[Intestazioni dei messaggi della protezione da posta indesiderata in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)**.
- Poiché Microsoft vuole garantire ai clienti la [protezione per impostazione predefinita](https://docs.microsoft.com/microsoft-365/security/office-365-security/secure-by-default#exceptions), alcuni criteri di override del tenant non vengono applicati ai malware e ai phishing ad alta probabilità. Questi override includono: o   Elenchi di mittenti o di domini consentiti (criteri contro la posta indesiderata) o   Mittenti attendibili di Outlook o   Elenco di indirizzi IP consentiti (filtro connessioni) 
- L'unico override che consente ai messaggi di phishing ad alta probabilità di aggirare il filtro sono le regole del flusso di posta di Exchange (note anche come regole di trasporto). Per usare le regole del flusso di posta per ignorare i filtri, vedere **[Usare le regole del flusso di posta per impostare il livello di confidenza di posta indesiderata (SCL) nei messaggi](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-mail-flow-rules-to-set-the-spam-confidence-level-scl-in-messages)**.