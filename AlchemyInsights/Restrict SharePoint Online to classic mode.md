---
title: Limitare la modalità classica di SharePoint Online
ms.author: kirks
author: Techwriter40
ms.date: 3/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.openlocfilehash: 6a7c0497243ef7425917f54815e61f1244838c54
ms.sourcegitcommit: b14aa00b42ce4ca9d7dc3aa1fd57e66eae115447
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/28/2019
ms.locfileid: "30953349"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="41133-102">Limitare la modalità classica di SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="41133-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="41133-103">Alcune organizzazioni richiedono ancora l'esperienza in modalità classica.</span><span class="sxs-lookup"><span data-stu-id="41133-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="41133-104">Anche se non si prevede di rimuovere la modalità classica a livello granulare, a partire dal 1 ° aprile 2019, non sarà più possibile limitare un'intera organizzazione (tenant) alla modalità classica per gli elenchi e le raccolte.</span><span class="sxs-lookup"><span data-stu-id="41133-104">While there are no plans to remove classic mode at a granular level, starting April 1,2019, it will no longer be possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="41133-105">L'amministratore avrà le seguenti opzioni per gestire singoli elenchi e raccolte in modalità classica utilizzando switch di opt-out granulare che vengono forniti ai livelli seguenti:</span><span class="sxs-lookup"><span data-stu-id="41133-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

<span data-ttu-id="41133-106">--raccolta siti--Site--List--Library</span><span class="sxs-lookup"><span data-stu-id="41133-106">-- site collection -- site -- list -- library</span></span>

<span data-ttu-id="41133-107">Inoltre, gli elenchi che utilizzano determinate caratteristiche e personalizzazioni non supportate dalla versione moderna continueranno a essere automaticamente passati alla modalità classica.</span><span class="sxs-lookup"><span data-stu-id="41133-107">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="41133-108">Dopo il 1 ° aprile, gli elenchi e le raccolte che si trovano in modalità classica a seguito dell'opt-out del tenant verranno gestiti automaticamente a livello di sito e di elenco.</span><span class="sxs-lookup"><span data-stu-id="41133-108">After April 1, lists and libraries that are in classic mode as a result of tenant opt-out will automatically be managed at the site level and list level.</span></span>

<span data-ttu-id="41133-109">Se si richiede la modalità classica, vedere altre informazioni qui e l'istruzione PnP PowerShell qui che descrive le opzioni e gli strumenti che è possibile utilizzare oggi per prepararsi per la rimozione dell'opt-out a livello di tenant il 1 ° aprile.</span><span class="sxs-lookup"><span data-stu-id="41133-109">If you require classic mode please see more information here and PnP Powershell instruction here that describes options and tools you can use today to prepare for the removal of the tenant level opt-out on April 1.</span></span>
