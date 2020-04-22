---
title: Impossibile attivare il flusso di lavoro mancante
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 2598111005c219c398b63ca374e8e99348efc02c
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43762105"
---
# <a name="missing-workflow-failed-to-activate"></a>Impossibile attivare il flusso di lavoro mancante

In una raccolta siti di Microsoft SharePoint non è possibile aggiungere un flusso di lavoro riutilizzabile a livello globale, ad esempio "approvazione-SharePoint 2010", a un elenco o una raccolta.
  
Per risolvere il problema, attenersi alla seguente procedura: 
  
1. Aprire il sito Web radice della raccolta siti in SharePoint Designer 2013.
  
2. In **oggetti sito**selezionare **flussi di lavoro**. 
  
3. Nella **nuova** sezione della barra multifunzione **flussi di lavoro** , selezionare **flusso di lavoro riutilizzabile**. 
  
4. Nel modulo **Crea flusso di lavoro riutilizzabile** , immettere il nome * * *Repair2010* * *. Per il **tipo di piattaforma**, fare clic su flusso di lavoro di **SharePoint 2010**e quindi fare clic su **OK**. 
  
1. Nella sezione **Salva** della barra multifunzione del **flusso di lavoro** Selezionare **pubblica**. 
  
2. Nella sezione **Gestisci** della barra multifunzione del **flusso di lavoro** Selezionare **pubblica globalmente**. Nella finestra di dialogo di conferma che viene visualizzata, selezionare **OK**. 
  
3. In un Web browser individuare il sito Web radice della raccolta siti e quindi accedere alle **funzionalità di raccolta siti** **delle impostazioni** \> del sito. Passare quindi alla funzionalità **flussi di lavoro** : 
  
· Se la funzionalità è *attivata* , fare clic su Disattiva **e quindi** su **attiva**. 
  
· Se la funzionalità è *disattivata* , fare clic su **attiva**. 
  
Per ulteriori informazioni, vedere l' [articolo](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)seguente.
  

