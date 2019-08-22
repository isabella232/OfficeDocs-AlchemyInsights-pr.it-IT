---
title: Sito moderno come sito radice
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 2f75f1e60af06da47fe846e84bbb370dd60084e9
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36543857"
---
# <a name="modern-site-as-root-site"></a>Sito moderno come sito radice

È stata avviata l'implementazione di una nuova funzionalità che consente di scambiare il sito radice del sito classico con un sito moderno. Utilizzare [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) per scambiare il percorso di un sito con un altro sito durante l'archiviazione del sito originale. Disponibile sia per il sito del team (non connesso a un gruppo) sia per il sito di comunicazione. 

>[!Important]
> Non eliminare il sito radice classico per creare un sito di comunicazione moderno. Questo non è supportato da Microsoft. L'eliminazione del sito radice renderà tutti i siti di SharePoint dell'organizzazione inaccessibili a tutti gli utenti, fino a quando non si ripristina il sito o si crea un nuovo sito nello stesso URL. Questa funzionalità verrà comunicata tramite il centro messaggi. È consigliabile che la caratteristica venga attivata brevemente nel tenant.

## <a name="known-issues-with-swapping-sites"></a>Problemi noti relativi ai siti di swapping
- Il sito di destinazione potrebbe restituire un errore "not found" (HTTP 404) per un breve periodo di tempo.
- Il contenuto dovrà essere sottoposto a ricerca per indicizzazione per aggiornare l'indice di ricerca. Non è necessario eseguire un passaggio manuale in questa fase, verrà eseguita automaticamente.
- È necessario correggere manualmente qualsiasi elemento dipendente dai collegamenti "statici", ad esempio i file di sincronizzazione e di OneNote.
- Potrebbe essere necessario convalidare i siti di Project Server per assicurarsi che siano ancora associati correttamente. 
