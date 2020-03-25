---
title: Altre informazioni sui problemi DLP
ms.author: pebaum
author: pebaum
manager: laurawi
ms.audience: admin
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2447"
- "3200001"
ms.openlocfilehash: 6525cee0555f1ae67b7d4e32445b9a1537d4a804
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932698"
---
# <a name="information-about-dlp-issues"></a><span data-ttu-id="0e464-102">Informazioni sui problemi DLP</span><span class="sxs-lookup"><span data-stu-id="0e464-102">Information about DLP issues</span></span>

<span data-ttu-id="0e464-103">**Importante**: molti clienti di SharePoint Online e OneDrive eseguono applicazioni aziendali critiche rispetto al servizio in esecuzione in background.</span><span class="sxs-lookup"><span data-stu-id="0e464-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="0e464-104">Tali applicazioni includono soluzioni per la migrazione del contenuto, di Prevenzione della perdita dei dati e per il backup.</span><span class="sxs-lookup"><span data-stu-id="0e464-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="0e464-105">In questi tempi straordinari, stiamo adottando misure per garantire che i servizi di SharePoint Online e OneDrive rimangano altamente disponibili e affidabili per gli utenti che dipendono ancor più dal servizio negli scenari di lavoro remoto.</span><span class="sxs-lookup"><span data-stu-id="0e464-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="0e464-106">A sostegno di questo obiettivo, abbiamo implementato limitazioni più rigide sulle app in background (migrazione, prevenzione della perdita dei dati e soluzioni di backup) durante il giorni nei giorni feriali.</span><span class="sxs-lookup"><span data-stu-id="0e464-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="0e464-107">In questo periodo sarà possibile notare una riduzione della velocità effettiva in queste app.</span><span class="sxs-lookup"><span data-stu-id="0e464-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="0e464-108">Tuttavia, nelle ore serali e durante il fine settimana nell'area il servizio sarà predisposto per elaborare una quantità notevolmente superiore di richieste delle app in background.</span><span class="sxs-lookup"><span data-stu-id="0e464-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="0e464-109">**Informazioni sui criteri DLP**</span><span class="sxs-lookup"><span data-stu-id="0e464-109">**Information on DLP policy**</span></span>

<span data-ttu-id="0e464-110">Con un criterio DLP, è possibile identificare, monitorare e proteggere automaticamente le informazioni riservate in Office 365.</span><span class="sxs-lookup"><span data-stu-id="0e464-110">With a DLP policy, you can identify, monitor, and automatically protect sensitive information across Office 365.</span></span>

<span data-ttu-id="0e464-111">Per ulteriori informazioni, visitare i collegamenti seguenti:</span><span class="sxs-lookup"><span data-stu-id="0e464-111">Please visit these links for more information:</span></span>

- [<span data-ttu-id="0e464-112">Panoramica della prevenzione della perdita dei dati</span><span class="sxs-lookup"><span data-stu-id="0e464-112">Overview of data loss prevention</span></span>](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies)
- [<span data-ttu-id="0e464-113">Cosa individuano le tipologie di informazioni sensibili</span><span class="sxs-lookup"><span data-stu-id="0e464-113">What the sensitive information types look for</span></span>](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
- [<span data-ttu-id="0e464-114">Creare una tipologia personalizzata di informazioni sensibili</span><span class="sxs-lookup"><span data-stu-id="0e464-114">Create a custom sensitive information type</span></span>](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type)
- [<span data-ttu-id="0e464-115">Inviare notifiche tramite posta elettronica e visualizzare suggerimenti per i criteri</span><span class="sxs-lookup"><span data-stu-id="0e464-115">Send email notifications and show policy tips</span></span>](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)
- [<span data-ttu-id="0e464-116">Proteggere i file di SharePoint Online con le etichette di conservazione e la prevenzione della perdita dei dati</span><span class="sxs-lookup"><span data-stu-id="0e464-116">Protect SharePoint Online files with retention labels and DLP</span></span>](https://docs.microsoft.com/office365/securitycompliance/protect-sharepoint-online-files-with-office-365-labels-and-dlp)
- [<span data-ttu-id="0e464-117">DLP e Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="0e464-117">DLP and Microsoft Teams</span></span>](https://docs.microsoft.com/office365/securitycompliance/dlp-microsoft-teams)

<span data-ttu-id="0e464-118">Per testare i dati con un tipo di informazioni riservate incorporato o personalizzato, utilizzare l' **opzione tipo di test** in **classificazione** > **tipi di informazioni riservate**.</span><span class="sxs-lookup"><span data-stu-id="0e464-118">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="0e464-119">Per ulteriori informazioni, vedere [testare i tipi di informazioni riservate personalizzate](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="0e464-119">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>