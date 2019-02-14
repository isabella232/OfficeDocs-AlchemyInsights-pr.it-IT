---
title: 1491-Search-NOT-Returning-expected-Results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: ''
ms.openlocfilehash: 881a579d7098578452c994b7ac66fe22a1d90dc2
ms.sourcegitcommit: 5182c9a73641079be59740e4524434b2e8be613a
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 02/12/2019
ms.locfileid: "29964893"
---
# <a name="content-search-not-returning-expected-results"></a>Ricerca del contenuto non restituisce i risultati previsti

Quando si esegue ricerche di contenuto da & la protezione di Office 365 centro conformità, è possibile ottenere risultati di ricerca imprevisti. Prendere in considerazione le operazioni seguenti che possono influire sui risultati di ricerca:

- **I percorsi di contenuti e le condizioni di ricerca**: assicurarsi di avere selezionato i percorsi di contenuti appropriati e i criteri di ricerca. Se si esegue una ricerca di grandi dimensioni (con più posizioni), prendere in considerazione la suddivisione in più ricerche.

- **Parzialmente voci indicizzate**: [voci indicizzate parzialmente](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) dalle cassette postali vengono inclusi nei risultati della ricerca stimati. Tuttavia, elementi indicizzati parzialmente dai siti di SharePoint e OneDrive non vengono incluse nella ricerca stima.

- **Errori di ricerca**: durante la ricerca di un numero elevato di cassette postali (più di 100.000 cassette postali), è possibile ottenere gli errori di ricerca, codici di errore, ad esempio 009 CS008 e CS012-002). In questo caso, ripetere la ricerca solo per i percorsi di contenuti non riuscite. [In questo articolo](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) per ulteriori informazioni, vedere.
