---
title: Risolvere i problemi con Apri con Esplora risorse
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
ms.openlocfilehash: 49d6d449af6e718d70c9948a03f7e2e1e21517d2
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323570"
---
# <a name="fix-problems-with-open-with-explorer"></a>Risolvere i problemi relativi all'apertura con Esplora risorse

Consente di risolvere i problemi comuni relativi all'apertura di una raccolta documenti SharePoint o OneDrive tramite il **comando Apri con Esplora** risorse: 
  
- Usa Internet Explorer 10 o Internet Explorer 11. **Apri con Explorer** non è compatibile con Microsoft Edge, Google Chrome, Firefox e altri. **L'opzione Apri con Esplora** risorse è disabilitata in tutti i browser ad eccezione di Internet Explorer. 
    
- **L'opzione Apri** con Esplora risorse non è disponibile nell'esperienza moderna per SharePoint raccolte. Usa **invece Visualizza in Esplora** file. Selezionare **Visualizza opzioni** Visualizza in Esplora \> **file.** La visualizzazione in Esplora file non è compatibile con Microsoft Edge, Google Chrome, Firefox e altri. **Visualizza in Esplora file** in disponibile solo in Internet Explorer. 
    
- Verificare che il servizio WebClient sia in esecuzione. Nella casella Windows ricerca digitare Esegui, selezionare l'app desktop Esegui, digitare services.msc e quindi premere INVIO. Scorrere verso il basso fino al servizio WebClient e verificare che nella colonna **Stato** sia visualizzato "In esecuzione". In caso contrario, fare doppio clic sul servizio, fare clic su **Avvia** e quindi su **OK.** Potrebbe essere necessario abilitare prima il servizio selezionando Manuale **o** **Automatico** nella casella **Tipo di** avvio. 
    
**Nota:** l'apertura di una raccolta in Esplora file è utile se devi copiare o spostare più file e cartelle una sola volta, ma se vuoi lavorare regolarmente nella raccolta, ti consigliamo di sincronizzarla. Per risolvere i problemi di apertura in Esplora file, vedi [Aprire in Esplora risorse.](https://go.microsoft.com/fwlink/?linkid=871665) Per info sulla configurazione della sincronizzazione, vedi [Sincronizzare SharePoint file con il nuovo client sincronizzazione OneDrive.](https://go.microsoft.com/fwlink/?linkid=871666)
  
Per ulteriori informazioni, vedere l'articolo Come usare il comando ["Apri con Esplora risorse"](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) per risolvere i problemi in SharePoint Online. 
  

