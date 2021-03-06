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
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/05/2021
ms.locfileid: "50500965"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a>Cercare ed eliminare messaggi di posta elettronica nell'organizzazione

Eseguire la procedura seguente:

1. If you're not a global admin, to search for messages your account must be added to the **eDiscovery Manager role group** or **Compliance Search management role**. Per eliminare i messaggi, è necessario aggiungersi al gruppo di ruoli **Gestione** organizzazione o al ruolo di gestione Ricerca **ed eliminazione.** Le autorizzazioni per questi ruoli vengono assegnate nel [Centro sicurezza & conformità.](https://protection.office.com)
2. [Creare una ricerca di contenuto](https://docs.microsoft.com/office365/securitycompliance/content-search) per trovare il messaggio da eliminare.
3. [Connettersi a PowerShell in Centro sicurezza e conformità](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell). Se si usa l'autenticazione a più fattori, vedere queste istruzioni: Connettersi a PowerShell & Centro sicurezza e [conformità con l'autenticazione a più fattori](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)
4. Eliminare il messaggio: eseguire il `New-ComplianceSearchAction` cmdlet per eliminare il messaggio. I messaggi eliminati vengono spostati nella cartella Elementi ripristinabili di un utente. Per un comando di esempio, vedere [Passaggio 3: Eliminare il messaggio.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)
