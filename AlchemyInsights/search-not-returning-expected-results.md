---
title: 1491-Search-not-returning-expected-results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 5c4452726c1dbe2232ee63e8a9ee4d089f5c76db
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740478"
---
# <a name="content-search-not-returning-expected-results"></a>Ricerca di contenuto che non restituisce i risultati previsti

Quando si eseguono ricerche di contenuto dal centro sicurezza & conformità di Microsoft 365, è possibile che vengano visualizzati risultati di ricerca imprevisti. Si consideri gli elementi seguenti che possono influire sui risultati della ricerca:

- **Percorsi di contenuto e condizioni di ricerca**: verificare di aver selezionato le posizioni di contenuto e le condizioni di ricerca appropriate. Se è stata eseguita una ricerca di grandi dimensioni (con molte posizioni), è consigliabile suddividerla in più ricerche.

- **Elementi parzialmente indicizzati**:  [gli elementi parzialmente indicizzati](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) delle cassette postali vengono inclusi nei risultati della ricerca stimati. Tuttavia, gli elementi parzialmente indicizzati provenienti da siti di SharePoint e OneDrive non sono inclusi nella stima della ricerca.

- Errori di ricerca: quando si esegue la ricerca di un numero elevato di cassette postali (oltre 100.000 cassette postali), è possibile che si verifichino **problemi**di ricerca, con codici di errore quali CS008-009 e CS012-002. In questo caso, riprovare la ricerca solo per i percorsi di contenuto non riusciti. Per ulteriori informazioni, vedere  [questo articolo](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) .
