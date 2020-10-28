---
title: Accesso alla sottoscrizione
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
ms.openlocfilehash: 166380cff09f2a2bd9b7e8914d5db4071b6c3f12
ms.sourcegitcommit: bec3554bf061ef28a009f460fb9d0a661b4fc008
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 10/27/2020
ms.locfileid: "48773775"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a>Non è possibile accedere a Azure a causa di problemi del browser (il browser si blocca, continua a girare, non viene caricato, ecc.)

Potrebbe essere influito su un'interruzione. Controllare se è presente un'interruzione continua: stato di integrità di [Azure](https://status.azure.com/status/history/).

Disconnettersi da tutte le sessioni di Azure attive. Avviare una modalità privata o in incognito del Web browser.

È inoltre possibile provare a aggiornare il browser, utilizzare un altro browser, eliminare i cookie della cache se sopra non funziona.

Per ulteriori informazioni, vedere [risolvere i problemi di accesso](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)

**Impossibile accedere alle sottoscrizioni**

Nel [portale di Azure](https://portal.azure.com/), verificare che la directory di Azure corretta sia selezionata dall'account in alto a destra.

Nel [centro account di Azure](https://account.windowsazure.com/Subscriptions), verificare che l'account utilizzato sia l'amministratore dell'account.

Ulteriori informazioni: [risoluzione dei problemi relativi a nessuna sottoscrizione trovata](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)

**Impossibile accedere alla cronologia di fatturazione**

L'amministratore dell'account deve accertarsi che l'utente che accede alle informazioni sulla fatturazione sia stato aggiunto in Azure Active Directory come utente Guest: [aggiungere o eliminare un nuovo utente](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

All'utente deve quindi essere assegnato un ruolo di amministratore globale: [assegnare il ruolo agli utenti](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

Dopo questo, all'utente può essere assegnato l'accesso alla fatturazione usando i criteri RBAC: [concedere l'accesso alla fatturazione](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).

**Documenti consigliati**

-   [Non è possibile accedere per gestire la sottoscrizione di Azure](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)