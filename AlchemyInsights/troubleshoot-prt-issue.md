---
title: Risolvere il problema del PRT
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: 8e654a38d720aa51daf21bf5c3fb0da8b9c3d8e7
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/04/2020
ms.locfileid: "49571970"
---
# <a name="troubleshoot-prt-issue"></a>Risolvere il problema del PRT

Affinché tutti i dispositivi vengano completati come autenticati, è necessario che siano completamente registrati e in grado di acquisire un token di aggiornamento primario (PRT).

Il processo di registrazione ibrido di Azure AD join richiede che i dispositivi si trovino in una rete aziendale. Funziona anche su VPN, ma ci sono alcune avvertenze. Sono stati ascoltati i clienti che hanno bisogno di assistenza per la risoluzione dei problemi del processo di registrazione del join di Azure AD in modalità remota. Di seguito viene indicato un problema relativo a ciò che accade sotto la cappa durante il processo di registrazione.

**Ambiente di autenticazione cloud (tramite l'autenticazione hash della password di Azure AD o pass-through)**

Questo flusso di registrazione è noto anche come "sincronizzazione join".

1. Windows 10 consente di individuare un record SCP al momento dell'accesso dell'utente al dispositivo.
    1. Il dispositivo tenta innanzitutto di recuperare le informazioni sul tenant dall'SCP sul fianco del client nel registro di sistema [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Per ulteriori informazioni, vedere questo [documento](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    2. In caso di esito negativo, il dispositivo comunica con Active Directory locale (AD) per ottenere informazioni sul tenant dal punto di connessione del servizio (SCP, Service Connection Point). Per verificare SCP, fare riferimento a questo [documento](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point). 

> [!NOTE]
> Si consiglia di abilitare SCP nell'annuncio e di utilizzare solo SCP sul fianco del client per la convalida iniziale.

2. Windows 10 tenta di comunicare con Azure AD nel contesto di sistema per autenticarsi con Azure AD. È possibile verificare se il dispositivo può accedere alle risorse Microsoft con l'account di sistema utilizzando lo script di connettività di registrazione del dispositivo di test.

3. Windows 10 genera un certificato autofirmato e lo archivia sotto l'oggetto computer in Active Directory locale. Questo richiede la linea di vista per il controller di dominio.

4. Un oggetto Device che dispone di un certificato viene sincronizzato con Azure ad tramite Azure AD Connect. Il ciclo di sincronizzazione è ogni 30 minuti per impostazione predefinita, ma dipende dalla configurazione di Azure AD Connect. Per ulteriori informazioni, fare riferimento a questo [documento](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).

5. In questa fase, è necessario essere in grado di visualizzare il dispositivo soggetto nello stato in sospeso in dispositivo Blade del portale di Azure.

6. Al successivo accesso utente a Windows 10, la registrazione sarà completata. 

> [!NOTE]
> Se si è in VPN e un processo di accesso di disconnessione termina la connettività del dominio, è possibile attivare la registrazione manualmente:
 1. Emettere un/join di dsregcmd localmente su prompt di amministratore o in remoto tramite PSExec al PC. Ad esempio, PsExec-s \\ win10client01 cmd, dsregcmd/join

 2. Per ulteriori informazioni sui problemi di join ibrido, vedere [risolvere i problemi relativi ai dispositivi](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).
