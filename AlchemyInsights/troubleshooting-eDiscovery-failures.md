---
title: 1490-risoluzione dei problemi-eDiscovery-errori
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1490"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: ff28f96d64ec14980e9a47b630246b394faf4610
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277811"
---
# <a name="troubleshoot-content-search-errors"></a><span data-ttu-id="1a82b-102">Risoluzione degli errori di ricerca contenuto</span><span class="sxs-lookup"><span data-stu-id="1a82b-102">Troubleshoot Content Search errors</span></span>

<span data-ttu-id="1a82b-103">Si riscontrano problemi con la ricerca di contenuto o si verificano errori durante l'esportazione dei risultati della ricerca?</span><span class="sxs-lookup"><span data-stu-id="1a82b-103">Are you experiencing problems with Content Search or getting failures when you export search results?</span></span>

<span data-ttu-id="1a82b-104">Ad esempio, si ricevono le seguenti operazioni durante l'esecuzione di ricerche?</span><span class="sxs-lookup"><span data-stu-id="1a82b-104">For example, are you receiving the following when running searches?</span></span>

- <span data-ttu-id="1a82b-105">Errori di CS008 o CS012</span><span class="sxs-lookup"><span data-stu-id="1a82b-105">CS008 or CS012 errors</span></span>

- <span data-ttu-id="1a82b-106">Errori di occupato/timeout del server</span><span class="sxs-lookup"><span data-stu-id="1a82b-106">Server busy/timeout errors</span></span>

- <span data-ttu-id="1a82b-107">Si è verificato un errore dell'applicazione</span><span class="sxs-lookup"><span data-stu-id="1a82b-107">Application error occurred</span></span>

<span data-ttu-id="1a82b-108">Quando si esegue la ricerca o l'esportazione dei risultati di un numero elevato di cassette postali (oltre 100.000 cassette postali), si ottengono errori di esportazione?</span><span class="sxs-lookup"><span data-stu-id="1a82b-108">Or when searching or exporting results from a large number of mailboxes (over 100,000 mailboxes), are you getting export errors?</span></span>

<span data-ttu-id="1a82b-109">Per questi tipi di errori, riprovare la ricerca per i percorsi di contenuto che hanno avuto esito negativo.</span><span class="sxs-lookup"><span data-stu-id="1a82b-109">For these types of errors, retry the search for the content locations that have failed.</span></span> <span data-ttu-id="1a82b-110">Per ulteriori informazioni, vedere  [questo articolo](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) .</span><span class="sxs-lookup"><span data-stu-id="1a82b-110">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>

<span data-ttu-id="1a82b-111">Se si stanno esportando più di 100K cassette postali, è necessario utilizzare la seguente PowerShell per scaricare i risultati di esportazione:  [esportare i risultati da più di 100K cassette postali](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="1a82b-111">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>
