---
title: Risolvere i problemi degli utenti guest
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
ms.openlocfilehash: 9e6030919721b4c0805a26ca45d365f31d88894e86ea08225f47576e7d152047
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939383"
---
# <a name="troubleshoot-guest-user-issues"></a>Risolvere i problemi degli utenti guest

1. Per indicazioni sulla gestione dell'accesso guest alle applicazioni, vedere [Manage guest access with Azure AD access reviews](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews).
1. Aggiungere utenti guest alla directory nel portale di [Azure:](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal)in questa guida introduttiva, si aggiungerà un nuovo utente guest alla directory di Azure AD tramite il portale di Azure, si invierà un invito e verrà visualizzato l'aspetto del processo di riscatto degli inviti dell'utente guest.
1. [Aggiungere un utente guest con PowerShell:](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell)in questa guida introduttiva verrà utilizzato il comando New-AzureADMSInvitation per aggiungere un utente guest al tenant di Azure.
1. Per informazioni su come assegnare utenti e gruppi alle applicazioni aziendali in Azure Active Directory (Azure AD), all'interno del portale di Azure o tramite PowerShell, vedere [Manage user assignment for an app in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal). 
1. Azure Active Directory collaborazione B2B (Azure AD) funziona con la maggior parte delle app che si integrano con Azure AD. In questo [articolo](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps)vengono fornite istruzioni dettagliate per configurare alcune app SaaS più popolari da usare con Azure AD B2B.
1. In quanto organizzazione che usa le funzionalità di collaborazione B2B di Azure Active Directory (Azure AD) per invitare gli utenti guest dalle organizzazioni partner ad Azure AD, ora puoi fornire a questi utenti B2B l'accesso alle app locali. Queste app locali possono usare l'autenticazione basata su SAML o L'autenticazione Windows integrata (IWA) con la delega vincolata Kerberos (KCD). Per ulteriori informazioni, vedere [Concedere agli utenti B2B in Azure AD l'accesso alle applicazioni locali.](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises)
1. Informazioni su come concedere agli account partner gestiti localmente l'accesso alle risorse [cloud usando la collaborazione B2B di Azure AD.](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud)