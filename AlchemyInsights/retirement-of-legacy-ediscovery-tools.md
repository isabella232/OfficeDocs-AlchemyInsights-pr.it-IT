---
title: Pensionamento degli strumenti di eDiscovery legacy
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 2315c4c651a83f0ecc78c0171f32aba13bc93f8c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727787"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="19955-102">Pensionamento degli strumenti di eDiscovery legacy</span><span class="sxs-lookup"><span data-stu-id="19955-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="19955-103">Come risultato della nuova e migliorata funzionalità di eDiscovery nel centro conformità di Microsoft 365, nei prossimi mesi verranno ritirati i seguenti strumenti di eDiscovery e commandlets legacy:</span><span class="sxs-lookup"><span data-stu-id="19955-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="19955-104">[EDiscovery sul posto](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) e [archiviazioni sul posto](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) nell'interfaccia di amministrazione di Exchange.</span><span class="sxs-lookup"><span data-stu-id="19955-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="19955-105">Cmdlet di Exchange Online PowerShell che supportano le archiviazioni sul posto di eDiscovery e sul posto.</span><span class="sxs-lookup"><span data-stu-id="19955-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="19955-106">Questi cmdlet sono identificati in modo collettivo come cmdlet \*-MailboxSearch. Sono inclusi i cmdlet seguenti:</span><span class="sxs-lookup"><span data-stu-id="19955-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="19955-107">New-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="19955-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="19955-108">Start-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="19955-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="19955-109">Stop-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="19955-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="19955-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="19955-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="19955-111">Il cmdlet [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) in Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="19955-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="19955-112">Le operazioni seguenti nell'API dei servizi Web di Exchange:</span><span class="sxs-lookup"><span data-stu-id="19955-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="19955-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="19955-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="19955-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="19955-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="19955-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="19955-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="19955-116">Advanced eDiscovery v 1.0</span><span class="sxs-lookup"><span data-stu-id="19955-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="19955-117">**Sequenza temporale per la pensione**:</span><span class="sxs-lookup"><span data-stu-id="19955-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="19955-118">**Luglio 1, 2020** Non è più possibile creare nuove ricerche e conservazioni, ma è possibile eseguire, modificare ed eliminare le ricerche esistenti a proprio rischio.</span><span class="sxs-lookup"><span data-stu-id="19955-118">**July 1, 2020** You can no longer create new searches and holds, but you can run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="19955-119">Il supporto Microsoft non supporta più eDiscovery sul posto & conserva nell'interfaccia di amministrazione di Exchange.</span><span class="sxs-lookup"><span data-stu-id="19955-119">Microsoft Support no longer supports In-Place eDiscovery & Holds in the EAC.</span></span>
    
- <span data-ttu-id="19955-120">**2020 ottobre 1** EDiscovery sul posto & contiene la funzionalità nell'interfaccia di amministrazione di Exchange verrà messa in modalità di sola lettura, in modo da poter rimuovere solo le ricerche e le esenzioni esistenti.</span><span class="sxs-lookup"><span data-stu-id="19955-120">**October 1, 2020** In-Place eDiscovery & Holds functionality in the EAC will be placed in read-only mode, so you can only remove existing searches and holds.</span></span>

<span data-ttu-id="19955-121">**Per ulteriori informazioni, vedere**:</span><span class="sxs-lookup"><span data-stu-id="19955-121">**For more information, see**:</span></span>

 - [<span data-ttu-id="19955-122">Eseguire la migrazione delle ricerche e delle esenzioni eDiscovery legacy al centro conformità di Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="19955-122">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="19955-123">Ritiro degli strumenti legacy di eDiscovery</span><span class="sxs-lookup"><span data-stu-id="19955-123">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="19955-124">Domande frequenti su eDiscovery sul posto e sulle archiviazioni sul posto</span><span class="sxs-lookup"><span data-stu-id="19955-124">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



