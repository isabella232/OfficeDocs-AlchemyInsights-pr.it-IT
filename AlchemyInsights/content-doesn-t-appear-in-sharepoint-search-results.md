---
title: Il contenuto non viene visualizzato nei risultati della ricerca di SharePoint
ms.author: tlarsen
author: tklarsen
ms.date: 1/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: ffb6bf349f9e8c2323186a8fc3183325d1d7e1bf
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36517035"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a><span data-ttu-id="70e41-102">Il contenuto non viene visualizzato nei risultati della ricerca di SharePoint</span><span class="sxs-lookup"><span data-stu-id="70e41-102">Content doesn't appear in SharePoint search results</span></span>

<span data-ttu-id="70e41-103">Seguire questi passaggi per la risoluzione dei problemi quando il contenuto previsto non viene visualizzato nei risultati della ricerca:</span><span class="sxs-lookup"><span data-stu-id="70e41-103">Follow these troubleshooting steps when expected content doesn't appear in search results:</span></span>
  
1. <span data-ttu-id="70e41-104">Verificare che il **sito** contenente il contenuto previsto sia impostato in modo che il contenuto venga visualizzato nei risultati della ricerca.</span><span class="sxs-lookup"><span data-stu-id="70e41-104">Check that the **site** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="70e41-105">Seguire la procedura illustrata in [Mostra contenuto di un sito nei risultati della ricerca](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="70e41-105">Follow the steps in [Show content on a site in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span></span>

2. <span data-ttu-id="70e41-106">Verificare che l' **elenco** o la **raccolta** che contiene il contenuto previsto sia impostata in modo che il contenuto venga visualizzato nei risultati della ricerca.</span><span class="sxs-lookup"><span data-stu-id="70e41-106">Check that the **list** or **library** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="70e41-107">Seguire la procedura illustrata in [Mostra contenuto da elenchi o raccolte nei risultati della ricerca](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="70e41-107">Follow the steps in [Show content from lists or libraries in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span></span>

3. <span data-ttu-id="70e41-108">Verificare che la pagina, il documento o il layout di pagina personalizzato sia pubblicato come **versione principale.**</span><span class="sxs-lookup"><span data-stu-id="70e41-108">Verify that the page, document, or custom page layout is published as a **Major version.**</span></span> <span data-ttu-id="70e41-109">Seguire il passaggio 3 nella [ricerca non restituisce tutti i risultati in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span><span class="sxs-lookup"><span data-stu-id="70e41-109">Follow step 3 in [Search doesn't return all results in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span></span>

4. <span data-ttu-id="70e41-110">Verificare che l'utente disponga **delle autorizzazioni** per visualizzare il contenuto.</span><span class="sxs-lookup"><span data-stu-id="70e41-110">Verify that the user has **permissions** to view the content.</span></span> <span data-ttu-id="70e41-111">Seguire la procedura illustrata in [informazioni sui livelli di autorizzazione in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="70e41-111">Follow the steps in [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
    
5. <span data-ttu-id="70e41-112">Se lo schema di ricerca è stato modificato aggiungendo una nuova proprietà gestita, modificando una proprietà gestita o rimuovendo una proprietà gestita, sarà necessario richiedere una ricerca per indicizzazione e reindicizzare.</span><span class="sxs-lookup"><span data-stu-id="70e41-112">If the search schema has been changed by adding a new managed property, by editing a managed property, or by removing a managed property then requesting a crawl and re-index will be required.</span></span> <span data-ttu-id="70e41-113">\*\*\*\* Reindicizzare il contenuto attenendosi alla procedura descritta in [eseguire manualmente la ricerca per indicizzazione e reindicizzazione di un sito, una raccolta o un elenco](https://docs.microsoft.com/sharepoint/crawl-site-content).</span><span class="sxs-lookup"><span data-stu-id="70e41-113">**Re-index** the content by following the steps in [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content).</span></span> <span data-ttu-id="70e41-114">Potrebbe essere necessario un po' di tempo, attendere 24 ore prima di controllare di nuovo i risultati.</span><span class="sxs-lookup"><span data-stu-id="70e41-114">This might take a while, wait 24 hours before checking the results again.</span></span>

<span data-ttu-id="70e41-115">Per ulteriori informazioni, vedere [abilitare il contenuto di un sito per la ricerca](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="70e41-115">For more information, see [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span> 
  
