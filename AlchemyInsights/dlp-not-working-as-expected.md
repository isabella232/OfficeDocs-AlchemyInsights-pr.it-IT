---
title: DLP non funziona come previsto
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: e96904e2f0da2fe1fafb3f8722465eaf22681b71
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507482"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="7c1f3-102">DLP non funziona come previsto</span><span class="sxs-lookup"><span data-stu-id="7c1f3-102">DLP not working as expected</span></span>

<span data-ttu-id="7c1f3-103">**Importante**: durante questi periodi senza precedenti, stiamo adottando misure per garantire che i servizi SharePoint Online e OneDrive rimangano disponibili. Per altre informazioni, vedere [Modifiche temporanee delle funzionalità di SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="7c1f3-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="7c1f3-104">**Configurazione di DLP**</span><span class="sxs-lookup"><span data-stu-id="7c1f3-104">**Setting up DLP**</span></span>

<span data-ttu-id="7c1f3-105">Se si riscontrano problemi con la **prevenzione della perdita di dati (DLP)** in Office 365, non funziona come previsto?</span><span class="sxs-lookup"><span data-stu-id="7c1f3-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="7c1f3-106">In caso affermativo, verificare che i **criteri DLP** siano configurati correttamente e che i dati contengano gli elementi desiderati dal **criterio DLP** quando viene valutato.</span><span class="sxs-lookup"><span data-stu-id="7c1f3-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="7c1f3-107">I criteri DLP consentono di identificare e proteggere le informazioni riservate nell'organizzazione.</span><span class="sxs-lookup"><span data-stu-id="7c1f3-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="7c1f3-108">Per configurare i criteri DLP, utilizzare le informazioni [qui](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="7c1f3-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="7c1f3-109">**Ricerca di criteri DLP**</span><span class="sxs-lookup"><span data-stu-id="7c1f3-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="7c1f3-110">Quando si utilizzano i **tipi di informazioni riservate incorporate** nei centri sicurezza e conformità, i criteri DLP cercano modelli ed elementi specifici quando si individuano questi tipi riservati.</span><span class="sxs-lookup"><span data-stu-id="7c1f3-110">When using the **built-in sensitive information types** in the Security and Compliance centers, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="7c1f3-111">**Tipi di informazioni riservate incorporate**</span><span class="sxs-lookup"><span data-stu-id="7c1f3-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="7c1f3-112">Per informazioni sui tipi riservati incorporati e sull'aspetto di un criterio DLP per il rilevamento del tipo di dati sensibili, vedere: [cosa cercano i tipi di informazioni riservate](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="7c1f3-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="7c1f3-113">**Tipi di informazioni riservate personalizzate**</span><span class="sxs-lookup"><span data-stu-id="7c1f3-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="7c1f3-114">Se si sta tentando di creare tipi di informazioni riservate personalizzate, utilizzare l'articolo seguente per informazioni su come creare un tipo di riservatezza personalizzato: [creare un tipo di informazioni riservate personalizzato](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="7c1f3-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="7c1f3-115">**Testare un criterio DLP**</span><span class="sxs-lookup"><span data-stu-id="7c1f3-115">**Test a DLP policy**</span></span>

<span data-ttu-id="7c1f3-116">Per testare i dati con un tipo di informazioni riservate incorporato o personalizzato, utilizzare l'opzione **tipo di test** in **classificazione**  >  **tipi di informazioni riservate**.</span><span class="sxs-lookup"><span data-stu-id="7c1f3-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="7c1f3-117">Per ulteriori informazioni, vedere [testare i tipi di informazioni riservate personalizzate](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="7c1f3-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="7c1f3-118">**Report**</span><span class="sxs-lookup"><span data-stu-id="7c1f3-118">**Reports**</span></span>
  
- <span data-ttu-id="7c1f3-119">Ottenere Insight dei dati sensibili con i [report DLP.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="7c1f3-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="7c1f3-120">Per informazioni dettagliate sull'evento, vedere un [rapporto sulle operazioni](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports)non consentite.</span><span class="sxs-lookup"><span data-stu-id="7c1f3-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span></span>
