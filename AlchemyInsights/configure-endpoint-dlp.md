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
ms.openlocfilehash: b9369b2c2ca31f7d2fceac37ef1e2252b82e933b
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 05/26/2021
ms.locfileid: "52657933"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="bc42c-102">Configurare Endpoint DLP</span><span class="sxs-lookup"><span data-stu-id="bc42c-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="bc42c-103">Microsoft Endpoint DLP consente di rafforzare la protezione e il controllo per la prevenzione della perdita dei dati sensibili sui dispositivi Windows 10.</span><span class="sxs-lookup"><span data-stu-id="bc42c-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="bc42c-104">Una volta completato l'onboarding dei dispositivi in Gestione dispositivi, è possibile creare criteri di prevenzione della perdita dei dati per applicare azioni di protezione per gli elementi.</span><span class="sxs-lookup"><span data-stu-id="bc42c-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="bc42c-105">Esplora attività può essere usato per monitorare le attività per gli elementi sensibili.</span><span class="sxs-lookup"><span data-stu-id="bc42c-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="bc42c-106">Per altre informazioni, vedere [Onboarding di dispositivi nella gestione dei dispositivi](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="bc42c-106">For more info, see [Onboarding devices into device management](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="bc42c-107">Per iniziare a usare Endpoint DLP:</span><span class="sxs-lookup"><span data-stu-id="bc42c-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="bc42c-108">Verificare di avere la licenza per SKU/abbonamenti appropriata.</span><span class="sxs-lookup"><span data-stu-id="bc42c-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="bc42c-109">Per altre informazioni, vedere [Licenze per SKU/abbonamenti](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="bc42c-109">For more info, see [SKU/subscriptions licensing](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="bc42c-110">Verificare le autorizzazioni necessarie per abilitare la gestione dei dispositivi, accedere alla pagina di onboarding, o attivare o disattivare il controllo dei dispositivi.</span><span class="sxs-lookup"><span data-stu-id="bc42c-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="bc42c-111">Per altre informazioni, vedere [Autorizzazioni](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="bc42c-111">For more info, see [Permissions](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="bc42c-112">Eseguire l'onboarding dei dispositivi in Gestione dispositivi seguendo la procedura di onboarding dei dispositivi.</span><span class="sxs-lookup"><span data-stu-id="bc42c-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="bc42c-113">Per altre informazioni, vedere [Onboarding di dispositivi](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="bc42c-113">For more info, see [Onboarding devices](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="bc42c-114">Creare i criteri di prevenzione della perdita dei dati per proteggere gli elementi sensibili.</span><span class="sxs-lookup"><span data-stu-id="bc42c-114">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="bc42c-115">Per altre informazioni, vedere [Scenari dei criteri di Endpoint DLP](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span><span class="sxs-lookup"><span data-stu-id="bc42c-115">For info, see [Endpoint DLP policy scenarios](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="bc42c-116">Per altre informazioni su Microsoft Endpoint DLP, veder [Informazioni sulla prevenzione della perdita di dati degli endpoint di Microsoft 365 (anteprima)](/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="bc42c-116">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="bc42c-117">**Passaggi importanti per la raccolta dei dati, se serve assistenza:**</span><span class="sxs-lookup"><span data-stu-id="bc42c-117">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="bc42c-118">Scaricare [MDATP Client Analyzer Preview](https://aka.ms/betamdatpanalyzer).</span><span class="sxs-lookup"><span data-stu-id="bc42c-118">Download [MDATP Client Analyzer Preview](https://aka.ms/betamdatpanalyzer).</span></span>
1. <span data-ttu-id="bc42c-119">Eseguire lo strumento come amministratore dalla finestra di comando:</span><span class="sxs-lookup"><span data-stu-id="bc42c-119">Run the tool as Admin from the cmd window:</span></span>

    <span data-ttu-id="bc42c-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span><span class="sxs-lookup"><span data-stu-id="bc42c-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span></span>

1. <span data-ttu-id="bc42c-121">Quando viene richiesto, **Immettere il numero di minuti per raccogliere le tracce:**, immettere il numero di minuti necessari per eseguire lo scenario.</span><span class="sxs-lookup"><span data-stu-id="bc42c-121">When prompted with **Enter the number of minutes to collect traces:**, enter the number of minutes required to run the scenario.</span></span>
1. <span data-ttu-id="bc42c-122">Eseguire lo scenario.</span><span class="sxs-lookup"><span data-stu-id="bc42c-122">Run the scenario.</span></span>

<span data-ttu-id="bc42c-123">Raccogliere l'output del file ZIP da fornire all'agente di supporto.</span><span class="sxs-lookup"><span data-stu-id="bc42c-123">Collect the Zip file output to give to the Support agent.</span></span>
