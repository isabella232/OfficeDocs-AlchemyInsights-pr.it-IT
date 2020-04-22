---
title: Sito moderno come sito radice
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 0388f95e2b7815dcbbb6aca200f44e55e9c5724f
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713795"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="0780f-102">Sito moderno come sito radice</span><span class="sxs-lookup"><span data-stu-id="0780f-102">Modern site as root site</span></span>

<span data-ttu-id="0780f-103">È stata avviata l'implementazione di una nuova funzionalità che consente di [scambiare il sito radice del sito classico con un sito moderno](https://docs.microsoft.com/sharepoint/modern-root-site).</span><span class="sxs-lookup"><span data-stu-id="0780f-103">We have begun to rollout a new feature that will allow you to [swap your classic site root site with a modern site](https://docs.microsoft.com/sharepoint/modern-root-site).</span></span> <span data-ttu-id="0780f-104">Utilizzare [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) per scambiare il percorso di un sito con un altro sito durante l'archiviazione del sito originale.</span><span class="sxs-lookup"><span data-stu-id="0780f-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="0780f-105">Disponibile sia per il sito del team (non connesso a un gruppo) sia per il sito di comunicazione.</span><span class="sxs-lookup"><span data-stu-id="0780f-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span>

>[!Important]
> <span data-ttu-id="0780f-106">Non eliminare il sito radice classico per creare un sito di comunicazione moderno.</span><span class="sxs-lookup"><span data-stu-id="0780f-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="0780f-107">Questo non è supportato da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="0780f-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="0780f-108">L'eliminazione del sito radice renderà tutti i siti di SharePoint dell'organizzazione inaccessibili a tutti gli utenti, fino a quando non si ripristina il sito o si crea un nuovo sito nello stesso URL.</span><span class="sxs-lookup"><span data-stu-id="0780f-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="0780f-109">Questa funzionalità verrà comunicata tramite il centro messaggi.</span><span class="sxs-lookup"><span data-stu-id="0780f-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="0780f-110">È consigliabile che la caratteristica venga attivata brevemente nel tenant.</span><span class="sxs-lookup"><span data-stu-id="0780f-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="0780f-111">Problemi noti relativi ai siti di swapping</span><span class="sxs-lookup"><span data-stu-id="0780f-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="0780f-112">Il sito di destinazione potrebbe restituire un errore "not found" (HTTP 404) per un breve periodo di tempo.</span><span class="sxs-lookup"><span data-stu-id="0780f-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="0780f-113">Il contenuto dovrà essere sottoposto a ricerca per indicizzazione per aggiornare l'indice di ricerca.</span><span class="sxs-lookup"><span data-stu-id="0780f-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="0780f-114">Non è necessario eseguire un passaggio manuale in questa fase, verrà eseguita automaticamente.</span><span class="sxs-lookup"><span data-stu-id="0780f-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="0780f-115">È necessario correggere manualmente qualsiasi elemento dipendente dai collegamenti "statici", ad esempio i file di sincronizzazione e di OneNote.</span><span class="sxs-lookup"><span data-stu-id="0780f-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="0780f-116">Potrebbe essere necessario convalidare i siti di Project Server per assicurarsi che siano ancora associati correttamente.</span><span class="sxs-lookup"><span data-stu-id="0780f-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
