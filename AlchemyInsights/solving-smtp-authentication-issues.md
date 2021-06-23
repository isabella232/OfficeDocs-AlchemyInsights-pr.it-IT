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
ms.openlocfilehash: 4695a2f111823739c4d87fa2b262a5e64e080955
ms.sourcegitcommit: 2103d706492ad7ee9596344714c0520569ebd6af
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 06/23/2021
ms.locfileid: "53077655"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a>Abilitare l'autenticazione SMTP e la risoluzione dei problemi

Se si vuole abilitare l'autenticazione SMTP per una cassetta postale o si riceve un errore "Client non autenticato", "Autenticazione non riuscita" o "SmtpClientAuthentication" con codice 5.7.57 o 5.7.3 o 5.7.139 quando si prova a inoltrare la posta elettronica autenticando un dispositivo o un'applicazione con Microsoft 365, eseguire queste tre azioni per risolvere il problema:

1. Disabilitare le [impostazioni predefinite per la sicurezza di Azure](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) impostando **Abilita le impostazioni predefinite per la sicurezza** su **No**.

    a. Accedere al portale di Azure come Amministratore della sicurezza, Amministratore di accesso condizionale o Amministratore globale.<BR/>
    b. Passare ad Azure Active Directory> **Proprietà**.<BR/>
    c. Selezionare **Gestire le impostazioni predefinite per la sicurezza**.<BR/>
    d. Impostare **Abilita le impostazioni predefinite per la sicurezza** su **No**.<BR/>
    e. Selezionare **Salva**.

2. [Abilitare l'invio del protocollo SMTP del client](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) nella cassetta postale con licenza.

    a. Nell'interfaccia di amministrazione di Microsoft 365 passare a **Utenti attivi** e selezionare l’utente.<BR/>
    b. Passare alla scheda Posta e in **App di posta elettronica** selezionare **Gestire le applicazioni di posta elettronica**.<BR/>
    d. Verificare che l’opzione **SMTP autenticato** sia selezionata (abilitata).<BR/>
    e. Selezionare **Salva modifiche**.<BR/>

3. [Disabilitare l'autenticazione a più fattori (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) nella cassetta postale con licenza.

    a. Passare all’interfaccia di amministrazione di Microsoft 365 e, nel riquadro di spostamento sinistro, selezionare **Utenti** > **Utenti attivi**.<BR/>
    b. Selezionare **Multi-Factor Authentication**.<BR/>
    c. Selezionare l'utente e disabilitare **Multi-Factor Authentication**.<BR/>
