---
title: Risoluzione dei problemi relativi alla registrazione DEP in Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d32afde-47ab-4b1e-a669-662e5dbdc213
ms.custom:
- "783"
- "6200002"
ms.openlocfilehash: 3df961859cc1e3394ed0e8d779718823ae446d37
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/28/2019
ms.locfileid: "35353649"
---
# <a name="troubleshoot-issues-with-dep-enrollment-in-microsoft-intune"></a>Risoluzione dei problemi relativi alla registrazione DEP in Microsoft Intune

Esaminare le risorse elencate di seguito per risolvere il problema.
  
1. Se il dispositivo DEP non è in grado di eseguire la registrazione e l'autenticazione a più fattori (multi-factor authentication) è abilitata, disabilitare AMF. Attualmente l'AMF non è supportata per la registrazione DEP

2. Utilizzare il portale per la [risoluzione dei problemi di Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) per diagnosticare e risolvere gli errori di registrazione comuni. Per ulteriori informazioni, vedere [questo documento](https://docs.microsoft.com/intune/help-desk-operators) .

3. Esaminare questi documenti per un elenco di errori comuni che impediscono la registrazione e le risoluzioni a ciascuno di essi: [Guida alla risoluzione dei problemi](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) e [risoluzione dei problemi relativi a doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)

4. Informazioni [sul programma di registrazione dei dispositivi](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios).
