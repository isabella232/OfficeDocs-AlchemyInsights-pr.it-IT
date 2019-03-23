---
title: 1491-Search-not-returning-expected-results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 1491
ms.assetid: ''
ms.openlocfilehash: 517d9b75fc3aef09c0c2d5870aa695cc0ab10f06
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/22/2019
ms.locfileid: "30776086"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="37ab7-102">Ricerca di contenuto che non restituisce i risultati previsti</span><span class="sxs-lookup"><span data-stu-id="37ab7-102">Content Search not returning expected results</span></span>

<span data-ttu-id="37ab7-103">Quando si eseguono ricerche di contenuto dal centro conformità di Office 365 Security &, è possibile che vengano visualizzati risultati di ricerca imprevisti.</span><span class="sxs-lookup"><span data-stu-id="37ab7-103">When running Content Searches from the Office 365 Security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="37ab7-104">Si conSideri gli elementi seguenti che possono influire sui risultati della ricerca:</span><span class="sxs-lookup"><span data-stu-id="37ab7-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="37ab7-105">**Percorsi di contenuto e condizioni di ricerca**: verificare di aver selezionato le posizioni di contenuto e le condizioni di ricerca appropriate.</span><span class="sxs-lookup"><span data-stu-id="37ab7-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="37ab7-106">Se è stata eseguita una ricerca di grandi dimensioni (con molte posizioni), è consigliabile suddividerla in più ricerche.</span><span class="sxs-lookup"><span data-stu-id="37ab7-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="37ab7-107">**Elementi parzialmente indicizzati**: [gli elementi parzialmente indicizzati](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) delle cassette postali vengono inclusi nei risultati della ricerca stimati.</span><span class="sxs-lookup"><span data-stu-id="37ab7-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="37ab7-108">Tuttavia, gli elementi parzialmente indicizzati provenienti da siti di SharePoint e OneDrive non sono inclusi nella stima della ricerca.</span><span class="sxs-lookup"><span data-stu-id="37ab7-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="37ab7-109">Errori di ricerca: quando si esegue la ricerca di un numero elevato di cassette postali (oltre 100.000 cassette postali), è possibile che si verifichino **problemi**di ricerca, con codici di errore quali CS008-009 e CS012-002.</span><span class="sxs-lookup"><span data-stu-id="37ab7-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="37ab7-110">In questo caso, riprovare la ricerca solo per i percorsi di contenuto non riusciti.</span><span class="sxs-lookup"><span data-stu-id="37ab7-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="37ab7-111">Per ulteriori informazioni, vedere [questo articolo](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) .</span><span class="sxs-lookup"><span data-stu-id="37ab7-111">See  [this article](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for more information.</span></span>
