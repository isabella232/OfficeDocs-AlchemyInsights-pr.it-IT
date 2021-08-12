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
ms.openlocfilehash: 224e6e613c306b50e354930bcbe6f43f1c08528766cb6e681b0e9826b2d55a4d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53914007"
---
# <a name="device-in-pending-state"></a>Dispositivo in stato in sospeso

**Prerequisiti:**

1. Se stai configurando le registrazioni dei dispositivi per la prima volta, assicurati di aver esaminato Introduzione alla gestione dei dispositivi [in Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) che ti guiderà su come ottenere i dispositivi sotto il controllo di Azure AD.
2. Se si registrano i dispositivi in Azure AD direttamente e li si registra [in](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) Intune, è necessario assicurarsi di aver configurato [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) e di disporre delle licenze per prime.
3. Assicurarsi di essere autorizzati a eseguire operazioni in Azure AD e in ACTIVE locale. Solo l’amministratore globale in Azure AD può gestire le impostazioni per la registrazione dei dispositivi. Inoltre, è necessario essere un amministratore di Active Directory e AD FS, se applicabile, se si stanno configurando le registrazioni automatiche in Active Directory locale.

Il processo ibrido di registrazione dell'aggiunta ad Azure AD richiede che i dispositivi siano nella rete aziendale. Funziona anche su VPN, ma ci sono alcune avvertenze a questo. Abbiamo sentito che i clienti hanno bisogno di assistenza per la risoluzione dei problemi del processo ibrido di registrazione dell'aggiunta ad Azure AD in circostanze lavorative remote.

**Ambiente di autenticazione cloud (con la sincronizzazione hash delle password di Azure AD o l'autenticazione pass-through)**

Questo flusso di registrazione è noto anche come "Sync Join".

Ecco una descrizione di ciò che accade durante il processo di registrazione:

1. Windows 10 individua il record SCP (Service Connection Point) quando l'utente accede al dispositivo.

    1. Il dispositivo tenta innanzitutto di recuperare le informazioni sul tenant da SCP sul lato client nel Registro di sistema [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Per ulteriori informazioni, vedere [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    1. In caso di esito negativo, il dispositivo comunica con Active Directory locale per ottenere informazioni sul tenant da SCP. Per verificare SCP, fare riferimento a questo [documento.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point)

    > [!NOTE]
    > È consigliabile abilitare SCP in Active Directory e utilizzare solo SCP sul lato client per la convalida iniziale.

2. Windows 10 tenta di comunicare con Azure AD nel contesto di sistema per autenticarsi in Azure AD.

    Puoi verificare se il dispositivo può accedere alle risorse Microsoft con l'account di sistema usando lo [script Test Device Registration Connectivity](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).

3. Windows 10 genera un certificato autofirmato e lo archivia sotto l'oggetto computer in Active Directory locale. Ciò richiede line-of-sight al controller di dominio.

4. L'oggetto dispositivo con certificato viene sincronizzato con Azure AD tramite Azure AD Connessione. Il ciclo di sincronizzazione è ogni 30 minuti per impostazione predefinita, ma dipende dalla configurazione di Azure AD Connessione. Per ulteriori informazioni, fare riferimento a questo [documento.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)

5. In questa fase, dovresti essere in grado di visualizzare il dispositivo soggetto nello stato **"** In sospeso " in Pannello dispositivo del portale di Azure.

6. Al successivo accesso utente a Windows 10, la registrazione verrà completata.

    > [!NOTE]
    > Se si utilizza una rete VPN e la disconnessione/accesso termina la connettività di dominio, è possibile attivare la registrazione manualmente. A questo scopo:
    >
    > Emettere un `dsregcmd /join` prompt di amministrazione locale o in remoto tramite PSExec nel PC.
    >
    > Ad esempio: `PsExec -s \\win10client01 cmd, dsregcmd /join`

Per problemi comuni con la registrazione Azure Active Directory dispositivo, vedi [Domande frequenti sui dispositivi.](https://docs.microsoft.com/azure/active-directory/devices/faq)
