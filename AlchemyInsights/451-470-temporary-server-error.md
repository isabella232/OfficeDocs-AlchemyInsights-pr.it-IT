---
title: 451 4.7.0 Errore temporaneo del server. Riprovare più tardi. PRX4
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2021
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "3000003"
- "12465"
ms.openlocfilehash: 16e16f087c2b13a9ad5fec7223b4f3395e42646e
ms.sourcegitcommit: 380ee556007d2be389b1a99795bca04bc1f9f60f
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/27/2021
ms.locfileid: "53604925"
---
# <a name="451-470-temporary-server-error-please-try-again-later-prx4"></a>451 4.7.0 Errore temporaneo del server. Riprovare più tardi. PRX4

Potrebbe verificarsi un problema durante l'invio di posta elettronica tramite Smarthost "smtp.office365.com" utilizzando il metodo di invio del client SMTP e viene visualizzato l'errore: "451 4.7.0 Temporary server error. Riprovare più tardi. PRX4 è per lo più temporaneo." 

Assicurarsi di non utilizzare una cassetta postale condivisa per l'invio del client SMTP, poiché il metodo di invio del client SMTP richiede una cassetta postale con licenza per l'invio della posta. Tuttavia, se non si utilizza una cassetta postale condivisa e il problema persiste, controllare quanto segue:

1. Abilitare l'invio SMTP client nella cassetta postale con licenza utilizzata eseguendo questo comando di PowerShell:

    ```Set-CASMailbox -Identity sean@contoso.com -SmtpClientAuthenticationDisabled $false```

    OPPURE

    1. Passare alla interfaccia di amministrazione di Microsoft 365 > **Utenti attivi** e selezionare l'utente.
    1. Vai alla scheda Posta > **app di** posta > selezionare Gestisci app di **posta elettronica**. 
    1. Verificare che **l'impostazione SMTP autenticato** sia selezionata (abilitata).
    1. Selezionare **Salva modifiche**.
    
    Per abilitare l'autenticazione SMTP per un'intera organizzazione, eseguire questo comando:

    `Set-TransportConfig -SmtpClientAuthenticationDisabled $true`
 
    **Nota:** per motivi di sicurezza, è consigliabile abilitare l'autenticazione SMTP solo per la cassetta postale in uso. L'impostazione a livello di utente sostituisce l'impostazione a livello di organizzazione.

2. Disabilitare le impostazioni predefinite di sicurezza di Azure impostando Abilita **impostazioni predefinite di sicurezza** su **No**:

    1. Accedere al portale di Azure come amministratore della sicurezza, amministratore di accesso condizionale o amministratore globale.
    1. Passare a Azure Active Directory >**  proprietà** e selezionare **Gestisci impostazioni predefinite sicurezza.**
    1. Impostare **l'interruttore Abilita impostazioni predefinite sicurezza** su **No**.
    1. Selezionare **Salva**.

3. Disabilitare Multi Factor Authentication (MFA) nella cassetta postale con licenza in uso.

    1. Passare al interfaccia di amministrazione di Microsoft 365 e nel menu di spostamento sinistro scegliere **Utenti**  >  **Utenti attivi**.
    1. Nella pagina **Utenti attivi**, scegliere **Autenticazione a più fattori**.
    1. Selezionare l'utente e disabilitare **l'autenticazione a più fattori.**

