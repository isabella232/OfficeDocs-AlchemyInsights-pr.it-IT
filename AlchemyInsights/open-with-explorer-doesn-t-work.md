---
title: Apertura con Esplora risorse non funziona
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 73d33e50449345c312abdd39afcc36e0c95fd1c4
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32419876"
---
# <a name="open-with-explorer-isnt-working"></a>Apertura con Esplora risorse non funzionante

Se l' **apertura con Esplora risorse** o la **visualizzazione in Esplora file** non funziona, verificare che il servizio WebClient sia impostato su **in esecuzione** attenendosi alla procedura riportata di seguito. Ad esempio, potrebbe richiedere molto tempo per aprire una raccolta di SharePoint o OneDrive quando il servizio non è in esecuzione. 
  
1. Nella casella di ricerca di Windows, digitare Run, selezionare l'app desktop Run, digitare Services. msc, quindi selezionare **invio**.
    
2. Scorrere verso il basso fino al servizio webClient e controllare la colonna **stato** . Se lo stato del servizio webClient non è **in esecuzione**, fare doppio clic sul servizio, fare clic sul pulsante **Start**e quindi fare clic su **OK**. Abilitare il servizio, se necessario, selezionando **manuale** o **automatico** nella casella **tipo di avvio** . 
    
> [!NOTE]
> Per risolvere i problemi relativi all'apertura in Esplora file, vedere [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Esplorare la sincronizzazione come alternativa migliore: [sincronizzare i file di SharePoint con il nuovo client di sincronizzazione di OneDrive](https://go.microsoft.com/fwlink/?linkid=871666). 
  

