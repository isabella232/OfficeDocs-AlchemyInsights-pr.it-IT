---
title: Problemi con le credenziali
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
- "9004330"
- "7723"
ms.openlocfilehash: e463e8181123277f3509c0b0bb6f871a1a09bed1
ms.sourcegitcommit: c3574f574afe5a40a6ea2c6e399c58977d18bb73
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/29/2021
ms.locfileid: "50052949"
---
# <a name="issues-with-credentials"></a>Problemi con le credenziali

Microsoft Identity Platform e il flusso delle credenziali [client OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) descrivono come programmare direttamente in base al flusso di concessione delle credenziali client OAuth 2.0.

**Come si gestiscono le credenziali della password o del certificato di un'applicazione?**

Nell'interfaccia cli di Azure puoi usare le credenziali [dell'app](https://docs.microsoft.com/cli/azure/ad/app/credential) pubblicitaria az per eliminare, elencare o reimpostare la password o le credenziali del certificato di un'applicazione.

**In che modo gli utenti reimpostano le password?**

Gli utenti devono [registrarsi per la reimpostazione della password self-service](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) prima di poter reimpostare le password. Dopo la registrazione, un utente può seguire le istruzioni riportate in questo articolo per reimpostare la password: Reimpostare la password dell'istituto di [istruzione o dell'istituto di istruzione.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account)

**In che modo gli utenti cambiano le password?**

Gli utenti possono seguire i passaggi descritti in questo articolo per cambiare le password: [Come modificare la password.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password)
Possono anche gestire [le password delle app per la verifica in due passaggi.](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords)

**L'utente riceve un errore durante la modifica o la reimpostazione della password**

Questo collegamento fornirà informazioni sui problemi comuni che possono verificarsi quando un utente tenta di reimpostare la password: [problemi comuni e relative soluzioni](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)

**Si è verificato un problema durante la reimpostazione della password di un utente**

- Assicurarsi di essere autorizzati a reimpostare le password. *Solo gli amministratori globali, delle password e degli utenti possono reimpostare le password degli utenti.* Gli amministratori globali possono anche reimpostare le password di altri amministratori con privilegi.

- Assicurarsi di comprendere i requisiti di licenza:

  - È necessario disporre di almeno una licenza assegnata nell'organizzazione:
    - **Utenti solo cloud** - Qualsiasi SKU a pagamento di Office 365 (O365) o Azure AD Basic
    - **Utenti cloud e/o** locali : Azure AD Premium P1 o P2, Enterprise Mobility + Security (EMS) o Secure Productive Enterprise (SPE)
    - Per altre informazioni sui requisiti di licenza, vedere [Requisiti di licenza per la reimpostazione della password in modalità self-service di Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- Per reimpostare la password di un utente, trova l'utente in Azure AD. Quindi, nel pannello di panoramica per l'utente, fare clic sul pulsante "reimposta password".

**Il pulsante di reimpostazione della password è in grigio**

Non si è autorizzati a reimpostare **le password** di questo utente. *Solo gli amministratori globali, delle password e degli utenti possono reimpostare le password degli utenti.* Gli amministratori globali possono anche reimpostare le password di altri amministratori con privilegi.

**Il pannello di reimpostazione della password non è visualizzato**

Non si è autorizzati a reimpostare le password. *Solo gli amministratori globali, delle password e degli utenti possono reimpostare le password degli utenti.* Gli amministratori globali possono anche reimpostare le password di altri amministratori con privilegi.

**Il pannello di integrazione locale non viene visualizzato nella reimpostazione della password**

- Il pannello di integrazione locale viene visualizzato solo negli ambienti ibridi, ovvero si utilizza il writeback delle password per modificare le password degli utenti locali.

- Questo pannello non viene visualizzato se:

  - Non si utilizza il writeback delle password
  - Si è verificato un problema con l'installazione/connettività del writeback delle password
  - Si è verificato un problema con l'installazione/connettività di Azure AD Connect
  - Per ulteriori procedure di risoluzione dei problemi relativi al writeback delle password, vedere [Risolvere i problemi relativi al writeback delle password](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)

**Non so come reimpostare la password di un utente**

1. Accedere al portale di Azure come amministratore appropriato.
2. Passare al pannello **Utenti e gruppi,** selezionare **Tutti gli utenti.**
3. Selezionare un utente dall'elenco.
4. Per l'utente selezionato, selezionare **Panoramica** e quindi nella barra dei comandi selezionare **Reimposta password.**
5. Seleziona il **pulsante Reimposta password** e segui le istruzioni visualizzate sullo schermo.
    - Solo le reimpostazioni eseguite tramite il **portale di Azure supportano** il writeback delle password.

**Reimpostazione della password di un utente locale dal portale di amministrazione di Office 365 o dall'applicazione per dispositivi mobili di Office 365, ma l'utente non è ancora in grado di accedere**

Il writeback delle password non è supportato in questo portale. Reimpostare di nuovo la password dell'utente nel portale di Azure.
