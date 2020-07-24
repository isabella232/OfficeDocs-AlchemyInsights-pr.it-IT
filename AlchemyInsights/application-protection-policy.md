---
title: Criteri di protezione delle applicazioni
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/22/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1073"
- "6700006"
ms.openlocfilehash: 7fed65e6749f72e6264070b360a52e72968fc8da
ms.sourcegitcommit: 6f7cbf1dc28c0693009ddf03d9768c1c65018964
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 07/22/2020
ms.locfileid: "45266469"
---
# <a name="application-protection-policy"></a><span data-ttu-id="ff3ba-102">Criteri di protezione delle applicazioni</span><span class="sxs-lookup"><span data-stu-id="ff3ba-102">Application protection policy</span></span>

<span data-ttu-id="ff3ba-103">Se non si ha familiarità con i criteri di protezione delle applicazioni (APP), vedere la [Panoramica dei criteri di protezione delle app](https://docs.microsoft.com/intune/apps/app-protection-policy).</span><span class="sxs-lookup"><span data-stu-id="ff3ba-103">If you're new to Application protection policy (APP), check out the [App protection policies overview](https://docs.microsoft.com/intune/apps/app-protection-policy).</span></span>

<span data-ttu-id="ff3ba-104">Per iniziare a usare i criteri di protezione delle applicazioni, vedere [Come creare e assegnare criteri di protezione delle app](https://docs.microsoft.com/intune/app-protection-policies).</span><span class="sxs-lookup"><span data-stu-id="ff3ba-104">To start using APP, see [How to create and assign app protection policies](https://docs.microsoft.com/intune/app-protection-policies).</span></span>

<span data-ttu-id="ff3ba-105">Requisiti dei criteri di protezione delle applicazioni:</span><span class="sxs-lookup"><span data-stu-id="ff3ba-105">Application protection policy requirements:</span></span>

- <span data-ttu-id="ff3ba-106">L'utente ha una licenza di Intune o EMS.</span><span class="sxs-lookup"><span data-stu-id="ff3ba-106">User has an Intune or EMS license.</span></span>
- <span data-ttu-id="ff3ba-107">L'utente appartiene a un gruppo a cui sono assegnati criteri di protezione delle applicazioni.</span><span class="sxs-lookup"><span data-stu-id="ff3ba-107">User belongs to a group targeted by application protection policies.</span></span>
- <span data-ttu-id="ff3ba-108">Un solo utente aziendale è connesso alle app protette su un dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ff3ba-108">Only one corporate user is signed into protected apps on a device.</span></span>
- <span data-ttu-id="ff3ba-109">L'applicazione ha implementato [Intune SDK](https://docs.microsoft.com/intune/app-sdk-get-started).</span><span class="sxs-lookup"><span data-stu-id="ff3ba-109">The application has implemented the [Intune SDK](https://docs.microsoft.com/intune/app-sdk-get-started).</span></span> <span data-ttu-id="ff3ba-110">Per un elenco delle app che supportano l'SDK, vedere [App protette di Microsoft Intune](https://docs.microsoft.com/intune/apps-supported-intune-apps).</span><span class="sxs-lookup"><span data-stu-id="ff3ba-110">For a list of apps that support the SDK, see [Microsoft Intune protected apps](https://docs.microsoft.com/intune/apps-supported-intune-apps).</span></span>

<span data-ttu-id="ff3ba-111">I criteri vengono applicati quando un utente che soddisfa i requisiti precedenti accede a un'app abilitata per Intune SDK.</span><span class="sxs-lookup"><span data-stu-id="ff3ba-111">Policies apply after a user who meets the above requirements signs into an Intune SDK enabled app.</span></span> <span data-ttu-id="ff3ba-112">Il modo più semplice per determinare se un criterio viene applicato consiste nel richiedere che l'utente imposti un PIN nel criterio.</span><span class="sxs-lookup"><span data-stu-id="ff3ba-112">The easiest way to determine if a policy is applied is by requiring that the user set a pin in the policy.</span></span> 

<span data-ttu-id="ff3ba-113">Per altre informazioni, vedere:</span><span class="sxs-lookup"><span data-stu-id="ff3ba-113">For more information, see:</span></span>

[<span data-ttu-id="ff3ba-114">Domande frequenti sulla risoluzione dei problemi relativi a criteri di protezione delle app e MAM</span><span class="sxs-lookup"><span data-stu-id="ff3ba-114">APP/MAM troubleshooting FAQ</span></span>](https://docs.microsoft.com/intune/apps/troubleshoot-mam)  

[<span data-ttu-id="ff3ba-115">Come convalidare la configurazione dei criteri di protezione delle app</span><span class="sxs-lookup"><span data-stu-id="ff3ba-115">How to validate your app protection policy setup</span></span>](https://docs.microsoft.com/intune/app-protection-policies-validate)

[<span data-ttu-id="ff3ba-116">Informazioni sui tempi di recapito dei criteri di protezione delle app</span><span class="sxs-lookup"><span data-stu-id="ff3ba-116">Understand App Protection Policy delivery timing</span></span>](https://docs.microsoft.com/intune/app-protection-policy-delivery)  

[<span data-ttu-id="ff3ba-117">Come monitorare i criteri di protezione delle app</span><span class="sxs-lookup"><span data-stu-id="ff3ba-117">How to monitor app protection policies</span></span>](https://docs.microsoft.com/intune/app-protection-policies-monitor)