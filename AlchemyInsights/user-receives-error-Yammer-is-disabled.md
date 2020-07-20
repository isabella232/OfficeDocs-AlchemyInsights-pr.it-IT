---
title: L'utente riceve l'errore AADSTS7000112 Yammer is disabled
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: c92b09ee9a9ca06f85906e7fce601582a7e83244
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 07/16/2020
ms.locfileid: "45157338"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a>L'utente riceve l'errore AADSTS7000112 Yammer is disabled

Se si riceve il messaggio di errore "AADSTS7000112: Application '00000005-0000-0ff1-ce00-000000000000'(Yammer) is disabled", si è verificato un problema con l'entità servizio in Azure AD. Un amministratore potrebbe aver disabilitato l'entità servizio per bloccare l'accesso a Yammer.

La disabilitazione dell'entità servizio non è consigliata e può causare altri problemi. Per altre informazioni sull'approccio supportato per bloccare l'accesso degli utenti a Yammer, vedere [Disattivare l'accesso Yammer per gli utenti di Microsoft 365](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).  

Per risolvere il problema nel portale di Azure e ripristinare l'accesso degli utenti a Yammer:

1.  Aprire la pagina di Azure Active Directory e selezionare **Applicazioni aziendali** in **Gestisci** nel riquadro di spostamento sinistro.
3.  Digitare **Office 365 Yammer** nella casella di ricerca e selezionare il nome dell'applicazione per aprire le impostazioni.
4.  Selezionare **Proprietà** in **Gestisci** nel riquadro di spostamento sinistro.
5.  Impostare il valore **Abilitato per l'accesso degli utenti?** su **Sì**, quindi selezionare **Salva**.
6.  Accedere nuovamente a Yammer. Potrebbe essere necessario cancellare i cookie.

In alternativa, eseguire i comandi di PowerShell per impostare il valore. Per ulteriori informazioni, vedere [Errore "Sorry, but we're having trouble signing you in" quando si fa clic sul riquadro di Yammer in Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365). 