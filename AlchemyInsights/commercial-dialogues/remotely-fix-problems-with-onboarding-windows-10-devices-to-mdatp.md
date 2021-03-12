---
title: Risolvere in remoto i problemi relativi all'onboarding di dispositivi Windows 10 in Microsoft Defender Advanced Threat Protection
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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50737009"
---
# <a name="remotely-fix-problems-with-onboarding-windows-10-devices-to-microsoft-defender-advanced-threat-protection"></a>Risolvere in remoto i problemi relativi all'onboarding di dispositivi Windows 10 in Microsoft Defender Advanced Threat Protection

Se è possibile accedere al computer remoto, attenersi alla seguente procedura:

1. Scaricare lo strumento di diagnostica [Client Connectivity Analyzer](https://go.microsoft.com/fwlink/?linkid=2143466).
2. Estrarre ed eseguire MDATPAnalyzer.cmd.
3. Individuare il registro di diagnostica nella cartella MDATPClientAnalyzerResult, che corrisponde alla stessa cartella in cui è stato scaricato lo strumento Analizzatore.
4. Per individuare i problemi relativi alla connettività o alle impostazioni del proxy Internet, esaminare il file di registro MDATPClientAnalyzer.txt.

Per ulteriori informazioni, vedere [Problemi con i computer di onboarding.](https://go.microsoft.com/fwlink/?linkid=2143634)
