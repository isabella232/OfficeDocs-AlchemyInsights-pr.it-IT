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
ms.openlocfilehash: 7b915ab18d10948b8588dc6e2ef6af9891524861a924e2193dd73c2c77ffe6da
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918899"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>"Required Alchemy Header H1, H2's don's don's work."
Procedure consigliate e linee guida per la creazione di alchimie:

1. **Non annidare Alchemy Insights cartelle,** in modo da interrompere la struttura dell'URL. Stiamo cercando di risolvere questo problema.
1. I file nella **cartella AlchemyInsights** devono contenere nomi di file minuscoli con trattini per spazi ex. **_how-to-enable-litigation-hold_**.
    1. Includere l'ID regola o l'ID bucket dal [portale di Alchemy Partner](https://alchemyportal.azurewebsites.net) nel campo ms.custom. ex. ***ms.custom: 100021***
1. Usa il resto dei metadati nella parte superiore di questo file come modello.
1. Nel [portale per i partner di Alchemy](https://alchemyportal.azurewebsites.net)passare alla sezione **Customer Insight Title:** e usarlo come punto di partenza per il titolo H1 per le informazioni dettagliate. 
    > [!NOTE]
    > L'Insights deve avere solo un singolo H1 nella parte superiore o si interromperà in produzione. H2s non esegue il rendering, quindi usa **il grassetto** o altre convenzioni per indicare sezioni separate.
1. Compilare quindi il corpo del testo utilizzando il materiale della bozza nella Customer Insights della pagina Regola di alchimia
    1. Gli elenchi puntati sono a posto
    1. Elenchi numerati
    1. **Grassetto** e *corsivo* sono a-ok
    1. I collegamenti devono sempre essere **"collegamenti al Web"/collegamenti** diretti o esterni a elementi dell'interfaccia **utente** e non collegamenti interni.
    1. Al momento le immagini non sono ufficialmente supportate, ma sono sulla roadmap.

E questo è già un po' troppo lungo. La procedura consigliata è di circa 400 caratteri ---------------------------------

Quando il contenuto è pronto, trascinalo nel ramo live. Quindi, vai al [portale di Alchemy Partner](https://alchemyportal.azurewebsites.net) e immetti il nome del file nel campo url. 