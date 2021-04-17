---
title: Il client di Teams si arresta in modo anomalo?
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
ms.openlocfilehash: 20f03b075787cab85ab15d5272c0416b88ebbaee
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826275"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="d5c4e-102">Il client di Teams si arresta in modo anomalo?</span><span class="sxs-lookup"><span data-stu-id="d5c4e-102">Teams client crashing?</span></span>

<span data-ttu-id="d5c4e-103">Se il client di Teams si arresta in modo anomalo, provare le operazioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="d5c4e-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="d5c4e-104">Se si usa l'applicazione desktop di Teams, [verificare che l'app sia completamente aggiornata](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="d5c4e-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="d5c4e-105">Assicurarsi che tutti gli [intervalli di indirizzi e gli URL di Microsoft 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) siano accessibili.</span><span class="sxs-lookup"><span data-stu-id="d5c4e-105">Make sure all the [Microsoft 365 URLs and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="d5c4e-106">Eseguire l'accesso con l'account amministratore del tenant e controllare il [Dashboard di integrità dei servizi](https://docs.microsoft.com/office365/enterprise/view-service-health) per verificare che non siano presenti interruzioni o riduzioni delle prestazioni del servizio.</span><span class="sxs-lookup"><span data-stu-id="d5c4e-106">Log in with your tenant admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="d5c4e-107">Disinstallare e reinstallare l'applicazione Teams (collegamento)</span><span class="sxs-lookup"><span data-stu-id="d5c4e-107">Uninstall and reinstall the Teams Application (link)</span></span>
    - <span data-ttu-id="d5c4e-108">Passare alla cartella %appdata%\Microsoft\teams\ nel computer e cancellare tutti i file di quella directory.</span><span class="sxs-lookup"><span data-stu-id="d5c4e-108">Browse to the %appdata%\Microsoft\teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="d5c4e-109">[Scaricare e installare l'app di Teams](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy) e, se possibile, installare Teams come amministratore (facendo clic destro sul programma di installazione di Teams e selezionando "Esegui come amministratore" se disponibile).</span><span class="sxs-lookup"><span data-stu-id="d5c4e-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), and if possible, install Teams as an administrator (right click the Teams installer and select "Run as administrator" if available).</span></span>

<span data-ttu-id="d5c4e-110">Se il client di Teams si arresta ancora in modo anomalo, è possibile riprodurre il problema?</span><span class="sxs-lookup"><span data-stu-id="d5c4e-110">If your Teams client is still crashing, can you reproduce the issue?</span></span> <span data-ttu-id="d5c4e-111">In tal caso:</span><span class="sxs-lookup"><span data-stu-id="d5c4e-111">If so:</span></span>

1. <span data-ttu-id="d5c4e-112">Usare la Registrazione azioni utente per acquisire la procedura.</span><span class="sxs-lookup"><span data-stu-id="d5c4e-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="d5c4e-113">Chiudere TUTTE le applicazioni inutili o riservate.</span><span class="sxs-lookup"><span data-stu-id="d5c4e-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="d5c4e-114">Avviare la Registrazione azioni utente e riprodurre il problema durante l'accesso con l'account utente interessato.</span><span class="sxs-lookup"><span data-stu-id="d5c4e-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="d5c4e-115">[Recuperare i log di Teams relativi ai passaggi di riproduzione registrati](https://docs.microsoft.com/microsoftteams/log-files).</span><span class="sxs-lookup"><span data-stu-id="d5c4e-115">[Collect the teams logs that capture the recorded repro steps](https://docs.microsoft.com/microsoftteams/log-files).</span></span> <span data-ttu-id="d5c4e-116">**Nota**: assicurarsi di acquisire l'indirizzo di autenticazione dell'utente interessato.</span><span class="sxs-lookup"><span data-stu-id="d5c4e-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="d5c4e-117">Recuperare le informazioni di dump e/o del fault bucket (Windows).</span><span class="sxs-lookup"><span data-stu-id="d5c4e-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="d5c4e-118">Avviare Windows PowerShell sul computer in cui si verifica l'arresto anomalo, ed eseguire questi comandi:</span><span class="sxs-lookup"><span data-stu-id="d5c4e-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands:</span></span>

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. <span data-ttu-id="d5c4e-119">Allegare il file al caso di supporto.</span><span class="sxs-lookup"><span data-stu-id="d5c4e-119">Attach the file to your support case.</span></span>
