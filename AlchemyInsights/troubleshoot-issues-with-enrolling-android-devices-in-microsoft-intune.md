---
title: Risolvere i problemi relativi alla registrazione dei dispositivi Android in Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: cc8c68a1e838f67c4510002b2c7ff5294a4649fe
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709002"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="98244-102">Risolvere i problemi relativi alla registrazione dei dispositivi Android in Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="98244-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="98244-103">Esaminare le risorse elencate di seguito per risolvere il problema.</span><span class="sxs-lookup"><span data-stu-id="98244-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="98244-104">Alcuni problemi comuni e procedure di risoluzione:</span><span class="sxs-lookup"><span data-stu-id="98244-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="98244-105">**Errore dispositivo non crittografato nel portale aziendale:** Le versioni più recenti di Android, in particolare a partire dalla versione 7.0, richiedono un passcode di avvio per assicurarsi che il dispositivo sia completamente crittografato.</span><span class="sxs-lookup"><span data-stu-id="98244-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="98244-106">Le soluzioni comuni sono abilitare un pin di avvio o crittografare completamente il dispositivo.</span><span class="sxs-lookup"><span data-stu-id="98244-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="98244-107">Per [ulteriori informazioni,](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) consultare questo documento.</span><span class="sxs-lookup"><span data-stu-id="98244-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="98244-108">**I dispositivi non riescono a eseguire l'archiviazione** con il servizio Intune o a visualizzare "Non integro" nella console di amministrazione di Intune: Alcuni dispositivi Samsung 4.4 e 5.5 potrebbero non archiviare il servizio.</span><span class="sxs-lookup"><span data-stu-id="98244-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="98244-109">Esistono 3 possibili soluzioni a questo problema:</span><span class="sxs-lookup"><span data-stu-id="98244-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="98244-110">Apri manualmente l'app Portale aziendale intune, che avvierà automaticamente la sincronizzazione del dispositivo.</span><span class="sxs-lookup"><span data-stu-id="98244-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="98244-111">Aggiorna il dispositivo a Android 6.0 o versione successiva.</span><span class="sxs-lookup"><span data-stu-id="98244-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="98244-112">Disabilitare La gestione del portale aziendale di Intune da parte di Samsung Smart Manager.</span><span class="sxs-lookup"><span data-stu-id="98244-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="98244-113">Leggere [questo documento](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) per ulteriori dettagli su questi problemi e soluzioni.</span><span class="sxs-lookup"><span data-stu-id="98244-113">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="98244-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span><span class="sxs-lookup"><span data-stu-id="98244-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="98244-115">Esaminare questi documenti per assegnare una licenza tramite l'interfaccia di amministrazione di Office o il portale di Azure.</span><span class="sxs-lookup"><span data-stu-id="98244-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="98244-116">Risorse aggiuntive per risolvere il problema:</span><span class="sxs-lookup"><span data-stu-id="98244-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="98244-117">Usare [il portale per la risoluzione dei](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) problemi di Intune per diagnosticare e risolvere gli errori di registrazione comuni.</span><span class="sxs-lookup"><span data-stu-id="98244-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="98244-118">Per [ulteriori dettagli,](https://docs.microsoft.com/intune/help-desk-operators) consultare questo documento.</span><span class="sxs-lookup"><span data-stu-id="98244-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="98244-119">Esaminare [questo documento per](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) un elenco degli errori comuni che impediscono la registrazione e le risoluzioni per ognuno di essi.</span><span class="sxs-lookup"><span data-stu-id="98244-119">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="98244-120">[Informazioni su come registrare i dispositivi Android in Microsoft Intune.](https://docs.microsoft.com/intune/android-enroll)</span><span class="sxs-lookup"><span data-stu-id="98244-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
