---
title: 'uguale al nome del file è la migliore [RULE #-Description]'
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: e248c2ee3cbb9a86f21c1f36be10c893df76ff52
ms.sourcegitcommit: 3070905131e6d8449981231a3551c0bb4ca38ae6
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/14/2019
ms.locfileid: "30634508"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>Obbligatorio intestazione di alchimia H1, H2's non funziona.
Procedure consigliate e linee guida per la creazione di alchimia:

1. **Non annidare Insights alchimia nelle cartelle**-questo si romperà la struttura URL. Stiamo cercando di risolvere la cosa.
1. I file nella cartella **AlchemyInsights** devono disporre dell'ID regola e del nome della regola dal [portale del partner](https://alchemyportal.azurewebsites.net) di alchimia nel nome del file.
    1. ex. ***976-How-to-Enable-controversia legale-conservazione***
1. Utilizzare i metadati nella parte superiore del file come modello. Non è necessario nient'altro.
1. Nel [portale del partner Alchemy](https://alchemyportal.azurewebsites.net), passare alla sezione **Customer Insight title:** e utilizzarlo come punto di partenza per il titolo H1 per Insight. 
    > [!NOTE]
    > L'alchimia Insights deve avere solo un singolo H1 nella parte superiore o si romperà in produzione. Non è possibile eseguire il rendering di H2s in modo da utilizzare convenzioni **audaci** o altre per indicare sezioni separate.
1. Successivamente, inserire il testo del corpo usando il materiale bozza nella sezione Customer Insights della pagina della regola di alchimia
    1. Gli elenchi puntati sono ottimali
    1. Elenchi numerati troppo
    1. **Grassetto** e *corsivo* sono a-OK
    1. I collegamenti devono essere sempre **"collegamenti al Web"/External** o **collegamenti profondi a elementi dell'interfaccia utente**, non collegamenti interni.

E questo è già un po' troppo lungo. La procedura consigliata è di circa 400 caratteri---------------------------------

Una volta che il contenuto è pronto, tirarlo sul ramo Live. Passare quindi al portale del [partner](https://alchemyportal.azurewebsites.net) di alchimia e immettere il nome del file nel campo URL. Assicurarsi che Insight revisionato e pubblicato dica "Sì" e quindi fare clic su Aggiorna regola. **(Questo aspetto sarà più bello nella nuova versione del portale-rilasciando al più presto).** 
 ![campo URL](media/for-content-team.PNG)

