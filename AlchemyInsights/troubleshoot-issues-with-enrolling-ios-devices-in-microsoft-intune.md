---
title: Risolvere i problemi relativi alla registrazione dei dispositivi iOS in Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 4aef78e5921b789b532fecc99380da3274173bdb
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708966"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="bec1d-102">Risolvere i problemi relativi alla registrazione dei dispositivi iOS in Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="bec1d-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="bec1d-103">Esaminare le risorse elencate di seguito per risolvere il problema.</span><span class="sxs-lookup"><span data-stu-id="bec1d-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="bec1d-104">Alcuni messaggi di errore comuni e procedure di risoluzione:</span><span class="sxs-lookup"><span data-stu-id="bec1d-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="bec1d-105">**Limite massimo dispositivo raggiunto** L'utente ha più dispositivi registrati rispetto al limite di dispositivi.</span><span class="sxs-lookup"><span data-stu-id="bec1d-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="bec1d-106">Esaminare questi documenti per [rimuovere un dispositivo o](https://docs.microsoft.com/intune/devices-wipe) modificare il limite del [dispositivo.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="bec1d-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="bec1d-107">**Questo servizio non è supportato. Nessun criterio di registrazione:** il servizio apns (Apple Push Notification Service) deve essere configurato o rinnovato.</span><span class="sxs-lookup"><span data-stu-id="bec1d-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="bec1d-108">Leggere [questo documento](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) per istruzioni su come eseguire questa operazione.</span><span class="sxs-lookup"><span data-stu-id="bec1d-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="bec1d-109">**Tipo di licenza utente non valido o Nome utente non riconosciuto:** All'utente deve essere assegnata una licenza di Intune o EMS.</span><span class="sxs-lookup"><span data-stu-id="bec1d-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="bec1d-110">Rivedere questi documenti per assegnare una licenza tramite [l'interfaccia di amministrazione di Office](https://docs.microsoft.com/intune/licenses-assign) o il portale di [Azure.](https://docs.microsoft.com/azure/active-directory/license-users-groups)</span><span class="sxs-lookup"><span data-stu-id="bec1d-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="bec1d-111">Risorse aggiuntive per risolvere il problema:</span><span class="sxs-lookup"><span data-stu-id="bec1d-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="bec1d-112">Usare [il portale per la risoluzione dei](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) problemi di Intune per diagnosticare e risolvere gli errori di registrazione comuni.</span><span class="sxs-lookup"><span data-stu-id="bec1d-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="bec1d-113">Per [ulteriori dettagli,](https://docs.microsoft.com/intune/help-desk-operators) consultare questo documento.</span><span class="sxs-lookup"><span data-stu-id="bec1d-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="bec1d-114">Leggere questi documenti per un elenco di errori comuni che impediscono la registrazione e le risoluzioni: [Guida alla risoluzione dei problemi](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) e [Documento di risoluzione dei problemi](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="bec1d-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="bec1d-115">[Informazioni su come registrare i dispositivi iOS in Microsoft Intune.](https://docs.microsoft.com/intune/ios-enroll)</span><span class="sxs-lookup"><span data-stu-id="bec1d-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

