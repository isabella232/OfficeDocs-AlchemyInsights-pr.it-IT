---
title: Contrassegnare un dominio o un mittente di posta elettronica come attendibile
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 7dc1576fd61e87b319c7486c59ed125943b4d959
ms.sourcegitcommit: 43acdecef129bfffc8bbe8ebb08fdd581b238a03
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 05/18/2020
ms.locfileid: "44281176"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Contrassegnare un dominio o un mittente di posta elettronica come attendibile

- L'uso degli **elenchi di mittenti attendibili non è consigliabile** poiché espone la propria organizzazione alla posta indesiderata, al phishing e agli attacchi di spoofing.
- Tuttavia, se è presente un requisito aziendale, **è consigliabile** usare le **[Regole dei flussi di posta](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** a tale scopo. La nostra guida garantisce l'autenticazione del mittente: verifica che il dominio di invio non venga contraffatto. **Nota**: non è consigliabile gestire i falsi positivi tramite gli elenchi di mittenti attendibili, perché le eccezioni al filtro della posta indesiderata possono esporre l'organizzazione agli attacchi di sicurezza. Se gli utenti ricevono messaggi non contrassegnati correttamente come posta indesiderata **[segnalare i messaggi e i file a Microsoft](https://protection.office.com/reportsubmission)**.
- I mittenti attendibili in Outlook, l'elenco di mittenti consentiti o l'elenco di domini consentiti nei criteri di posta indesiderata **devono essere evitati** perché i mittenti evitano tutti le protezioni dalla posta indesiderata, lo spoofing e il phishing e l'autenticazione del mittente (SPF, DKIM, DMARC). È consigliabile usare questo metodo solo per test temporanei.
