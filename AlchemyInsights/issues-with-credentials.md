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
ms.openlocfilehash: 975d4850c1ecffae786dd19b7f4363e0c95378cff4f3ae6bb1968af33ef810b0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53986823"
---
# <a name="issues-with-credentials"></a>Problemi con le credenziali

Microsoft Identity Platform flusso di credenziali [client OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) descrive come programmare direttamente in base al flusso di concessione delle credenziali client OAuth 2.0.

**Come si gestiscono la password o le credenziali del certificato di un'applicazione?**

Nell'interfaccia della riga di comando di Azure, è possibile usare le credenziali [dell'app](https://docs.microsoft.com/cli/azure/ad/app/credential) annunci az per eliminare, elencare o reimpostare le credenziali di un'applicazione o del certificato.

**In che modo gli utenti possono reimpostare le proprie password**

Gli utenti devono [registrarsi per la reimpostazione della password self-service](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) prima di poter reimpostare le password. Una volta che un utente si è registrato, può seguire le istruzioni in questo articolo per reimpostare la password: [Reimpostare la password dell'istituto di istruzione o dell'istituto di istruzione.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account)

**In che modo gli utenti possono cambiano le password**

Gli utenti possono seguire i passaggi descritti in questo articolo per modificare le password: [Come modificare la password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).
Possono anche gestire [le password delle app per la verifica in due passaggi.](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords)

**L'utente riceve un errore durante la modifica o la reimpostazione della password**

Questo collegamento fornirà informazioni sui problemi comuni che possono verificarsi quando un utente tenta di reimpostare la password: [Problemi comuni e relative soluzioni](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)

**Si è verificato un problema durante la reimpostazione della password di un utente**

- Assicurarsi di essere autorizzati a reimpostare le password. *Solo gli amministratori globali, password e utenti possono reimpostare le password degli utenti.* Gli amministratori globali possono anche reimpostare le password di altri amministratori con privilegi.

- Assicurarsi di comprendere i requisiti di licenza:

  - È necessario disporre di almeno una licenza assegnata nell'organizzazione:
    - **Utenti solo cloud** - SKU Office 365 (O365) a pagamento o Azure AD Basic
    - **Utenti cloud e/o** locali - Azure AD Premium P1 o P2, Enterprise Mobility + Security (EMS) o Secure Productive Enterprise (SPE)
    - Per altre informazioni sui requisiti di licenza, vedi [Requisiti di licenza per la reimpostazione della password in modalità self-service](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)di Azure AD.
- Per reimpostare la password di un utente, individuarlo in Azure AD. Quindi, nel pannello panoramica per l'utente, fare clic sul pulsante "reimposta password".

**Il pulsante di reimpostazione della password è in grigio**

Non si è autorizzati a reimpostare **le password** di questo utente. *Solo gli amministratori globali, password e utenti possono reimpostare le password degli utenti.* Gli amministratori globali possono anche reimpostare le password di altri amministratori con privilegi.

**Il pannello di reimpostazione della password non è visualizzato**

Non si è autorizzati a reimpostare le password. *Solo gli amministratori globali, password e utenti possono reimpostare le password degli utenti.* Gli amministratori globali possono anche reimpostare le password di altri amministratori con privilegi.

**Il pannello di integrazione locale non viene visualizzato nella reimpostazione della password**

- Il pannello di integrazione locale viene visualizzato solo negli ambienti ibridi, ovvero si utilizza il writeback delle password per modificare le password degli utenti locali.

- Questo pannello non viene visualizzato se:

  - Non si utilizza il writeback delle password
  - Si è verificato un problema con l'installazione/connettività del writeback delle password
  - Si è verificato un problema con l'installazione/connettività di Azure AD Connessione
  - Per ulteriori procedure di risoluzione dei problemi relativi al writeback delle password, vedere [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)

**Non so come reimpostare la password di un utente**

1. Accedere al portale di Azure come amministratore appropriato.
2. Passare al **pannello Utenti e gruppi,** selezionare Tutti gli **utenti**.
3. Selezionare un utente dall'elenco.
4. Per l'utente selezionato, selezionare **Panoramica** e quindi nella barra dei comandi selezionare **Reimposta password.**
5. Seleziona il **pulsante Reimposta password** e segui le istruzioni visualizzate.
    - Solo le reimpostazioni eseguite tramite il **portale di Azure supportano** il writeback delle password.

**Reimpostazione della password di un utente locale dal portale di Amministrazione di Office 365 o dall'applicazione Office 365 per dispositivi mobili, ma l'utente non è ancora in grado di accedere**

Il writeback delle password non è supportato in questo portale. Reimpostare di nuovo la password dell'utente nel portale di Azure.
