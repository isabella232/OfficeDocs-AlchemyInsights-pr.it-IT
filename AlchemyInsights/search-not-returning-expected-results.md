---
title: 1491-Search-not-returning-expected-results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 1491
ms.assetid: ''
ms.openlocfilehash: 517d9b75fc3aef09c0c2d5870aa695cc0ab10f06
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32383839"
---
# <a name="content-search-not-returning-expected-results"></a>Ricerca di contenuto che non restituisce i risultati previsti

Quando si eseguono ricerche di contenuto dal centro conformità di Office 365 Security &, è possibile che vengano visualizzati risultati di ricerca imprevisti. Si conSideri gli elementi seguenti che possono influire sui risultati della ricerca:

- **Percorsi di contenuto e condizioni di ricerca**: verificare di aver selezionato le posizioni di contenuto e le condizioni di ricerca appropriate. Se è stata eseguita una ricerca di grandi dimensioni (con molte posizioni), è consigliabile suddividerla in più ricerche.

- **Elementi parzialmente indicizzati**: [gli elementi parzialmente indicizzati](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) delle cassette postali vengono inclusi nei risultati della ricerca stimati. Tuttavia, gli elementi parzialmente indicizzati provenienti da siti di SharePoint e OneDrive non sono inclusi nella stima della ricerca.

- Errori di ricerca: quando si esegue la ricerca di un numero elevato di cassette postali (oltre 100.000 cassette postali), è possibile che si verifichino **problemi**di ricerca, con codici di errore quali CS008-009 e CS012-002. In questo caso, riprovare la ricerca solo per i percorsi di contenuto non riusciti. Per ulteriori informazioni, vedere [questo articolo](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) .
