---
title: Risoluzione dei problemi relativi all'utilizzo di Open con Esplora risorse
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
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: 6e67c2916e0c5739f6126064d45e175a7fd6f8d4
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36500219"
---
# <a name="fix-problems-with-open-with-explorer"></a>Risolvere i problemi relativi all'apertura con Esplora risorse

Risolvere i problemi comuni relativi all'apertura di una raccolta documenti in SharePoint o OneDrive tramite il comando **Apri con Esplora risorse** : 
  
- Utilizzare Internet Explorer 10 o Internet Explorer 11. **Apri con Esplora risorse** non è compatibile con Microsoft Edge, Google Chrome, Firefox e altri. **Apri con Esplora risorse** è disabilitato in tutti i browser tranne Internet Explorer. 
    
- **Apri con Esplora risorse** non è disponibile nell'esperienza moderna per le raccolte di SharePoint. Utilizzare invece la **visualizzazione in Esplora file** . Selezionare Visualizza **Opzioni** \> visualizzazione **in Esplora file**. La visualizzazione in Esplora file non è compatibile con Microsoft Edge, Google Chrome, Firefox e altri. **Visualizza in Esplora file** in disponibile solo in Internet Explorer. 
    
- Verificare che il servizio WebClient sia in esecuzione. Nella casella di ricerca di Windows, digitare Run, selezionare l'app desktop Run, digitare Services. msc, quindi premere INVIO. Scorrere verso il basso fino al servizio WebClient e verificare che nella colonna **stato** venga visualizzato il messaggio "Running". In caso contrario, fare doppio clic sul servizio, fare clic sul pulsante **Start**e quindi fare clic su **OK**. Potrebbe essere necessario abilitare prima il servizio selezionando **manuale** o **automatico** nella casella **tipo di avvio** . 
    
> [!NOTE]
> L'apertura di una raccolta in Esplora file è utile se è necessario copiare o spostare più file e cartelle una sola volta, ma se si desidera lavorare regolarmente nella raccolta, è consigliabile sincronizzarla. Per risolvere i problemi relativi all'apertura in Esplora file, vedere [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Per informazioni su come configurare la sincronizzazione, vedere [sincronizzare i file di SharePoint con il nuovo client di sincronizzazione di OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).
  
Per ulteriori informazioni, vedere l'articolo su [come utilizzare il comando "Apri con Esplora risorse" per risolvere i problemi in SharePoint Online](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) . 
  

