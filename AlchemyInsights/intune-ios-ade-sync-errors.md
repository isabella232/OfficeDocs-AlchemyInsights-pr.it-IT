---
title: Errori di sincronizzazione di Registrazione automatica dispositivi Apple
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: 912c9e56b4c468fb333769f15bd7c212594dc11a
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448926"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="8af7d-102">Errori di sincronizzazione di Registrazione automatica dispositivi Apple</span><span class="sxs-lookup"><span data-stu-id="8af7d-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="8af7d-103">"È stato rilevato che si dispone di uno o più token ADE/DEP in uno stato di errore.</span><span class="sxs-lookup"><span data-stu-id="8af7d-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="8af7d-104">Finché lo stato di errore non viene risolto per ogni token interessato, la funzionalità ADE non funzionerà come previsto.".</span><span class="sxs-lookup"><span data-stu-id="8af7d-104">Until the error state is resolved for each affected token, the ADE functionality will not work as expected.”.</span></span>

<span data-ttu-id="8af7d-105">Questo errore potrebbe manifestarsi in diversi modi, tra cui:</span><span class="sxs-lookup"><span data-stu-id="8af7d-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="8af7d-106">I dispositivi potrebbero non essere sincronizzati da ABM/ASM a Intune</span><span class="sxs-lookup"><span data-stu-id="8af7d-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="8af7d-107">Le assegnazioni del profilo di registrazione potrebbero non riuscire</span><span class="sxs-lookup"><span data-stu-id="8af7d-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="8af7d-108">I dispositivi potrebbero non completare correttamente la registrazione ADE</span><span class="sxs-lookup"><span data-stu-id="8af7d-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="8af7d-109">Controlla l'errore di sincronizzazione segnalato nella console di Intune in Dispositivi > Registrazione dispositivi > i token del programma di registrazione Apple > **registrazione.**</span><span class="sxs-lookup"><span data-stu-id="8af7d-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens**.</span></span>

<span data-ttu-id="8af7d-110">Una delle cause più comuni dell'errore di sincronizzazione è la scadenza del token corrente.</span><span class="sxs-lookup"><span data-stu-id="8af7d-110">One of the most common causes of sync error is expiration of the current token.</span></span> <span data-ttu-id="8af7d-111">In molti casi, il rinnovo del token interessato risolverà il problema.</span><span class="sxs-lookup"><span data-stu-id="8af7d-111">In many cases,renewal of the affected token will resolve the issue.</span></span>

<span data-ttu-id="8af7d-112">Se uno o più token sono scaduti, vedere la documentazione seguente per rinnovarli in base alle esigenze:</span><span class="sxs-lookup"><span data-stu-id="8af7d-112">If one or more of your tokens has expired,  see the following documentation to help you renew them as appropriate:</span></span>

[<span data-ttu-id="8af7d-113">Rinnovare un token di registrazione automatica dei dispositivi</span><span class="sxs-lookup"><span data-stu-id="8af7d-113">Renew an Automated Device Enrollment token</span></span>](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

<span data-ttu-id="8af7d-114">Inoltre, è possibile vedere la documentazione seguente per vedere possibili correzioni per altri errori che causano errori di sincronizzazione dei token:</span><span class="sxs-lookup"><span data-stu-id="8af7d-114">In addition, you can see the following documentation to see potential remediations for other errors causing token synchronization failures:</span></span>

[<span data-ttu-id="8af7d-115">Errori di sincronizzazione ABM/ASM per i token di registrazione dispositivi automatizzati iOS/iPadOS e macOS</span><span class="sxs-lookup"><span data-stu-id="8af7d-115">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[<span data-ttu-id="8af7d-116">Errori di sincronizzazione ABM/ASM per i token di registrazione dispositivi automatizzati iOS/iPadOS e macOS</span><span class="sxs-lookup"><span data-stu-id="8af7d-116">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
