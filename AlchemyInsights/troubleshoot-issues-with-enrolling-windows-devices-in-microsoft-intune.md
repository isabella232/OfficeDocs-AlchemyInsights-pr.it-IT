---
title: Risoluzione dei problemi relativi alla registrazione di dispositivi Windows in Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: be66135b80f32f78266ef2b6a7b3f5b30e24d5fc
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36559665"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="f4b49-102">Risoluzione dei problemi relativi alla registrazione di dispositivi Windows in Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="f4b49-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="f4b49-103">Esaminare le risorse elencate di seguito per risolvere il problema.</span><span class="sxs-lookup"><span data-stu-id="f4b49-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="f4b49-104">Alcuni messaggi di errore comuni e passaggi di risoluzione:</span><span class="sxs-lookup"><span data-stu-id="f4b49-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="f4b49-105">**Non è possibile installare il software, 0x80cf4017:** Il certificato dell'account è scaduto.</span><span class="sxs-lookup"><span data-stu-id="f4b49-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="f4b49-106">Scaricare di nuovo il pacchetto software client per PC nella console di amministrazione di Intune.</span><span class="sxs-lookup"><span data-stu-id="f4b49-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="f4b49-107">Per ulteriori informazioni, vedere la documentazione seguente.</span><span class="sxs-lookup"><span data-stu-id="f4b49-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="f4b49-108">**Codice di errore 0x801c0003:** È possibile che l'errore si verifichi negli scenari seguenti:</span><span class="sxs-lookup"><span data-stu-id="f4b49-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
1. <span data-ttu-id="f4b49-109">L'utente dispone di più dispositivi registrati rispetto al limite di dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f4b49-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="f4b49-110">Esaminare questi documenti per [rimuovere un dispositivo](https://docs.microsoft.com/intune/devices-wipe) o [modificare il limite del dispositivo](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="f4b49-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

2. <span data-ttu-id="f4b49-111">"Gli utenti possono aggiungere dispositivi ad Azure AD" è impostato su "None".</span><span class="sxs-lookup"><span data-stu-id="f4b49-111">"Users may join devices to Azure AD" is set to "none".</span></span> <span data-ttu-id="f4b49-112">Impostarla su tutti gli utenti o selezionarli.</span><span class="sxs-lookup"><span data-stu-id="f4b49-112">Set it to all or select users.</span></span> <span data-ttu-id="f4b49-113">Per ulteriori informazioni, vedere [la documentazione seguente](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) .</span><span class="sxs-lookup"><span data-stu-id="f4b49-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

3. <span data-ttu-id="f4b49-114">Il dispositivo è già registrato da un altro utente.</span><span class="sxs-lookup"><span data-stu-id="f4b49-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="f4b49-115">In questo caso, rimuovere il dispositivo dalla console di Azure Intune o annullare la registrazione manuale del dispositivo prima di riprovare.</span><span class="sxs-lookup"><span data-stu-id="f4b49-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

4. <span data-ttu-id="f4b49-116">Il dispositivo è Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="f4b49-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="f4b49-117">Solo gli SKU di Windows 10 Pro, Education e Enterprise sono in grado di partecipare a Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f4b49-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="f4b49-118">Risorse aggiuntive che consentono di risolvere il problema:</span><span class="sxs-lookup"><span data-stu-id="f4b49-118">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="f4b49-119">Utilizzare il portale per la [risoluzione dei problemi di Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) per diagnosticare e risolvere gli errori di registrazione comuni.</span><span class="sxs-lookup"><span data-stu-id="f4b49-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="f4b49-120">Per ulteriori informazioni, vedere [questo documento](https://docs.microsoft.com/intune/help-desk-operators) .</span><span class="sxs-lookup"><span data-stu-id="f4b49-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="f4b49-121">Esaminare questi documenti per un elenco di errori comuni che impediscono la registrazione e le risoluzioni a ciascuno di essi: [Guida alla risoluzione dei problemi](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) e [risoluzione dei problemi relativi al documento](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="f4b49-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="f4b49-122">[Informazioni su come registrare i dispositivi Windows in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="f4b49-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
