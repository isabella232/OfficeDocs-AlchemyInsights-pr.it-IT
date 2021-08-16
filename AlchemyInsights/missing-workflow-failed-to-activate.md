---
title: Impossibile attivare il flusso di lavoro mancante
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: d703e87f355f05bf4a1d71e5daddce96db988380bb48accc81c95f1ba91fbb2b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54065432"
---
# <a name="missing-workflow-failed-to-activate"></a>Impossibile attivare il flusso di lavoro mancante

In una raccolta siti di Microsoft SharePoint, non è possibile aggiungere un flusso di lavoro riutilizzabile a livello globale (ad esempio "Approvazione - SharePoint 2010") a un elenco o a una raccolta.
  
Per risolvere il problema, attenersi alla seguente procedura: 
  
1. Aprire il sito Web radice della raccolta siti in SharePoint Designer 2013.
  
2. In **Oggetti sito** selezionare Flussi di **lavoro.** 
  
3. Nella sezione **Nuovo** della barra multifunzione **Flussi di** lavoro selezionare Flusso di **lavoro riutilizzabile.** 
  
4. Nel modulo **Crea flusso di lavoro riutilizzabile** immettere il nome ** *Repair2010* **. In **Tipo di piattaforma** fare clic SharePoint flusso di lavoro **2010** e quindi fare clic su **OK.** 
  
1. Nella sezione **Salva** della barra **multifunzione flusso di** lavoro selezionare **Pubblica.** 
  
2. Nella sezione **Gestisci** della barra **multifunzione flusso di** lavoro selezionare Pubblica **globalmente.** Nella finestra di dialogo di conferma visualizzata selezionare **OK.** 
  
3. In un Web browser individuare il sito Web radice della raccolta siti e quindi accedere a Caratteristiche raccolta **siti** Impostazioni \> **sito**. Attivare e disattivare quindi **la funzionalità Flussi di** lavoro: 
  
· Se la funzionalità è *attivata,* fare clic **su Disattiva e** quindi su **Attiva.** 
  
· Se la funzionalità è *disattivata, fare* clic su **Attiva.** 
  
Per ulteriori informazioni, fare riferimento all'articolo [seguente.](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)
  

