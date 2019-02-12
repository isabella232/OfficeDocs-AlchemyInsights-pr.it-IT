---
title: Contenuto non viene visualizzata nei risultati della ricerca di SharePoint
ms.author: tlarsen
author: tklarsen
ms.date: 1/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: de607b75f973322359888c300ba1849e117d0092
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 02/12/2019
ms.locfileid: "29900436"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>Contenuto non viene visualizzata nei risultati della ricerca di SharePoint

Eseguire passaggi di risoluzione dei problemi quando non viene visualizzato il contenuto previsto nei risultati della ricerca:
  
1. Verificare che il **sito** che contiene il contenuto previsto è impostata su Consenti contenuto venga visualizzato nei risultati della ricerca. Seguire i passaggi descritti in [Mostra il contenuto in un sito nei risultati della ricerca](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).
    
2. Verificare che **l'elenco** o **raccolta** che contiene il contenuto previsto sia impostata su Consenti contenuto venga visualizzato nei risultati della ricerca. Seguire i passaggi descritti in [Mostra il contenuto di elenchi o raccolte nei risultati della ricerca](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results). 
    
3. Verificare che la pagina, un documento o un layout di pagina personalizzato deve essere pubblicato come un **versione principale.** Eseguire passaggio 3 della [ricerca non restituisce tutti i risultati in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).
    
4. Verificare che l'utente disponga **delle autorizzazioni** per visualizzare il contenuto. Seguire i passaggi descritti in [livelli di autorizzazione Understanding in SharePoint](https://go.microsoft.com/fwlink/?linkid=867071).
    
5. **Reindicizzare** il contenuto eseguendo la procedura descritta in [richieste manualmente la ricerca per indicizzazione e la reindicizzazione di un sito, un elenco o una raccolta](https://docs.microsoft.com/sharepoint/crawl-site-content). Ciò potrebbe richiedere alcuni minuti, attendere 24 ore prima di controllare nuovamente i risultati.
    
Per ulteriori informazioni, vedere [abilitare il contenuto in un sito per le ricerche](https://docs.microsoft.com/sharepoint/make-site-content-searchable). 
  

