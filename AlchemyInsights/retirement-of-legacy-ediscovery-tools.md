---
title: Ritiro degli strumenti legacy di eDiscovery
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 986c78f20e7b8c303c302913d63d817a56ce2896
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51798553"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="4d699-102">Ritiro degli strumenti legacy di eDiscovery</span><span class="sxs-lookup"><span data-stu-id="4d699-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="4d699-103">Come risultato della nuova e migliorata funzionalità di eDiscovery nel Centro conformità Microsoft 365, i seguenti strumenti e commandlet legacy di eDiscovery verranno ritirati nei prossimi mesi:</span><span class="sxs-lookup"><span data-stu-id="4d699-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="4d699-104">[EDiscovery sul posto](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) e [blocchi sul posto](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) nell'interfaccia di amministrazione di Exchange.</span><span class="sxs-lookup"><span data-stu-id="4d699-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="4d699-105">I cmdlet di PowerShell di Exchange Online che supportano In-Place eDiscovery e In-Place blocchi.</span><span class="sxs-lookup"><span data-stu-id="4d699-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="4d699-106">Questi cmdlet sono identificati collettivamente come cmdlet \*-MailboxSearch. Sono inclusi i cmdlet seguenti:</span><span class="sxs-lookup"><span data-stu-id="4d699-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="4d699-107">New-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="4d699-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="4d699-108">Start-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="4d699-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="4d699-109">Stop-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="4d699-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="4d699-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="4d699-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="4d699-111">Il cmdlet [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) in PowerShell di Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="4d699-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="4d699-112">Nell'API dei servizi Web Exchange vengono eseguite le operazioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="4d699-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="4d699-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="4d699-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="4d699-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="4d699-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="4d699-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="4d699-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="4d699-116">Advanced eDiscovery v1.0</span><span class="sxs-lookup"><span data-stu-id="4d699-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="4d699-117">**Sequenza temporale per il ritiro**:</span><span class="sxs-lookup"><span data-stu-id="4d699-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="4d699-118">**1 luglio 2020** Non è più possibile creare nuove ricerche e blocchi, ma è possibile eseguire, modificare ed eliminare le ricerche esistenti a proprio rischio.</span><span class="sxs-lookup"><span data-stu-id="4d699-118">**July 1, 2020** You can no longer create new searches and holds, but you can run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="4d699-119">Il supporto Microsoft non supporta più In-Place eDiscovery & blocchi nell'interfaccia di amministrazione di Exchange.</span><span class="sxs-lookup"><span data-stu-id="4d699-119">Microsoft Support no longer supports In-Place eDiscovery & Holds in the EAC.</span></span>
    
- <span data-ttu-id="4d699-120">**1 ottobre 2020** In-Place funzionalità di eDiscovery & I blocchi nell'interfaccia di amministrazione di Exchange verranno posizionati in modalità di sola lettura, pertanto è possibile rimuovere solo le ricerche e i blocchi esistenti.</span><span class="sxs-lookup"><span data-stu-id="4d699-120">**October 1, 2020** In-Place eDiscovery & Holds functionality in the EAC will be placed in read-only mode, so you can only remove existing searches and holds.</span></span>

<span data-ttu-id="4d699-121">**Per ulteriori informazioni, vedere**:</span><span class="sxs-lookup"><span data-stu-id="4d699-121">**For more information, see**:</span></span>

 - [<span data-ttu-id="4d699-122">Eseguire la migrazione delle ricerche e dei blocchi legacy di eDiscovery nel Centro conformità Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="4d699-122">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="4d699-123">Ritiro degli strumenti legacy di eDiscovery</span><span class="sxs-lookup"><span data-stu-id="4d699-123">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="4d699-124">Domande frequenti su In-Place eDiscovery e In-Place blocchi</span><span class="sxs-lookup"><span data-stu-id="4d699-124">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



