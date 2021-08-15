---
title: Accesso all'abbonamento
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003799"
- "6805"
ms.openlocfilehash: b138c05e87e70c18bb6528819a34f8a9501446d57dcf4dbac0734f70fbc3466b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53999244"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a>Impossibile accedere ad Azure a causa di problemi del browser (il browser si blocca, continua a ruotare, non si carica e così via)

È possibile che si sia verificata un'interruzione. Verificare se si è verificata un'interruzione in corso: [Stato di Azure Health.](https://status.azure.com/status/history/)

Disconnettersi da tutte le sessioni di Azure attive. Avviare una modalità in privato o in incognito del Web browser.

Puoi anche provare ad aggiornare il browser, usare un altro browser, eliminare i cookie della cache se non funziona.

Ulteriori informazioni: [Risolvere i problemi di accesso](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)

**Impossibile accedere alle sottoscrizioni**

Nel portale [di Azure](https://portal.azure.com/)assicurati che sia selezionata la directory di Azure corretta nell'account in alto a destra.

Nel Centro [account di Azure,](https://account.windowsazure.com/Subscriptions)assicurati che l'account usato sia l'amministratore dell'account.

Ulteriori informazioni: [Risolvere i problemi relativi alle sottoscrizioni non trovate](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)

**Impossibile accedere alla cronologia della fatturazione**

L'amministratore dell'account deve assicurarsi che l'utente che accede alle informazioni di fatturazione sia aggiunto in Azure Active Directory come utente guest: [Aggiungere o eliminare un nuovo utente.](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support)

All'utente deve quindi essere assegnato un ruolo amministratore globale: [Assegnare il ruolo agli utenti](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

Post this, the user can be given billing access using RBAC policies: [Grant access to billing](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).

**Documenti consigliati**

-   [Non è possibile accedere per gestire la sottoscrizione di Azure](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)