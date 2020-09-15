---
title: Problemi di accesso a Microsoft 365 Apps
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 3c016b198ad43f35c8149dde71c28a2f7fc3bd38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695291"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Schermata di accesso vuota in Microsoft 365 Apps

Per risolvere il problema, provare a eseguire le operazioni seguenti:
- Installare gli aggiornamenti più recenti per [Windows](https://support.microsoft.com/help/4027667/windows-10-update) e [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Reimpostare le opzioni di Internet Explorer: andare a **strumenti**  >  **Internet opzioni**  >  **Avanzate**  >  **reimpostare le impostazioni di Internet Explorer** (si noti che si perderanno le impostazioni personalizzate) e quindi provare a eseguire di nuovo l'accesso a Office.
- Disabilitare Windows Defender Application Guard (WDAG) o qualsiasi altro programma firewall o antivirus analogo al seguente:
    1. Nel pannello di controllo, andare a **programmi**, quindi scegliere **attiva o disattiva le funzionalità di Windows**.
    2. Se è abilitata la protezione dell'applicazione di Windows Defender, provare a disabilitarla.<br/>
    **Nota:** Potrebbe essere necessario riavviare il computer.
- Verificare che il [plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) Microsoft. AAD. BROKERPLUGIN AAD WAM non venga bloccato da alcun programma di applicazioni o firewall/antivirus.
- [Cancellare le credenziali di Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) utilizzando Gestione credenziali di Windows.<br/>
    **Nota:** I percorsi del registro di sistema per Office 2016 sono stati modificati in 16,0. (Es: \Software\Microsoft\Office\16.0\Common\Identity\)

Per ulteriori informazioni, vedere [Connection issues in Sign-in after update to Office 2016 Build 16.0.7967 in Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).