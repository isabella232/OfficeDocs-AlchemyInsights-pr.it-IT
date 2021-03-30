---
title: Configurare Endpoint DLP
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 36af769b67f8c9aa4b8d17e9f4f3f3b82c8a8534
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402431"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="c71e7-102">Configurare Endpoint DLP</span><span class="sxs-lookup"><span data-stu-id="c71e7-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="c71e7-103">Microsoft Endpoint DLP consente di rafforzare la protezione e il controllo per la prevenzione della perdita dei dati sensibili sui dispositivi Windows 10.</span><span class="sxs-lookup"><span data-stu-id="c71e7-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="c71e7-104">Una volta completato l'onboarding dei dispositivi in Gestione dispositivi, è possibile creare criteri di prevenzione della perdita dei dati per applicare azioni di protezione per gli elementi.</span><span class="sxs-lookup"><span data-stu-id="c71e7-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="c71e7-105">Esplora attività può essere usato per monitorare le attività per gli elementi sensibili.</span><span class="sxs-lookup"><span data-stu-id="c71e7-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="c71e7-106">Per altre informazioni, vedere [Onboarding di dispositivi nella gestione dei dispositivi](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="c71e7-106">For more info, see [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="c71e7-107">Per iniziare a usare Endpoint DLP:</span><span class="sxs-lookup"><span data-stu-id="c71e7-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="c71e7-108">Verificare di avere la licenza per SKU/abbonamenti appropriata.</span><span class="sxs-lookup"><span data-stu-id="c71e7-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="c71e7-109">Per altre informazioni, vedere [Licenze per SKU/abbonamenti](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="c71e7-109">For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="c71e7-110">Verificare le autorizzazioni necessarie per abilitare la gestione dei dispositivi, accedere alla pagina di onboarding, o attivare o disattivare il controllo dei dispositivi.</span><span class="sxs-lookup"><span data-stu-id="c71e7-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="c71e7-111">Per altre informazioni, vedere [Autorizzazioni](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="c71e7-111">For more info, see [Permissions](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="c71e7-112">Eseguire l'onboarding dei dispositivi in Gestione dispositivi seguendo la procedura di onboarding dei dispositivi.</span><span class="sxs-lookup"><span data-stu-id="c71e7-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="c71e7-113">Se l'opzione Onboarding dispositivi (anteprima) non è presente nelle **Impostazioni** del Centro conformità di M365, verificare di avere la licenza e le autorizzazioni appropriate indicate sopra.</span><span class="sxs-lookup"><span data-stu-id="c71e7-113">If you're missing the Device Onboarding (preview) option under M365 Compliance  **Settings**, confirm you have the appropriate license and permissions referenced above.</span></span> <span data-ttu-id="c71e7-114">Per altre informazioni, vedere [Onboarding di dispositivi](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="c71e7-114">For more info, see [Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="c71e7-115">Creare i criteri di prevenzione della perdita dei dati per proteggere gli elementi sensibili.</span><span class="sxs-lookup"><span data-stu-id="c71e7-115">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="c71e7-116">Per altre informazioni, vedere [Scenari dei criteri di Endpoint DLP](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="c71e7-116">For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).</span></span>

<span data-ttu-id="c71e7-117">Per altre informazioni su Microsoft Endpoint DLP, veder [Informazioni sulla prevenzione della perdita di dati degli endpoint di Microsoft 365 (anteprima)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="c71e7-117">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="c71e7-118">**Passaggi importanti per la raccolta dei dati, se serve assistenza:**</span><span class="sxs-lookup"><span data-stu-id="c71e7-118">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="c71e7-119">scaricare MDATP Client Analyzer Preview da [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")</span><span class="sxs-lookup"><span data-stu-id="c71e7-119">Download MDATP Client Analyzer Preview from [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")</span></span>
2. <span data-ttu-id="c71e7-120">Eseguire lo strumento come amministratore dalla finestra di comando:</span><span class="sxs-lookup"><span data-stu-id="c71e7-120">Run the tool as Admin from the cmd window:</span></span>
3. <span data-ttu-id="c71e7-121">MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t</span><span class="sxs-lookup"><span data-stu-id="c71e7-121">MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t</span></span>
4. <span data-ttu-id="c71e7-122">Quando viene chiesto di immettere il numero di minuti per raccogliere le tracce, immettere il numero di minuti necessari per eseguire lo scenario</span><span class="sxs-lookup"><span data-stu-id="c71e7-122">When prompted with “Enter the number of minutes to collect traces: ", enter the number of minutes that are required to run the scenario</span></span>
5. <span data-ttu-id="c71e7-123">Eseguire lo scenario</span><span class="sxs-lookup"><span data-stu-id="c71e7-123">Run the scenario</span></span>

<span data-ttu-id="c71e7-124">Raccogliere l'output del file ZIP da fornire all'agente di supporto.</span><span class="sxs-lookup"><span data-stu-id="c71e7-124">Collect the Zip file output to be given to the Support agent.</span></span>
