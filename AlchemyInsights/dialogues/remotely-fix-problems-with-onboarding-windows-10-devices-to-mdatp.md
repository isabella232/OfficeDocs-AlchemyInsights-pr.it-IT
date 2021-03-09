---
title: Risolvere in remoto i problemi relativi all'onboarding dei dispositivi Windows 10 in Microsoft Defender Advanced Threat Protection
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 5473d090f6d4680f9a62f34f943ac6cea53b2079
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/08/2021
ms.locfileid: "50530005"
---
# <a name="remotely-fix-problems-with-onboarding-windows-10-devices-to-microsoft-defender-advanced-threat-protection"></a><span data-ttu-id="12c12-102">Risolvere in remoto i problemi relativi all'onboarding dei dispositivi Windows 10 in Microsoft Defender Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="12c12-102">Remotely fix problems with onboarding Windows 10 devices to Microsoft Defender Advanced Threat Protection</span></span>

<span data-ttu-id="12c12-103">Se è possibile accedere al computer remoto, attenersi alla seguente procedura:</span><span class="sxs-lookup"><span data-stu-id="12c12-103">If you can access the remote computer, follow these steps:</span></span>

1. <span data-ttu-id="12c12-104">Scaricare lo strumento di diagnostica [Client Connectivity Analyzer](https://go.microsoft.com/fwlink/?linkid=2143466).</span><span class="sxs-lookup"><span data-stu-id="12c12-104">Download the [Client Connectivity Analyzer](https://go.microsoft.com/fwlink/?linkid=2143466) diagnostic tool.</span></span>
2. <span data-ttu-id="12c12-105">Estrarre ed eseguire MDATPAnalyzer.cmd.</span><span class="sxs-lookup"><span data-stu-id="12c12-105">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="12c12-106">Individuare il registro di diagnostica nella cartella MDATPClientAnalyzerResult, che corrisponde alla stessa cartella in cui è stato scaricato lo strumento Analizzatore.</span><span class="sxs-lookup"><span data-stu-id="12c12-106">Locate the diagnostic log in the MDATPClientAnalyzerResult folder, which is the same folder where the Analyzer tool was downloaded.</span></span>
4. <span data-ttu-id="12c12-107">Per individuare i problemi relativi alle impostazioni di connettività o proxy Internet, esaminare il file di registro MDATPClientAnalyzer.txt.</span><span class="sxs-lookup"><span data-stu-id="12c12-107">To find issues with connectivity or Internet proxy settings, review the log file MDATPClientAnalyzer.txt.</span></span>

<span data-ttu-id="12c12-108">Per altre informazioni, vedi [Problemi con i computer di onboarding.](https://go.microsoft.com/fwlink/?linkid=2143634)</span><span class="sxs-lookup"><span data-stu-id="12c12-108">To learn more, see [Issues with onboarding machines](https://go.microsoft.com/fwlink/?linkid=2143634).</span></span>
