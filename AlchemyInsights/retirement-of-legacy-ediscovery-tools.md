---
title: Pensionamento degli strumenti di eDiscovery legacy
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: af9a0bd8ff4294575ac68f37d4997bb50b132ce7
ms.sourcegitcommit: 9ab422063e5a474c92ed956d42d222b90336fecb
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/11/2020
ms.locfileid: "42600377"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="c16b1-102">Pensionamento degli strumenti di eDiscovery legacy</span><span class="sxs-lookup"><span data-stu-id="c16b1-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="c16b1-103">Come risultato della nuova e migliorata funzionalità di eDiscovery nel centro conformità di Microsoft 365, nei prossimi mesi verranno ritirati i seguenti strumenti di eDiscovery e commandlets legacy:</span><span class="sxs-lookup"><span data-stu-id="c16b1-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="c16b1-104">[EDiscovery sul posto](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) e [archiviazioni sul posto](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) nell'interfaccia di amministrazione di Exchange.</span><span class="sxs-lookup"><span data-stu-id="c16b1-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="c16b1-105">Cmdlet di Exchange Online PowerShell che supportano le archiviazioni sul posto di eDiscovery e sul posto.</span><span class="sxs-lookup"><span data-stu-id="c16b1-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="c16b1-106">Questi cmdlet sono identificati in modo collettivo come cmdlet \*-MailboxSearch. Sono inclusi i cmdlet seguenti:</span><span class="sxs-lookup"><span data-stu-id="c16b1-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="c16b1-107">New-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="c16b1-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="c16b1-108">Start-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="c16b1-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="c16b1-109">Stop-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="c16b1-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="c16b1-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="c16b1-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="c16b1-111">Il cmdlet [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) in Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="c16b1-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="c16b1-112">Le operazioni seguenti nell'API dei servizi Web di Exchange:</span><span class="sxs-lookup"><span data-stu-id="c16b1-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="c16b1-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="c16b1-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="c16b1-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="c16b1-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="c16b1-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="c16b1-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="c16b1-116">Office 365 Advanced eDiscovery v 1.0</span><span class="sxs-lookup"><span data-stu-id="c16b1-116">Office 365 Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="c16b1-117">**Sequenza temporale per la pensione**:</span><span class="sxs-lookup"><span data-stu-id="c16b1-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="c16b1-118">2020 aprile 1: non sarà possibile creare nuove ricerche e conservazioni, ma è comunque possibile eseguire, modificare ed eliminare le ricerche esistenti a proprio rischio.</span><span class="sxs-lookup"><span data-stu-id="c16b1-118">April 1, 2020: You won't be able to create new searches and holds, but you can still run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="c16b1-119">Il supporto tecnico Microsoft non supporterà più il eDiscovery sul posto & conserva nell'interfaccia di amministrazione di Exchange.</span><span class="sxs-lookup"><span data-stu-id="c16b1-119">Microsoft Support will no longer support In-Place eDiscovery & Holds in the EAC.</span></span>

- <span data-ttu-id="c16b1-120">2020 luglio 1: la eDiscovery sul posto & contiene la funzionalità nell'interfaccia di amministrazione di Exchange verrà messa in modalità di sola lettura.</span><span class="sxs-lookup"><span data-stu-id="c16b1-120">July 1, 2020: The In-Place eDiscovery & Holds functionality in the EAC will be placed in a read-only mode.</span></span> <span data-ttu-id="c16b1-121">Questo significa che sarà possibile rimuovere solo le ricerche e le esenzioni esistenti.</span><span class="sxs-lookup"><span data-stu-id="c16b1-121">This means you'll only be able to remove existing searches and holds.</span></span>

<span data-ttu-id="c16b1-122">**Per ulteriori informazioni, vedere**:</span><span class="sxs-lookup"><span data-stu-id="c16b1-122">**For more information, see**:</span></span>

 - [<span data-ttu-id="c16b1-123">Eseguire la migrazione delle ricerche e delle esenzioni eDiscovery legacy al centro conformità di Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="c16b1-123">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="c16b1-124">Pensionamento degli strumenti di eDiscovery legacy</span><span class="sxs-lookup"><span data-stu-id="c16b1-124">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="c16b1-125">Domande frequenti su eDiscovery sul posto e sulle archiviazioni sul posto</span><span class="sxs-lookup"><span data-stu-id="c16b1-125">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



