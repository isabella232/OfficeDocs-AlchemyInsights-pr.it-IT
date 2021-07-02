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
# <a name="teams-client-crashing"></a><span data-ttu-id="84e37-102">Il client di Teams si arresta in modo anomalo</span><span class="sxs-lookup"><span data-stu-id="84e37-102">Teams client crashing</span></span>

<span data-ttu-id="84e37-103">Se il client di Teams si arresta in modo anomalo, provare le operazioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="84e37-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="84e37-104">Se si usa l'applicazione desktop di Teams, [verificare che l'app sia completamente aggiornata](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="84e37-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="84e37-105">Assicurarsi che tutti gli [intervalli di indirizzi e gli URL di Microsoft 365](/microsoftteams/connectivity-issues) siano accessibili.</span><span class="sxs-lookup"><span data-stu-id="84e37-105">Make sure all the [Microsoft 365 URLs and address ranges](/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="84e37-106">Eseguire l'accesso con l'account amministratore del tenant e controllare il [Dashboard di integrità dei servizi](/office365/enterprise/view-service-health) per verificare che non siano presenti interruzioni o riduzioni delle prestazioni del servizio.</span><span class="sxs-lookup"><span data-stu-id="84e37-106">Log in with your tenant admin account and check your [Service Health Dashboard](/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="84e37-107">Disinstallare e reinstallare l'applicazione Teams</span><span class="sxs-lookup"><span data-stu-id="84e37-107">Uninstall and reinstall the Teams Application</span></span>
    - <span data-ttu-id="84e37-108">Passare alla cartella %appdata%\Microsoft\Teams\ sul computer ed eliminare tutti i file di quella directory.</span><span class="sxs-lookup"><span data-stu-id="84e37-108">Browse to the %appdata%\Microsoft\Teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="84e37-109">[Scaricare e installare l'app di Teams](https://www.microsoft.com/microsoft-teams/download-app) e, se possibile, installare Teams come amministratore (facendo clic con il pulsante destro del mouse sul programma di installazione di Teams e selezionando **Esegui come amministratore**, se disponibile).</span><span class="sxs-lookup"><span data-stu-id="84e37-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-teams/download-app), and if possible, install Teams as an administrator (right-click the Teams installer, and select **Run as administrator** if available).</span></span>

<span data-ttu-id="84e37-110">Se il client di Teams si arresta ancora in modo anomalo, provare a riprodurre il problema.</span><span class="sxs-lookup"><span data-stu-id="84e37-110">If your Teams client is still crashing, try to reproduce the issue.</span></span> <span data-ttu-id="84e37-111">Se è possibile:</span><span class="sxs-lookup"><span data-stu-id="84e37-111">If you can:</span></span>

1. <span data-ttu-id="84e37-112">Usare la Registrazione azioni utente per acquisire la procedura.</span><span class="sxs-lookup"><span data-stu-id="84e37-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="84e37-113">Chiudere TUTTE le applicazioni inutili o riservate.</span><span class="sxs-lookup"><span data-stu-id="84e37-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="84e37-114">Avviare la Registrazione azioni utente e riprodurre il problema durante l'accesso con l'account utente interessato.</span><span class="sxs-lookup"><span data-stu-id="84e37-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="84e37-115">[Recuperare i log di Teams relativi ai passaggi di riproduzione registrati](/microsoftteams/log-files).</span><span class="sxs-lookup"><span data-stu-id="84e37-115">[Collect the teams logs that capture the recorded repro steps](/microsoftteams/log-files).</span></span> <span data-ttu-id="84e37-116">**Nota**: assicurarsi di acquisire l'indirizzo di autenticazione dell'utente interessato.</span><span class="sxs-lookup"><span data-stu-id="84e37-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="84e37-117">Recuperare le informazioni di dump e/o del fault bucket (Windows).</span><span class="sxs-lookup"><span data-stu-id="84e37-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="84e37-118">Avviare Windows PowerShell sul computer in cui si verifica l'arresto anomalo, ed eseguire questi comandi (dopo ogni comando, premere INVIO):</span><span class="sxs-lookup"><span data-stu-id="84e37-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands (after each command, press Enter):</span></span>

    <span data-ttu-id="84e37-119">`cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`</span><span class="sxs-lookup"><span data-stu-id="84e37-119">`cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`</span></span>
    `notepad .\FaultBuckets.txt`
    
2. <span data-ttu-id="84e37-120">Dopo che il file di testo è stato generato e visualizzato sullo schermo, salvare il file e allegarlo alla richiesta di assistenza.</span><span class="sxs-lookup"><span data-stu-id="84e37-120">After the text file is generated and appears on your screen, save the file and attach it to the service request.</span></span> 
