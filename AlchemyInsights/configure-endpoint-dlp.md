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
ms.openlocfilehash: d0363d6bdecdb266a5f4a3a14bd496ede6bb9931
ms.sourcegitcommit: 76b147af688f0dc39878a913a050c0e56af054a8
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/29/2020
ms.locfileid: "48305447"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="95e95-102">Configurare Endpoint DLP</span><span class="sxs-lookup"><span data-stu-id="95e95-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="95e95-103">Microsoft Endpoint DLP consente di rafforzare la protezione e il controllo per la prevenzione della perdita dei dati sensibili sui dispositivi Windows 10.</span><span class="sxs-lookup"><span data-stu-id="95e95-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="95e95-104">Una volta completato l'onboarding dei dispositivi in Gestione dispositivi, è possibile creare criteri di prevenzione della perdita dei dati per applicare azioni di protezione per gli elementi.</span><span class="sxs-lookup"><span data-stu-id="95e95-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="95e95-105">Esplora attività può essere usato per monitorare le attività per gli elementi sensibili.</span><span class="sxs-lookup"><span data-stu-id="95e95-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="95e95-106">Per altre informazioni, vedere [Onboarding di dispositivi nella gestione dei dispositivi](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="95e95-106">For more info, see [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="95e95-107">Per iniziare a usare Endpoint DLP:</span><span class="sxs-lookup"><span data-stu-id="95e95-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="95e95-108">Verificare di avere la licenza per SKU/abbonamenti appropriata.</span><span class="sxs-lookup"><span data-stu-id="95e95-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="95e95-109">Per altre informazioni, vedere [Licenze per SKU/abbonamenti](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="95e95-109">For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="95e95-110">Verificare le autorizzazioni necessarie per abilitare la gestione dei dispositivi, accedere alla pagina di onboarding, o attivare o disattivare il controllo dei dispositivi.</span><span class="sxs-lookup"><span data-stu-id="95e95-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="95e95-111">Per altre informazioni, vedere [Autorizzazioni](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="95e95-111">For more info, see [Permissions](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="95e95-112">Eseguire l'onboarding dei dispositivi in Gestione dispositivi seguendo la procedura di onboarding dei dispositivi.</span><span class="sxs-lookup"><span data-stu-id="95e95-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="95e95-113">Se l'opzione Onboarding dispositivi (anteprima) non è presente nelle **Impostazioni** del Centro conformità di M365, verificare di avere la licenza e le autorizzazioni appropriate indicate sopra.</span><span class="sxs-lookup"><span data-stu-id="95e95-113">If you're missing the Device Onboarding (preview) option under M365 Compliance  **Settings**, confirm you have the appropriate license and permissions referenced above.</span></span> <span data-ttu-id="95e95-114">Per altre informazioni, vedere [Onboarding di dispositivi](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="95e95-114">For more info, see [Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="95e95-115">Creare i criteri di prevenzione della perdita dei dati per proteggere gli elementi sensibili.</span><span class="sxs-lookup"><span data-stu-id="95e95-115">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="95e95-116">Per altre informazioni, vedere [Scenari dei criteri di Endpoint DLP](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span><span class="sxs-lookup"><span data-stu-id="95e95-116">For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="95e95-117">Per altre informazioni su Microsoft Endpoint DLP, veder [Informazioni sulla prevenzione della perdita di dati degli endpoint di Microsoft 365 (anteprima)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="95e95-117">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="95e95-118">**Passaggi importanti per la raccolta dei dati, se serve assistenza:**</span><span class="sxs-lookup"><span data-stu-id="95e95-118">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="95e95-119">scaricare MDATP Client Analyzer Preview da [http://aka.ms/betamdatpanalyzer](http://aka.ms/betamdatpanalyzer "http://aka.ms/betamdatpanalyzer")</span><span class="sxs-lookup"><span data-stu-id="95e95-119">Download MDATP Client Analyzer Preview from [http://aka.ms/betamdatpanalyzer](http://aka.ms/betamdatpanalyzer "http://aka.ms/betamdatpanalyzer")</span></span>
2. <span data-ttu-id="95e95-120">Eseguire lo strumento come amministratore dalla finestra di comando:</span><span class="sxs-lookup"><span data-stu-id="95e95-120">Run the tool as Admin from the cmd window:</span></span>
3. <span data-ttu-id="95e95-121">MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t</span><span class="sxs-lookup"><span data-stu-id="95e95-121">MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t</span></span>
4. <span data-ttu-id="95e95-122">Quando viene chiesto di immettere il numero di minuti per raccogliere le tracce, immettere il numero di minuti necessari per eseguire lo scenario</span><span class="sxs-lookup"><span data-stu-id="95e95-122">When prompted with “Enter the number of minutes to collect traces: ", enter the number of minutes that are required to run the scenario</span></span>
5. <span data-ttu-id="95e95-123">Eseguire lo scenario</span><span class="sxs-lookup"><span data-stu-id="95e95-123">Run the scenario</span></span>

<span data-ttu-id="95e95-124">Raccogliere l'output del file ZIP da fornire all'agente di supporto.</span><span class="sxs-lookup"><span data-stu-id="95e95-124">Collect the Zip file output to be given to the Support agent.</span></span>
