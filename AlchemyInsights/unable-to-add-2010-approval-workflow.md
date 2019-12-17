---
title: Impossibile aggiungere il flusso di lavoro di approvazione 2010
ms.author: pebaum
author: pebaum
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: 11ba9bf04f826b0d7465a9a81a36c327e79f4d13
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049557"
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
  

