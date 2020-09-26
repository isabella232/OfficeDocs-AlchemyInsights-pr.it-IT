---
title: 1490-risoluzione dei problemi-eDiscovery-errori
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
ms.openlocfilehash: ff28f96d64ec14980e9a47b630246b394faf4610
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277811"
---
# <a name="troubleshoot-content-search-errors"></a>Risoluzione degli errori di ricerca contenuto

Si riscontrano problemi con la ricerca di contenuto o si verificano errori durante l'esportazione dei risultati della ricerca?

Ad esempio, si ricevono le seguenti operazioni durante l'esecuzione di ricerche?

- Errori di CS008 o CS012

- Errori di occupato/timeout del server

- Si è verificato un errore dell'applicazione

Quando si esegue la ricerca o l'esportazione dei risultati di un numero elevato di cassette postali (oltre 100.000 cassette postali), si ottengono errori di esportazione?

Per questi tipi di errori, riprovare la ricerca per i percorsi di contenuto che hanno avuto esito negativo. Per ulteriori informazioni, vedere  [questo articolo](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) .

Se si stanno esportando più di 100K cassette postali, è necessario utilizzare la seguente PowerShell per scaricare i risultati di esportazione:  [esportare i risultati da più di 100K cassette postali](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).
