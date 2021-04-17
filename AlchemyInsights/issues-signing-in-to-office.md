---
title: Problemi di accesso alle app di Microsoft 365
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
ms.openlocfilehash: e6cbab7401fd6168041e7fc31ac97e3be036536d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833043"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="e05d3-102">Schermata di accesso vuota nelle app di Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="e05d3-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="e05d3-103">Per risolvere il problema, provare a eseguire le operazioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="e05d3-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="e05d3-104">Installare gli aggiornamenti più recenti per [Windows](https://support.microsoft.com/help/4027667/windows-10-update) e [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="e05d3-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="e05d3-105">Reimposta le opzioni di Internet Explorer: vai **a** Strumenti Opzioni Internet Reimposta impostazioni  >    >    >  **di Internet Explorer** (tieni presente che le impostazioni personalizzate andranno persi), quindi prova di nuovo ad accedere a Office.</span><span class="sxs-lookup"><span data-stu-id="e05d3-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="e05d3-106">Disabilitare Windows Defender Application Guard (WDAG) o qualsiasi programma firewall o antivirus simile:</span><span class="sxs-lookup"><span data-stu-id="e05d3-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="e05d3-107">Nel Pannello di controllo passare a **Programmi** e quindi scegliere Attiva o disattiva **funzionalità di Windows.**</span><span class="sxs-lookup"><span data-stu-id="e05d3-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="e05d3-108">Se Windows Defender Application Guard è abilitato, provare a disabilitarlo.</span><span class="sxs-lookup"><span data-stu-id="e05d3-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="e05d3-109">**Nota:** Potrebbe essere necessario riavviare il computer.</span><span class="sxs-lookup"><span data-stu-id="e05d3-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="e05d3-110">Verificare che il plug-in Microsoft.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) non sia bloccato da alcuna applicazione o programma firewall/antivirus.</span><span class="sxs-lookup"><span data-stu-id="e05d3-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="e05d3-111">[Cancellare le credenziali di Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) tramite Gestione credenziali di Windows.</span><span class="sxs-lookup"><span data-stu-id="e05d3-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="e05d3-112">**Nota:** I percorsi del Registro di sistema per Office 2016 sono stati modificati in 16.0.</span><span class="sxs-lookup"><span data-stu-id="e05d3-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="e05d3-113">(Ad esempio: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="e05d3-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="e05d3-114">Per ulteriori informazioni, vedere [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)</span><span class="sxs-lookup"><span data-stu-id="e05d3-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>