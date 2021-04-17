---
title: Risolvere i problemi relativi alla registrazione di Protezione esecuzione programmi in Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d32afde-47ab-4b1e-a669-662e5dbdc213
ms.custom:
- "783"
- "6200002"
ms.openlocfilehash: 27abeafba5588ca74569ba6bebc5d940b767ea3f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824511"
---
# <a name="troubleshoot-issues-with-dep-enrollment-in-microsoft-intune"></a>Risolvere i problemi relativi alla registrazione di Protezione esecuzione programmi in Microsoft Intune

Esaminare le risorse elencate di seguito per risolvere il problema.
  
1. Se il dispositivo Dep non è in grado di registrare e la MFA (Multi-Factor Authentication) è abilitata, disabilitare la MFA. L'autenticazione a più fattori attualmente non è supportata per la registrazione di Protezione esecuzione programmi

2. Usare [Intune Troubleshooting Portal per](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnosticare e risolvere gli errori di registrazione comuni. Esaminare [questo documento](https://docs.microsoft.com/intune/help-desk-operators) per ulteriori dettagli.

3. Esaminare questi documenti per un elenco degli errori comuni che impediscono la registrazione e le risoluzioni a ognuno: [Guida alla](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) risoluzione dei problemi e Documentazione per la risoluzione [dei problemi](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)

4. [Informazioni sul programma di registrazione dei dispositivi](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios).
