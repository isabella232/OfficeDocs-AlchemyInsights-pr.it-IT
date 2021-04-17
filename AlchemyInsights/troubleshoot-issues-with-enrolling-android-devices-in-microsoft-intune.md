---
title: Risolvere i problemi relativi alla registrazione di dispositivi Android in Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 08620a44dcf693482c65ff05e19f11870f67afbe
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830946"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="7d701-102">Risolvere i problemi relativi alla registrazione di dispositivi Android in Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="7d701-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="7d701-103">Esaminare le risorse elencate di seguito per risolvere il problema.</span><span class="sxs-lookup"><span data-stu-id="7d701-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="7d701-104">Alcuni problemi comuni e passaggi di risoluzione:</span><span class="sxs-lookup"><span data-stu-id="7d701-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="7d701-105">**Errore dispositivo non crittografato nel portale aziendale:** Le versioni più recenti di Android, in particolare a partire da v7.0, richiedono un passcode di avvio per assicurarsi che il dispositivo sia completamente crittografato.</span><span class="sxs-lookup"><span data-stu-id="7d701-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="7d701-106">Le soluzioni comuni sono abilitare un pin di avvio o crittografare completamente il dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7d701-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="7d701-107">Per [ulteriori informazioni,](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) vedere questo documento.</span><span class="sxs-lookup"><span data-stu-id="7d701-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="7d701-108">**I dispositivi non riescono a eseguire il check-in** con il servizio Intune o vengono visualizzati come "non integri" nella console di amministrazione di Intune: Alcuni dispositivi Samsung 4.4 e 5.5 potrebbero non archiviare il servizio.</span><span class="sxs-lookup"><span data-stu-id="7d701-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="7d701-109">Esistono 3 possibili soluzioni a questo problema:</span><span class="sxs-lookup"><span data-stu-id="7d701-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="7d701-110">Apri manualmente l'app Portale aziendale intune, che avvierà automaticamente una sincronizzazione del dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7d701-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="7d701-111">Aggiorna il dispositivo a Android 6.0 o versione successiva.</span><span class="sxs-lookup"><span data-stu-id="7d701-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="7d701-112">Disabilitare Samsung Smart Manager dalla gestione del portale aziendale di Intune.</span><span class="sxs-lookup"><span data-stu-id="7d701-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="7d701-113">Esaminare [questo documento](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) per ulteriori dettagli su questi problemi e soluzioni.</span><span class="sxs-lookup"><span data-stu-id="7d701-113">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="7d701-114">**Tipo di licenza utente Errore** non valido o Nome utente non **riconosciuto:** all'utente deve essere assegnata una licenza di Intune o EMS.</span><span class="sxs-lookup"><span data-stu-id="7d701-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="7d701-115">Esaminare questi documenti per assegnare una licenza tramite: Interfaccia di amministrazione di Office o portale di Azure.</span><span class="sxs-lookup"><span data-stu-id="7d701-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="7d701-116">Risorse aggiuntive per risolvere il problema:</span><span class="sxs-lookup"><span data-stu-id="7d701-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="7d701-117">Usare [Intune Troubleshooting Portal per](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnosticare e risolvere gli errori di registrazione comuni.</span><span class="sxs-lookup"><span data-stu-id="7d701-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="7d701-118">Esaminare [questo documento](https://docs.microsoft.com/intune/help-desk-operators) per ulteriori dettagli.</span><span class="sxs-lookup"><span data-stu-id="7d701-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="7d701-119">Esaminare [questo documento](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) per un elenco degli errori comuni che impediscono la registrazione e le risoluzioni per ognuno di essi.</span><span class="sxs-lookup"><span data-stu-id="7d701-119">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="7d701-120">[Scopri come registrare i dispositivi Android in Microsoft Intune.](https://docs.microsoft.com/intune/android-enroll)</span><span class="sxs-lookup"><span data-stu-id="7d701-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
