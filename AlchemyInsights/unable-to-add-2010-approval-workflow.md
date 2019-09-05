---
title: Impossibile aggiungere il flusso di lavoro di approvazione 2010
ms.author: pebaum
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: 13e3ed6db8c31adb1eb5a556c0e5fbc437b3fdb1
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/04/2019
ms.locfileid: "36748688"
---
# <a name="unable-to-add-2010-approval-workflow"></a>Impossibile aggiungere il flusso di lavoro di approvazione 2010

In una raccolta siti di Microsoft SharePoint non è possibile aggiungere un flusso di lavoro riutilizzabile a livello globale, ad esempio "approvazione-SharePoint 2010", a un elenco o una raccolta.
  
Per risolvere il problema, attenersi alla seguente procedura: 
  
1. Aprire il sito Web radice della raccolta siti in SharePoint Designer 2013.
  
2. In **oggetti sito**selezionare **flussi di lavoro**. 
  
3. Nella **nuova** sezione della barra multifunzione **flussi di lavoro** , selezionare **flusso di lavoro riutilizzabile**. 
  
4. Nel modulo **Crea flusso di lavoro riutilizzabile** , immettere il nome * * *Repair2010* * *. Per il **tipo di piattaforma**, fare clic su flusso di lavoro di **SharePoint 2010**e quindi fare clic su **OK**. 
  
1. Nella sezione **Salva** della barra multifunzione del **flusso di lavoro** Selezionare **pubblica**. 
  
2. Nella sezione **Gestisci** della barra multifunzione del **flusso di lavoro** Selezionare **pubblica globalmente**. Nella finestra di dialogo di conferma che viene visualizzata, selezionare **OK**. 
  
3. In un Web browser individuare il sito Web radice della raccolta siti e quindi accedere alle **funzionalità di raccolta siti** **delle impostazioni** \> del sito. Attiva/disattiva la caratteristica **flussi di lavoro** : 
  
· Se la funzionalità è *attivata* , fare clic su Disattiva **e quindi** su **attiva**. 
  
· Se la funzionalità è *disattivata* , fare clic su **attiva**. 
  
Per ulteriori informazioni, vedere l' [articolo](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)seguente.
  

