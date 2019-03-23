---
title: Apertura con Esplora risorse non funziona
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 73d33e50449345c312abdd39afcc36e0c95fd1c4
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/22/2019
ms.locfileid: "30764912"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="fb4e2-102">Apertura con Esplora risorse non funzionante</span><span class="sxs-lookup"><span data-stu-id="fb4e2-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="fb4e2-103">Se l' **apertura con Esplora risorse** o la **visualizzazione in Esplora file** non funziona, verificare che il servizio WebClient sia impostato su **in esecuzione** attenendosi alla procedura riportata di seguito.</span><span class="sxs-lookup"><span data-stu-id="fb4e2-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="fb4e2-104">Ad esempio, potrebbe richiedere molto tempo per aprire una raccolta di SharePoint o OneDrive quando il servizio non è in esecuzione.</span><span class="sxs-lookup"><span data-stu-id="fb4e2-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="fb4e2-105">Nella casella di ricerca di Windows, digitare Run, selezionare l'app desktop Run, digitare Services. msc, quindi selezionare **invio**.</span><span class="sxs-lookup"><span data-stu-id="fb4e2-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="fb4e2-106">Scorrere verso il basso fino al servizio webClient e controllare la colonna **stato** .</span><span class="sxs-lookup"><span data-stu-id="fb4e2-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="fb4e2-107">Se lo stato del servizio webClient non è **in esecuzione**, fare doppio clic sul servizio, fare clic sul pulsante **Start**e quindi fare clic su **OK**.</span><span class="sxs-lookup"><span data-stu-id="fb4e2-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="fb4e2-108">Abilitare il servizio, se necessario, selezionando **manuale** o **automatico** nella casella **tipo di avvio** .</span><span class="sxs-lookup"><span data-stu-id="fb4e2-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="fb4e2-109">Per risolvere i problemi relativi all'apertura in Esplora file, vedere [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="fb4e2-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="fb4e2-110">Esplorare la sincronizzazione come alternativa migliore: [sincronizzare i file di SharePoint con il nuovo client di sincronizzazione di OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="fb4e2-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

