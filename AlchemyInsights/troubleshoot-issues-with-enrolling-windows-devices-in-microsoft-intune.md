---
title: Risolvere i problemi relativi alla registrazione dei dispositivi Windows in Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 88105671ef6dc34553a265937bf1fb3463353963
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708894"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="2e60c-102">Risolvere i problemi relativi alla registrazione dei dispositivi Windows in Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="2e60c-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="2e60c-103">Esaminare le risorse elencate di seguito per risolvere il problema.</span><span class="sxs-lookup"><span data-stu-id="2e60c-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="2e60c-104">Alcuni messaggi di errore comuni e procedure di risoluzione:</span><span class="sxs-lookup"><span data-stu-id="2e60c-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="2e60c-105">**Il software non può essere installato, 0x80cf4017:** Il certificato dell'account è scaduto.</span><span class="sxs-lookup"><span data-stu-id="2e60c-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="2e60c-106">Scaricare di nuovo il pacchetto software del client PC nella console di amministrazione di Intune.</span><span class="sxs-lookup"><span data-stu-id="2e60c-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="2e60c-107">Per ulteriori informazioni, vedere questa documentazione.</span><span class="sxs-lookup"><span data-stu-id="2e60c-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="2e60c-108">**Codice di errore 0x801c0003:** L'errore può verificarsi negli scenari seguenti:</span><span class="sxs-lookup"><span data-stu-id="2e60c-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="2e60c-109">L'utente ha più dispositivi registrati rispetto al limite di dispositivi.</span><span class="sxs-lookup"><span data-stu-id="2e60c-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="2e60c-110">Esaminare questi documenti per [rimuovere un dispositivo o](https://docs.microsoft.com/intune/devices-wipe) modificare il limite del [dispositivo.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="2e60c-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="2e60c-111">"Gli utenti possono aggiungere dispositivi ad Azure AD" è impostato su "nessuno".</span><span class="sxs-lookup"><span data-stu-id="2e60c-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="2e60c-112">Impostarla su tutti gli utenti o selezionarli.</span><span class="sxs-lookup"><span data-stu-id="2e60c-112">Set it to all or select users.</span></span> <span data-ttu-id="2e60c-113">Per [ulteriori informazioni, consultare](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) questa documentazione.</span><span class="sxs-lookup"><span data-stu-id="2e60c-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="2e60c-114">Il dispositivo è già registrato da un altro utente.</span><span class="sxs-lookup"><span data-stu-id="2e60c-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="2e60c-115">In questo caso, rimuovere il dispositivo dalla console di Azure Intune o annullare manualmente la registrazione del dispositivo prima di riprovare.</span><span class="sxs-lookup"><span data-stu-id="2e60c-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="2e60c-116">Il dispositivo è Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="2e60c-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="2e60c-117">Solo le SKU Windows 10 Pro, Education ed Enterprise possono aggiungersi ad Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="2e60c-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="2e60c-118">Risorse aggiuntive per risolvere il problema:</span><span class="sxs-lookup"><span data-stu-id="2e60c-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="2e60c-119">Usare [il portale per la risoluzione dei](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) problemi di Intune per diagnosticare e risolvere gli errori di registrazione comuni.</span><span class="sxs-lookup"><span data-stu-id="2e60c-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="2e60c-120">Per [ulteriori dettagli,](https://docs.microsoft.com/intune/help-desk-operators) consultare questo documento.</span><span class="sxs-lookup"><span data-stu-id="2e60c-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="2e60c-121">Leggere questi documenti per un elenco di errori comuni che impediscono la registrazione e le risoluzioni: [Guida alla risoluzione dei problemi](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) e [Documento di risoluzione dei problemi](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="2e60c-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="2e60c-122">[Informazioni su come registrare i dispositivi Windows in Microsoft Intune.](https://docs.microsoft.com/intune/windows-enroll)</span><span class="sxs-lookup"><span data-stu-id="2e60c-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
