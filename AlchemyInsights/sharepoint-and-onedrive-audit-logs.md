---
title: Report del registro di controllo di SharePoint classico
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: be95034bea3c58a4fde96cfb0f9ba525e810758e
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/05/2019
ms.locfileid: "37992622"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="6afae-102">Registri di controllo di SharePoint e OneDrive</span><span class="sxs-lookup"><span data-stu-id="6afae-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="6afae-103">Registri di controllo di SharePoint Classic</span><span class="sxs-lookup"><span data-stu-id="6afae-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="6afae-104">Il controllo legacy di SPO è stato migrato nel log di controllo unificato (UAL).</span><span class="sxs-lookup"><span data-stu-id="6afae-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="6afae-105">Tutti i report di controllo legacy di SPO saranno ora alimentati tramite UAL e i segnali di controllo legacy sono stati migrati a UAL.</span><span class="sxs-lookup"><span data-stu-id="6afae-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="6afae-106">Modifiche principali:</span><span class="sxs-lookup"><span data-stu-id="6afae-106">Key changes:</span></span>

* <span data-ttu-id="6afae-107">Il ritaglio non è disponibile come funzionalità.</span><span class="sxs-lookup"><span data-stu-id="6afae-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="6afae-108">La scelta di eventi specifici da controllare non è disponibile.</span><span class="sxs-lookup"><span data-stu-id="6afae-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="6afae-109">Fare riferimento a [questo documento](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) per un elenco completo degli eventi controllati disponibili per impostazione predefinita.</span><span class="sxs-lookup"><span data-stu-id="6afae-109">Refer to [this document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="6afae-110">L'opzione **percorso** in **report personalizzati** non è disponibile.</span><span class="sxs-lookup"><span data-stu-id="6afae-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="6afae-111">L'opzione eventi di **apertura o download di documenti** non è disponibile.</span><span class="sxs-lookup"><span data-stu-id="6afae-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="6afae-112">Configurare le impostazioni di controllo per una raccolta siti</span><span class="sxs-lookup"><span data-stu-id="6afae-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="6afae-113">Registri di controllo unificato di SharePoint e OneDrive moderni dalla conformità</span><span class="sxs-lookup"><span data-stu-id="6afae-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="6afae-114">Attivazione/disattivazione della registrazione di controllo unificato</span><span class="sxs-lookup"><span data-stu-id="6afae-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="6afae-115">Non è necessaria alcuna configurazione aggiuntiva all'interno di SharePoint o OneDrive.</span><span class="sxs-lookup"><span data-stu-id="6afae-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="6afae-116">Utilizzare la ricerca della registrazione di controllo per controllare l'attività dei file, delle cartelle, degli utenti, delle autorizzazioni:</span><span class="sxs-lookup"><span data-stu-id="6afae-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="6afae-117">Attività di file e pagine</span><span class="sxs-lookup"><span data-stu-id="6afae-117">File and page activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="6afae-118">Attività cartella</span><span class="sxs-lookup"><span data-stu-id="6afae-118">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="6afae-119">Attività di condivisione e accesso alle richieste</span><span class="sxs-lookup"><span data-stu-id="6afae-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="6afae-120">Attività di sincronizzazione</span><span class="sxs-lookup"><span data-stu-id="6afae-120">Synchronization activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="6afae-121">Attività amministrative del sito</span><span class="sxs-lookup"><span data-stu-id="6afae-121">Site administration activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="6afae-122">Per ulteriori informazioni su come recuperare questi eventi, vedere [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="6afae-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
