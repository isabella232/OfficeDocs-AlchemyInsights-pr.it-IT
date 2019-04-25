---
title: Risolvere i problemi relativi alla registrazione dei dispositivi iOS in Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: d28dca4fccf823e627dd179f828ba3b8baf843a6
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32391011"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="8e138-102">Risolvere i problemi relativi alla registrazione dei dispositivi iOS in Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="8e138-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="8e138-103">Esaminare le risorse elencate di seguito per risolvere il problema.</span><span class="sxs-lookup"><span data-stu-id="8e138-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="8e138-104">Alcuni messaggi di errore comuni e passaggi di risoluzione:</span><span class="sxs-lookup"><span data-stu-id="8e138-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="8e138-105">**Tappo del dispositivo raggiunto** L'utente dispone di più dispositivi registrati rispetto al limite di dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8e138-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="8e138-106">Esaminare questi documenti per [rimuovere un dispositivo](https://docs.microsoft.com/intune/devices-wipe) o [modificare il limite del dispositivo](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="8e138-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="8e138-107">**Questo servizio non è supportato. Nessun criterio di registrazione:** è necessario configurare o rinnovare il servizio di notifica push di Apple (APNS).</span><span class="sxs-lookup"><span data-stu-id="8e138-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="8e138-108">Leggere [questo documento](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) per istruzioni su come eseguire questa operazione.</span><span class="sxs-lookup"><span data-stu-id="8e138-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="8e138-109">**Tipo di licenza utente non valido o nome utente non riconosciuto:** All'utente deve essere assegnata una licenza Intune o EMS.</span><span class="sxs-lookup"><span data-stu-id="8e138-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="8e138-110">Esaminare questi documenti per assegnare una licenza tramite: interfaccia di [amministrazione di Office](https://docs.microsoft.com/intune/licenses-assign) o [portale di Azure](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="8e138-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="8e138-111">Risorse aggiuntive che consentono di risolvere il problema:</span><span class="sxs-lookup"><span data-stu-id="8e138-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="8e138-112">Utilizzare il portale per la [risoluzione dei problemi di Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) per diagnosticare e risolvere gli errori di registrazione comuni.</span><span class="sxs-lookup"><span data-stu-id="8e138-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="8e138-113">Per ulteriori informazioni, vedere [questo documento](https://docs.microsoft.com/intune/help-desk-operators) .</span><span class="sxs-lookup"><span data-stu-id="8e138-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="8e138-114">Esaminare questi documenti per un elenco di errori comuni che impediscono la registrazione e le risoluzioni a ciascuno di essi: [Guida alla risoluzione dei problemi](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) e [risoluzione dei problemi relativi al documento](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="8e138-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="8e138-115">[Informazioni su come registrare i dispositivi iOS in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="8e138-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

