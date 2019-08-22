---
title: Ricerca in SharePoint Online
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 3c3f6384172b2b4d59db6059618572db11059228
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507635"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a>Indicizzazione e indicizzazione del contenuto in SharePoint Online

Il contenuto deve essere sottoposto a ricerca per indicizzazione e aggiunto all'indice di ricerca per consentire agli utenti di trovare ciò che stanno cercando in SharePoint Online. Il contenuto viene sottoposto a ricerca per indicizzazione in base a una pianificazione di ricerca per indicizzazione predefinita (la pianificazione della ricerca per indicizzazione Il crawler recupera il contenuto modificato dall'ultima ricerca per indicizzazione e aggiorna l'indice. Per assicurarsi che il contenuto venga sottoposto a ricerca per indicizzazione e che l'indice venga aggiornato

- Verificare che il contenuto possa essere trovato facendo in modo che il [contenuto del sito](https://docs.microsoft.com/sharepoint/make-site-content-searchable)sia ricercabile.

- Quando si modifica una proprietà gestita o quando si modifica il mapping delle proprietà sottoposte a ricerca per indicizzazione o gestite, è necessario sottoporre di nuovo il sito a ricerca per indicizzazione per riflettere le modifiche nell'indice di ricerca. 

    Poiché le modifiche vengono apportate nello schema di ricerca e non nel sito effettivo, il crawler non reindicizzerà automaticamente il sito. 

    Per altre informazioni, vedere [ricerca per indicizzazione e reindicizzazione manuale di un sito, di una raccolta o di un elenco](https://docs.microsoft.com/sharepoint/crawl-site-conten).

- Attendere almeno 24 ore dopo aver richiesto manualmente una ricerca per indicizzazione e una reindicizzazione completa per verificare se si è verificato un problema. 

    Se sono passate più di 24 ore da quando è stata avviata la ricerca per indicizzazione e la reindicizzazione completa, accedere a un caso di supporto. In molti casi, stiamo già lavorando a una soluzione. Per completare una soluzione, è possibile fornirci almeno 24 ore.

> [!IMPORTANT]
> Se un sito, un documento (raccolta) o un elenco è stato eliminato e ancora viene visualizzato nei risultati della ricerca, gli utenti devono ricevere un **file di errore 404 non trovato** durante il tentativo di accedervi. Questo problema dovrebbe essere registrato come caso di supporto per ulteriori indagini. 



