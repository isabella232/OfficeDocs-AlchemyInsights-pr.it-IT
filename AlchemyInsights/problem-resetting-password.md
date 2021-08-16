---
title: Problema durante la reimpostazione della password
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "9360"
ms.openlocfilehash: 535b5273d367e24ac45b3f60dbc7b6a2da6a3d9affa5a67499989d19a1904768
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54039970"
---
# <a name="problems-resetting-password"></a>Problemi durante la reimpostazione della password

Di seguito sono riportati alcuni dei problemi che potrebbero verificarsi durante la reimpostazione della password e le possibili soluzioni:

**Si è verificato un problema con la reimpostazione della password non coperta nelle altre categorie**

- Assicurarsi di essere autorizzati a reimpostare le password. Solo gli amministratori globali, password e utenti possono reimpostare le password degli utenti. Gli amministratori globali possono anche reimpostare le password di altri amministratori con privilegi.
- Assicurarsi di comprendere i requisiti di licenza:
    - È necessario disporre di almeno una licenza assegnata nell'organizzazione
        - Utenti solo cloud - SKU Office 365 (O365) a pagamento o Azure AD Basic
        - Utenti cloud e/o locali - Azure AD Premium P1 o P2, Enterprise Mobility + Security (EMS) o Secure Productive Enterprise (SPE)
        - Per altre informazioni sui requisiti di licenza, vedi l'articolo [Requisiti di licenza per la reimpostazione della password self-service](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)di Azure AD.

**Si sono verificati problemi durante il test del criterio di reimpostazione della password impostato**

- I criteri applicati di recente possono richiedere diversi minuti per la replica in tutti i data center e gli end point. Anche la distanza fisica dal data center influisce sulla velocità di applicazione delle modifiche.
- Testare con un utente finale, non un amministratore e pilota con un piccolo set di utenti. I criteri configurati nel portale di Azure si applicano SOLO agli utenti finali, non agli amministratori. Microsoft applica un criterio predefinito di reimpostazione della password predefinito per qualsiasi ruolo di amministratore di Azure (ad esempio: amministratore globale, amministratore helpdesk, amministratore password e così via)
    - Ulteriori informazioni sui [criteri per gli amministratori](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences).

**Voglio distribuire la reimpostazione della password, ma non voglio che gli utenti registrino altre info di sicurezza**

Precompilare i dati per gli utenti in modo che non sia necessario. - Gli amministratori possono impostare le proprietà del telefono e della posta elettronica per gli utenti prima di eseguire la reimpostazione della password nell'organizzazione. A tale scopo, puoi usare un'API, PowerShell o Azure AD Connessione. Altre informazioni qui:
- [Distribuzione della reimpostazione della password senza richiedere agli utenti di eseguire la registrazione](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [Quali dati vengono utilizzati dalla reimpostazione della password](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Il pulsante di reimpostazione della password è in grigio**

Non si è autorizzati a reimpostare le password di questo utente. Solo gli amministratori globali, password e utenti possono reimpostare le password degli utenti. Gli amministratori globali possono anche reimpostare le password di altri amministratori con privilegi.

**Il pannello di reimpostazione della password non è visualizzato**

Non si è autorizzati a reimpostare le password. Solo gli amministratori globali, password e utenti possono reimpostare le password degli utenti. Gli amministratori globali possono anche reimpostare le password di altri amministratori con privilegi.

**Il pannello di integrazione locale non viene visualizzato nella reimpostazione della password**

- Il pannello di integrazione locale viene visualizzato solo negli ambienti ibridi, ovvero si utilizza il writeback delle password per modificare le password degli utenti locali.
- Questo pannello non viene visualizzato se:
    - Non si utilizza il writeback delle password
    - Si è verificato un problema con l'installazione/connettività del writeback delle password
    - Si è verificato un problema con l'installazione/connettività di Azure AD Connessione
    - Per ulteriori procedure di risoluzione dei problemi relativi al writeback delle password, vedere la sezione Risolvere i problemi relativi al [writeback delle password](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Non so come reimpostare la password di un utente**

1. Accedere al portale di Azure come amministratore appropriato.
1. Passare al pannello Utenti e gruppi, selezionare **Tutti gli utenti**.
1. Selezionare un utente dall'elenco.
1. Per l'utente selezionato, selezionare **Panoramica** e quindi nella barra dei comandi fare clic su **Reimposta password.**
1. Seguire le istruzioni visualizzate sullo schermo.
    - Solo le reimpostazioni eseguite tramite il portale di Azure supportano il writeback delle password.

**Reimpostazione della password di un utente locale dal portale di Amministrazione di Office 365 o dall'applicazione Office 365 per dispositivi mobili, ma l'utente non è ancora in grado di accedere**

Il writeback delle password non è supportato in questo portale. Reimpostare di nuovo la password dell'utente nel portale di Azure - portal.azure.com

