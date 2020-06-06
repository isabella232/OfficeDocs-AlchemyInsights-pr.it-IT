---
title: Problemi di accesso a Microsoft 365 Apps
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 4658b4df8a48072b4cc9d72bf503d7911bb5126b
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579905"
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