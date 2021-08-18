---
title: Problemi di accesso alle Microsoft 365 app
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 7a8a0b68fc211e99b22e857d51d1de54e53a69357f75a0c60b1e83078cd5b27f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088040"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Schermata di accesso vuota nelle Microsoft 365 app

Per risolvere il problema, provare a eseguire le operazioni seguenti:
- Installare gli aggiornamenti più recenti per [Windows](https://support.microsoft.com/help/4027667/windows-10-update) [e Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Reimposta le opzioni di Internet Explorer: vai a Strumenti  >  **Opzioni Internet**  >  **Advanced** Reset Internet  >  **Explorer Impostazioni** (tieni presente che perderai le impostazioni personalizzate), quindi prova ad accedere di Office di nuovo.
- Disabilitare Windows Defender Application Guard (WDAG) o qualsiasi programma firewall o antivirus simile:
    1. Nel Pannello di controllo passare a **Programmi** e quindi scegliere **Attiva Windows funzionalità.**
    2. Se Windows Defender Application Guard è abilitato, provare a disabilitarlo.<br/>
    **Nota:** Potrebbe essere necessario riavviare il computer.
- Verificare che il plug-in Microsoft.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) non sia bloccato da alcuna applicazione o programma firewall/antivirus.
- [Cancella Office credenziali usando](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) gestione Windows credenziali.<br/>
    **Nota:** I percorsi del Registro di Office 2016 sono stati modificati in 16.0. (Ad esempio: \Software\Microsoft\Office\16.0\Common\Identity\)

Per ulteriori informazioni, vedere [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).