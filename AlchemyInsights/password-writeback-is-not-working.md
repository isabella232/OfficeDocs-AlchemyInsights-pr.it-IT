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
ms.openlocfilehash: d7766f908f025b5db8299aa45d01dc5389b321ec
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 02/12/2021
ms.locfileid: "50232721"
---
# <a name="password-writeback-is-not-working"></a>Il writeback delle password non funziona

**Si verificano problemi durante la configurazione del writeback delle password**

- Il writeback delle password è una funzionalità premium.
- Assicurarsi di comprendere i requisiti di licenza:
  - È necessario disporre di almeno una licenza assegnata nell'organizzazione
  - **Utenti solo cloud** - Qualsiasi SKU a pagamento di Office 365 (O365) o Azure AD Basic
  - **Utenti cloud e/o** locali : Azure AD Premium P1 o P2, Enterprise Mobility + Security (EMS) o Secure Productive Enterprise (SPE)
    - Per altre informazioni sui requisiti di licenza, vedere [Requisiti di licenza per la reimpostazione della password in modalità self-service di Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- Si dispone di almeno un account amministratore e di un account utente di test con una della licenza appropriata.
- Per il funzionamento del writeback delle password, devi connettere Azure AD Connect all'emulatore del controller di dominio primario. È possibile configurare Azure AD Connect per l'utilizzo  di un controller di dominio primario facendo clic con il pulsante destro del mouse sulle proprietà del connettore di sincronizzazione di Active Directory, quindi selezionando **Configura partizioni di directory.** Da qui, cercare la sezione relativa alle impostazioni di connessione **del controller** di dominio e selezionare la casella intitolato Utilizzare solo i controller di **dominio preferiti.**
  > [!NOTE]
  > Se il controller di dominio preferito non è un emulatore PDC, Azure AD Connect continuerà a contattare il PDC per il writeback delle password.
- La reimpostazione della password è stata configurata e abilitata nel tenant. Per altre informazioni, vedere Consentire [agli utenti di reimpostare le password di Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)
- Assicurarsi che l'account amministratore utilizzato per abilitare il writeback delle password sia un account amministratore cloud (creato in Azure AD non locale ad)
- Si dispone di una distribuzione locale di Active Directory a foresta singola o a più foreste che esegue Windows Server 2008 R2, Windows Server 2012 o Windows Server 2012 R2 con i Service Pack più recenti installati
- Hai installato lo strumento Azure AD Connect e hai preparato l'ambiente AD per la sincronizzazione con il cloud. Prima di testare il writeback delle password, assicurati di completare un'importazione completa e una sincronizzazione completa da AD e Azure AD in Azure AD Connect.
- Per altre informazioni, vedere come eseguire una sincronizzazione completa e [l'importazione completa in Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)

**Si è verificato un problema con la connettività per il writeback delle password**

1. Scaricare e abilitare la versione più recente di [Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)
2. Configurazione firewall: lo strumento Azure AD Connect (1.1.443 e successive) avrà bisogno dell'accesso **HTTPS** in uscita a:
    - passwordreset.microsoftonline.com
    - servicebus.windows.networks
3. Consenti la persistenza delle connessioni inattive per almeno 2-3 minuti

**I'm still having problems with password writeback**

- Se si hanno ancora difficoltà, provare a disabilitare e abilitare di nuovo il servizio di writeback delle password nello strumento Azure AD Connect
- Per altre informazioni, vedere come disabilitare e [abilitare di nuovo il writeback delle password](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)
