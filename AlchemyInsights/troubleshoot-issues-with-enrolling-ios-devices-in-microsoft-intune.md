---
title: Risolvere i problemi relativi alla registrazione dei dispositivi iOS in Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 14f7a897f0c7504db1b605485e170183c3a1afb2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823467"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="6bc08-102">Risolvere i problemi relativi alla registrazione dei dispositivi iOS in Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="6bc08-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="6bc08-103">Esaminare le risorse elencate di seguito per risolvere il problema.</span><span class="sxs-lookup"><span data-stu-id="6bc08-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="6bc08-104">Alcuni messaggi di errore comuni e passaggi di risoluzione:</span><span class="sxs-lookup"><span data-stu-id="6bc08-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="6bc08-105">**Raggiunto il limite massimo del dispositivo** L'utente ha registrato più dispositivi rispetto al limite del dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6bc08-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="6bc08-106">Esaminare questi documenti per [rimuovere un dispositivo o](https://docs.microsoft.com/intune/devices-wipe) modificare il limite del [dispositivo.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="6bc08-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="6bc08-107">**Questo servizio non è supportato. Nessun criterio di registrazione:** apple push notification service (APNS) deve essere configurato o rinnovato.</span><span class="sxs-lookup"><span data-stu-id="6bc08-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="6bc08-108">Leggere [questo documento](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) per istruzioni su come eseguire questa operazione.</span><span class="sxs-lookup"><span data-stu-id="6bc08-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="6bc08-109">**Tipo di licenza utente Non valido o Nome utente non riconosciuto:** All'utente deve essere assegnata una licenza di Intune o EMS.</span><span class="sxs-lookup"><span data-stu-id="6bc08-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="6bc08-110">Esaminare questi documenti per assegnare una licenza tramite: [Interfaccia di amministrazione di Office](https://docs.microsoft.com/intune/licenses-assign) o portale di [Azure.](https://docs.microsoft.com/azure/active-directory/license-users-groups)</span><span class="sxs-lookup"><span data-stu-id="6bc08-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="6bc08-111">Risorse aggiuntive per risolvere il problema:</span><span class="sxs-lookup"><span data-stu-id="6bc08-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="6bc08-112">Usare [Intune Troubleshooting Portal per](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnosticare e risolvere gli errori di registrazione comuni.</span><span class="sxs-lookup"><span data-stu-id="6bc08-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="6bc08-113">Esaminare [questo documento](https://docs.microsoft.com/intune/help-desk-operators) per ulteriori dettagli.</span><span class="sxs-lookup"><span data-stu-id="6bc08-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="6bc08-114">Leggere questi documenti per un elenco di errori comuni che impediscono la registrazione e le risoluzioni: [Guida alla risoluzione dei problemi](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) e [Documento di risoluzione dei problemi](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="6bc08-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="6bc08-115">[Scopri come registrare i dispositivi iOS in Microsoft Intune.](https://docs.microsoft.com/intune/ios-enroll)</span><span class="sxs-lookup"><span data-stu-id="6bc08-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

