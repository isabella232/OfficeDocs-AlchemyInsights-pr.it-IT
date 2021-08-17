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
ms.openlocfilehash: 7b819b9bb18b5c0a635e708eccc0f23271267874707e5f3a7d41b633a05f2822
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105572"
---
# <a name="troubleshoot-content-search-errors"></a>Risolvere gli errori di Ricerca contenuto

Si verificano problemi con Ricerca contenuto o si verificano errori durante l'esportazione dei risultati della ricerca?

Ad esempio, si riceve quanto segue quando si eseguono ricerche?

- Errori CS008 o CS012

- Errori di timeout/occupato del server

- Si è verificato un errore dell'applicazione

Oppure durante la ricerca o l'esportazione dei risultati da un numero elevato di cassette postali (oltre 100.000 cassette postali), si verificano errori di esportazione?

Per questi tipi di errori, ritentare la ricerca dei percorsi di contenuto non riusciti. Per  [ulteriori informazioni,](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) vedere questo articolo.

Se si esportano più di 100.000 cassette postali, è necessario utilizzare powershell seguente per scaricare i risultati di esportazione: Esportazione dei risultati da più di  [100.000](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)cassette postali .
