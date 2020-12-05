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
ms.openlocfilehash: 7c4c9d1a76f395dfb2f831d555199b76c354ca57
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/04/2020
ms.locfileid: "49576527"
---
# <a name="rbac-rules"></a>Regole RBAC

Se viene visualizzato l'errore di autorizzazione: 

- **Il client con ID oggetto non dispone dell'autorizzazione per eseguire l'azione su ambito (codice: AuthorizationFailed)**: quando si tenta di creare una risorsa, verificare di aver eseguito l'accesso con un utente a cui è assegnato un ruolo che disponga dell'autorizzazione di scrittura per la risorsa nell'ambito selezionato. Ad esempio, per gestire le macchine virtuali in un gruppo di risorse, è necessario avere il ruolo di [collaboratore della macchina virtuale](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) nel gruppo di risorse (o nell'ambito padre). Per un elenco delle autorizzazioni per ogni ruolo incorporato, vedere [ruoli incorporati per le risorse di Azure](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).
- **Non si dispone dell'autorizzazione necessaria per creare una richiesta di supporto**: quando si tenta di creare o aggiornare un ticket di supporto, verificare di aver eseguito l'accesso con un utente a cui è assegnato un ruolo che disponga dell'autorizzazione Microsoft. support/supportTickets/Write, ad esempio [supporto richieste collaboratore](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).
- **Non è possibile creare più assegnazioni di ruolo (codice: RoleAssignmentLimitExceeded)**: quando si tenta di assegnare un ruolo, provare a ridurre il numero di assegnazioni di ruolo assegnando invece i ruoli ai gruppi. Azure supporta fino a **2000** assegnazioni di ruolo per ogni sottoscrizione.

Per ulteriori informazioni sui ruoli RBAC di Azure, vedere [ruoli RBAC di Azure](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).
