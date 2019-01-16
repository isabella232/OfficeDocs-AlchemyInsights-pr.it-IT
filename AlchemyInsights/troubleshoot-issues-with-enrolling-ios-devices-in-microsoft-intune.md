---
title: Risoluzione dei problemi con la registrazione di dispositivi iOS in Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 663ff9b101494be781095ca550a4ed3deedca175
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/15/2019
ms.locfileid: "28296944"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="1bb12-102">Risoluzione dei problemi con la registrazione di dispositivi iOS in Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="1bb12-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="1bb12-103">Esaminare le risorse elencate di seguito per risolvere il problema ora.</span><span class="sxs-lookup"><span data-stu-id="1bb12-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="1bb12-104">Alcuni messaggi di errore comuni e la risoluzione dei passaggi:</span><span class="sxs-lookup"><span data-stu-id="1bb12-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="1bb12-p101">**Cap dispositivo raggiunto** L'utente dispone di più dispositivi registrati rispetto al limite di dispositivi. Leggere questi documenti per [rimuovere un dispositivo](https://docs.microsoft.com/en-us/intune/devices-wipe) o [cambiare il limite di dispositivi](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="1bb12-p101">**Device Cap Reached** The user has more devices enrolled than the device limit. Review these documents to [remove a device](https://docs.microsoft.com/en-us/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="1bb12-p102">**Questo servizio non è supportato. Nessun criterio di registrazione:** Apple Push Notification Service (APNS) deve essere configurato o rinnovato. Leggere [questo documento](https://docs.microsoft.com/en-us/intune/apple-mdm-push-certificate-get) per istruzioni su come effettuare tale operazione.</span><span class="sxs-lookup"><span data-stu-id="1bb12-p102">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed. Review [this document](https://docs.microsoft.com/en-us/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="1bb12-p103">**Tipo di licenza utente non valido o il nome utente non riconosciuto:** L'utente deve essere assegnato una licenza Intune o EMS. Leggere questi documenti per assegnare una licenza tramite: [Interfaccia di amministrazione di Office](https://docs.microsoft.com/en-us/intune/licenses-assign) o [portale Azure](https://docs.microsoft.com/en-us/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="1bb12-p103">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license. Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/en-us/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/en-us/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="1bb12-111">Risorse aggiuntive per risolvere il problema:</span><span class="sxs-lookup"><span data-stu-id="1bb12-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="1bb12-p104">Utilizzare [Il portale di risoluzione dei problemi Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) per diagnosticare e risolvere gli errori comuni di registrazione. Leggere [questo documento](https://docs.microsoft.com/en-us/intune/help-desk-operators) per ulteriori informazioni.</span><span class="sxs-lookup"><span data-stu-id="1bb12-p104">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/en-us/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="1bb12-114">Leggere questi documenti per un elenco di errori comuni che impediscono la registrazione e le soluzioni per ognuna: [Guida alla risoluzione dei problemi](https://support.microsoft.com/en-us/help/4039809/troubleshooting-ios-device-enrollment-in-intune) e [risoluzione dei problemi doc](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="1bb12-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/en-us/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="1bb12-115">[Informazioni su come registrare dispositivi iOS in Microsoft Intune](https://docs.microsoft.com/en-us/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="1bb12-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/en-us/intune/ios-enroll).</span></span>
    

