---
title: 1491-search-not-returning-expected-results
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
ms.openlocfilehash: 846034d68a59d053cbe37aeba3a75e20a60786fd7ff24106964229b1deb77608
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052714"
---
# <a name="content-search-not-returning-expected-results"></a>Ricerca contenuto non restituisce i risultati previsti

Quando si eseguono ricerche di contenuto Microsoft 365 sicurezza & Centro conformità, è possibile che si ricevano risultati di ricerca imprevisti. Considerare gli aspetti seguenti che possono influire sui risultati della ricerca:

- **Percorsi di contenuto e condizioni di ricerca:** assicurarsi di aver selezionato i percorsi di contenuto e le condizioni di ricerca appropriate. Se è stata eseguita una ricerca di grandi dimensioni (con molte posizioni), è consigliabile suddividerla in più ricerche.

- **Elementi parzialmente indicizzati:**  [gli elementi parzialmente indicizzati](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) dalle cassette postali sono inclusi nei risultati di ricerca stimati. Tuttavia, gli elementi parzialmente indicizzati dai siti SharePoint e OneDrive non sono inclusi nella stima della ricerca.

- **Errori di ricerca**: quando si esegue una ricerca in un numero elevato di cassette postali (oltre 100.000 cassette postali), è possibile che si verificano errori di ricerca, con codici di errore quali CS008-009 e CS012-002. In questo caso, ritentare la ricerca solo per i percorsi di contenuto non riusciti. Per  [ulteriori informazioni,](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) vedere questo articolo.
