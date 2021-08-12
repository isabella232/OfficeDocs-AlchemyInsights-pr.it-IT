---
title: Come aggiungere e gestire gli amministratori - Passaggi consigliati
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/07/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7194"
ms.openlocfilehash: 5aa6f11d31ed62078fdd05090af5722289544c5ab2244a369182f4e0f9214183
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53963791"
---
# <a name="how-to-add-and-manage-administrators---recommended-steps"></a>Come aggiungere e gestire gli amministratori - Passaggi consigliati

In base alla descrizione del problema, è stata trovata una soluzione. La maggior parte dei clienti è riuscita a risolvere il problema da sola dopo aver seguito la documentazione.

**Modificare l'amministratore della sottoscrizione o il co-amministratore**

- L'amministratore dell'account può modificare entrambi i ruoli, mentre l'amministratore della sottoscrizione può modificare solo i co-amministratori nel [portale di Azure.](https://ms.portal.azure.com/#home)
- [Aggiungere o modificare gli amministratori della sottoscrizione di Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

**Aggiornare l'amministratore della sottoscrizione o Co-Administrator per le sottoscrizioni interne (AIRS)**

L'amministratore del servizio o il co-amministratore può eseguire questa azione autonomamente utilizzando la procedura seguente:

1. Accedi al portale [di Azure e fai](https://ms.portal.azure.com/#home) clic su Gestione costi + **Fatturazione** nel pannello sinistro.
2. Fai clic sulla voce con l'abbonamento. Verrà visualizzata la panoramica per l'abbonamento.
3. Nel pannello **Sottoscrizione** fare clic su **Proprietà.** 
4. Fai clic **sul pulsante Service Admin.**
5. Immettere il messaggio di posta elettronica dell'utente che si desidera impostare come amministratore del servizio e fare clic su **OK.**

**Aggiungi/Cambia/Rimuovi co-amministratore**

1. Accedere al portale [di Azure come](https://ms.portal.azure.com/#home) amministratore del servizio.
2. Aprire [Sottoscrizioni](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) e selezionare una sottoscrizione. I co-amministratori possono essere assegnati solo nell'ambito della sottoscrizione.
3. Passare a Controllo di accesso **(IAM)** Amministratori classici Aggiungi coamam per aprire il riquadro Aggiungi  >    >    >   **co-amministratore** (se l'opzione Aggiungi coam amministratore è disabilitata, significa che non si dispone delle autorizzazioni).
4. Selezionare l'utente che si desidera aggiungere e fare clic su **Aggiungi.**

**Ulteriori informazioni:**
- [Aggiungere un co-amministratore](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Rimuovere un co-amministratore](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Modificare l'amministratore del servizio](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Visualizzare l'amministratore account](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Gestire l'accesso tramite RBAC e portale di Azure](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

**Aggiungere/eliminare utenti con Azure Active Directory (AD)**

È possibile aggiungere nuovi utenti o eliminare gli utenti esistenti dall'organizzazione Azure Active Directory (Azure AD):

1. Per aggiungere un nuovo utente, accedere al portale [di Azure](https://ms.portal.azure.com/#home) come amministratore utente per l'organizzazione.
2. Selezionare **Azure Active Directory**, selezionare **Utenti** e quindi fare clic su **Nuovo utente**.
3. Nella **pagina Utente** compilare le informazioni necessarie. Fai clic su **Crea**. L'utente viene creato e aggiunto al tenant di Azure AD.

**Ulteriori informazioni:**

- [Aggiungere un nuovo utente](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Eliminare un utente](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Aggiungere o aggiornare le informazioni del profilo di un utente Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

**Documenti consigliati**

- [Che cos'è il controllo di accesso basato sui ruoli ??](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [Comprendere i diversi ruoli in Azure](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [Autorizzazioni del ruolo di amministratore in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [Esercitazione: Concedere l'accesso a un utente tramite RBAC e il portale di Azure](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [Risolvere i problemi relativi al controllo degli accessi in base al ruolo in Azure](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [Organizzare le risorse con i gruppi di gestione di Azure](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [Come richiedere la copia della fattura di Azure tramite posta elettronica](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [Come aggiungere, aggiornare o rimuovere una carta di credito o di debito da Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [Gestire (riattivare/annullare/cambiare) sottoscrizione](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



