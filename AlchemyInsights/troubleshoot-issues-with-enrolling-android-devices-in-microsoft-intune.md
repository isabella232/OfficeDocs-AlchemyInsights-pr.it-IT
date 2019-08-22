---
title: Risoluzione dei problemi relativi alla registrazione di dispositivi Android in Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: 1e1d50c31df588a3416d758d40fbd7bde3f73b21
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36500075"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="342a9-102">Risoluzione dei problemi relativi alla registrazione di dispositivi Android in Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="342a9-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="342a9-103">Esaminare le risorse elencate di seguito per risolvere il problema.</span><span class="sxs-lookup"><span data-stu-id="342a9-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="342a9-104">Alcuni problemi comuni e passaggi di risoluzione:</span><span class="sxs-lookup"><span data-stu-id="342a9-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="342a9-105">**Errore del dispositivo non crittografato nel portale aziendale:** Le versioni più recenti di Android, in particolare a partire da v 7.0, richiedono un codice di accesso all'avvio per assicurarsi che il dispositivo sia completamente crittografato.</span><span class="sxs-lookup"><span data-stu-id="342a9-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="342a9-106">Le soluzioni comuni sono l'abilitazione di un pin di avvio o la crittografia completa del dispositivo.</span><span class="sxs-lookup"><span data-stu-id="342a9-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="342a9-107">Per ulteriori informazioni, vedere [questo documento](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) .</span><span class="sxs-lookup"><span data-stu-id="342a9-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="342a9-108">I **dispositivi non riescono a eseguire il check-in con il servizio Intune o a essere visualizzati come "non integri" nella console di amministrazione di Intune:** Alcuni dispositivi Samsung 4,4 e 5,5 potrebbero non archiviare il servizio.</span><span class="sxs-lookup"><span data-stu-id="342a9-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="342a9-109">Esistono tre possibili soluzioni per questo problema:</span><span class="sxs-lookup"><span data-stu-id="342a9-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="342a9-110">Aprire manualmente l'app portale aziendale di Intune, che avvierà automaticamente la sincronizzazione di un dispositivo.</span><span class="sxs-lookup"><span data-stu-id="342a9-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="342a9-111">Aggiornare il dispositivo a Android 6,0 o versione successiva.</span><span class="sxs-lookup"><span data-stu-id="342a9-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="342a9-112">Disabilitare Samsung Smart Manager dalla gestione del portale aziendale di Intune.</span><span class="sxs-lookup"><span data-stu-id="342a9-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="342a9-113">Leggere [questo documento](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) per ulteriori informazioni su questi problemi e risoluzioni.</span><span class="sxs-lookup"><span data-stu-id="342a9-113">Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="342a9-114">**Tipo di licenza utente non valido** o **nome utente errore non riconosciuto:** all'utente deve essere assegnata una licenza Intune o EMS.</span><span class="sxs-lookup"><span data-stu-id="342a9-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="342a9-115">Esaminare questi documenti per assegnare una licenza tramite: interfaccia di amministrazione di Office o portale di Azure.</span><span class="sxs-lookup"><span data-stu-id="342a9-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="342a9-116">Risorse aggiuntive che consentono di risolvere il problema:</span><span class="sxs-lookup"><span data-stu-id="342a9-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="342a9-117">Utilizzare il portale per la [risoluzione dei problemi di Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) per diagnosticare e risolvere gli errori di registrazione comuni.</span><span class="sxs-lookup"><span data-stu-id="342a9-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="342a9-118">Per ulteriori informazioni, vedere [questo documento](https://docs.microsoft.com/intune/help-desk-operators) .</span><span class="sxs-lookup"><span data-stu-id="342a9-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="342a9-119">Esaminare [questo documento](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) per un elenco di errori comuni che impediscono la registrazione e le risoluzioni a ciascuno di essi.</span><span class="sxs-lookup"><span data-stu-id="342a9-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="342a9-120">[Informazioni su come registrare i dispositivi Android in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="342a9-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
