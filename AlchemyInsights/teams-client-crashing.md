---
title: Il client di Teams si arresta in modo anomalo?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: 39310233eae83ceb18c6ff82451ae747f3c50048
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691111"
---
# <a name="teams-client-crashing"></a>Il client di Teams si arresta in modo anomalo?

Se il client di Teams si arresta in modo anomalo, provare le operazioni seguenti:

- Se si usa l'applicazione desktop di Teams, [verificare che l'app sia completamente aggiornata](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Assicurarsi che tutti gli [intervalli di indirizzi e gli URL di Microsoft 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) siano accessibili.

- Eseguire l'accesso con l'account amministratore del tenant e controllare il [Dashboard di integrità dei servizi](https://docs.microsoft.com/office365/enterprise/view-service-health) per verificare che non siano presenti interruzioni o riduzioni delle prestazioni del servizio.

- Disinstallare e reinstallare l'applicazione Teams (collegamento)
    - Passare alla cartella %appdata%\Microsoft\teams\ nel computer e cancellare tutti i file di quella directory.
    - [Scaricare e installare l'app di Teams](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy) e, se possibile, installare Teams come amministratore (facendo clic destro sul programma di installazione di Teams e selezionando "Esegui come amministratore" se disponibile).

Se il client di Teams si arresta ancora in modo anomalo, è possibile riprodurre il problema? In tal caso:

1. Usare la Registrazione azioni utente per acquisire la procedura.
    - Chiudere TUTTE le applicazioni inutili o riservate.
    - Avviare la Registrazione azioni utente e riprodurre il problema durante l'accesso con l'account utente interessato.
    - [Recuperare i log di Teams relativi ai passaggi di riproduzione registrati](https://docs.microsoft.com/microsoftteams/log-files). **Nota**: assicurarsi di acquisire l'indirizzo di autenticazione dell'utente interessato.
    - Recuperare le informazioni di dump e/o del fault bucket (Windows). Avviare Windows PowerShell sul computer in cui si verifica l'arresto anomalo, ed eseguire questi comandi:

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. Allegare il file al caso di supporto.
