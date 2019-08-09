---
title: Scambiare il sito radice classico con un sito moderno
ms.author: efrene
author: efrene
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: 0f6f962314d9099bd21c281a23ad2e95742da4a8
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270748"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="cb992-102">Scambiare il sito radice classico con un sito moderno</span><span class="sxs-lookup"><span data-stu-id="cb992-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="cb992-103">Se l'ambiente è stato configurato prima di aprile 2019, è possibile modificare il sito radice in un sito moderno tramite Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="cb992-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="cb992-104">Se si dispone di un sito diverso che si desidera utilizzare come sito radice, è possibile sostituire (scambiare) il sito radice con esso.</span><span class="sxs-lookup"><span data-stu-id="cb992-104">If you have a different site that you want to use as your root site, you can replace (swap) the root site with it.</span></span> 
    - <span data-ttu-id="cb992-105">Utilizzare [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) per scambiare il percorso di un sito con un altro sito durante l'archiviazione del sito originale.</span><span class="sxs-lookup"><span data-stu-id="cb992-105">Use [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="cb992-106">Disponibile sia per il sito del team (non connesso a un gruppo) sia per il sito di comunicazione.</span><span class="sxs-lookup"><span data-stu-id="cb992-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="cb992-107">Le funzionalità aggiuntive verranno introdotte a breve che consentiranno di continuare a utilizzare il contenuto del sito, ma di convertire il sito esistente in un sito di comunicazione.</span><span class="sxs-lookup"><span data-stu-id="cb992-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="cb992-108">Queste funzionalità verranno Srotolate gradualmente.</span><span class="sxs-lookup"><span data-stu-id="cb992-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="cb992-109">Continuare a controllare il centro messaggi di Office 365 per gli aggiornamenti.</span><span class="sxs-lookup"><span data-stu-id="cb992-109">Continue to check the Office 365 Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="cb992-110">Problemi noti relativi ai siti di swapping</span><span class="sxs-lookup"><span data-stu-id="cb992-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="cb992-111">Il sito di destinazione potrebbe restituire un errore "not found" (HTTP 404) per un breve periodo di tempo.</span><span class="sxs-lookup"><span data-stu-id="cb992-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="cb992-112">Il contenuto dovrà essere sottoposto a ricerca per indicizzazione per aggiornare l'indice di ricerca.</span><span class="sxs-lookup"><span data-stu-id="cb992-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="cb992-113">Non è necessario un passaggio manuale: questo verrà effettuato automaticamente.</span><span class="sxs-lookup"><span data-stu-id="cb992-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="cb992-114">È necessario correggere manualmente qualsiasi elemento dipendente dai collegamenti "statici", ad esempio i file di sincronizzazione e di OneNote.</span><span class="sxs-lookup"><span data-stu-id="cb992-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="cb992-115">Se il sito di origine è un sito di notizie organizzative, aggiornare l'URL.</span><span class="sxs-lookup"><span data-stu-id="cb992-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="cb992-116">Ottenere un elenco di tutti i siti di notizie dell'organizzazione.</span><span class="sxs-lookup"><span data-stu-id="cb992-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="cb992-117">Potrebbe essere necessario convalidare i siti di Project Server per assicurarsi che siano ancora associati correttamente.</span><span class="sxs-lookup"><span data-stu-id="cb992-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>





