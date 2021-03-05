---
title: Risoluzione dei problemi relativi a SSPR
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.topic: article
ms.audience: Admin
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "6128"
ms.openlocfilehash: 85bfc812dcffce008a6fa5394a6069bd64c514d6
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/04/2021
ms.locfileid: "50428831"
---
# <a name="troubleshoot-sspr"></a>Risoluzione dei problemi relativi a SSPR

**I'm having trouble configuring password reset**

- Se si è amministratori e si sta cercando informazioni su come abilitare la reimpostazione della password in modalità self-service, vedere [Tutorial enable SSPR](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr), per configurare la reimpostazione della password per l'organizzazione. È inoltre possibile esaminare i requisiti [di licenza.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support) È necessario disporre di almeno una licenza assegnata nell'organizzazione.
    - **Utenti solo cloud** - Qualsiasi SKU a pagamento di Office 365 (O365) o Azure AD Basic
    - **Utenti cloud e/o** locali : Azure AD Premium P1 o P2, Enterprise Mobility + Security (EMS) o Secure Productive Enterprise (SPE)
- Per altre domande sulla reimpostazione della password self-service, consultare [le domande frequenti.](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support)

**Viene visualizzato un messaggio di errore**

Leggere questo articolo per individuare gli errori comuni e le relative soluzioni: [risolvere i problemi relativi alla reimpostazione della password self-service](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)

**Si è verificato un problema con il criterio di reimpostazione della password**

- Se il criterio di reimpostazione della password non si comporta come previsto o se hai domande sui criteri di reimpostazione delle password, leggi questo articolo: Criteri e restrizioni per le password [in Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support)
- I criteri di reimpostazione della password non si applicano agli amministratori. Microsoft applica un criterio predefinito di reimpostazione della password a due porte per qualsiasi ruolo di amministratore di Azure. Assicurarsi di eseguire test con un utente che non è un amministratore. Per ulteriori informazioni sui criteri di reimpostazione dell'amministratore, vedere questo articolo: [Differenze dei criteri di reimpostazione dell'amministratore.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences)

**I don't want my users to register additional security info for password reset**

Puoi precompilare i dati (attributi di posta elettronica e telefono) per gli utenti usando un'API, PowerShell o Azure AD Connect. Per informazioni su come leggere:

- [Distribuzione della reimpostazione della password senza richiedere agli utenti di registrarsi](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [Quali dati vengono utilizzati dalla reimpostazione della password](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Voglio che gli utenti registrino le informazioni di sicurezza aggiuntive per la reimpostazione della password**

1. Fare in modo che gli utenti registrino le informazioni di sicurezza per la reimpostazione della password self-service indirizzandoli [a aka.ms/ssprsetup](https://mysignins.microsoft.com/security-info).
1. Dopo aver popolato i dati per l'utente (dall'utente o dall'amministratore), indirizzare l'utente [a aka.ms/sspr](https://passwordreset.microsoftonline.com/) in modo che gli utenti possano essere autorizzati a reimpostare le proprie password.
1. Se gli utenti riscontrano ancora problemi, è molto probabile che siano utenti **federati** o sincronizzati **con hash delle password.** Ciò significa che è probabile che si sia verificato un problema con il servizio writeback delle password.