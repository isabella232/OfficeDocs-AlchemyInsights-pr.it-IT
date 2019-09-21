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
ms.openlocfilehash: af5b3c76b82db13bc89c917247e41fa1d8779b68
ms.sourcegitcommit: d5bf97a0bf0547f36b6da9684ce9f16a13a7749e
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/20/2019
ms.locfileid: "37068027"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="9da3a-102">Registri di controllo di SharePoint e OneDrive</span><span class="sxs-lookup"><span data-stu-id="9da3a-102">SharePoint and OneDrive audit logs</span></span>

<span data-ttu-id="9da3a-103">**Registri di controllo unificato di SharePoint e OneDrive moderni dalla conformità**</span><span class="sxs-lookup"><span data-stu-id="9da3a-103">**SharePoint and OneDrive Modern Unified Audit logs from compliance**</span></span>

- [<span data-ttu-id="9da3a-104">Attivazione/disattivazione della registrazione di controllo unificato</span><span class="sxs-lookup"><span data-stu-id="9da3a-104">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="9da3a-105">Non è necessaria alcuna configurazione aggiuntiva all'interno di SharePoint o OneDrive.</span><span class="sxs-lookup"><span data-stu-id="9da3a-105">No additional configuration is required within SharePoint or OneDrive.</span></span>

- <span data-ttu-id="9da3a-106">Utilizzare la ricerca della registrazione di controllo per controllare l'attività dei file, delle cartelle, degli utenti, delle autorizzazioni:</span><span class="sxs-lookup"><span data-stu-id="9da3a-106">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

    - [<span data-ttu-id="9da3a-107">Attività di file e pagine</span><span class="sxs-lookup"><span data-stu-id="9da3a-107">File and page activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
    - [<span data-ttu-id="9da3a-108">Attività cartella</span><span class="sxs-lookup"><span data-stu-id="9da3a-108">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    - [<span data-ttu-id="9da3a-109">Attività di condivisione e accesso alle richieste</span><span class="sxs-lookup"><span data-stu-id="9da3a-109">Sharing and access request activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
    - [<span data-ttu-id="9da3a-110">Attività di sincronizzazione</span><span class="sxs-lookup"><span data-stu-id="9da3a-110">Synchronization activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
    - [<span data-ttu-id="9da3a-111">Attività amministrative del sito</span><span class="sxs-lookup"><span data-stu-id="9da3a-111">Site administration activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)
- <span data-ttu-id="9da3a-112">Per ulteriori informazioni su come recuperare questi eventi, vedere [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="9da3a-112">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>

<span data-ttu-id="9da3a-113">**Registri di controllo di SharePoint Classic**</span><span class="sxs-lookup"><span data-stu-id="9da3a-113">**SharePoint classic Audit logs**</span></span>

<span data-ttu-id="9da3a-114">È stata eseguita la migrazione del controllo legacy di SPO al log di controllo unificato (UAL).</span><span class="sxs-lookup"><span data-stu-id="9da3a-114">We migrated SPO legacy auditing to Unified Audit Log (UAL).</span></span> <span data-ttu-id="9da3a-115">Questo significa in sostanza che tutti i report di controllo legacy di SPO saranno ora alimentati tramite UAL e i segnali di controllo legacy sono stati migrati a UAL.</span><span class="sxs-lookup"><span data-stu-id="9da3a-115">This essentially means that all SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="9da3a-116">Modifiche principali:</span><span class="sxs-lookup"><span data-stu-id="9da3a-116">Key changes:</span></span>

- <span data-ttu-id="9da3a-117">Il taglio come funzionalità non è disponibile.</span><span class="sxs-lookup"><span data-stu-id="9da3a-117">Trimming as a capability is NOT available.</span></span>
- <span data-ttu-id="9da3a-118">La sezione in cui si scelgono gli eventi specifici da controllare non è disponibile.</span><span class="sxs-lookup"><span data-stu-id="9da3a-118">The section where you choose specific events to audit is NOT available.</span></span> <span data-ttu-id="9da3a-119">Fare riferimento a [questo documento](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) per un elenco completo degli eventi controllati disponibili per impostazione predefinita.</span><span class="sxs-lookup"><span data-stu-id="9da3a-119">Please refer to [this document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
- <span data-ttu-id="9da3a-120">L'opzione "location" in **report personalizzati** non è disponibile.</span><span class="sxs-lookup"><span data-stu-id="9da3a-120">The "Location" option under **Customized reports** is NOT available.</span></span> 
- <span data-ttu-id="9da3a-121">Gli eventi "apertura o download di documenti" non sono disponibili.</span><span class="sxs-lookup"><span data-stu-id="9da3a-121">“Opening or downloading documents” events is NOT available.</span></span> 

