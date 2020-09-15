---
title: Impossibile aggiungere il flusso di lavoro di approvazione 2010
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: aa61f1615b60d27cffad15f02f6ce5dbac1b607f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47699739"
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
  
3. In un Web browser individuare il sito Web radice della raccolta siti e quindi accedere alle **Site Settings** \> **funzionalità di raccolta siti**delle impostazioni del sito. Attiva/disattiva la caratteristica **flussi di lavoro** : 
  
· Se la funzionalità è  *attivata*  , fare clic su Disattiva **e quindi** su **attiva**. 
  
· Se la funzionalità è  *disattivata*  , fare clic su **attiva**. 
  
Per ulteriori informazioni, vedere l' [articolo](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)seguente.
  

