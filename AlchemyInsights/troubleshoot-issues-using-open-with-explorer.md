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
ms.openlocfilehash: 0cbcfb506295d5732f7109be7a103bbdef530a529c7408c6d9d45a7b38a89915
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54048160"
---
# <a name="fix-problems-with-open-with-explorer"></a>Risolvere i problemi relativi all'apertura con Esplora risorse

Consente di risolvere i problemi comuni relativi all'apertura di una raccolta documenti in SharePoint o OneDrive tramite il **comando Apri con Esplora** risorse: 
  
- Usa Internet Explorer 10 o Internet Explorer 11. **Apri con Explorer** non è compatibile con Microsoft Edge, Google Chrome, Firefox e altri. **L'opzione Apri con Esplora** risorse è disabilitata in tutti i browser ad eccezione di Internet Explorer. 
    
- **L'opzione Apri** con Esplora risorse non è disponibile nell'esperienza moderna per SharePoint raccolte. Usa **invece Visualizza in Esplora** file. Selezionare **Visualizza opzioni** Visualizza in Esplora \> **file.** La visualizzazione in Esplora file non è compatibile con Microsoft Edge, Google Chrome, Firefox e altri. **Visualizza in Esplora file** in disponibile solo in Internet Explorer. 
    
- Verificare che il servizio WebClient sia in esecuzione. Nella casella Windows ricerca digitare Esegui, selezionare l'app desktop Esegui, digitare services.msc e quindi premere INVIO. Scorrere verso il basso fino al servizio WebClient e verificare che nella colonna **Stato** sia visualizzato "In esecuzione". In caso contrario, fare doppio clic sul servizio, fare clic su **Avvia** e quindi su **OK.** Potrebbe essere necessario abilitare prima il servizio selezionando Manuale **o** **Automatico** nella casella **Tipo di** avvio. 
    
> [!NOTE]
> L'apertura di una raccolta in Esplora file è utile se è necessario copiare o spostare più file e cartelle una sola volta, ma se si desidera lavorare regolarmente nella raccolta, è consigliabile sincronizzarla. Per risolvere i problemi di apertura in Esplora file, vedi [Aprire in Esplora risorse.](https://go.microsoft.com/fwlink/?linkid=871665) Per info sulla configurazione della sincronizzazione, vedi [Sincronizzare SharePoint file con il nuovo client sincronizzazione OneDrive.](https://go.microsoft.com/fwlink/?linkid=871666)
  
Per altre informazioni, vedi l'articolo Come usare il comando ["Apri con Esplora risorse"](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) per risolvere i problemi in SharePoint Online. 
  

