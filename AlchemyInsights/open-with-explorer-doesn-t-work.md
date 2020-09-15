---
title: Apertura con Esplora risorse non funziona
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
ms.openlocfilehash: 5bf28982533d8ca9998605cf3592f317c0ef99b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47694460"
---
# <a name="open-with-explorer-isnt-working"></a>Apertura con Esplora risorse non funzionante

Se l' **apertura con Esplora risorse** o la **visualizzazione in Esplora file** non funziona, verificare che il servizio WebClient sia impostato su **in esecuzione** attenendosi alla procedura riportata di seguito. Ad esempio, potrebbe richiedere molto tempo per aprire una raccolta di SharePoint o OneDrive quando il servizio non è in esecuzione. 
  
1. Nella casella di ricerca di Windows, digitare Run, selezionare l'app desktop Run, digitare Services. msc, quindi selezionare **invio**.
    
2. Scorrere verso il basso fino al servizio WebClient e controllare la colonna **stato** . Se lo stato del servizio WebClient non è **in esecuzione**, fare doppio clic sul servizio, fare clic sul pulsante **Start**e quindi fare clic su **OK**. Abilitare il servizio, se necessario, selezionando **manuale** o **automatico** nella casella **tipo di avvio** . 
    
> [!NOTE]
> Per risolvere i problemi relativi all'apertura in Esplora file, vedere [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Esplorare la sincronizzazione come alternativa migliore: [sincronizzare i file di SharePoint con il nuovo client di sincronizzazione di OneDrive](https://go.microsoft.com/fwlink/?linkid=871666). 
  

