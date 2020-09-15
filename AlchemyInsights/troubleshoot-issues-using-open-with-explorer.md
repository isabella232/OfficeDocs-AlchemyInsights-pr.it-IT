---
title: Risoluzione dei problemi relativi all'utilizzo di Open con Esplora risorse
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
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: e7fe59b94d216d89c2f2f7100a3d8bf7a0b0196e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47659062"
---
# <a name="fix-problems-with-open-with-explorer"></a>Risolvere i problemi relativi all'apertura con Esplora risorse

Risolvere i problemi comuni relativi all'apertura di una raccolta documenti in SharePoint o OneDrive tramite il comando **Apri con Esplora risorse** : 
  
- Utilizzare Internet Explorer 10 o Internet Explorer 11. **Apri con Esplora risorse** non è compatibile con Microsoft Edge, Google Chrome, Firefox e altri. **Apri con Esplora risorse** è disabilitato in tutti i browser tranne Internet Explorer. 
    
- **Apri con Esplora risorse** non è disponibile nell'esperienza moderna per le raccolte di SharePoint. Utilizzare invece la **visualizzazione in Esplora file** . Selezionare Visualizza **Opzioni** visualizzazione \> **in Esplora file**. La visualizzazione in Esplora file non è compatibile con Microsoft Edge, Google Chrome, Firefox e altri. **Visualizza in Esplora file** in disponibile solo in Internet Explorer. 
    
- Verificare che il servizio WebClient sia in esecuzione. Nella casella di ricerca di Windows, digitare Run, selezionare l'app desktop Run, digitare Services. msc, quindi premere INVIO. Scorrere verso il basso fino al servizio WebClient e verificare che nella colonna **stato** venga visualizzato il messaggio "Running". In caso contrario, fare doppio clic sul servizio, fare clic sul pulsante **Start**e quindi fare clic su **OK**. Potrebbe essere necessario abilitare prima il servizio selezionando **manuale** o **automatico** nella casella **tipo di avvio** . 
    
> [!NOTE]
> L'apertura di una raccolta in Esplora file è utile se è necessario copiare o spostare più file e cartelle una sola volta, ma se si desidera lavorare regolarmente nella raccolta, è consigliabile sincronizzarla. Per risolvere i problemi relativi all'apertura in Esplora file, vedere [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Per informazioni su come configurare la sincronizzazione, vedere [sincronizzare i file di SharePoint con il nuovo client di sincronizzazione di OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).
  
Per ulteriori informazioni, vedere l'articolo su [come utilizzare il comando "Apri con Esplora risorse" per risolvere i problemi in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) . 
  

