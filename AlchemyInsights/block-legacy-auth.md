---
title: BlockLegacyAuth
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
- "3154"
- "9001194"
ms.openlocfilehash: 06ded694893c020f862864215700853b19d35f08
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820182"
---
# <a name="blocking-legacy-authentication"></a>Blocco dell'autenticazione legacy

Con il termine autenticazione legacy si fa riferimento a una richiesta di autenticazione effettuata da:

- Client di Office meno recenti che non utilizzano l'autenticazione moderna (ad esempio, client di Office 2010).

- Qualsiasi client che usi protocolli di posta elettronica legacy come IMAP/SMTP/POP3.

Per ulteriori informazioni sul blocco dell'autenticazione legacy e sull'abilitazione dell'autenticazione [moderna,](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication)vedere Blocking legacy authentication .

Le impostazioni predefinite di sicurezza in Azure Active Directory (Azure AD) semplificano la protezione e consentono di proteggere l'organizzazione. Le impostazioni predefinite di sicurezza contengono impostazioni di sicurezza preconfigurate per gli attacchi comuni.
Per ulteriori informazioni sulle impostazioni predefinite di sicurezza, vedere [Che cosa sono le impostazioni predefinite di sicurezza?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults). 

**Nota:** se il tenant è stato creato il 22 ottobre 2019 o dopo il 22 ottobre 2019, è possibile che si verifichi il nuovo comportamento di protezione per impostazione predefinita e che siano già abilitate le impostazioni predefinite di sicurezza nel tenant.  Per proteggere tutti gli utenti, le impostazioni predefinite di sicurezza vengono implementare in tutti i nuovi tenant creati.
