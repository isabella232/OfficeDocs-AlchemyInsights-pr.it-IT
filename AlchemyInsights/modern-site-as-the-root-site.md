---
title: Sito moderno come sito radice
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: a0f48dc79b51168c9cc045078ad8fc7d668343c7
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58327606"
---
# <a name="modern-site-as-root-site"></a>Sito moderno come sito radice

È stata avviata l'implementazione di una nuova funzionalità che consente di scambiare il sito radice del sito classico [con un sito moderno.](https://docs.microsoft.com/sharepoint/modern-root-site) Utilizzare [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) per scambiare il percorso di un sito con un altro sito durante l'archiviazione del sito originale. Disponibile sia per il sito del team (non connesso a un gruppo) che per il sito di comunicazione.

**Importante:** non eliminare il sito radice classico per creare un sito di comunicazione moderno. Questo non è supportato da Microsoft. L'eliminazione del sito radice rende inaccessibili tutti i siti SharePoint dell'organizzazione fino a quando non si ripristina il sito o non si crea un nuovo sito con lo stesso URL. Questa funzionalità verrà comunicata tramite il Centro messaggi. È consigliabile che la funzionalità sia attivata nel tenant a breve.

## <a name="known-issues-with-swapping-sites"></a>Problemi noti con lo scambio di siti
- Il sito di destinazione potrebbe restituire un errore "non trovato" (HTTP 404) per un breve periodo di tempo.
- Per aggiornare l'indice di ricerca, sarà necessario eseguire nuovamente la ricerca per indicizzazione del contenuto. Non è necessario alcun passaggio manuale qui, questa operazione verrà eseguita automaticamente.
- Tutto ciò che dipende dai collegamenti "statici" (ad esempio, Sincronizzazione file e OneNote file) dovrà essere corretto manualmente.
- Project Potrebbe essere necessario convalidare i siti server per assicurarsi che siano ancora associati correttamente. 
