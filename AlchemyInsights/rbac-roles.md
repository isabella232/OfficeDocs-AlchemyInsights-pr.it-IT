---
title: 'Ruoli RBAC '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "7265"
ms.openlocfilehash: 1faa9f69942d39b8d78c8f3e1316f93b52eeede6408dfabc89d0f7fe38b86fb3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923135"
---
# <a name="rbac-rules"></a>Regole RBAC

Se viene visualizzato l'errore di autorizzazione: 

- Il client con ID oggetto non dispone dell'autorizzazione per eseguire azioni sull'ambito **(codice: AuthorizationFailed):** quando si tenta di creare una risorsa, verificare di aver effettuato l'accesso con un utente a cui è assegnato un ruolo che dispone dell'autorizzazione di scrittura per la risorsa nell'ambito selezionato. Ad esempio, per gestire le macchine virtuali in [](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) un gruppo di risorse, è necessario disporre del ruolo Collaboratore macchina virtuale nel gruppo di risorse (o nell'ambito padre). Per un elenco delle autorizzazioni per ogni ruolo incorporato, vedere [Ruoli predefiniti per le risorse di Azure.](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support)
- Non si dispone dell'autorizzazione per creare una richiesta di supporto: quando si tenta di creare o aggiornare un ticket di supporto, verificare di aver effettuato l'accesso con un utente a cui è assegnato un ruolo con **l'autorizzazione** Microsoft.Support/supportTickets/write, ad esempio Collaboratore richiesta di [supporto.](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor)
- Non è possibile creare altre assegnazioni di ruolo **(codice: RoleAssignmentLimitExceeded):** quando si tenta di assegnare un ruolo, provare a ridurre il numero di assegnazioni di ruolo assegnando ruoli ai gruppi. Azure supporta fino a **2000 assegnazioni** di ruolo per sottoscrizione.

Per ulteriori dettagli sui ruoli RBAC di Azure, vedere [Ruoli RBAC di Azure](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).
