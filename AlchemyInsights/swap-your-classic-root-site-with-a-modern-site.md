---
title: Scambiare il sito radice classico con un sito moderno
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: 7209595f5cda9b31e53241d9d5696fa584ff5e5ab3d237aae28542bf7aec9398
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53940823"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Scambiare il sito radice classico con un sito moderno

Se l'ambiente è stato configurato prima di aprile 2019, è possibile modificare il sito radice in un sito moderno utilizzando Microsoft PowerShell:

- Se si dispone di un sito diverso che si desidera utilizzare come sito radice, è possibile sostituire [(scambiare) il sito radice](https://docs.microsoft.com/sharepoint/modern-root-site) con esso. 
    - Utilizzare [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) per scambiare il percorso di un sito con un altro sito durante l'archiviazione del sito originale. Disponibile sia per il sito del team (non connesso a un gruppo) che per il sito di comunicazione. 

- A breve verranno introdotte funzionalità aggiuntive che consentiranno di continuare a utilizzare il contenuto del sito, ma di convertire il sito esistente in un sito di comunicazione. 
>[!Important]
>Queste funzionalità verranno implementazioni gradualmente. Continuare a controllare il Centro messaggi per gli aggiornamenti. 

## <a name="known-issues-with-swapping-sites"></a>Problemi noti con lo scambio di siti

- Il sito di destinazione potrebbe restituire un errore "non trovato" (HTTP 404) per un breve periodo di tempo.
- Per aggiornare l'indice di ricerca, sarà necessario eseguire nuovamente la ricerca per indicizzazione del contenuto. Non è richiesto alcun passaggio manuale, che verrà eseguito automaticamente.
- Qualsiasi elemento dipendente dai collegamenti "statici" (ad esempio File Sync e OneNote file) dovrà essere corretto manualmente.
- Se il sito di origine era un sito di notizie dell'organizzazione, aggiornare l'URL. Ottenere un elenco di tutti i siti di notizie dell'organizzazione.
- Project Potrebbe essere necessario convalidare i siti server per assicurarsi che siano ancora associati correttamente.
