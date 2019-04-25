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
ms.openlocfilehash: c51e48fe5694f964aef74c2973f774b44415ebb8
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32422179"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="9fccd-102">Limitare la modalità classica di SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="9fccd-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="9fccd-103">Alcune organizzazioni richiedono ancora l'esperienza in modalità classica.</span><span class="sxs-lookup"><span data-stu-id="9fccd-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="9fccd-104">Anche se non si prevede di rimuovere la modalità classica a livello granulare, a partire dal 1 ° aprile 2019, non sarà più possibile limitare un'intera organizzazione (tenant) alla modalità classica per gli elenchi e le raccolte.</span><span class="sxs-lookup"><span data-stu-id="9fccd-104">While there are no plans to remove classic mode at a granular level, starting April 1,2019, it will no longer be possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="9fccd-105">L'amministratore avrà le seguenti opzioni per gestire singoli elenchi e raccolte in modalità classica utilizzando switch di opt-out granulare che vengono forniti ai livelli seguenti:</span><span class="sxs-lookup"><span data-stu-id="9fccd-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="9fccd-106">raccolta siti</span><span class="sxs-lookup"><span data-stu-id="9fccd-106">site collection</span></span>
- <span data-ttu-id="9fccd-107">sito</span><span class="sxs-lookup"><span data-stu-id="9fccd-107">site</span></span>
- <span data-ttu-id="9fccd-108">elenco</span><span class="sxs-lookup"><span data-stu-id="9fccd-108">list</span></span>
- <span data-ttu-id="9fccd-109">libreria</span><span class="sxs-lookup"><span data-stu-id="9fccd-109">library</span></span>

<span data-ttu-id="9fccd-110">Inoltre, gli elenchi che utilizzano determinate caratteristiche e personalizzazioni non supportate dalla versione moderna continueranno a essere automaticamente passati alla modalità classica.</span><span class="sxs-lookup"><span data-stu-id="9fccd-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="9fccd-111">Dopo il 1 ° aprile, gli elenchi e le raccolte che si trovano in modalità classica a seguito dell'opt-out del tenant verranno gestiti automaticamente a livello di sito e di elenco.</span><span class="sxs-lookup"><span data-stu-id="9fccd-111">After April 1, lists and libraries that are in classic mode as a result of tenant opt-out will automatically be managed at the site level and list level.</span></span>

<span data-ttu-id="9fccd-112">Se si richiede la modalità classica, vedere altre informazioni qui e l'istruzione PnP PowerShell qui che descrive le opzioni e gli strumenti che è possibile utilizzare oggi per prepararsi per la rimozione dell'opt-out a livello di tenant il 1 ° aprile.</span><span class="sxs-lookup"><span data-stu-id="9fccd-112">If you require classic mode please see more information here and PnP Powershell instruction here that describes options and tools you can use today to prepare for the removal of the tenant level opt-out on April 1.</span></span>
