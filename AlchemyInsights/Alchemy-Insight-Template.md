---
title: uguale al nome del file è la migliore
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 31a578800468e9f3a69fff4f6e2e1945943c779c
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 10/18/2019
ms.locfileid: "35800049"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>Obbligatorio intestazione di alchimia H1, H2's non funziona.
Procedure consigliate e linee guida per la creazione di alchimia:

1. **Non annidare Insights alchimia nelle cartelle**-questo si romperà la struttura URL. Stiamo cercando di risolvere la cosa.
1. I file presenti nella cartella **AlchemyInsights** devono avere nomi filecaratteri minuscoli con trattini per gli spazi ex. ***How-to-Enable-controversia legale-*** conservazione.
    1. Includere l'ID della regola o l'ID del bucket dal [portale del partner di Alchemy](https://alchemyportal.azurewebsites.net) nel campo ms. Custom. ex. ***ms. Custom: 100021***
1. Utilizzare il resto dei metadati nella parte superiore del file come modello.
1. Nel [portale del partner Alchemy](https://alchemyportal.azurewebsites.net), passare alla sezione **Customer Insight title:** e utilizzarlo come punto di partenza per il titolo H1 per Insight. 
    > [!NOTE]
    > L'alchimia Insights deve avere solo un singolo H1 nella parte superiore o si romperà in produzione. Non è possibile eseguire il rendering di H2s in modo da utilizzare convenzioni **audaci** o altre per indicare sezioni separate.
1. Successivamente, inserire il testo del corpo usando il materiale bozza nella sezione Customer Insights della pagina della regola di alchimia
    1. Gli elenchi puntati sono ottimali
    1. Elenchi numerati troppo
    1. **Grassetto** e *corsivo* sono a-OK
    1. I collegamenti devono essere sempre **"collegamenti al Web"/External** o **collegamenti profondi a elementi dell'interfaccia utente**, non collegamenti interni.
    1. Le immagini non sono supportate ufficialmente in questo momento, ma sono presenti nella roadmap.

E questo è già un po' troppo lungo. La procedura consigliata è di circa 400 caratteri---------------------------------

Una volta che il contenuto è pronto, tirarlo sul ramo Live. Passare quindi al portale del [partner di alchimia](https://alchemyportal.azurewebsites.net) e immettere il nome del file nel campo URL. 