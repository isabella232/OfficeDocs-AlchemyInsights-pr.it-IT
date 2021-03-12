---
title: DLP non funziona come previsto
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 0f07e64c95675a4f6a0aeb6df110fe4e6a21d72f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707814"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="e9138-102">DLP non funziona come previsto</span><span class="sxs-lookup"><span data-stu-id="e9138-102">DLP not working as expected</span></span>

<span data-ttu-id="e9138-103">**Importante**: durante questi periodi senza precedenti, stiamo adottando misure per garantire che i servizi SharePoint Online e OneDrive rimangano disponibili. Per altre informazioni, vedere [Modifiche temporanee delle funzionalità di SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="e9138-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="e9138-104">**Configurazione della prevenzione della perdita dei dati**</span><span class="sxs-lookup"><span data-stu-id="e9138-104">**Setting up DLP**</span></span>

<span data-ttu-id="e9138-105">Si verificano problemi con la prevenzione della perdita dei dati **(DLP)** in Office 365 non funziona come previsto?</span><span class="sxs-lookup"><span data-stu-id="e9138-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="e9138-106">In tal caso, assicurarsi che il criterio **DLP** sia configurato correttamente e che i dati contengano ciò che il criterio **DLP** sta cercando durante la valutazione.</span><span class="sxs-lookup"><span data-stu-id="e9138-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="e9138-107">I criteri DLP consentono di identificare e proteggere le informazioni riservate nell'organizzazione.</span><span class="sxs-lookup"><span data-stu-id="e9138-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="e9138-108">Per configurare i criteri DLP, utilizzare le informazioni [riportate di seguito.](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template)</span><span class="sxs-lookup"><span data-stu-id="e9138-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template).</span></span>
  
 <span data-ttu-id="e9138-109">**Ricerca dei criteri DLP**</span><span class="sxs-lookup"><span data-stu-id="e9138-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="e9138-110">Quando si utilizzano **i tipi** di informazioni riservate predefiniti nei Centri sicurezza e conformità, i criteri DLP ricercano modelli ed elementi specifici quando rilevano questi tipi di dati sensibili.</span><span class="sxs-lookup"><span data-stu-id="e9138-110">When using the **built-in sensitive information types** in the Security and Compliance centers, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="e9138-111">**Tipi di informazioni riservate predefiniti**</span><span class="sxs-lookup"><span data-stu-id="e9138-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="e9138-112">Per informazioni sui tipi di informazioni sensibili predefiniti e sugli elementi cercati da un criterio DLP per rilevare il tipo di dati sensibili, vedere: Cosa vengono cercati i [tipi di informazioni riservate.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="e9138-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="e9138-113">**Tipi di informazioni sensibili personalizzati**</span><span class="sxs-lookup"><span data-stu-id="e9138-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="e9138-114">Se si sta tentando di creare tipi di informazioni sensibili personalizzati, utilizzare l'articolo seguente per informazioni su come creare un tipo di informazioni sensibili personalizzato: Creare un tipo di [informazioni sensibili personalizzato.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)</span><span class="sxs-lookup"><span data-stu-id="e9138-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="e9138-115">**Testare un criterio DLP**</span><span class="sxs-lookup"><span data-stu-id="e9138-115">**Test a DLP policy**</span></span>

<span data-ttu-id="e9138-116">Per testare i dati con un tipo di informazioni sensibili predefinito o personalizzato, usare l'opzione Tipo di **test** in **Classificazioni**  >  **Tipi di informazioni sensibili.**</span><span class="sxs-lookup"><span data-stu-id="e9138-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="e9138-117">Per ulteriori informazioni, vedere [Testare i tipi di informazioni sensibili personalizzati.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center)</span><span class="sxs-lookup"><span data-stu-id="e9138-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="e9138-118">**Report**</span><span class="sxs-lookup"><span data-stu-id="e9138-118">**Reports**</span></span>
  
- <span data-ttu-id="e9138-119">Ottenere informazioni dettagliate sui dati sensibili con [i report DLP.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="e9138-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="e9138-120">Visualizzare dettagli specifici dell'evento con un [Rapporto operazioni non consentite.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports)</span><span class="sxs-lookup"><span data-stu-id="e9138-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span></span>
