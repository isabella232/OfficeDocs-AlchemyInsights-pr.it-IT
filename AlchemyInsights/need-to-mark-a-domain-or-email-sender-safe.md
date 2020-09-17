---
title: Contrassegnare un dominio o un mittente di posta elettronica come attendibile
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 0ea089b95ad7de25e77017196fb2db895d4d0178
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47803249"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="ecce9-102">Contrassegnare un dominio o un mittente di posta elettronica come attendibile</span><span class="sxs-lookup"><span data-stu-id="ecce9-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="ecce9-103">L'uso degli **elenchi di mittenti attendibili non è consigliabile** poiché espone la propria organizzazione alla posta indesiderata, al phishing e agli attacchi di spoofing.</span><span class="sxs-lookup"><span data-stu-id="ecce9-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="ecce9-104">Tuttavia, se è presente un requisito aziendale, **è consigliabile** usare le **[Regole dei flussi di posta](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** a tale scopo.</span><span class="sxs-lookup"><span data-stu-id="ecce9-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="ecce9-105">La nostra guida garantisce l'autenticazione del mittente: verifica che il dominio di invio non venga contraffatto.</span><span class="sxs-lookup"><span data-stu-id="ecce9-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="ecce9-106">**Nota**: non è consigliabile gestire i falsi positivi tramite gli elenchi di mittenti attendibili, perché le eccezioni al filtro della posta indesiderata possono esporre l'organizzazione agli attacchi di sicurezza.</span><span class="sxs-lookup"><span data-stu-id="ecce9-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="ecce9-107">Se gli utenti ricevono messaggi non contrassegnati correttamente come posta indesiderata **[segnalare i messaggi e i file a Microsoft](https://protection.office.com/reportsubmission)**.</span><span class="sxs-lookup"><span data-stu-id="ecce9-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="ecce9-108">I mittenti attendibili in Outlook, l'elenco di mittenti consentiti o l'elenco di domini consentiti nei criteri di posta indesiderata **devono essere evitati** perché i mittenti evitano tutti le protezioni dalla posta indesiderata, lo spoofing e il phishing e l'autenticazione del mittente (SPF, DKIM, DMARC).</span><span class="sxs-lookup"><span data-stu-id="ecce9-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="ecce9-109">È consigliabile usare questo metodo solo per test temporanei.</span><span class="sxs-lookup"><span data-stu-id="ecce9-109">This method is best used for temporary testing only.</span></span>
