---
title: Risolvere in remoto i problemi relativi all'onboarding Windows 10 dispositivi a Microsoft Defender Advanced Threat Protection
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
ms.openlocfilehash: 44969436c99b182cb4202fa60e2deb7d6ea3f460e48ee4649de1cfb646970f34
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034038"
---
# <a name="remotely-fix-problems-with-onboarding-windows-10-devices-to-microsoft-defender-advanced-threat-protection"></a>Risolvere in remoto i problemi relativi all'onboarding Windows 10 dispositivi a Microsoft Defender Advanced Threat Protection

Se è possibile accedere al computer remoto, attenersi alla seguente procedura:

1. Scaricare lo strumento di diagnostica [Client Connectivity Analyzer](https://go.microsoft.com/fwlink/?linkid=2143466).
2. Estrarre ed eseguire MDATPAnalyzer.cmd.
3. Individuare il registro di diagnostica nella cartella MDATPClientAnalyzerResult, che corrisponde alla stessa cartella in cui è stato scaricato lo strumento Analizzatore.
4. Per individuare i problemi relativi alla connettività o alle impostazioni del proxy Internet, esaminare il file di registro MDATPClientAnalyzer.txt.

Per ulteriori informazioni, vedere [Problemi con i computer di onboarding.](https://go.microsoft.com/fwlink/?linkid=2143634)
