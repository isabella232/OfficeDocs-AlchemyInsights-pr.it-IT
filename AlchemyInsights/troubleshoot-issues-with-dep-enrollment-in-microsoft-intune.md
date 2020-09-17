---
title: Risoluzione dei problemi relativi alla registrazione DEP in Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 50aab6e1e3c0d74d2e305e0bdd47c92b3a27c79f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47797300"
---
# <a name="troubleshoot-issues-with-dep-enrollment-in-microsoft-intune"></a><span data-ttu-id="085b2-102">Risoluzione dei problemi relativi alla registrazione DEP in Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="085b2-102">Troubleshoot issues with DEP enrollment in Microsoft Intune</span></span>

<span data-ttu-id="085b2-103">Esaminare le risorse elencate di seguito per risolvere il problema.</span><span class="sxs-lookup"><span data-stu-id="085b2-103">Review the resources listed below to resolve your issue now.</span></span>
  
1. <span data-ttu-id="085b2-104">Se il dispositivo DEP non è in grado di eseguire la registrazione e l'autenticazione a più fattori (multi-factor authentication) è abilitata, disabilitare AMF.</span><span class="sxs-lookup"><span data-stu-id="085b2-104">If DEP device is unable to enroll and MFA (Multi-Factor Authentication) is enabled, please disable MFA.</span></span> <span data-ttu-id="085b2-105">Attualmente l'AMF non è supportata per la registrazione DEP</span><span class="sxs-lookup"><span data-stu-id="085b2-105">Currently MFA is not supported for DEP enrollment</span></span>

2. <span data-ttu-id="085b2-106">Utilizzare il portale per la [risoluzione dei problemi di Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) per diagnosticare e risolvere gli errori di registrazione comuni.</span><span class="sxs-lookup"><span data-stu-id="085b2-106">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="085b2-107">Per ulteriori informazioni, vedere [questo documento](https://docs.microsoft.com/intune/help-desk-operators) .</span><span class="sxs-lookup"><span data-stu-id="085b2-107">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

3. <span data-ttu-id="085b2-108">Esaminare questi documenti per un elenco di errori comuni che impediscono la registrazione e le risoluzioni a ciascuno di essi: [Guida alla risoluzione dei problemi](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) e [risoluzione dei problemi relativi a doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="085b2-108">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)</span></span>

4. <span data-ttu-id="085b2-109">Informazioni [sul programma di registrazione dei dispositivi](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios).</span><span class="sxs-lookup"><span data-stu-id="085b2-109">[Learn about device enrollment program](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios).</span></span>
