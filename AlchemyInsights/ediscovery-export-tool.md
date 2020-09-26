---
title: Strumento di esportazione di eDiscovery
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
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: 67e59182a5053111a08f5fb2be814931a1aa815d
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277943"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a><span data-ttu-id="2a6a8-102">Non è possibile installare o eseguire lo strumento di esportazione di eDiscovery?</span><span class="sxs-lookup"><span data-stu-id="2a6a8-102">Can't install or run the eDiscovery Export Tool?</span></span>

<span data-ttu-id="2a6a8-103">Se non è possibile installare o eseguire lo strumento di esportazione di eDiscovery per scaricare i risultati della ricerca, verificare le seguenti operazioni:</span><span class="sxs-lookup"><span data-stu-id="2a6a8-103">If you can't install or run the eDiscovery Export Tool to download search results, check the following things:</span></span>
  
- <span data-ttu-id="2a6a8-104">Il computer che si sta utilizzando soddisfa questi prerequisiti:</span><span class="sxs-lookup"><span data-stu-id="2a6a8-104">The computer you're using meets these pre-requisites:</span></span>

  - <span data-ttu-id="2a6a8-105">Windows 7 a 32 o 64 bit e versioni successive</span><span class="sxs-lookup"><span data-stu-id="2a6a8-105">32- or 64-bit versions of Windows 7 and later versions</span></span>

  - <span data-ttu-id="2a6a8-106">Microsoft .NET Framework 4.7</span><span class="sxs-lookup"><span data-stu-id="2a6a8-106">Microsoft .NET Framework 4.7</span></span>

  - <span data-ttu-id="2a6a8-107">Browser supportato:</span><span class="sxs-lookup"><span data-stu-id="2a6a8-107">A supported browser:</span></span>

  - <span data-ttu-id="2a6a8-108">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="2a6a8-108">Microsoft Edge</span></span>

    <span data-ttu-id="2a6a8-109">Oppure</span><span class="sxs-lookup"><span data-stu-id="2a6a8-109">Or</span></span>

  - <span data-ttu-id="2a6a8-110">Internet Explorer 10 e versioni successive</span><span class="sxs-lookup"><span data-stu-id="2a6a8-110">Internet Explorer 10 and later versions</span></span>

    <span data-ttu-id="2a6a8-111">Altri browser, come Google Chrome e Mozilla Firefox, non sono supportati.</span><span class="sxs-lookup"><span data-stu-id="2a6a8-111">Other browsers, such as Google Chrome and Mozilla Firefox aren't supported.</span></span>

- <span data-ttu-id="2a6a8-112">L'organizzazione può connettersi all'endpoint in Azure, che è \*\* \* . blob.Core.Windows.NET\*\* (il carattere jolly rappresenta un identificatore univoco per il processo di esportazione).</span><span class="sxs-lookup"><span data-stu-id="2a6a8-112">Your organization can connect to the endpoint in Azure, which is **\*.blob.core.windows.net** (the wildcard represents a unique identifier for your export job).</span></span>

- <span data-ttu-id="2a6a8-113">Al centro sicurezza e conformità di Microsoft 365 è assegnato il ruolo Export &amp; .</span><span class="sxs-lookup"><span data-stu-id="2a6a8-113">You're assigned the Export role in the Microsoft 365 Security &amp; Compliance Center.</span></span> <span data-ttu-id="2a6a8-114">Per impostazione predefinita, questo ruolo viene assegnato solo al gruppo di ruoli eDiscovery Manager.</span><span class="sxs-lookup"><span data-stu-id="2a6a8-114">By default, this role is only assigned to the eDiscovery Manager role group.</span></span> <span data-ttu-id="2a6a8-115">Vedere [assegnare le autorizzazioni di eDiscovery](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span><span class="sxs-lookup"><span data-stu-id="2a6a8-115">See [Assign eDiscovery permissions](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span></span>

<span data-ttu-id="2a6a8-116">Per ulteriori informazioni, vedere [Export content search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span><span class="sxs-lookup"><span data-stu-id="2a6a8-116">For more information, see [Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>

<span data-ttu-id="2a6a8-117">Se si stanno esportando più di 100K cassette postali, è necessario utilizzare la seguente PowerShell per scaricare i risultati di esportazione:  [esportare i risultati da più di 100K cassette postali](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="2a6a8-117">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>