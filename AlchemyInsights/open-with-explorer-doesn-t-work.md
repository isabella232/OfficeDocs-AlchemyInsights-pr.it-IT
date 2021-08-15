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
ms.openlocfilehash: 164d5fe8c992df825d1f52f19792e1623526c35c58ff2f1e1ab601fdcf5f0f53
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54011340"
---
# <a name="open-with-explorer-isnt-working"></a>L'apertura con Esplora risorse non funziona

Se **Apri con Esplora risorse** o Visualizza in Esplora **file** non funziona, assicurati che il servizio WebClient sia impostato su **In** esecuzione seguendo la procedura seguente. Ad esempio, potrebbe essere necessario molto tempo per aprire una raccolta SharePoint o OneDrive quando il servizio non è in esecuzione. 
  
1. Nella casella Windows ricerca digitare Esegui, selezionare l'app desktop Esegui, digitare services.msc e quindi selezionare **Invio**.
    
2. Scorrere verso il basso fino al servizio WebClient e controllare la **colonna** Stato. Se lo stato del servizio WebClient non è **In esecuzione,** fare doppio clic sul servizio, fare clic su **Avvia** e quindi su **OK.** Abilitare il servizio, se necessario, selezionando **Manuale** o **Automatico** nella casella **Tipo di** avvio. 
    
> [!NOTE]
> Per risolvere i problemi di apertura in Esplora file, vedi [Aprire in Esplora risorse.](https://go.microsoft.com/fwlink/?linkid=871665) Esplorare la sincronizzazione come alternativa migliore: [sincronizzare SharePoint file con il nuovo client sincronizzazione OneDrive .](https://go.microsoft.com/fwlink/?linkid=871666) 
  

