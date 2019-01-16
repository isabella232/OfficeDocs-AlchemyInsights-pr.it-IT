---
title: Apri con Esplora non funziona
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: b55fc7bd5670e655334ef7be368b245c8899633a
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/15/2019
ms.locfileid: "28295763"
---
# <a name="open-with-explorer-isnt-working"></a>Apri con Esplora non funziona

Se non funziona **Apri con Esplora risorse** o in **visualizzazione in Esplora File** verificare che il servizio Web client è impostato su **in esecuzione** eseguendo la procedura seguente. Ad esempio, può richiedere molto tempo per aprire una raccolta SharePoint o OneDrive quando il servizio non è in esecuzione. 
  
1. Nella casella di ricerca di Windows, tipo eseguita, selezionare l'app desktop Esegui, digitare Services. msc e quindi selezionare **INVIO**.
    
2. Scorrere verso il basso per il servizio Web client e controllare la colonna **stato** . Se lo stato del servizio WebClient non è **in esecuzione**, fare doppio clic sul servizio, fare clic su **Start**e quindi fare clic su **OK**. Abilitare il servizio, se necessario, tramite la selezione nella casella **tipo avvio** **manuale** o **automatico** . 
    
> [!NOTE]
> Per risolvere i problemi aprire Esplora File, vedere [Open nell'elenco cartelle](https://go.microsoft.com/fwlink/?linkid=871665). Esplorazione di sincronizzazione come un'alternativa migliore: [file di sincronizzazione di SharePoint con il nuovo client di sincronizzazione OneDrive](https://go.microsoft.com/fwlink/?linkid=871666). 
  

