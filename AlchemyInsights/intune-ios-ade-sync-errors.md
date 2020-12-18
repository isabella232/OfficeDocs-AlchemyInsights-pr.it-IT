---
title: Errori di sincronizzazione della registrazione automatica del dispositivo Apple
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: d7a9398046a1073e30fdbe2950f750bb55d4fa2f
ms.sourcegitcommit: 87c8d0a1e6668211b9dd5427f98984ccdcadb02d
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/17/2020
ms.locfileid: "49707893"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="7f724-102">Errori di sincronizzazione della registrazione automatica del dispositivo Apple</span><span class="sxs-lookup"><span data-stu-id="7f724-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="7f724-103">"È stato rilevato che si dispone di uno o più token di ADE/DEP che si trovano in uno stato di errore.</span><span class="sxs-lookup"><span data-stu-id="7f724-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="7f724-104">Fino a quando non viene risolto lo stato di errore per ogni token coinvolto, la funzionalità ADE non funzionerà per lo stesso ".</span><span class="sxs-lookup"><span data-stu-id="7f724-104">Until the error state is resolved for each affected token, the ADE functionality will not work for the same”.</span></span>

<span data-ttu-id="7f724-105">Questo errore potrebbe manifestarsi in vari modi, tra cui:</span><span class="sxs-lookup"><span data-stu-id="7f724-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="7f724-106">I dispositivi potrebbero non essere sincronizzati da ABM/ASM a Intune</span><span class="sxs-lookup"><span data-stu-id="7f724-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="7f724-107">Le assegnazioni dei profili di registrazione potrebbero non riuscire</span><span class="sxs-lookup"><span data-stu-id="7f724-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="7f724-108">I dispositivi potrebbero non eseguire correttamente la registrazione ADE</span><span class="sxs-lookup"><span data-stu-id="7f724-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="7f724-109">Controllare l'errore di sincronizzazione riportato nella console di Intune in **dispositivi > registrare i dispositivi > registrazione Apple > i token del programma** di registrazione e consultare la documentazione seguente per visualizzare eventuali correzioni possibili:</span><span class="sxs-lookup"><span data-stu-id="7f724-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens** and review the following documentation to see any potential remediation:</span></span>

[<span data-ttu-id="7f724-110">Errori di sincronizzazione ABM/ASM per i token di registrazione dei dispositivi automatizzati iOS/iPados e macOS</span><span class="sxs-lookup"><span data-stu-id="7f724-110">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
