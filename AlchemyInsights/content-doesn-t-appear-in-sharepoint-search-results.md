---
title: Il contenuto non viene visualizzato nei risultati SharePoint ricerca
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: ca03c31def64e43935d734a17735b10373e5ca85b5f4ea0f0e886b9ea39884cd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54081614"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>Il contenuto non viene visualizzato nei risultati SharePoint ricerca

Seguire questi passaggi per la risoluzione dei problemi quando il contenuto previsto non viene visualizzato nei risultati della ricerca:
  
1. Verificare che il **sito contenente** il contenuto previsto sia impostato per consentire la visualizzazione del contenuto nei risultati della ricerca. Seguire i passaggi descritti in [Show content on a site in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).

2. Verificare che **l'elenco** o **la raccolta** contenente il contenuto previsto sia impostato per consentire la visualizzazione del contenuto nei risultati della ricerca. Seguire i passaggi descritti in [Show content from lists or libraries in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).

3. Verificare che la pagina, il documento o il layout di pagina personalizzato sia pubblicato come **versione principale.** Seguire il passaggio 3 in [Search doesn't return all results in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).

4. Verificare che l'utente abbia **le autorizzazioni** per visualizzare il contenuto. Seguire i passaggi descritti in [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
    
5. Se lo schema di ricerca è stato modificato aggiungendo una nuova proprietà gestita, modificando una proprietà gestita o rimuovendo una proprietà gestita, sarà necessario richiedere una ricerca per indicizzazione e un nuovo indice. **Indicizzare nuovamente il** contenuto seguendo la procedura descritta in Richiedere manualmente la ricerca per indicizzazione e la nuova indicizzazione di un sito, una [raccolta o un elenco.](https://docs.microsoft.com/sharepoint/crawl-site-content) Potrebbe essere necessario attendere 24 ore prima di controllare di nuovo i risultati.

Per ulteriori informazioni, vedere [Enable content on a site to be searchable.](https://docs.microsoft.com/sharepoint/make-site-content-searchable) 
  
