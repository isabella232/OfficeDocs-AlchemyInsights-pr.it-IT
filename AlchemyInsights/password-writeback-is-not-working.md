---
title: Il writeback delle password non funziona
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
- "9004595"
- "8210"
ms.openlocfilehash: 679dea6d488cf74f51baee2b3b498dc64b95530e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324927"
---
# <a name="password-writeback-is-not-working"></a>Il writeback delle password non funziona

**Si sono verificati problemi durante la configurazione del writeback delle password**

- Il writeback delle password è una funzionalità premium.
- Assicurarsi di aver compreso i requisiti di licenza:
  - È necessario disporre di almeno una licenza assegnata nell'organizzazione
  - **Utenti solo cloud** - SKU Office 365 (O365) a pagamento o Azure AD Basic
  - **Utenti cloud e/o** locali - Azure AD Premium P1 o P2, Enterprise Mobility + Security (EMS) o Secure Productive Enterprise (SPE)
    - Per altre informazioni sui requisiti di licenza, vedere [Requisiti di licenza per la reimpostazione della password in modalità self-service](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing) di Azure AD
- Si dispone di almeno un account amministratore e di un account utente di prova con una delle licenze appropriate.
- È necessario connettere Azure AD Connessione al controller di dominio primario Emulator per il funzionamento del writeback delle password. È possibile configurare Azure AD Connessione per l'utilizzo di  un controller di dominio primario facendo clic con il pulsante destro del mouse sulle proprietà del connettore di sincronizzazione di Active Directory, quindi selezionando **configura partizioni di directory.** Da qui, cercare la sezione impostazioni di connessione **del controller** di dominio e selezionare la casella intitolato Utilizzare solo i controller di **dominio preferiti**.
    **Nota:** se il controller di dominio preferito non è un emulatore PDC, Azure AD Connessione continuerà a contattare il PDC per il writeback delle password.
- La reimpostazione della password è stata configurata e abilitata nel tenant. Per ulteriori informazioni, vedere [Consentire agli utenti di reimpostare le password di Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)
- Verificare che l'account amministratore utilizzato per abilitare il writeback delle password sia un account amministratore cloud (creato in Azure AD non in locale ad Active Directory)
- Si dispone di una distribuzione locale di Active Directory a foresta singola o a più foreste che esegue Windows Server 2008 R2, Windows Server 2012 o Windows Server 2012 R2 con i Service Pack più recenti installati
- È installato lo strumento azure AD Connessione ed è stato preparato l'ambiente AD per la sincronizzazione con il cloud. Prima di testare il writeback delle password, assicurati di completare l'importazione completa e la sincronizzazione completa sia da AD che da Azure AD in Azure AD Connessione.
- Per altre informazioni, vedere come eseguire una sincronizzazione completa [e un'importazione completa in Azure AD Connessione](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)

**Si è verificato un problema con la connettività di writeback delle password**

1. Scaricare e abilitare la versione più recente di [Azure AD Connessione](https://www.microsoft.com/download/details.aspx?id=47594)
2. Configurazione firewall: lo strumento azure AD Connessione (1.1.443 e successive) avrà bisogno dell'accesso **HTTPS** in uscita a:
    - passwordreset.microsoftonline.com
    - servicebus.windows.networks
3. Consenti la persistenza delle connessioni inattive per almeno 2-3 minuti

**I'm still having problems with password writeback**

- Se si verificano ancora problemi, provare a disabilitare e ri-abilitare il servizio writeback delle password nello strumento di Connessione Azure AD
- Per ulteriori informazioni, vedere come disabilitare [e riattivare](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot) il writeback delle password
