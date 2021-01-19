---
title: Risoluzione dei problemi relativi agli utenti Guest
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004358"
- "7822"
ms.openlocfilehash: 0f2a10b918fee067b167ab58ac2544a89e0c8ea1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/18/2021
ms.locfileid: "49897748"
---
# <a name="troubleshoot-guest-user-issues"></a>Risoluzione dei problemi relativi agli utenti Guest

1. Per istruzioni sulla gestione dell'accesso guest alle applicazioni, vedere Gestione dell'accesso [Guest con le recensioni di Azure ad Access](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews).
1. [Aggiungere gli utenti guest alla directory nel portale di Azure](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal): in questa Guida introduttiva, è possibile aggiungere un nuovo utente guest alla directory di Azure ad tramite il portale di Azure, inviare un invito e vedere cosa assomiglia al processo di riscatto dell'invito dell'utente ospite.
1. [Aggiungere un utente guest con PowerShell](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell): in questa Guida introduttiva, è possibile utilizzare il comando New-AzureADMSInvitation per aggiungere un utente Guest al tenant di Azure.
1. Per informazioni su come assegnare utenti e gruppi a applicazioni Enterprise in Azure Active Directory (Azure AD), dall'interno del portale di Azure o tramite PowerShell, vedere [Manage User Assignment for an app in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal). 
1. La collaborazione B2B di Azure Active Directory (Azure AD) è compatibile con la maggior parte delle app che si integrano con Azure AD. In questo [articolo](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps)vengono illustrate le istruzioni per la configurazione di alcune famose app SaaS per l'utilizzo con Azure ad B2B.
1. Come organizzazione che utilizza le funzionalità di collaborazione B2B di Azure Active Directory (Azure AD) per invitare gli utenti Guest dalle organizzazioni partner a Azure AD, è ora possibile fornire a questi utenti B2B l'accesso alle app locali. Queste app locali possono utilizzare l'autenticazione basata su SAML o l'autenticazione integrata di Windows (IWA) con la delega vincolata Kerberos (KCD). Per ulteriori informazioni, vedere [concedere agli utenti di B2B nell'accesso ad Azure ad le applicazioni locali](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises).
1. Informazioni su come [concedere agli account partner gestiti localmente l'accesso alle risorse cloud tramite la collaborazione di Azure ad B2B](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud).