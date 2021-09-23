---
title: 1490-troubleshooting-eDiscovery-failures
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
- "1490"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: b60cfc298ee05375523e3660f407ab03e630c861
ms.sourcegitcommit: e9e282be4997b0ee95f1ff4491e0943f8fc52444
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/22/2021
ms.locfileid: "59481794"
---
# <a name="troubleshoot-content-search-errors"></a>Risolvere gli errori di Ricerca contenuto

Si verificano problemi con Ricerca contenuto o si verificano errori durante l'esportazione dei risultati della ricerca?
Ad esempio, si riceve quanto segue quando si eseguono le ricerche?

- Errori CS007, CS008 o CS012

- Errori di timeout/occupato del server

- Si è verificato un errore dell'applicazione

In caso contrario, si verificano errori di esportazione quando si esportino risultati da un numero elevato (oltre 100.000) di cassette postali?

Per questi errori, ritentare la ricerca per i percorsi di contenuto che hanno avuto esito negativo o aggiornare la ricerca riducendo la complessità della query di ricerca. Ad esempio, una ricerca con caratteri jolly potrebbe restituire troppi risultati per l'elaborazione da parte del sistema, causando un errore CS007.   

Per ulteriori informazioni, vedere [Retry a Content Search to resolve a content location error](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) oppure [Investigate, troubleshoot, and resolve common eDiscovery issues](https://docs.microsoft.com/microsoft-365/compliance/ediscovery-troubleshooting-common-issues).

Se si esportano più di 100.000 cassette postali, è necessario scaricare i risultati dell'esportazione. Per informazioni dettagliate, vedere [Export Content search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).
