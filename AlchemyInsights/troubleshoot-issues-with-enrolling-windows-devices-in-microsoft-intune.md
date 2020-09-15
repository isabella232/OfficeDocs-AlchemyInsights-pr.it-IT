---
title: Risoluzione dei problemi relativi alla registrazione di dispositivi Windows in Microsoft Intune
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
ms.openlocfilehash: 13dc77fd2a575fbd227a2a880438b78aaa2c3fb2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658882"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="b9a0e-102">Risoluzione dei problemi relativi alla registrazione di dispositivi Windows in Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="b9a0e-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="b9a0e-103">Esaminare le risorse elencate di seguito per risolvere il problema.</span><span class="sxs-lookup"><span data-stu-id="b9a0e-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="b9a0e-104">Alcuni messaggi di errore comuni e passaggi di risoluzione:</span><span class="sxs-lookup"><span data-stu-id="b9a0e-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="b9a0e-105">**Non è possibile installare il software, 0x80cf4017:** Il certificato dell'account è scaduto.</span><span class="sxs-lookup"><span data-stu-id="b9a0e-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="b9a0e-106">Scaricare di nuovo il pacchetto software client per PC nella console di amministrazione di Intune.</span><span class="sxs-lookup"><span data-stu-id="b9a0e-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="b9a0e-107">Per ulteriori informazioni, vedere la documentazione seguente.</span><span class="sxs-lookup"><span data-stu-id="b9a0e-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="b9a0e-108">**Codice di errore 0x801c0003:** È possibile che l'errore si verifichi negli scenari seguenti:</span><span class="sxs-lookup"><span data-stu-id="b9a0e-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="b9a0e-109">L'utente dispone di più dispositivi registrati rispetto al limite di dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b9a0e-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="b9a0e-110">Esaminare questi documenti per [rimuovere un dispositivo](https://docs.microsoft.com/intune/devices-wipe) o [modificare il limite del dispositivo](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="b9a0e-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="b9a0e-111">"Gli utenti possono aggiungere dispositivi ad Azure AD" è impostato su "None".</span><span class="sxs-lookup"><span data-stu-id="b9a0e-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="b9a0e-112">Impostarla su tutti gli utenti o selezionarli.</span><span class="sxs-lookup"><span data-stu-id="b9a0e-112">Set it to all or select users.</span></span> <span data-ttu-id="b9a0e-113">Per ulteriori informazioni, vedere [la documentazione seguente](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) .</span><span class="sxs-lookup"><span data-stu-id="b9a0e-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="b9a0e-114">Il dispositivo è già registrato da un altro utente.</span><span class="sxs-lookup"><span data-stu-id="b9a0e-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="b9a0e-115">In questo caso, rimuovere il dispositivo dalla console di Azure Intune o annullare la registrazione manuale del dispositivo prima di riprovare.</span><span class="sxs-lookup"><span data-stu-id="b9a0e-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="b9a0e-116">Il dispositivo è Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="b9a0e-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="b9a0e-117">Solo gli SKU di Windows 10 Pro, Education e Enterprise sono in grado di partecipare a Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b9a0e-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="b9a0e-118">Risorse aggiuntive che consentono di risolvere il problema:</span><span class="sxs-lookup"><span data-stu-id="b9a0e-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="b9a0e-119">Utilizzare il portale per la [risoluzione dei problemi di Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) per diagnosticare e risolvere gli errori di registrazione comuni.</span><span class="sxs-lookup"><span data-stu-id="b9a0e-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="b9a0e-120">Per ulteriori informazioni, vedere [questo documento](https://docs.microsoft.com/intune/help-desk-operators) .</span><span class="sxs-lookup"><span data-stu-id="b9a0e-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="b9a0e-121">Leggere questi documenti per un elenco di errori comuni che impediscono la registrazione e le risoluzioni: [Guida alla risoluzione dei problemi](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) e [Documento di risoluzione dei problemi](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="b9a0e-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="b9a0e-122">[Informazioni su come registrare i dispositivi Windows in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="b9a0e-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
