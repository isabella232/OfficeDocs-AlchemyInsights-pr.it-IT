---
title: Criteri per le password
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "9277"
ms.openlocfilehash: 826e266d08aa68c0d4213d8058a0244f404fe965
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50718204"
---
# <a name="password-policies"></a>Criteri per le password

**I'm having problems with the password policy for a user**

- I criteri password per un utente dipendono dal fatto che l'utente sia solo cloud o locale.
- Gli utenti solo cloud devono scegliere una password che soddisfi i requisiti riportati in questo articolo: Criteri per le password che si applicano solo [agli account utente cloud](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)
- Gli utenti locali devono scegliere una password che soddisfi i requisiti locali. Se un utente locale non è in grado di impostare la password, controllare i requisiti locali.

**Non so come impostare o controllare i criteri di scadenza delle password**

- È possibile impostare e controllare i criteri di scadenza per gli utenti cloud nel tenant tramite PowerShell. Seguire le istruzioni in questo articolo: [Impostare o controllare i criteri password tramite PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- I criteri di scadenza delle password per gli utenti locali sono impostati in Active Directory locale.

**Altri collegamenti utili:**
- [Introduzione alla reimpostazione della password](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- [Risoluzione dei problemi relativi alla reimpostazione della password avviata dall'amministratore](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshoot-the-password-reset-portal)
