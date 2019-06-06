---
title: Gestire i dizionari di ricerca in SharePoint Online
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: c2960093bb1cfb649c26528c9f671e6d720ff237
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/05/2019
ms.locfileid: "34736057"
---
# <a name="search-in-sharepoint-online"></a>Ricerca in SharePoint Online

Il contenuto deve essere sottoposto a ricerca per indicizzazione e aggiunto all'indice di ricerca per consentire agli utenti di trovare ciò che stanno cercando in SharePoint Online. Il contenuto viene sottoposto a ricerca per indicizzazione in base a una pianificazione di ricerca per indicizzazione predefinita (la pianificazione della ricerca per indicizzazione Il crawler recupera il contenuto modificato dall'ultima ricerca per indicizzazione e aggiorna l'indice. Per assicurarsi che il contenuto venga sottoposto a ricerca per indicizzazione e che l'indice venga aggiornato, eseguire la procedura seguente.

Verificare che il contenuto possa essere trovato facendo in modo che il contenuto del sito sia ricercabile. Per altre informazioni, vedere [abilitare il contenuto di un sito per la ricerca](https://docs.microsoft.com/en-us/sharepoint/make-site-content-searchable).

Quando si modifica una proprietà gestita o quando si modifica il mapping delle proprietà sottoposte a ricerca per indicizzazione o gestite, è necessario sottoporre di nuovo il sito a ricerca per indicizzazione per riflettere le modifiche nell'indice di ricerca. 

Poiché le modifiche vengono apportate nello schema di ricerca e non nel sito effettivo, il crawler non reindicizzerà automaticamente il sito. 

Per altre informazioni, vedere [ricerca per indicizzazione e reindicizzazione manuale di un sito, di una raccolta o di un elenco](https://docs.microsoft.com/en-us/sharepoint/crawl-site-conten).

 Attendere almeno 24 ore dopo aver richiesto manualmente una ricerca per indicizzazione e una reindicizzazione completa per verificare se si è verificato un problema. 

Se sono passate più di 24 ore da quando è stata avviata la ricerca per indicizzazione e la reindicizzazione completa, accedere a un caso di supporto. In molti casi, stiamo già lavorando a una soluzione. Per completare una soluzione, è possibile fornirci almeno 24 ore.

**Importante**: se un sito, un documento (raccolta) o un elenco è stato eliminato e ancora viene visualizzato nei risultati di ricerca, gli utenti devono ricevere un file di errore 404 non trovato durante il tentativo di accesso. Questo problema dovrebbe essere registrato come caso di supporto per ulteriori indagini. 



