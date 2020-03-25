---
title: Suggerimenti per i criteri DLP non funzionanti
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 51b4472fa721443192eb542cac45965df67634df
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932590"
---
# <a name="dlp-policy-tip-issues"></a><span data-ttu-id="5d353-102">Problemi relativi ai suggerimenti per i criteri DLP</span><span class="sxs-lookup"><span data-stu-id="5d353-102">DLP Policy Tip issues</span></span>

<span data-ttu-id="5d353-103">**Importante**: molti clienti di SharePoint Online e OneDrive eseguono applicazioni aziendali critiche rispetto al servizio in esecuzione in background.</span><span class="sxs-lookup"><span data-stu-id="5d353-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="5d353-104">Tali applicazioni includono soluzioni per la migrazione del contenuto, di Prevenzione della perdita dei dati e per il backup.</span><span class="sxs-lookup"><span data-stu-id="5d353-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="5d353-105">In questi tempi straordinari, stiamo adottando misure per garantire che i servizi di SharePoint Online e OneDrive rimangano altamente disponibili e affidabili per gli utenti che dipendono ancor più dal servizio negli scenari di lavoro remoto.</span><span class="sxs-lookup"><span data-stu-id="5d353-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="5d353-106">A sostegno di questo obiettivo, abbiamo implementato limitazioni più rigide sulle app in background (migrazione, prevenzione della perdita dei dati e soluzioni di backup) durante il giorni nei giorni feriali.</span><span class="sxs-lookup"><span data-stu-id="5d353-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="5d353-107">In questo periodo sarà possibile notare una riduzione della velocità effettiva in queste app.</span><span class="sxs-lookup"><span data-stu-id="5d353-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="5d353-108">Tuttavia, nelle ore serali e durante il fine settimana nell'area il servizio sarà predisposto per elaborare una quantità notevolmente superiore di richieste delle app in background.</span><span class="sxs-lookup"><span data-stu-id="5d353-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="5d353-109">**Suggerimenti per i criteri DLP**</span><span class="sxs-lookup"><span data-stu-id="5d353-109">**DLP policy tips**</span></span>

<span data-ttu-id="5d353-110">Quando si utilizzano i **criteri DLP**, gli utenti possono ricevere la notifica di una violazione dei criteri con suggerimenti per i **criteri**.</span><span class="sxs-lookup"><span data-stu-id="5d353-110">When using **DLP policies**, users can be notified of a policy violation with **policy tips**.</span></span> <span data-ttu-id="5d353-111">Gli amministratori possono configurare Suggerimenti per i criteri da visualizzare durante il testing del criterio DLP o quando il criterio è in modalità di applicazione completa.</span><span class="sxs-lookup"><span data-stu-id="5d353-111">Admins can configure policy tips to display while testing their DLP policy or when the policy is in full enforcement mode.</span></span>
  
<span data-ttu-id="5d353-112">Per configurare i suggerimenti per i criteri per i criteri DLP nel centro sicurezza e conformità in modalità di applicazione completa, eseguire le operazioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="5d353-112">To configure policy tips on your DLP policy in the Security and Compliance center in full enforcement mode, do the following:</span></span>
  
- <span data-ttu-id="5d353-113">Verificare che i suggerimenti per i criteri siano stati **abilitati** nella regola DLP utilizzando i passaggi riportati di [seguito](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span><span class="sxs-lookup"><span data-stu-id="5d353-113">Ensure policy tips have been **enabled** on the DLP rule using the steps [here](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span></span>

- <span data-ttu-id="5d353-114">Verificare che il **contenuto corrisponda** a ciò che è **necessario** per attivare la regola descritta in [questo articolo.](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="5d353-114">Ensure your **content matches** what is **required** to trigger the rule outlined in this article [here](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="5d353-115">I suggerimenti per i criteri vengono visualizzati sia in OWA che in Outlook.</span><span class="sxs-lookup"><span data-stu-id="5d353-115">Policy tips display in both OWA and Outlook.</span></span> <span data-ttu-id="5d353-116">Tuttavia, quando si utilizza **Outlook 2013 o versione successiva**, i suggerimenti per i criteri vengono visualizzati solo in determinate condizioni.</span><span class="sxs-lookup"><span data-stu-id="5d353-116">However, when using **Outlook 2013 or later**, policy tips are only displayed under certain conditions.</span></span> <span data-ttu-id="5d353-117">Queste condizioni sono elencate di seguito: [condizioni supportate per Outlook 2013 o versioni successive per la visualizzazione dei suggerimenti per i criteri](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span><span class="sxs-lookup"><span data-stu-id="5d353-117">These conditions are listed here: [Supported conditions for Outlook 2013 or later for displaying Policy Tips](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span></span>

<span data-ttu-id="5d353-118">Per ulteriori informazioni sui suggerimenti per i criteri DLP, vedere: [Mostra suggerimenti per i criteri per](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips) il criterio DLP</span><span class="sxs-lookup"><span data-stu-id="5d353-118">For additional information on DLP policy tips, see: [Show policy tips for DLP Policies](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span></span>
  