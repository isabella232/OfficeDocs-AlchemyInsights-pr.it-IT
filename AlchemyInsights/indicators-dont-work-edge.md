---
title: Gli indicatori non funzionano con il browser Microsoft Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11230"
- "9005470"
ms.openlocfilehash: df62d965e0dc2ddb656571af99b1e4c3cb52ea35
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 05/25/2021
ms.locfileid: "52651509"
---
# <a name="indicators-dont-work-using-edge-browser"></a><span data-ttu-id="cda92-102">Gli indicatori non funzionano con il browser Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="cda92-102">Indicators don't work using Edge browser</span></span>

<span data-ttu-id="cda92-103">Dopo la creazione, l'indicatore non viene rispettato da Microsoft Edge (SmartScreen).</span><span class="sxs-lookup"><span data-stu-id="cda92-103">After you created an Indicator, it's not honored by Edge (Smartscreen).</span></span> <span data-ttu-id="cda92-104">Per altre informazioni, vedere [Creare indicatori per IP e URL/domini](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span><span class="sxs-lookup"><span data-stu-id="cda92-104">For more information, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>

## <a name="step-1-ensure-the-following"></a><span data-ttu-id="cda92-105">Passaggio 1: verificare quanto segue</span><span class="sxs-lookup"><span data-stu-id="cda92-105">Step 1: Ensure the following</span></span>

- <span data-ttu-id="cda92-106">Verificare che l'indicatore sia corretto (nessun errore di digitazione in IP/URL, azione corretta, gruppi RBAC corretti).</span><span class="sxs-lookup"><span data-stu-id="cda92-106">Verify that the indicator is correct (no typos in IP/URL, correct action, the correct RBAC groups).</span></span>
- <span data-ttu-id="cda92-107">Attendere almeno 2 ore dopo la creazione dell'indicatore per prendere in considerazione l'eventuale latenza.</span><span class="sxs-lookup"><span data-stu-id="cda92-107">Wait the minimum 2 hours after creating the indicator to take into account any possible latency.</span></span>
- <span data-ttu-id="cda92-108">Verificare che sia stato eseguito l’onboarding dei sistemi in Microsoft Defender per endpoint.</span><span class="sxs-lookup"><span data-stu-id="cda92-108">Confirm that the system(s) are onboarded to Microsoft Defender for Endpoint.</span></span>
- <span data-ttu-id="cda92-109">Verificare che i sistemi riescano a comunicare con il cloud.</span><span class="sxs-lookup"><span data-stu-id="cda92-109">Verify that system(s) can communicate with the Cloud.</span></span>
- <span data-ttu-id="cda92-110">Per verificare che SmartScreen sia abilitato e raggiungibile, accedere al [sito di test](https://demo.smartscreen.msft.net).</span><span class="sxs-lookup"><span data-stu-id="cda92-110">Verify that Smartscreen is enabled and reachable by going to the [test site](https://demo.smartscreen.msft.net).</span></span>

## <a name="step-2-troubleshoot-the-potential-issue"></a><span data-ttu-id="cda92-111">Passaggio 2: risolvere il problema potenziale</span><span class="sxs-lookup"><span data-stu-id="cda92-111">Step 2: Troubleshoot the potential issue</span></span>

- <span data-ttu-id="cda92-112">Verificare che il client soddisfi i requisiti.</span><span class="sxs-lookup"><span data-stu-id="cda92-112">Make sure the client meets the requirements.</span></span> <span data-ttu-id="cda92-113">Per informazioni dettagliate, vedere [Creare indicatori per IP e URL/domini](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span><span class="sxs-lookup"><span data-stu-id="cda92-113">For details, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>
- <span data-ttu-id="cda92-114">Verificare di eseguire la versione più recente del Web browser Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="cda92-114">Make sure you're running the latest version of the Edge browser.</span></span> <span data-ttu-id="cda92-115">Per informazioni sulla versione più recente, vedere [Scopri quale versione di Microsoft Edge possiedi](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb).</span><span class="sxs-lookup"><span data-stu-id="cda92-115">To find out the latest version, see [Find out which version of Microsoft Edge you have](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb).</span></span>
- <span data-ttu-id="cda92-116">Riavviare il Web browser Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="cda92-116">Restart the Edge browser.</span></span>
- <span data-ttu-id="cda92-117">Passare al sito per cui è stato configurato un indicatore.</span><span class="sxs-lookup"><span data-stu-id="cda92-117">Navigate to the site for which you have setup an indicator.</span></span> <span data-ttu-id="cda92-118">Se il sito non viene visualizzato come previsto, procedere al passaggio 3.</span><span class="sxs-lookup"><span data-stu-id="cda92-118">If the site does not appear as expected, continue to Step 3.</span></span> 

## <a name="step-3-collect-data"></a><span data-ttu-id="cda92-119">Passaggio 3: raccogliere dati</span><span class="sxs-lookup"><span data-stu-id="cda92-119">Step 3: Collect data</span></span>

- <span data-ttu-id="cda92-120">Raccogliere i dati di diagnostica **MDEClientAnalyzer**.</span><span class="sxs-lookup"><span data-stu-id="cda92-120">Collect **MDEClientAnalyzer** diagnostic data.</span></span> <span data-ttu-id="cda92-121">Per istruzioni, vedere [Problemi con l’onboarding delle macchine a Microsoft Defender per endpoint](issues-with-onboarding-machines.md).</span><span class="sxs-lookup"><span data-stu-id="cda92-121">For instructions, see [Issues with onboarding machines to Microsoft Defender for Endpoint](issues-with-onboarding-machines.md).</span></span>
- <span data-ttu-id="cda92-122">Se si ha familiarità con l'installazione e la raccolta di una traccia di Fiddler, vedere [Telerik Fiddler](http://www.telerik.com/fiddler).</span><span class="sxs-lookup"><span data-stu-id="cda92-122">If you are comfortable installing and collecting a Fiddler trace, see [Telerik Fiddler](http://www.telerik.com/fiddler).</span></span>
- <span data-ttu-id="cda92-123">Se si preferisce ottenere indicazioni dal supporto tecnico Microsoft, selezionare l'icona Supporto di seguito per aprire un caso di supporto.</span><span class="sxs-lookup"><span data-stu-id="cda92-123">If you prefer guidance from Microsoft Support, select the Support icon below to open a support case.</span></span>
