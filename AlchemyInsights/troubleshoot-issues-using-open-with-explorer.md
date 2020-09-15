---
title: Risoluzione dei problemi relativi all'utilizzo di Open con Esplora risorse
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
ms.openlocfilehash: e7fe59b94d216d89c2f2f7100a3d8bf7a0b0196e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47659062"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="b5fa6-102">Risolvere i problemi relativi all'apertura con Esplora risorse</span><span class="sxs-lookup"><span data-stu-id="b5fa6-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="b5fa6-103">Risolvere i problemi comuni relativi all'apertura di una raccolta documenti in SharePoint o OneDrive tramite il comando **Apri con Esplora risorse** :</span><span class="sxs-lookup"><span data-stu-id="b5fa6-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="b5fa6-104">Utilizzare Internet Explorer 10 o Internet Explorer 11.</span><span class="sxs-lookup"><span data-stu-id="b5fa6-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="b5fa6-105">**Apri con Esplora risorse** non è compatibile con Microsoft Edge, Google Chrome, Firefox e altri.</span><span class="sxs-lookup"><span data-stu-id="b5fa6-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="b5fa6-106">**Apri con Esplora risorse** è disabilitato in tutti i browser tranne Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="b5fa6-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="b5fa6-107">**Apri con Esplora risorse** non è disponibile nell'esperienza moderna per le raccolte di SharePoint.</span><span class="sxs-lookup"><span data-stu-id="b5fa6-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="b5fa6-108">Utilizzare invece la **visualizzazione in Esplora file** .</span><span class="sxs-lookup"><span data-stu-id="b5fa6-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="b5fa6-109">Selezionare Visualizza **Opzioni** visualizzazione \> **in Esplora file**.</span><span class="sxs-lookup"><span data-stu-id="b5fa6-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="b5fa6-110">La visualizzazione in Esplora file non è compatibile con Microsoft Edge, Google Chrome, Firefox e altri.</span><span class="sxs-lookup"><span data-stu-id="b5fa6-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="b5fa6-111">**Visualizza in Esplora file** in disponibile solo in Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="b5fa6-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="b5fa6-112">Verificare che il servizio WebClient sia in esecuzione.</span><span class="sxs-lookup"><span data-stu-id="b5fa6-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="b5fa6-113">Nella casella di ricerca di Windows, digitare Run, selezionare l'app desktop Run, digitare Services. msc, quindi premere INVIO.</span><span class="sxs-lookup"><span data-stu-id="b5fa6-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="b5fa6-114">Scorrere verso il basso fino al servizio WebClient e verificare che nella colonna **stato** venga visualizzato il messaggio "Running".</span><span class="sxs-lookup"><span data-stu-id="b5fa6-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="b5fa6-115">In caso contrario, fare doppio clic sul servizio, fare clic sul pulsante **Start**e quindi fare clic su **OK**.</span><span class="sxs-lookup"><span data-stu-id="b5fa6-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="b5fa6-116">Potrebbe essere necessario abilitare prima il servizio selezionando **manuale** o **automatico** nella casella **tipo di avvio** .</span><span class="sxs-lookup"><span data-stu-id="b5fa6-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="b5fa6-117">L'apertura di una raccolta in Esplora file è utile se è necessario copiare o spostare più file e cartelle una sola volta, ma se si desidera lavorare regolarmente nella raccolta, è consigliabile sincronizzarla.</span><span class="sxs-lookup"><span data-stu-id="b5fa6-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="b5fa6-118">Per risolvere i problemi relativi all'apertura in Esplora file, vedere [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="b5fa6-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="b5fa6-119">Per informazioni su come configurare la sincronizzazione, vedere [sincronizzare i file di SharePoint con il nuovo client di sincronizzazione di OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="b5fa6-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="b5fa6-120">Per ulteriori informazioni, vedere l'articolo su [come utilizzare il comando "Apri con Esplora risorse" per risolvere i problemi in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) .</span><span class="sxs-lookup"><span data-stu-id="b5fa6-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span> 
  

