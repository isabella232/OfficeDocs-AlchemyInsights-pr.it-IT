---
title: Report del registro di controllo di SharePoint classico
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: daf79f8d75ccdff8ad54f0f307648a5832a6bb71
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662212"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="adc8a-102">Registri di controllo di SharePoint e OneDrive</span><span class="sxs-lookup"><span data-stu-id="adc8a-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="adc8a-103">Registri di controllo di SharePoint Classic</span><span class="sxs-lookup"><span data-stu-id="adc8a-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="adc8a-104">Il controllo legacy di SPO è stato migrato nel log di controllo unificato (UAL).</span><span class="sxs-lookup"><span data-stu-id="adc8a-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="adc8a-105">Tutti i report di controllo legacy di SPO saranno ora alimentati tramite UAL e i segnali di controllo legacy sono stati migrati a UAL.</span><span class="sxs-lookup"><span data-stu-id="adc8a-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="adc8a-106">Modifiche principali:</span><span class="sxs-lookup"><span data-stu-id="adc8a-106">Key changes:</span></span>

* <span data-ttu-id="adc8a-107">Il ritaglio non è disponibile come funzionalità.</span><span class="sxs-lookup"><span data-stu-id="adc8a-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="adc8a-108">La scelta di eventi specifici da controllare non è disponibile.</span><span class="sxs-lookup"><span data-stu-id="adc8a-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="adc8a-109">Fare riferimento a [questo documento](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) per un elenco completo degli eventi controllati disponibili per impostazione predefinita.</span><span class="sxs-lookup"><span data-stu-id="adc8a-109">Refer to [this document](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="adc8a-110">L'opzione **percorso** in **report personalizzati** non è disponibile.</span><span class="sxs-lookup"><span data-stu-id="adc8a-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="adc8a-111">L'opzione eventi di **apertura o download di documenti** non è disponibile.</span><span class="sxs-lookup"><span data-stu-id="adc8a-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="adc8a-112">Configurare le impostazioni di controllo per una raccolta siti</span><span class="sxs-lookup"><span data-stu-id="adc8a-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="adc8a-113">Registri di controllo unificato di SharePoint e OneDrive moderni dalla conformità</span><span class="sxs-lookup"><span data-stu-id="adc8a-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="adc8a-114">Attivazione/disattivazione della registrazione di controllo unificato</span><span class="sxs-lookup"><span data-stu-id="adc8a-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="adc8a-115">Non è necessaria alcuna configurazione aggiuntiva all'interno di SharePoint o OneDrive.</span><span class="sxs-lookup"><span data-stu-id="adc8a-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="adc8a-116">Utilizzare la ricerca della registrazione di controllo per controllare l'attività dei file, delle cartelle, degli utenti, delle autorizzazioni:</span><span class="sxs-lookup"><span data-stu-id="adc8a-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="adc8a-117">Attività su file e pagine</span><span class="sxs-lookup"><span data-stu-id="adc8a-117">File and page activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="adc8a-118">Attività su cartelle</span><span class="sxs-lookup"><span data-stu-id="adc8a-118">Folder activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="adc8a-119">Attività di richiesta di accesso e condivisione</span><span class="sxs-lookup"><span data-stu-id="adc8a-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="adc8a-120">Attività di sincronizzazione</span><span class="sxs-lookup"><span data-stu-id="adc8a-120">Synchronization activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="adc8a-121">Attività di amministrazione siti</span><span class="sxs-lookup"><span data-stu-id="adc8a-121">Site administration activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="adc8a-122">Per ulteriori informazioni su come recuperare questi eventi, vedere [Search the audit log](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="adc8a-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
