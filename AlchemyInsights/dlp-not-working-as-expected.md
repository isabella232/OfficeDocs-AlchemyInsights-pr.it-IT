---
title: DLP non funziona come previsto
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 3d8316502b4e51a101197a908cf691f0ab7f845a
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/28/2019
ms.locfileid: "35389617"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="72290-102">DLP non funziona come previsto</span><span class="sxs-lookup"><span data-stu-id="72290-102">DLP not working as expected</span></span>

<span data-ttu-id="72290-103">Se si riscontrano problemi con la **prevenzione della perdita di dati (DLP)** in Office 365, non funziona come previsto?</span><span class="sxs-lookup"><span data-stu-id="72290-103">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="72290-104">In caso affermativo, verificare che i **criteri DLP** siano configurati correttamente e che i dati contengano gli elementi desiderati dal **criterio DLP** quando viene valutato.</span><span class="sxs-lookup"><span data-stu-id="72290-104">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
 <span data-ttu-id="72290-105">**Configurazione del DLP:**</span><span class="sxs-lookup"><span data-stu-id="72290-105">**Setting up DLP:**</span></span>
  
<span data-ttu-id="72290-106">I criteri DLP consentono di identificare e proteggere le informazioni riservate nell'organizzazione.</span><span class="sxs-lookup"><span data-stu-id="72290-106">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="72290-107">Per configurare i criteri DLP, utilizzare le informazioni [qui](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="72290-107">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="72290-108">**Quali criteri DLP cercano:**</span><span class="sxs-lookup"><span data-stu-id="72290-108">**What DLP policies look for:**</span></span>
  
<span data-ttu-id="72290-109">Quando si utilizzano i **tipi di informazioni riservate incorporate** nel centro sicurezza e conformità di Office 365, i criteri DLP cercano modelli ed elementi specifici quando si individuano questi tipi riservati.</span><span class="sxs-lookup"><span data-stu-id="72290-109">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="72290-110">**Tipi di informazioni riservate incorporate:**</span><span class="sxs-lookup"><span data-stu-id="72290-110">**Built-in Sensitive Information Types:**</span></span>

    <span data-ttu-id="72290-111">Per informazioni sui tipi riservati incorporati e sull'aspetto di un criterio DLP per il rilevamento del tipo di dati sensibili, vedere: [cosa cercano i tipi di informazioni riservate](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="72290-111">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="72290-112">**Tipi di informazioni riservate personalizzate:**</span><span class="sxs-lookup"><span data-stu-id="72290-112">**Custom Sensitive Information Types:**</span></span>

    <span data-ttu-id="72290-113">Se si sta tentando di creare tipi di informazioni riservate personalizzate, utilizzare l'articolo seguente per informazioni su come creare un tipo di riservatezza personalizzato: [creare un tipo di informazioni riservate personalizzato](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="72290-113">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

 <span data-ttu-id="72290-114">**Rapporti**</span><span class="sxs-lookup"><span data-stu-id="72290-114">**Reports:**</span></span>
  
- <span data-ttu-id="72290-115">Ottenere Insight dei dati sensibili con i [report DLP.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="72290-115">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="72290-116">Per informazioni dettagliate sull'evento, vedere un [rapporto sulle operazioni](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports)non consentite.</span><span class="sxs-lookup"><span data-stu-id="72290-116">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
