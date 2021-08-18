---
title: Abilitare l'autenticazione SMTP e la risoluzione dei problemi
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 14f1454ad687b4d76cf419583b442685fa19b5a2
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58321757"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a>Abilitare l'autenticazione SMTP e la risoluzione dei problemi

Se si vuole abilitare l'autenticazione SMTP per una cassetta postale o si riceve un errore "Client non autenticato", "Autenticazione non riuscita" o "SmtpClientAuthentication" con codice 5.7.57 o 5.7.3 o 5.7.139 quando si prova a inoltrare la posta elettronica autenticando un dispositivo o un'applicazione con Microsoft 365, eseguire queste tre azioni per risolvere il problema:

1. Disabilitare le [impostazioni predefinite per la sicurezza di Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) impostando **Abilita le impostazioni predefinite per la sicurezza** su **No**.

    a. Accedere al portale di Azure come Amministratore della sicurezza, Amministratore dell'accesso condizionale o Amministratore globale.<BR/>
    b. Passare ad Azure Active Directory> **Proprietà**.<BR/>
    c. Selezionare **Gestisci le impostazioni predefinite per la sicurezza**.<BR/>
    d. Impostare **Abilita le impostazioni predefinite per la sicurezza** su **No**.<BR/>
    e. Selezionare **Salva**.

2. [Abilitare l'invio del protocollo SMTP del client](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) nella cassetta postale con licenza.

    a. Nell'interfaccia di amministrazione di Microsoft 365 passare a **Utenti attivi** e selezionare l’utente.<BR/>
    b. Passare alla scheda Posta e in **App di posta elettronica** selezionare **Gestisci le impostazioni delle app di posta elettronica**.<BR/>
    c. Verificare che l’opzione **SMTP autenticato** sia selezionata (abilitata).<BR/>
    d. Selezionare **Salva modifiche**.<BR/>

3. [Disabilitare l'autenticazione a più fattori (MFA)](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) nella cassetta postale con licenza.

    a. Passare all’interfaccia di amministrazione di Microsoft 365 e, nel riquadro di spostamento sinistro, selezionare **Utenti** > **Utenti attivi**.<BR/>
    b. Selezionare **Multi-Factor Authentication**.<BR/>
    c. Selezionare l'utente e disabilitare **Multi-Factor Authentication**.<BR/>
