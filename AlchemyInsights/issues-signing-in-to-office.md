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
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="da94e-102">Schermata di accesso vuota in Microsoft 365 Apps</span><span class="sxs-lookup"><span data-stu-id="da94e-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="da94e-103">Per risolvere il problema, provare a eseguire le operazioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="da94e-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="da94e-104">Installare gli aggiornamenti più recenti per [Windows](https://support.microsoft.com/help/4027667/windows-10-update) e [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="da94e-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="da94e-105">Reimpostare le opzioni di Internet Explorer: andare a **strumenti**  >  **Internet opzioni**  >  **Avanzate**  >  **reimpostare le impostazioni di Internet Explorer** (si noti che si perderanno le impostazioni personalizzate) e quindi provare a eseguire di nuovo l'accesso a Office.</span><span class="sxs-lookup"><span data-stu-id="da94e-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="da94e-106">Disabilitare Windows Defender Application Guard (WDAG) o qualsiasi altro programma firewall o antivirus analogo al seguente:</span><span class="sxs-lookup"><span data-stu-id="da94e-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="da94e-107">Nel pannello di controllo, andare a **programmi**, quindi scegliere **attiva o disattiva le funzionalità di Windows**.</span><span class="sxs-lookup"><span data-stu-id="da94e-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="da94e-108">Se è abilitata la protezione dell'applicazione di Windows Defender, provare a disabilitarla.</span><span class="sxs-lookup"><span data-stu-id="da94e-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="da94e-109">**Nota:** Potrebbe essere necessario riavviare il computer.</span><span class="sxs-lookup"><span data-stu-id="da94e-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="da94e-110">Verificare che il [plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) Microsoft. AAD. BROKERPLUGIN AAD WAM non venga bloccato da alcun programma di applicazioni o firewall/antivirus.</span><span class="sxs-lookup"><span data-stu-id="da94e-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="da94e-111">[Cancellare le credenziali di Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) utilizzando Gestione credenziali di Windows.</span><span class="sxs-lookup"><span data-stu-id="da94e-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="da94e-112">**Nota:** I percorsi del registro di sistema per Office 2016 sono stati modificati in 16,0.</span><span class="sxs-lookup"><span data-stu-id="da94e-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="da94e-113">(Es: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="da94e-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="da94e-114">Per ulteriori informazioni, vedere [Connection issues in Sign-in after update to Office 2016 Build 16.0.7967 in Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="da94e-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>