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
# <a name="troubleshoot-issues-with-dep-enrollment-in-microsoft-intune"></a><span data-ttu-id="ce20e-102">Risolvere i problemi relativi alla registrazione di Protezione esecuzione programmi in Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="ce20e-102">Troubleshoot issues with DEP enrollment in Microsoft Intune</span></span>

<span data-ttu-id="ce20e-103">Esaminare le risorse elencate di seguito per risolvere il problema.</span><span class="sxs-lookup"><span data-stu-id="ce20e-103">Review the resources listed below to resolve your issue now.</span></span>
  
1. <span data-ttu-id="ce20e-104">Se il dispositivo Dep non è in grado di registrare e la MFA (Multi-Factor Authentication) è abilitata, disabilitare la MFA.</span><span class="sxs-lookup"><span data-stu-id="ce20e-104">If DEP device is unable to enroll and MFA (Multi-Factor Authentication) is enabled, please disable MFA.</span></span> <span data-ttu-id="ce20e-105">L'autenticazione a più fattori attualmente non è supportata per la registrazione di Protezione esecuzione programmi</span><span class="sxs-lookup"><span data-stu-id="ce20e-105">Currently MFA is not supported for DEP enrollment</span></span>

2. <span data-ttu-id="ce20e-106">Usare [Intune Troubleshooting Portal per](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnosticare e risolvere gli errori di registrazione comuni.</span><span class="sxs-lookup"><span data-stu-id="ce20e-106">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="ce20e-107">Esaminare [questo documento](https://docs.microsoft.com/intune/help-desk-operators) per ulteriori dettagli.</span><span class="sxs-lookup"><span data-stu-id="ce20e-107">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

3. <span data-ttu-id="ce20e-108">Esaminare questi documenti per un elenco degli errori comuni che impediscono la registrazione e le risoluzioni a ognuno: [Guida alla](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) risoluzione dei problemi e Documentazione per la risoluzione [dei problemi](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="ce20e-108">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span></span>

4. <span data-ttu-id="ce20e-109">[Informazioni sul programma di registrazione dei dispositivi](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios).</span><span class="sxs-lookup"><span data-stu-id="ce20e-109">[Learn about device enrollment program](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios).</span></span>
