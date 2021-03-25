---
title: L'accesso condizionale con un dispositivo aggiunto a un dominio viene bloccato
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/20/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9834"
- "9003257"
ms.openlocfilehash: 052311ffe71bcb65de2b5c2a964932b1fb99c373
ms.sourcegitcommit: c34ba92e19419dcb2d251b8a1afe4d180a939617
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 03/20/2021
ms.locfileid: "50965465"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a>L'accesso condizionale con un dispositivo aggiunto a un dominio viene bloccato

**Strumenti altamente consigliati**

[Strumento di risoluzione dei problemi di registrazione dei dispositivi](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/): lo strumento che consente di risolvere i problemi di registrazione dei dispositivi più comuni.

[Script di test della connettività per la registrazione dei dispositivi](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/): lo script che consente di verificare che un dispositivo possa accedere agli endpoint di registrazione dei dispositivi nell'account di sistema.

[Script di pulizia dei dispositivi Azure AD](https://github.com/mzmaili/AzureADDeviceCleanup): lo script che consente di cercare e gestire dispositivi obsoleti nell'ambiente.

Ecco alcuni motivi comuni per cui l'accesso condizionale potrebbe non riuscire in un dispositivo aggiunto a un dominio (Azure AD ibrido).

1. **Non è presente un PRT di Azure AD nel dispositivo**: è necessario verificare che il dispositivo disponga di un token di aggiornamento primario (PRT) di Azure AD. Per altre informazioni sul PRT, consultare questo [documento](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).

Per verificare la presenza di un PRT di Azure AD, è possibile eseguire il comando `dsregcmd/status` nel dispositivo e verificare se "AzureAdPrt" è uguale a "YES".

Se "AzureAdPrt" è "NO", verificare quanto segue:

- **Se è presente un ambiente federato con AD FS e non è raggiungibile dalle reti domestiche degli utenti**: in questo caso, verificare che gli endpoint "usernamemixed" siano accessibili dalla Extranet. Se AD FS è dietro una VPN, verificare che gli utenti siano connessi alla VPN e accedere di nuovo al dispositivo. Per altre informazioni, consultare questo [documento](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).

- **Se il TPM del dispositivo è difettoso e non è possibile autenticare il dispositivo**: controllare "tpm.msc" per vedere se lo stato del TPM è "Ready". In caso contrario, eseguire `dsregcmd/leave` e consentire al dispositivo di aggiungersi di nuovo ad Azure AD. Quindi riprovare. Per altre informazioni, consultare questo [documento](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).

- **È in uso un provider di identità di terze parti che non supporta il protocollo WS-Trust**. Come descritto nei documenti, i dispositivi aggiunti ad Azure AD ibrido non possono funzionare in questo caso. Contattare il provider di identità per ricevere assistenza.

2. **Gli utenti usano il browser Chrome senza account di Windows 10** oppure l'**estensione Office per Chrome non usa automaticamente il PRT nei dispositivi aggiunti ad AAD o ad AAD ibrido**: questo causa l'errore dei criteri di accesso condizionale basati su dispositivo, con il messaggio di errore "Dispositivo non registrato" visualizzato. Per usare correttamente il browser Chrome, è necessario installare "Account Windows 10" o l'"estensione di Office per il browser Chrome degli utenti" tramite SCCM o Intune. Per altre informazioni, consultare questo [documento](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).

Se non è possibile eseguire il push dell'estensione da remoto, avvisare gli utenti di installare manualmente una delle estensioni precedenti per accedere alle applicazioni dietro l'accesso condizionale basato su dispositivo. Per altre informazioni, consultare questo [documento](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).

3. **Il dispositivo è stato aggiunto ad Azure AD ibrido correttamente ma è stato eliminato o disabilitato inavvertitamente, a causa di modifiche alla sincronizzazione in Azure AD Connect o del portale di Azure**: in questo caso, l'oggetto del dispositivo non è più riconosciuto come dispositivo aggiunto anche se lo stato di "AzureAdJoined" e "PRT" risulta valido nel dispositivo.

Per risolvere il problema, eseguire `dsregcmd/leave` nei dispositivi interessati e consentire loro di aggiungersi di nuovo ad Azure AD. Per altre informazioni, consultare questo [documento](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).

> [!NOTE]
> Se i dispositivi sono in esecuzione con l'aggiornamento 1809 di Windows 10, con proxy VPN/Cloud e si verificano problemi con lo stato di "AzureAdPrt" o con un'app con problemi di SSO (Outlook non si connette alla cassetta postale anche se è presente un PRT), verificare di disporre della patch [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) o dell'aggiornamento cumulativo di aprile [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) per evitare errori di PRT in tali computer.

















