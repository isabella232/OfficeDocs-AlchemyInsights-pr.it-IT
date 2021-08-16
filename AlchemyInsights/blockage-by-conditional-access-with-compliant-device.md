---
title: L'accesso condizionale con un dispositivo conforme viene bloccato
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9835"
- "9003257"
ms.openlocfilehash: 709749b1a62f2d9cdabfb3fe4b7538c22101d7109204d9163f6059336b817bf8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54019152"
---
# <a name="im-getting-blocked-by-conditional-access-with-compliant-device"></a>L'accesso condizionale con un dispositivo conforme viene bloccato

**Strumenti altamente consigliati**

- [Strumento di risoluzione dei problemi di registrazione dei dispositivi](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - Uno strumento completo che consente di risolvere i problemi di registrazione dei dispositivi più comuni.
- [Test script connettività registrazione dei dispositivi](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - Strumento usato per verificare che un dispositivo possa accedere agli endpoint di registrazione dei dispositivi nell'account di sistema.
- [Script di pulizia dispositivi Azure AD](https://github.com/mzmaili/AzureADDeviceCleanup): uno strumento usato per cercare e gestire dispositivi obsoleti nell'ambiente.

Ecco alcuni motivi comuni per cui l'accesso condizionale potrebbe non riuscire per un dispositivo conforme o perché gli utenti potrebbero ricevere **Non è possibile accedere da questo** messaggio durante una richiesta di accesso a una risorsa dell'organizzazione.

1. **Il dispositivo non è in uno stato del dispositivo richiesto con un MDM**:

Verificare che il dispositivo sia registrato con un provider MSM approvato, come Intune *contrassegnato come conforme*. Per altre informazioni su Intune, vedere questo [documento](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment). Per una maggiore comprensione della conformità dei dispositivi e Intune, [usare i criteri di conformità per impostare regole per i dispositivi gestiti con Intune](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started). In caso di problemi di registrazione di un dispositivo con Intune, vedere i dettagli sulla risoluzione dei problemi [Risoluzione dei problemi per la registrazione dei dispositivi in Microsoft](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune). Per ulteriore assistenza con Intune, creare una richiesta di supporto. A questo scopo, visitare la pagina [Guida e supporto tecnico di Intune](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport).

2. **Il dispositivo non fa parte della rete dell'organizzazione**:

Per accedere alle risorse dell'organizzazione, il dispositivo deve essere connesso alla rete dell'organizzazione, tramite connessione diretta o VPN, e deve anche far parte di una rete locale o di Azure Active Directory. Per aggiungere un dispositivo aziendale alla rete dell'organizzazione, vedere [Aggiungere il dispositivo di lavoro alla rete dell'organizzazione](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network). Per registrare un dispositivo personale/BYOD, vedere [Registrare il dispositivo personale nella rete dell'organizzazione](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network).

- Per verificare se il dispositivo si è aggiunto alla rete, è possibile seguire i passaggi per i dispositivi registrati [qui](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered) o i dispositivi di lavoro [qui](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined). Per impostare l'ambito del problema sulla connettività di rete dell'organizzazione, seguire le linee guida seguenti:

    1. Accedere a Windows usando l'account di lavoro o della scuola, ad esempio, giuseppe@contoso.com.
    2. Connettersi alla rete dell'organizzazione tramite VPN o DirectAccess.
    3. Una volta connessi, premere il **TASTO WINDOWS+L** per bloccare il dispositivo.
    4. Sbloccare il dispositivo usando l'account aziendale o dell'istituto di istruzione e quindi provare di nuovo ad accedere all'applicazione o al servizio che presenta il problema.

Se viene visualizzato il messaggio di errore **Non è possibile accedere da qua,**, è probabile che il problema si sia verificato in un'altra posizione.

3. **Il sistema operativo non è supportato**:

Assicurarsi di eseguire una versione supportata del sistema operativo, tra cui:

- **Windows Client**: Windows 7 o versione successiva

- **Windows Server**: Windows Server 2008 R2 o versione successiva

- **macOS**: macOS X o versione successiva

- **Android e iOS**: versione più recente dei sistemi operativi per dispositivi mobili Android e iOS

4. **Il webbrowser non è supportato**:

Di seguito sono elencati i browser supportati. Per il supporto di Chrome con Windows 1703 o versioni successive è necessaria l'estensione Account di Windows 10. Per Edge 85+, l'utente deve aver eseguito l'accesso per passare correttamente le informazioni di conformità dei dispositivi. Per ulteriori dettagli, vedere[qui](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).

- **Windows 10**: Microsoft Edge, Internet Explorer, Chrome
- **Windows 8/ 8.1**: Internet Explorer, Chrome
- **Windows 7**: Internet Explorer, Chrome
- **iOS**: Microsoft Edge, Intune Managed Browser, Safari
- **Android**: **Microsoft Edge**: Intune Managed Browser, Chrome
- **Windows Phone**: Microsoft Edge, Internet Explorer
- **Windows Server 2019**: Microsoft Edge, Internet Explorer, Chrome
- **Windows Server 2016**: Internet Explorer
- **Windows Server 2012 R2**: Internet Explorer
- **Windows Server 2008 R2**: Internet Explorer
- **macOS**: Chrome, Safari

Per altre informazioni sui messaggi **Non puoi raggiungere la località direttamente da qui** e le procedure per la risoluzione dei problemi [vedere](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation).
