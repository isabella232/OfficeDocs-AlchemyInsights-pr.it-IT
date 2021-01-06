---
title: Come aggiungere e gestire gli amministratori-procedura consigliata
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
ms.openlocfilehash: ed3aa5defabdd4f505ee4f74570023d990910dcb
ms.sourcegitcommit: 04bf13605a30ad4a2218ad9e94dcffcee4cc9aa6
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/05/2021
ms.locfileid: "49755839"
---
# <a name="how-to-add-and-manage-administrators---recommended-steps"></a>Come aggiungere e gestire gli amministratori-procedura consigliata

In base alla descrizione del problema, è stata trovata una soluzione per l'utente. La maggior parte dei clienti è stata in grado di risolvere il problema da solo dopo aver seguito la nostra documentazione.

**Modificare l'amministratore della sottoscrizione o il coamministratore**

- L'amministratore dell'account può modificare entrambi i ruoli, mentre l'amministratore della sottoscrizione può modificare solo gli amministratori del [portale di Azure](https://ms.portal.azure.com/#home).
- [Aggiungere o modificare gli amministratori delle sottoscrizioni di Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

**Aggiornare l'amministratore della sottoscrizione o Co-Administrator per le sottoscrizioni interne (arie)**

L'amministratore del servizio o il coamministratore può gestire autonomamente questa azione attenendosi alla procedura seguente:

1. Accedere al portale di [Azure](https://ms.portal.azure.com/#home) e fare clic su **Cost Management + Billing** nel Blade sinistro.
2. Fare clic sull'elemento pubblicitario con l'abbonamento. In questo articolo viene aperta la panoramica dell'abbonamento.
3. Nel Blade **sottoscrizione** , fare clic su **Proprietà**. 
4. Fare clic sul pulsante di **amministrazione del servizio** .
5. Immettere l'indirizzo di posta elettronica dell'utente che si desidera impostare come amministratore del servizio e fare clic su **OK**.

**Aggiungi/modifica/Rimuovi coamministratore**

1. Accedere al portale di [Azure](https://ms.portal.azure.com/#home) come amministratore del servizio.
2. Aprire le [sottoscrizioni](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) e selezionare un abbonamento. (Il co-amministratori può essere assegnato solo nell'ambito della sottoscrizione).
3. Passare a **controllo di accesso (IAM)**  >  gli **amministratori classici**  >  **aggiungono**  >  **Aggiungi coamministratore** per aprire il riquadro **Aggiungi co-** amministratore (se l'opzione Aggiungi coamministratore è disabilitata, indica che non si dispone delle autorizzazioni).
4. Selezionare l'utente che si desidera aggiungere e fare clic su **Aggiungi**.

**Ulteriori informazioni:**
- [Aggiungere un coamministratore](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Rimuovere un coamministratore](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Modificare l'amministratore del servizio](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Visualizzare l'amministratore dell'account](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Gestire l'accesso tramite RBAC e il portale di Azure](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

**Aggiungere/eliminare utenti che utilizzano Azure Active Directory (AD)**

È possibile aggiungere nuovi utenti o eliminare utenti esistenti dall'organizzazione di Azure Active Directory (Azure AD):

1. Per aggiungere un nuovo utente, eseguire l'accesso al [portale di Azure](https://ms.portal.azure.com/#home) come amministratore dell'organizzazione.
2. Selezionare **Azure Active Directory**, selezionare **utenti** e quindi fare clic su **nuovo utente**.
3. Nella pagina **utente** , compilare le informazioni necessarie. Fare clic su **Crea**. L'utente viene creato e aggiunto al tenant di Azure AD.

Per ulteriori **informazioni**, vedere:

- [Aggiungere un nuovo utente](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Eliminare un utente](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Aggiungere o aggiornare le informazioni del profilo di un utente tramite Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

**Documenti consigliati**

- [Che cos'è il controllo di accesso basato sui ruoli (RBAC)?](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [Comprendere i diversi ruoli in Azure](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [Autorizzazioni del ruolo di amministratore in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [Esercitazione: concedere l'accesso per un utente tramite RBAC e il portale di Azure](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [Risoluzione dei problemi relativi a RBAC in Azure](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [Organizzare le risorse con i gruppi di gestione di Azure](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [Come richiedere una copia della fattura di Azure tramite posta elettronica](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [Informazioni su come aggiungere, aggiornare o rimuovere una carta di credito o di debito da Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [Sottoscrizione di gestione (riattivazione/annullamento/commutazione)](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



