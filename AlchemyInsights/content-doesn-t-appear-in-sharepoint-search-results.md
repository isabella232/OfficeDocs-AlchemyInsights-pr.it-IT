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
ms.openlocfilehash: 8215b0a5cde5adffa3bec37d6699418557f914dd
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/28/2019
ms.locfileid: "35363814"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>Il contenuto non viene visualizzato nei risultati della ricerca di SharePoint

Seguire questi passaggi per la risoluzione dei problemi quando il contenuto previsto non viene visualizzato nei risultati della ricerca:
  
1. Verificare che il **sito** contenente il contenuto previsto sia impostato in modo che il contenuto venga visualizzato nei risultati della ricerca. Seguire la procedura illustrata in [Mostra contenuto di un sito nei risultati della ricerca](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).

2. Verificare che l' **elenco** o la **raccolta** che contiene il contenuto previsto sia impostata in modo che il contenuto venga visualizzato nei risultati della ricerca. Seguire la procedura illustrata in [Mostra contenuto da elenchi o raccolte nei risultati della ricerca](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).

3. Verificare che la pagina, il documento o il layout di pagina personalizzato sia pubblicato come **versione principale.** Seguire il passaggio 3 nella [ricerca non restituisce tutti i risultati in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).

4. Verificare che l'utente disponga **delle autorizzazioni** per visualizzare il contenuto. Seguire la procedura illustrata in [informazioni sui livelli di autorizzazione in SharePoint](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels).
    
5. Se lo schema di ricerca è stato modificato aggiungendo una nuova proprietà gestita, modificando una proprietà gestita o rimuovendo una proprietà gestita, sarà necessario richiedere una ricerca per indicizzazione e reindicizzare. **** Reindicizzare il contenuto attenendosi alla procedura descritta in [eseguire manualmente la ricerca per indicizzazione e reindicizzazione di un sito, una raccolta o un elenco](https://docs.microsoft.com/sharepoint/crawl-site-content). Potrebbe essere necessario un po' di tempo, attendere 24 ore prima di controllare di nuovo i risultati.

Per ulteriori informazioni, vedere [abilitare il contenuto di un sito per la ricerca](https://docs.microsoft.com/sharepoint/make-site-content-searchable). 
  
