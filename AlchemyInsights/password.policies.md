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
ms.openlocfilehash: 12751288d04a2ec5993bf4a546b7d0c862f8f171f5bfd7a337cb79cb95792056
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54040834"
---
# <a name="password-policies"></a>Criteri per le password

**Si verificano problemi con i criteri password per un utente**

- I criteri password per un utente dipendono dal fatto che l'utente sia solo cloud o locale.
- Gli utenti solo cloud devono scegliere una password che soddisfi i requisiti di questo articolo: Criteri password che si applicano solo [agli account utente cloud](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)
- Gli utenti locali devono scegliere una password che soddisfi i requisiti locali. Se un utente locale non è in grado di impostare la password, controllare i requisiti locali.

**Non so come impostare o controllare i criteri di scadenza delle password**

- È possibile impostare e controllare i criteri di scadenza per gli utenti cloud nel tenant tramite PowerShell. Seguire le istruzioni in questo articolo: [Impostare o controllare i criteri password tramite PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- I criteri di scadenza delle password per gli utenti locali sono impostati nell'ad locale.

**Altri collegamenti utili:**
- [Introduzione alla reimpostazione della password](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- [Risolvere i problemi relativi alla reimpostazione della password avviata dall'amministratore](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshoot-the-password-reset-portal)
