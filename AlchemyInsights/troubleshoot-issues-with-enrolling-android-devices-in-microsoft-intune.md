---
title: Risoluzione dei problemi con la registrazione di dispositivi Android Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.openlocfilehash: 0e727bd47a7d549a439e4666fa9dbb8a02e39778
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 02/12/2019
ms.locfileid: "29939352"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="abee9-102">Risoluzione dei problemi con la registrazione di dispositivi Android Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="abee9-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="abee9-103">Esaminare le risorse elencate di seguito per risolvere il problema ora.</span><span class="sxs-lookup"><span data-stu-id="abee9-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="abee9-104">Alcuni problemi comuni e la risoluzione dei passaggi:</span><span class="sxs-lookup"><span data-stu-id="abee9-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="abee9-p101">**Dispositivo non crittografate errore nel portale aziendale:** Versioni più recenti di Android, in particolare a partire da v 7.0, richiedono un passcode di avvio per verificare che il dispositivo è completamente crittografato. Per attivare un pin avvio o completamente crittografare il dispositivo sono soluzioni comuni. Leggere [questo documento](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) per ulteriori informazioni.</span><span class="sxs-lookup"><span data-stu-id="abee9-p101">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted. Common solutions are to enable a startup pin or fully encrypt the device. Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span> 
  
 <span data-ttu-id="abee9-p102">**Riusciranno a verificare con il servizio Intune o visualizzato come "Problematica" la console di amministrazione Intune:** Alcuni 4.4 Samsung e 5.5 dispositivi non possono controllare nel servizio. Sono disponibili 3 possibili soluzioni a questo problema:</span><span class="sxs-lookup"><span data-stu-id="abee9-p102">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service. There are 3 possible solutions to this issue:</span></span> 
  
1. <span data-ttu-id="abee9-110">Aprire manualmente app Intune portale della società, che verrà avviata automaticamente la sincronizzazione del dispositivo.</span><span class="sxs-lookup"><span data-stu-id="abee9-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>
    
2. <span data-ttu-id="abee9-111">Aggiornare il dispositivo a Android 6.0 o versioni successive.</span><span class="sxs-lookup"><span data-stu-id="abee9-111">Update the device to Android 6.0 or higher.</span></span>
    
3. <span data-ttu-id="abee9-p103">Disabilitare Samsung Smart Manager di gestione del portale aziendale Intune. Leggere [questo documento](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) per ulteriori informazioni su questi problemi e soluzioni.</span><span class="sxs-lookup"><span data-stu-id="abee9-p103">Disable Samsung Smart Manager from managing the Intune Company Portal. Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span> 
    
 <span data-ttu-id="abee9-p104">**Utente licenza tipo valido** o **nome utente non riconosciuto errore:** è necessario assegnare una licenza Intune o em. Leggere questi documenti per assegnare una licenza a: portale di interfaccia di amministrazione di Office o Azure.</span><span class="sxs-lookup"><span data-stu-id="abee9-p104">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license. Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span> 
  
<span data-ttu-id="abee9-116">Risorse aggiuntive per risolvere il problema:</span><span class="sxs-lookup"><span data-stu-id="abee9-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="abee9-p105">Utilizzare [Il portale di risoluzione dei problemi Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) per diagnosticare e risolvere gli errori comuni di registrazione. Leggere [questo documento](https://docs.microsoft.com/intune/help-desk-operators) per ulteriori informazioni.</span><span class="sxs-lookup"><span data-stu-id="abee9-p105">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="abee9-119">Leggere [questo documento](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) per un elenco di errori comuni che impediscono la registrazione e le soluzioni per ognuno.</span><span class="sxs-lookup"><span data-stu-id="abee9-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span> 
    
3. <span data-ttu-id="abee9-120">[Informazioni su come registrare dispositivi Android Intune Microsoft](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="abee9-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
    

