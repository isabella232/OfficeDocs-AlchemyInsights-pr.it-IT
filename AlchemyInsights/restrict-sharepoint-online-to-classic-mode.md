---
title: Limitare la modalità classica di SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: c5ea5d264b62e4c349623bd431776207b38da470
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742473"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="42158-102">Limitare la modalità classica di SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="42158-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="42158-103">Alcune organizzazioni richiedono ancora l'esperienza in modalità classica.</span><span class="sxs-lookup"><span data-stu-id="42158-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="42158-104">Anche se non vi sono piani per rimuovere la modalità classica a un livello granulare, non è più possibile limitare un'intera organizzazione (tenant) alla modalità classica per gli elenchi e le raccolte.</span><span class="sxs-lookup"><span data-stu-id="42158-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="42158-105">L'amministratore avrà le seguenti opzioni per gestire singoli elenchi e raccolte in modalità classica utilizzando switch di opt-out granulare che vengono forniti ai livelli seguenti:</span><span class="sxs-lookup"><span data-stu-id="42158-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="42158-106">raccolta siti</span><span class="sxs-lookup"><span data-stu-id="42158-106">site collection</span></span>
- <span data-ttu-id="42158-107">sito</span><span class="sxs-lookup"><span data-stu-id="42158-107">site</span></span>
- <span data-ttu-id="42158-108">elenco</span><span class="sxs-lookup"><span data-stu-id="42158-108">list</span></span>
- <span data-ttu-id="42158-109">libreria</span><span class="sxs-lookup"><span data-stu-id="42158-109">library</span></span>

<span data-ttu-id="42158-110">Inoltre, gli elenchi che utilizzano determinate caratteristiche e personalizzazioni non supportate dalla versione moderna continueranno a essere automaticamente passati alla modalità classica.</span><span class="sxs-lookup"><span data-stu-id="42158-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="42158-111">A partire dal 1 ° aprile 2019, il processo di disabilitazione del livello tenant opt-out dell'elenco e delle raccolte moderne inizierà e continuerà fino al 31 maggio 2019.</span><span class="sxs-lookup"><span data-stu-id="42158-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="42158-112">Gli elenchi e le raccolte che si trovano in modalità classica a seguito dell'opt-out del tenant verranno automaticamente spostati in versione moderna.</span><span class="sxs-lookup"><span data-stu-id="42158-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="42158-113">Se si richiede la modalità classica, vedere [qui](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) altre informazioni e istruzioni di PowerShell PNP che descrivono le opzioni e gli [strumenti che è](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) possibile utilizzare oggi per utilizzare l'esperienza in modalità classica.</span><span class="sxs-lookup"><span data-stu-id="42158-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
