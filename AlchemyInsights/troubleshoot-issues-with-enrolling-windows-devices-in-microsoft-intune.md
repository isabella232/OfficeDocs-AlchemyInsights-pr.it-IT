---
title: Risoluzione dei problemi con la registrazione di dispositivi Windows Intune Microsoft
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.openlocfilehash: 8d19bbd5a5782c7793c87499baf62b2eb7de82ae
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/24/2019
ms.locfileid: "29475933"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="ca156-102">Risoluzione dei problemi con la registrazione di dispositivi Windows Intune Microsoft</span><span class="sxs-lookup"><span data-stu-id="ca156-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="ca156-103">Esaminare le risorse elencate di seguito per risolvere il problema ora.</span><span class="sxs-lookup"><span data-stu-id="ca156-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="ca156-104">Alcuni messaggi di errore comuni e la risoluzione dei passaggi:</span><span class="sxs-lookup"><span data-stu-id="ca156-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="ca156-p101">**Non è installato il software, 0x80cf4017:** Il certificato per l'account è scaduto. Scaricare nuovamente il pacchetto di software PC Client nella Console di amministrazione Intune. Esaminare la documentazione per ulteriori informazioni.</span><span class="sxs-lookup"><span data-stu-id="ca156-p101">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired. Re-download the PC Client software package in the Intune Admin Console. Review this documentation for more information.</span></span> 
  
 <span data-ttu-id="ca156-108">**Codice di errore 0x801c0003:** L'errore può verificarsi nei casi seguenti:</span><span class="sxs-lookup"><span data-stu-id="ca156-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span> 
  
1. <span data-ttu-id="ca156-p102">L'utente dispone di più dispositivi registrati rispetto al limite di dispositivi. Leggere questi documenti per [rimuovere un dispositivo](https://docs.microsoft.com/en-us/intune/devices-wipe) o [cambiare il limite di dispositivi](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="ca156-p102">The user has more devices enrolled than the device limit. Review these documents to [remove a device](https://docs.microsoft.com/en-us/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
2. <span data-ttu-id="ca156-p103">"Gli utenti possono partecipare a dispositivi per Azure Active Directory" è impostato su "none". Impostare su all o selezionare gli utenti. Esaminare la [documentazione](https://docs.microsoft.com/en-us/azure/active-directory/device-management-azure-portal#configure-device-settings) per ulteriori informazioni.</span><span class="sxs-lookup"><span data-stu-id="ca156-p103">"Users may join devices to Azure AD" is set to "none". Set it to all or select users. Review [this documentation](https://docs.microsoft.com/en-us/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span> 
    
3. <span data-ttu-id="ca156-p104">Il dispositivo è già iscritti da un altro utente. In tal caso, rimuovere il dispositivo dalla console Intune Azure o Annulla manualmente iscrizione del dispositivo prima di tentare nuovamente.</span><span class="sxs-lookup"><span data-stu-id="ca156-p104">The device is already enrolled by another user. If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>
    
4. <span data-ttu-id="ca156-p105">Il dispositivo è 10 Windows Home Page. Solo Windows 10 Pro, Education Enterprise SKU e possono partecipare alle Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ca156-p105">The device is Windows 10 Home. Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>
    
<span data-ttu-id="ca156-118">Risorse aggiuntive per risolvere il problema:</span><span class="sxs-lookup"><span data-stu-id="ca156-118">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="ca156-p106">Utilizzare [Il portale di risoluzione dei problemi Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) per diagnosticare e risolvere gli errori comuni di registrazione. Leggere [questo documento](https://docs.microsoft.com/en-us/intune/help-desk-operators) per ulteriori informazioni.</span><span class="sxs-lookup"><span data-stu-id="ca156-p106">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/en-us/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="ca156-121">Leggere questi documenti per un elenco di errori comuni che impediscono la registrazione e le soluzioni per ognuna: [Guida alla risoluzione dei problemi](https://support.microsoft.com/en-us/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) e [risoluzione dei problemi doc](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="ca156-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/en-us/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
<span data-ttu-id="ca156-122">[Informazioni su come registrare i dispositivi Windows Intune Microsoft](https://docs.microsoft.com/en-us/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="ca156-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/en-us/intune/windows-enroll).</span></span>
  

