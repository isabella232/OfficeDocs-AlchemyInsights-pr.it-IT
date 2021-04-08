---
title: Aggiunta ad Azure Active Directory
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9890"
ms.openlocfilehash: 59e3798131956847a61af2416c2e4210199cffa5
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403835"
---
# <a name="azure-active-directory-join"></a><span data-ttu-id="e9c95-102">Aggiunta ad Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="e9c95-102">Azure Active Directory join</span></span>

1. <span data-ttu-id="e9c95-103">Se stai configurando le registrazioni dei dispositivi per la prima volta, assicurati di aver esaminato Introduzione alla gestione dei dispositivi [in Azure Active Directory](/azure/active-directory/devices/overview) che ti guiderà su come ottenere i dispositivi sotto il controllo di Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e9c95-103">If you are setting up device registrations for the first time, ensure that you have reviewed [Introduction to device management in Azure Active Directory](/azure/active-directory/devices/overview) that will guide you on how to get Devices under the control to Azure AD.</span></span> 
1. <span data-ttu-id="e9c95-104">Se si registrano i dispositivi in Azure AD direttamente e li si registra [in](/mem/intune/fundamentals/licenses-assign) Intune, è necessario assicurarsi di aver configurato [Intune](/mem/intune/enrollment/device-enrollment) e di disporre delle licenze per prime.</span><span class="sxs-lookup"><span data-stu-id="e9c95-104">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](/mem/intune/enrollment/device-enrollment) and have the [licensing](/mem/intune/fundamentals/licenses-assign) in place first.</span></span>
1. <span data-ttu-id="e9c95-105">Assicurarsi di essere autorizzati a eseguire operazioni in Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e9c95-105">Ensure you are authorized to perform operations in Azure AD.</span></span> <span data-ttu-id="e9c95-106">Solo un amministratore globale in Azure AD può gestire le impostazioni per le registrazioni dei dispositivi.</span><span class="sxs-lookup"><span data-stu-id="e9c95-106">Only a global administrator in Azure AD can manage settings for device registrations.</span></span>
1. <span data-ttu-id="e9c95-107">Per eseguire l'implementazione dell'aggiunta ad Azure AD, vedere [Plan Azure AD Join.](/azure/active-directory/devices/azureadjoin-plan)</span><span class="sxs-lookup"><span data-stu-id="e9c95-107">To do Azure AD join implementation, see [Plan Azure AD Join](/azure/active-directory/devices/azureadjoin-plan).</span></span>

<span data-ttu-id="e9c95-108">Per altri dettagli sulla risoluzione dei problemi comuni con l'aggiunta ad Azure AD, vedi Domande frequenti sull'aggiunta ad [Azure Ad](/azure/active-directory/devices/faq) e per il dispositivo Windows 10 pro, vedi Impossibile aggiungere il computer [Windows 10 Pro](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900)ad Azure AD - Necessità di eseguire l'aggiornamento a - Microsoft Community.</span><span class="sxs-lookup"><span data-stu-id="e9c95-108">For more details on resolving common issues with Azure AD join, see [Azure Ad Join FAQ](/azure/active-directory/devices/faq) and for Windows 10 pro device, see [Unable to join Windows 10 Pro machine to Azure AD - Need to upgrade to - Microsoft Community](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900).</span></span>