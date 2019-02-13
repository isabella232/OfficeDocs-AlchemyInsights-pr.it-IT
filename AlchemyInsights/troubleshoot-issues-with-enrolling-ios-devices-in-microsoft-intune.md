---
title: Risoluzione dei problemi con la registrazione di dispositivi iOS in Microsoft Intune
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
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 02/12/2019
ms.locfileid: "29924772"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="73daa-102">Risoluzione dei problemi con la registrazione di dispositivi iOS in Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="73daa-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="73daa-103">Esaminare le risorse elencate di seguito per risolvere il problema ora.</span><span class="sxs-lookup"><span data-stu-id="73daa-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="73daa-104">Alcuni messaggi di errore comuni e la risoluzione dei passaggi:</span><span class="sxs-lookup"><span data-stu-id="73daa-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="73daa-p101">**Cap dispositivo raggiunto** L'utente dispone di più dispositivi registrati rispetto al limite di dispositivi. Leggere questi documenti per [rimuovere un dispositivo](https://docs.microsoft.com/intune/devices-wipe) o [cambiare il limite di dispositivi](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="73daa-p101">**Device Cap Reached** The user has more devices enrolled than the device limit. Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="73daa-p102">**Questo servizio non è supportato. Nessun criterio di registrazione:** Apple Push Notification Service (APNS) deve essere configurato o rinnovato. Leggere [questo documento](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) per istruzioni su come effettuare tale operazione.</span><span class="sxs-lookup"><span data-stu-id="73daa-p102">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed. Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="73daa-p103">**Tipo di licenza utente non valido o il nome utente non riconosciuto:** L'utente deve essere assegnato una licenza Intune o EMS. Leggere questi documenti per assegnare una licenza tramite: [Interfaccia di amministrazione di Office](https://docs.microsoft.com/intune/licenses-assign) o [portale Azure](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="73daa-p103">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license. Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="73daa-111">Risorse aggiuntive per risolvere il problema:</span><span class="sxs-lookup"><span data-stu-id="73daa-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="73daa-p104">Utilizzare [Il portale di risoluzione dei problemi Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) per diagnosticare e risolvere gli errori comuni di registrazione. Leggere [questo documento](https://docs.microsoft.com/intune/help-desk-operators) per ulteriori informazioni.</span><span class="sxs-lookup"><span data-stu-id="73daa-p104">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="73daa-114">Leggere questi documenti per un elenco di errori comuni che impediscono la registrazione e le soluzioni per ognuna: [Guida alla risoluzione dei problemi](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) e [risoluzione dei problemi doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="73daa-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="73daa-115">[Informazioni su come registrare dispositivi iOS in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="73daa-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

