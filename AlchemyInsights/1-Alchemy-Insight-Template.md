---
title: 'stesso come nome del file è consigliabile [regola #-descrizione]'
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 278a26f4b986a85e33442baef690d3bb44462ace
ms.sourcegitcommit: 32355b76d45b730a069575efeec708149d4aeaa3
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 02/01/2019
ms.locfileid: "29697134"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>Obbligatorio Alchemy intestazione s1, s2 non funzionano.
Procedure consigliate e linee guida per la creazione e modifica Alchemy:

1. **Non nidificare Alchemy Insights nelle cartelle**- questa operazione si interrompe la struttura url. Vengono cercati nella correzione seguente.
1. File nella cartella **AlchemyInsights** devono avere ID della regola e nome della regola dal [portale per i Partner Alchemy](https://alchemyportal.azurewebsites.net) il nome di file.
    1. ad esempio ***976-How-to-enable-litigation-hold***
1. Utilizzare i metadati nella parte superiore del file del modello. Niente è obbligatorio.
1. Nel [portale dei Partner Alchemy](https://alchemyportal.azurewebsites.net), passare alla sezione **Customer delle conoscenze Title:** e l'utilizzo che un avviare punti per il titolo di s1 per la comprensione. 
    > [!NOTE]
    > Alchemy informativa deve essere un singolo H1 nella parte superiore o interromperanno nell'ambiente di produzione. Non eseguire il rendering H2s così utilizza **il formato grassetto** o altre convenzioni per segnalare la presenza di sezioni separate.
1. Successivamente, completare il corpo del testo utilizzando il materiale bozza nella sezione Osservazioni dei clienti della pagina Alchemy regola
    1. Gli elenchi puntati non siano danneggiati
    1. Elenchi numerati troppo
    1. Sono a-ok **grassetto** e *corsivo*
    1. Collegamenti devono essere sempre uno **"collegamenti Web" / esterno** OR **approfondita collegamenti agli elementi dell'interfaccia utente**, i collegamenti non interni.

Si tratta veramente già un po' troppo lungo. Procedura consigliata è di circa 400 caratteri--

Dopo che il contenuto è pronto, estrarlo al ramo live. Accedere al [portale dei Partner Alchemy](https://alchemyportal.azurewebsites.net) , quindi immettere il nome del file nel campo url. Verificare che informa che delle conoscenze rivisto e pubblicato "Sì" e quindi fare clic su regola di aggiornamento. **(Si avrà un aspetto spiegazione nella nuova versione del portale - rilascio presto disponibili.)** 
 ![campo url](media/for-content-team.PNG)

