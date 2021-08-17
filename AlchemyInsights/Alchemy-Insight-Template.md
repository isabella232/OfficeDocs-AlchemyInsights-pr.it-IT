---
title: come filename è la soluzione migliore
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: b6fbaf3f2ab30888d7a8f9d6f5aeccb65b5cfd0b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58312829"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>"Intestazione alchimia obbligatoria H1, H2 non funziona."
Procedure consigliate e linee guida per la creazione di alchimie:

1. **Non annidare Alchemy Insights nelle cartelle,** in modo da interrompere la struttura dell'URL. Stiamo cercando di risolvere questo problema.
1. I file nella **cartella AlchemyInsights** devono contenere nomi di file minuscoli con trattini per spazi ex. **_how-to-enable-litigation-hold_**.
    1. Includere l'ID regola o l'ID bucket dal [portale di Alchemy Partner](https://alchemyportal.azurewebsites.net) nel campo ms.custom. ex. ***ms.custom: 100021***
1. Usa il resto dei metadati nella parte superiore di questo file come modello.
1. Nel [portale per i partner di Alchemy](https://alchemyportal.azurewebsites.net)passare alla sezione **Customer Insight Title:** e usarlo come punto di partenza per il titolo H1 per le informazioni dettagliate. 

**Nota:** l'alchimia Insights deve avere solo una singola H1 nella parte superiore o si interromperà in produzione. H2s non esegue il rendering, quindi usa **il grassetto** o altre convenzioni per indicare sezioni separate.
1. Compilare quindi il corpo del testo utilizzando il materiale della bozza nella Customer Insights della pagina Regola di alchimia
    1. Gli elenchi puntati sono a posto
    1. Elenchi numerati
    1. **Grassetto** e *corsivo* sono a-ok
    1. I collegamenti devono essere sempre **"collegamenti al Web"/collegamenti** diretti o esterni a elementi dell'interfaccia **utente** e non collegamenti interni.
    1. Al momento le immagini non sono ufficialmente supportate, ma sono sulla roadmap.

E questo è già un po' troppo lungo. La procedura consigliata è di circa 400 caratteri ---------------------------------

Quando il contenuto è pronto, trascinalo nel ramo live. Quindi, vai al [portale di Alchemy Partner](https://alchemyportal.azurewebsites.net) e immetti il nome del file nel campo url. 