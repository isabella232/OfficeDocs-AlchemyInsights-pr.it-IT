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
ms.openlocfilehash: a56e18ddadef3a2f9056978b8542c1dba8f29665
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932626"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="0044f-102">DLP non funziona come previsto</span><span class="sxs-lookup"><span data-stu-id="0044f-102">DLP not working as expected</span></span>

<span data-ttu-id="0044f-103">**Importante**: molti clienti di SharePoint Online e OneDrive eseguono applicazioni aziendali critiche rispetto al servizio in esecuzione in background.</span><span class="sxs-lookup"><span data-stu-id="0044f-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="0044f-104">Tali applicazioni includono soluzioni per la migrazione del contenuto, di Prevenzione della perdita dei dati e per il backup.</span><span class="sxs-lookup"><span data-stu-id="0044f-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="0044f-105">In questi tempi straordinari, stiamo adottando misure per garantire che i servizi di SharePoint Online e OneDrive rimangano altamente disponibili e affidabili per gli utenti che dipendono ancor più dal servizio negli scenari di lavoro remoto.</span><span class="sxs-lookup"><span data-stu-id="0044f-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="0044f-106">A sostegno di questo obiettivo, abbiamo implementato limitazioni più rigide sulle app in background (migrazione, prevenzione della perdita dei dati e soluzioni di backup) durante il giorni nei giorni feriali.</span><span class="sxs-lookup"><span data-stu-id="0044f-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="0044f-107">In questo periodo sarà possibile notare una riduzione della velocità effettiva in queste app.</span><span class="sxs-lookup"><span data-stu-id="0044f-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="0044f-108">Tuttavia, nelle ore serali e durante il fine settimana nell'area il servizio sarà predisposto per elaborare una quantità notevolmente superiore di richieste delle app in background.</span><span class="sxs-lookup"><span data-stu-id="0044f-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

 <span data-ttu-id="0044f-109">**Configurazione di DLP**</span><span class="sxs-lookup"><span data-stu-id="0044f-109">**Setting up DLP**</span></span>

<span data-ttu-id="0044f-110">Se si riscontrano problemi con la **prevenzione della perdita di dati (DLP)** in Office 365, non funziona come previsto?</span><span class="sxs-lookup"><span data-stu-id="0044f-110">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="0044f-111">In caso affermativo, verificare che i **criteri DLP** siano configurati correttamente e che i dati contengano gli elementi desiderati dal **criterio DLP** quando viene valutato.</span><span class="sxs-lookup"><span data-stu-id="0044f-111">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="0044f-112">I criteri DLP consentono di identificare e proteggere le informazioni riservate nell'organizzazione.</span><span class="sxs-lookup"><span data-stu-id="0044f-112">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="0044f-113">Per configurare i criteri DLP, utilizzare le informazioni [qui](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="0044f-113">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="0044f-114">**Ricerca di criteri DLP**</span><span class="sxs-lookup"><span data-stu-id="0044f-114">**What DLP policies look for**</span></span>
  
<span data-ttu-id="0044f-115">Quando si utilizzano i **tipi di informazioni riservate incorporate** nel centro sicurezza e conformità di Office 365, i criteri DLP cercano modelli ed elementi specifici quando si individuano questi tipi riservati.</span><span class="sxs-lookup"><span data-stu-id="0044f-115">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="0044f-116">**Tipi di informazioni riservate incorporate**</span><span class="sxs-lookup"><span data-stu-id="0044f-116">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="0044f-117">Per informazioni sui tipi riservati incorporati e sull'aspetto di un criterio DLP per il rilevamento del tipo di dati sensibili, vedere: [cosa cercano i tipi di informazioni riservate](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="0044f-117">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="0044f-118">**Tipi di informazioni riservate personalizzate**</span><span class="sxs-lookup"><span data-stu-id="0044f-118">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="0044f-119">Se si sta tentando di creare tipi di informazioni riservate personalizzate, utilizzare l'articolo seguente per informazioni su come creare un tipo di riservatezza personalizzato: [creare un tipo di informazioni riservate personalizzato](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="0044f-119">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="0044f-120">**Testare un criterio DLP**</span><span class="sxs-lookup"><span data-stu-id="0044f-120">**Test a DLP policy**</span></span>

<span data-ttu-id="0044f-121">Per testare i dati con un tipo di informazioni riservate incorporato o personalizzato, utilizzare l' **opzione tipo di test** in **classificazione** > **tipi di informazioni riservate**.</span><span class="sxs-lookup"><span data-stu-id="0044f-121">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="0044f-122">Per ulteriori informazioni, vedere [testare i tipi di informazioni riservate personalizzate](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="0044f-122">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="0044f-123">**Report**</span><span class="sxs-lookup"><span data-stu-id="0044f-123">**Reports**</span></span>
  
- <span data-ttu-id="0044f-124">Ottenere Insight dei dati sensibili con i [report DLP.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="0044f-124">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="0044f-125">Per informazioni dettagliate sull'evento, vedere un [rapporto sulle operazioni](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports)non consentite.</span><span class="sxs-lookup"><span data-stu-id="0044f-125">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
