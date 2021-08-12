---
title: Cercare ed eliminare messaggi di posta elettronica nell'organizzazione
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: bd25d9bb2af8114786503e129de105c9a0f602c98b206f01770605d1957e3a1b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53948887"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a>Cercare ed eliminare messaggi di posta elettronica nell'organizzazione

Eseguire la procedura seguente:

1. Se non si è un amministratore globale, per cercare i messaggi è necessario aggiungere l'account al gruppo di ruoli Di **eDiscovery Manager** o al ruolo di gestione **ricerca di conformità**. Per eliminare i messaggi, è necessario aggiungere il gruppo di ruoli **Gestione** organizzazione o il ruolo di gestione Ricerca **ed eliminazione.** Le autorizzazioni per questi ruoli vengono assegnate nel [Centro sicurezza & conformità.](https://protection.office.com)
2. [Creare una ricerca di contenuto](https://docs.microsoft.com/office365/securitycompliance/content-search) per trovare il messaggio da eliminare.
3. [Connettersi a PowerShell in Centro sicurezza e conformità](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell). Se si usa MFA, vedere le istruzioni seguenti: Connessione [a PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell) del Centro sicurezza & conformità con l'autenticazione a più fattori
4. Eliminare il messaggio: eseguire il `New-ComplianceSearchAction` cmdlet per eliminare il messaggio. I messaggi eliminati vengono spostati nella cartella Elementi ripristinabili di un utente. Per un comando di esempio, vedere [Passaggio 3: Eliminare il messaggio.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)
