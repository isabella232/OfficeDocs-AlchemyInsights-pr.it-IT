---
title: Create user
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003231"
- "9403"
ms.openlocfilehash: a144b172787563b1aa57bdec790df1805a13f078
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323290"
---
# <a name="create-user"></a>Create user

**ANNUNCIO:**

- [Deprecation of WebView sign-in support from Google starting January 4, 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) . Verifica se le tue app potrebbero essere interessate seguendo le indicazioni [di Google](https://go.microsoft.com/fwlink/?linkid=2157323) per testare la compatibilità.
- Assicurati di usare la visualizzazione Web di sistema o il browser di sistema per accedere agli utenti con account Google consumer. Per ulteriori informazioni, vedere [Problemi durante l'accesso alle applicazioni solo tramite il browser Chrome](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).

**Impossibile creare un nuovo utente nella directory Azure AD**

1. Verificare che si disponga dell'autorizzazione per creare un nuovo utente standard. Solo il ruolo amministratore globale o amministratore utente in Azure Active Directory (AD) può creare un nuovo utente standard. Se non di dispone di uno dei ruoli di cui sopra, chiedere a un amministratore di essere aggiunto a uno di questi ruoli o di creare un nuovo account utente.
1. Verificare che il nome utente sia in un dominio verificato in Azure AD. Se non si dispone di un nome dominio verificato personalizzato in Azure AD, è possibile usare il dominio Azure AD iniziale, che termina con *.onmicrosoft.com.
1. Verificare che il nome utente sia in un dominio non federato ad Azure AD dall'istanza locale di AD. Gli utenti non possono essere aggiunti nel cloud con i nomi di dominio federati da istanze locali.
1. Verificare che nessun altro utente o contatto disponga già del nome utente che si desidera assegnare al nuovo utente. I nomi utente devono essere univoci in Azure AD.
1. Vedere [Ruoli e amministratori Azure AD](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) per la propria istanza di Azure AD.
1. Vedere i [nomi di dominio](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) per la propria istanza di Azure AD.
1. Rivedere [Log di audit](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) per ulteriori informazioni su un utente creato o eliminato di recente, come chi abbia eseguito un'azione e quando.
1. Per altre informazioni sull'aggiunta di nuovi utenti, vedi [Usare il portale di Azure per creare un nuovo utente in Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-users-create-azure-portal)
1. [Ruoli amministrativi di Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles): autorizzazioni del ruolo di amministratore in Azure Active Directory
1. È inoltre possibile [usare Azure AD PowerShell per creare un nuovo utente.](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser?view=azureadps-2.0)
