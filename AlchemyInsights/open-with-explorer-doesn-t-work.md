---
title: Apri con Esplora non funziona
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: b55fc7bd5670e655334ef7be368b245c8899633a
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/24/2019
ms.locfileid: "29475381"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="1f994-102">Apri con Esplora non funziona</span><span class="sxs-lookup"><span data-stu-id="1f994-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="1f994-p101">Se non funziona **Apri con Esplora risorse** o in **visualizzazione in Esplora File** verificare che il servizio Web client è impostato su **in esecuzione** eseguendo la procedura seguente. Ad esempio, può richiedere molto tempo per aprire una raccolta SharePoint o OneDrive quando il servizio non è in esecuzione.</span><span class="sxs-lookup"><span data-stu-id="1f994-p101">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below. For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="1f994-105">Nella casella di ricerca di Windows, tipo eseguita, selezionare l'app desktop Esegui, digitare Services. msc e quindi selezionare **INVIO**.</span><span class="sxs-lookup"><span data-stu-id="1f994-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="1f994-p102">Scorrere verso il basso per il servizio Web client e controllare la colonna **stato** . Se lo stato del servizio WebClient non è **in esecuzione**, fare doppio clic sul servizio, fare clic su **Start**e quindi fare clic su **OK**. Abilitare il servizio, se necessario, tramite la selezione nella casella **tipo avvio** **manuale** o **automatico** .</span><span class="sxs-lookup"><span data-stu-id="1f994-p102">Scroll down to the WebClient service and check the **Status** column. If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**. Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="1f994-p103">Per risolvere i problemi aprire Esplora File, vedere [Open nell'elenco cartelle](https://go.microsoft.com/fwlink/?linkid=871665). Esplorazione di sincronizzazione come un'alternativa migliore: [file di sincronizzazione di SharePoint con il nuovo client di sincronizzazione OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="1f994-p103">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

