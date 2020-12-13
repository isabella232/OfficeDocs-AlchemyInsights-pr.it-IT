---
title: Dispositivo in stato in sospeso
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
- "9003244"
- "7319"
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/11/2020
ms.locfileid: "49652189"
---
# <a name="device-in-pending-state"></a>Dispositivo in stato in sospeso

**Prerequisiti**

1. Se si stanno configurando le registrazioni del dispositivo per la prima volta, assicurarsi di aver esaminato l' [Introduzione alla gestione dei dispositivi in Azure Active Directory (Azure ad)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) che guiderà l'utente su come ottenere i dispositivi sotto il controllo di Azure ad.
2. Se si sta registrando i dispositivi in Azure AD direttamente e si esegue la registrazione in Intune, è necessario assicurarsi di aver [configurato Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) e di disporre della [licenza](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) per prima.
3. Assicurarsi di essere autorizzati a eseguire operazioni in Azure Active Directory e Active Directory locale. Solo un amministratore globale di Azure AD è in grado di gestire le impostazioni per le registrazioni dei dispositivi. Inoltre, se si stanno configurando le registrazioni automatiche in Active Directory locale, è necessario essere un amministratore di Active Directory e AD FS (se applicabile).

Il processo di registrazione ibrido di Azure AD join richiede che i dispositivi siano sulla rete aziendale. Funziona anche su VPN, ma ci sono alcune avvertenze. Sono stati ascoltati i clienti che hanno bisogno di assistenza per la risoluzione dei problemi relativi al processo di registrazione di join di Azure AD in condizioni di lavoro remote.

**Ambiente di autenticazione cloud (tramite l'autenticazione hash della password di Azure AD o pass-through)**

Questo flusso di registrazione è noto anche come "sincronizzazione join".

Di seguito viene indicato un guasto di ciò che avviene durante il processo di registrazione:

1. Windows 10 rileva il record SCP (Service Connection Point) quando l'utente esegue l'accesso al dispositivo.

    1. Il dispositivo tenta innanzitutto di recuperare le informazioni sul tenant dall'SCP sul fianco del client nel registro di sistema [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Per ulteriori informazioni, vedere [Document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    1. In caso di esito negativo, il dispositivo comunica con Active Directory locale per ottenere informazioni sul tenant da SCP. Per verificare SCP, fare riferimento a questo [documento](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).

    > [!NOTE]
    > Si consiglia di abilitare SCP in Active Directory e di utilizzare solo SCP sul fianco client per la convalida iniziale.

2. Windows 10 tenta di comunicare con Azure AD nel contesto di sistema per autenticarsi con Azure AD.

    È possibile verificare se il dispositivo può accedere alle risorse Microsoft con l'account di sistema utilizzando lo [script di connettività di registrazione del dispositivo di test](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).

3. Windows 10 genera un certificato autofirmato e lo archivia sotto l'oggetto computer in Active Directory locale. Questo richiede la linea di vista per il controller di dominio.

4. Oggetto Device con certificato ottenuto sincronizzato con Azure ad tramite Azure AD Connect. Il ciclo di sincronizzazione è ogni 30 minuti per impostazione predefinita, ma dipende dalla configurazione di Azure AD Connect. Per ulteriori informazioni, fare riferimento a questo [documento](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).

5. In questa fase, è necessario essere in grado di visualizzare il dispositivo soggetto nello stato in **sospeso** in dispositivo Blade del portale di Azure.

6. Al successivo accesso utente a Windows 10, la registrazione sarà completata.

    > [!NOTE]
    > Se si è in VPN e la disconnessione/accesso termina la connettività del dominio, è possibile attivare la registrazione manualmente. A questo scopo:
    >
    > Emettere un `dsregcmd /join` prompt di amministratore localmente o in remoto tramite PsExec nel PC.
    >
    > Ad esempio: `PsExec -s \\win10client01 cmd, dsregcmd /join`

Per i problemi comuni relativi alla registrazione del dispositivo di Azure Active Directory, vedere [FAQ sui dispositivi](https://docs.microsoft.com/azure/active-directory/devices/faq).
