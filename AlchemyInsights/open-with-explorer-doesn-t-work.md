---
title: L'apertura con Esplora risorse non funziona
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 2ba6f08b40dd194bf1ffd9a455a134a2fc553b51
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58321865"
---
# <a name="open-with-explorer-isnt-working"></a>L'apertura con Esplora risorse non funziona

Se **Apri con Esplora risorse** o Visualizza in Esplora **file** non funziona, assicurati che il servizio WebClient sia impostato su **In** esecuzione seguendo la procedura seguente. Ad esempio, potrebbe essere necessario molto tempo per aprire una raccolta SharePoint o OneDrive quando il servizio non è in esecuzione. 
  
1. Nella casella Windows ricerca digitare Esegui, selezionare l'app desktop Esegui, digitare services.msc e quindi selezionare **Invio**.
    
2. Scorrere verso il basso fino al servizio WebClient e controllare la **colonna** Stato. Se lo stato del servizio WebClient non è **In esecuzione,** fare doppio clic sul servizio, fare clic su **Avvia** e quindi su **OK.** Abilitare il servizio, se necessario, selezionando **Manuale** o **Automatico** nella casella **Tipo di** avvio. 
    
**Nota:** per risolvere i problemi di apertura in Esplora file, vedi [Aprire in Esplora file.](https://go.microsoft.com/fwlink/?linkid=871665) Esplorare la sincronizzazione come alternativa migliore: [sincronizzare SharePoint file con il nuovo client sincronizzazione OneDrive.](https://go.microsoft.com/fwlink/?linkid=871666) 
  

