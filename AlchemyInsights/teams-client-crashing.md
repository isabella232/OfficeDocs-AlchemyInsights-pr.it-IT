---
title: Il client di Teams si arresta in modo anomalo
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: 7acb2f5f87a9cfbd67cd94efca696665fd80fc4a
ms.sourcegitcommit: 3cdfde87b7311c200431196031af92c640fd0d8d
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 06/29/2021
ms.locfileid: "53187725"
---
# <a name="teams-client-crashing"></a>Il client di Teams si arresta in modo anomalo

Se il client di Teams si arresta in modo anomalo, provare le operazioni seguenti:

- Se si usa l'applicazione desktop di Teams, [verificare che l'app sia completamente aggiornata](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Assicurarsi che tutti gli [intervalli di indirizzi e gli URL di Microsoft 365](/microsoftteams/connectivity-issues) siano accessibili.

- Eseguire l'accesso con l'account amministratore del tenant e controllare il [Dashboard di integrità dei servizi](/office365/enterprise/view-service-health) per verificare che non siano presenti interruzioni o riduzioni delle prestazioni del servizio.

- Disinstallare e reinstallare l'applicazione Teams
    - Passare alla cartella %appdata%\Microsoft\Teams\ sul computer ed eliminare tutti i file di quella directory.
    - [Scaricare e installare l'app di Teams](https://www.microsoft.com/microsoft-teams/download-app) e, se possibile, installare Teams come amministratore (facendo clic con il pulsante destro del mouse sul programma di installazione di Teams e selezionando **Esegui come amministratore**, se disponibile).

Se il client di Teams si arresta ancora in modo anomalo, provare a riprodurre il problema. Se è possibile:

1. Usare la Registrazione azioni utente per acquisire la procedura.
    - Chiudere TUTTE le applicazioni inutili o riservate.
    - Avviare la Registrazione azioni utente e riprodurre il problema durante l'accesso con l'account utente interessato.
    - [Recuperare i log di Teams relativi ai passaggi di riproduzione registrati](/microsoftteams/log-files). **Nota**: assicurarsi di acquisire l'indirizzo di autenticazione dell'utente interessato.
    - Recuperare le informazioni di dump e/o del fault bucket (Windows). Avviare Windows PowerShell sul computer in cui si verifica l'arresto anomalo, ed eseguire questi comandi (dopo ogni comando, premere INVIO):

    `cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`
    `notepad .\FaultBuckets.txt`
    
2. Dopo che il file di testo è stato generato e visualizzato sullo schermo, salvare il file e allegarlo alla richiesta di assistenza. 
