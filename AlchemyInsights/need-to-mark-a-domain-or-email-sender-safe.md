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
ms.openlocfilehash: a1c4c4d2fadaf75eda9b5b322aca35c32dfee8ea
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51792136"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Contrassegnare un dominio o un mittente di posta elettronica come attendibile

- L'uso degli **elenchi di mittenti attendibili non è consigliabile** poiché espone la propria organizzazione alla posta indesiderata, al phishing e agli attacchi di spoofing.
- Tuttavia, se è presente un requisito aziendale, **è consigliabile** usare le **[Regole dei flussi di posta](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** a tale scopo. La nostra guida garantisce l'autenticazione del mittente: verifica che il dominio di invio non venga contraffatto. **Nota**: non è consigliabile gestire i falsi positivi tramite gli elenchi di mittenti attendibili, perché le eccezioni al filtro della posta indesiderata possono esporre l'organizzazione agli attacchi di sicurezza. Se gli utenti ricevono messaggi non contrassegnati correttamente come posta indesiderata **[segnalare i messaggi e i file a Microsoft](https://protection.office.com/reportsubmission)**.
- I mittenti attendibili in Outlook, l'elenco di mittenti consentiti o l'elenco di domini consentiti nei criteri di posta indesiderata **devono essere evitati** perché i mittenti evitano tutti le protezioni dalla posta indesiderata, lo spoofing e il phishing e l'autenticazione del mittente (SPF, DKIM, DMARC). È consigliabile usare questo metodo solo per test temporanei.
