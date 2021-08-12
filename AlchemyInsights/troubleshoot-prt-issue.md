---
title: Risolvere il problema di PRT
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
ms.openlocfilehash: fd285d1158d7b358e4c698cf6014422cc2fb536e1fbdf98630bebda359f9c553
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972720"
---
# <a name="troubleshoot-prt-issue"></a>Risolvere il problema di PRT

Per completare l'autenticazione di qualsiasi dispositivo, deve essere registrato completamente e in buone condizioni e in grado di acquisire un token di aggiornamento primario (PRT).

Il processo ibrido di registrazione dell'aggiunta ad Azure AD richiede che i dispositivi siano in una rete aziendale. Funziona anche su VPN, ma ci sono alcune avvertenze a questo. Abbiamo sentito i clienti che necessitano assistenza per la risoluzione dei problemi del processo ibrido di registrazione dell'aggiunta ad Azure AD in circostanze di lavoro remoto. Ecco una descrizione di ciò che accade "sotto il cofano" durante il processo di registrazione.

**Ambiente di autenticazione cloud (con la sincronizzazione hash delle password di Azure AD o l'autenticazione pass-through)**

Questo flusso di registrazione è noto anche come "Sync Join".

1. Windows 10 individua un record SCP all'accesso dell'utente al dispositivo.
    1. Il dispositivo tenta innanzitutto di recuperare le informazioni sul tenant da SCP sul lato client nel Registro di sistema [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Per altre informazioni, consultare questo [documento](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    2. In caso di esito negativo, il dispositivo comunica con Active Directory (AD) locale per ottenere informazioni sul tenant da Service Connection Point (SCP). Per verificare SCP, fare riferimento a questo [documento.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point) 

> [!NOTE]
> Ti consigliamo di abilitare SCP in Active Directory e di usare solo SCP sul lato client per la convalida iniziale.

2. Windows 10 tenta di comunicare con Azure AD nel contesto di sistema per autenticarsi in Azure AD. Puoi verificare se il dispositivo può accedere alle risorse Microsoft con l'account di sistema usando lo script Test Device Registration Connectivity.

3. Windows 10 un certificato autofirmato e lo archivia sotto l'oggetto computer in Active Directory locale. Ciò richiede line-of-sight al controller di dominio.

4. Un oggetto dispositivo con un certificato viene sincronizzato con Azure AD tramite Azure AD Connessione. Il ciclo di sincronizzazione è ogni 30 minuti per impostazione predefinita, ma dipende dalla configurazione di Azure AD Connessione. Per ulteriori informazioni, fare riferimento a questo [documento.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)

5. In questa fase, dovresti essere in grado di visualizzare il dispositivo soggetto nello stato "In sospeso" in Pannello dispositivo del portale di Azure.

6. Al successivo accesso utente a Windows 10, la registrazione verrà completata. 

> [!NOTE]
> Se si è su VPN e un processo di accesso alla disconnessione termina la connettività di dominio, è possibile attivare la registrazione manualmente:
 1. Emettere un dsregcmd /join localmente al prompt di amministrazione o in remoto tramite PSExec al PC. Ad esempio, PsExec -s \\ win10client01 cmd, dsregcmd /join

 2. Per altri dettagli sui problemi relativi all'aggiunta ibrida, vedi [Risolvere i problemi relativi ai dispositivi.](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344)
