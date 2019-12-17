---
title: Gestire lo schema di ricerca in SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 9836cf139e97fc556995a8f0ad38c51c5c2392ac
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40042967"
---
# <a name="manage-search-schema-in-sharepoint-online"></a><span data-ttu-id="d3b79-102">Gestire lo schema di ricerca in SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="d3b79-102">Manage search schema in SharePoint Online</span></span>

<span data-ttu-id="d3b79-103">Lo schema di ricerca controlla gli elementi che gli utenti possono cercare, il modo in cui gli utenti possono cercarli e come è possibile presentare i risultati nei siti Web di ricerca.</span><span class="sxs-lookup"><span data-stu-id="d3b79-103">The search schema controls what users can search for, how users can search it, and how you can present the results on your search websites.</span></span> 

<span data-ttu-id="d3b79-104">Vedere [gestire lo schema di ricerca in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) per informazioni su come eseguire le operazioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="d3b79-104">See [Manage the Search Schema in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) to learn how to:</span></span> 
- <span data-ttu-id="d3b79-105">Modificare lo schema di ricerca.</span><span class="sxs-lookup"><span data-stu-id="d3b79-105">Change the search schema.</span></span>
- <span data-ttu-id="d3b79-106">Creare proprietà gestite.</span><span class="sxs-lookup"><span data-stu-id="d3b79-106">Create managed properties.</span></span>
- <span data-ttu-id="d3b79-107">Mapping delle proprietà sottoposte a ricerca per indicizzazione map alle proprietà gestite.</span><span class="sxs-lookup"><span data-stu-id="d3b79-107">Map crawled map crawled properties to managed properties.</span></span>

<span data-ttu-id="d3b79-108">Tenere presente quanto segue per quanto riguarda la gestione dello schema di ricerca:</span><span class="sxs-lookup"><span data-stu-id="d3b79-108">Note the following in regards to managing your Search Schema:</span></span>

- <span data-ttu-id="d3b79-109">Se viene visualizzato un messaggio di avviso indicante che **l'applicazione è stata sospesa** quando si effettua una modifica dello schema, questa è solo temporanea perché si verifica la manutenzione del servizio.</span><span class="sxs-lookup"><span data-stu-id="d3b79-109">If you receive a warning stating **the application is paused** when making a schema change, this is only temporary as there is service maintenance occurring.</span></span> 

    <span data-ttu-id="d3b79-110">Se sono passate più di 24 ore e si verifica ancora l'avviso, registrare un caso di supporto.</span><span class="sxs-lookup"><span data-stu-id="d3b79-110">If more than 24 hours have passed and you still experience the warning, please log a support case.</span></span>
- <span data-ttu-id="d3b79-111">Quando si modificano le proprietà gestite o si aggiungono nuove, le modifiche diventano effettive solo dopo che il contenuto è stato nuovamente sottoposto a ricerca per indicizzazione.</span><span class="sxs-lookup"><span data-stu-id="d3b79-111">When you change managed properties or add new ones, the changes take effect only after the content has been re-crawled.</span></span> <span data-ttu-id="d3b79-112">In SharePoint Online, la ricerca per indicizzazione avviene automaticamente in base alla pianificazione della ricerca per indicizzazione definita</span><span class="sxs-lookup"><span data-stu-id="d3b79-112">In SharePoint Online, crawling happens automatically based on the defined crawl schedule.</span></span>
- <span data-ttu-id="d3b79-113">Per assicurarsi che le modifiche vengano sottoposte a ricerca per indicizzazione, è possibile [richiedere una nuova indicizzazione dell'elenco o della raccolta](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list) .</span><span class="sxs-lookup"><span data-stu-id="d3b79-113">To make sure that your changes are crawled, you can specifically [request a re-indexing of the list or library](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span></span> 

<span data-ttu-id="d3b79-114">Per una panoramica completa dello schema di ricerca, vedere [Introducing Search schema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span><span class="sxs-lookup"><span data-stu-id="d3b79-114">For a complete overview of the Search Schema, see [Introducing Search Schema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span></span> 


