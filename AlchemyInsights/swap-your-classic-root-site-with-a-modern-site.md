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
ms.openlocfilehash: 10e8e4bf5e0def9a8256066e1a3c39b9923d31b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691183"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Scambiare il sito radice classico con un sito moderno

Se l'ambiente è stato configurato prima di aprile 2019, è possibile modificare il sito radice in un sito moderno tramite Microsoft PowerShell:

- Se si dispone di un sito diverso che si desidera utilizzare come sito radice, è possibile sostituire [(scambiare) il sito radice](https://docs.microsoft.com/sharepoint/modern-root-site) con esso. 
    - Utilizzare [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) per scambiare il percorso di un sito con un altro sito durante l'archiviazione del sito originale. Disponibile sia per il sito del team (non connesso a un gruppo) sia per il sito di comunicazione. 

- Le funzionalità aggiuntive verranno introdotte a breve che consentiranno di continuare a utilizzare il contenuto del sito, ma di convertire il sito esistente in un sito di comunicazione. 
>[!Important]
>Queste funzionalità verranno Srotolate gradualmente. Continuare a controllare il centro messaggi per gli aggiornamenti. 

## <a name="known-issues-with-swapping-sites"></a>Problemi noti relativi ai siti di swapping

- Il sito di destinazione potrebbe restituire un errore "not found" (HTTP 404) per un breve periodo di tempo.
- Il contenuto dovrà essere sottoposto a ricerca per indicizzazione per aggiornare l'indice di ricerca. Non è necessario un passaggio manuale: questo verrà effettuato automaticamente.
- È necessario correggere manualmente qualsiasi elemento dipendente dai collegamenti "statici", ad esempio i file di sincronizzazione e di OneNote.
- Se il sito di origine è un sito di notizie organizzative, aggiornare l'URL.Ottenere un elenco di tutti i siti di notizie dell'organizzazione.
- Potrebbe essere necessario convalidare i siti di Project Server per assicurarsi che siano ancora associati correttamente.
