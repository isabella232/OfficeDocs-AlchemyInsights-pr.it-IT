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
ms.openlocfilehash: e935b10083459b81fc58e12bb59c9511defefa6d
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50737001"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a>Cercare ed eliminare messaggi di posta elettronica nell'organizzazione

Eseguire la procedura seguente:

1. Se non si è un amministratore globale, per cercare i messaggi è necessario aggiungere l'account al gruppo di ruoli Di **eDiscovery Manager** o al ruolo di gestione **ricerca di conformità**. Per eliminare i messaggi, è necessario aggiungere il gruppo di ruoli **Gestione** organizzazione o il ruolo di gestione Ricerca **ed eliminazione.** Le autorizzazioni per questi ruoli vengono assegnate nel [Centro sicurezza & conformità.](https://protection.office.com)
2. [Creare una ricerca di contenuto](https://docs.microsoft.com/office365/securitycompliance/content-search) per trovare il messaggio da eliminare.
3. [Connettersi a PowerShell in Centro sicurezza e conformità](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell). Se si usa MFA, vedere queste istruzioni: [Connettersi a PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell) del Centro sicurezza & conformità usando l'autenticazione a più fattori
4. Eliminare il messaggio: eseguire il `New-ComplianceSearchAction` cmdlet per eliminare il messaggio. I messaggi eliminati vengono spostati nella cartella Elementi ripristinabili di un utente. Per un comando di esempio, vedere [Passaggio 3: Eliminare il messaggio.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)
