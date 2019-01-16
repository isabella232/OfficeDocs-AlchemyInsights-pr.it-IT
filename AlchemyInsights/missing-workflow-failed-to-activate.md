---
title: Mancanti del flusso di lavoro non riuscito per l'attivazione
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 33b92c2cae1f641b0cd88c82fd4ae5e8632d76c2
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/15/2019
ms.locfileid: "28296870"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="5de33-102">Mancanti del flusso di lavoro non riuscito per l'attivazione</span><span class="sxs-lookup"><span data-stu-id="5de33-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="5de33-103">In una raccolta siti di Microsoft SharePoint, è possibile aggiungere un flusso di lavoro riutilizzabile globalmente (ad esempio "approvazione - SharePoint 2010") per un elenco o raccolta.</span><span class="sxs-lookup"><span data-stu-id="5de33-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="5de33-104">Per risolvere questo problema, eseguire la procedura seguente:</span><span class="sxs-lookup"><span data-stu-id="5de33-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="5de33-105">Aprire il sito Web principale della raccolta siti in SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="5de33-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="5de33-106">In **Oggetti dei siti**, selezionare **i flussi di lavoro**.</span><span class="sxs-lookup"><span data-stu-id="5de33-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="5de33-107">Nella sezione **Nuovo** della barra multifunzione di **flussi di lavoro** , selezionare **Flusso di lavoro riutilizzabile**.</span><span class="sxs-lookup"><span data-stu-id="5de33-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="5de33-p101">Nella maschera **Crea flusso di lavoro riutilizzabile** , immettere il nome \* \* *Repair2010* \* \*. Per **Tipo di piattaforma**, fare clic su **Flusso di lavoro di SharePoint 2010**e quindi fare clic su **OK**.</span><span class="sxs-lookup"><span data-stu-id="5de33-p101">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*. For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="5de33-110">Nella sezione **Salva** della barra multifunzione di **flusso di lavoro** , selezionare **pubblica**.</span><span class="sxs-lookup"><span data-stu-id="5de33-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="5de33-p102">Nella sezione **Gestisci** della barra multifunzione di **flusso di lavoro** , selezionare **La pubblicazione a livello globale**. Nella finestra di conferma visualizzata scegliere **OK**.</span><span class="sxs-lookup"><span data-stu-id="5de33-p102">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**. In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="5de33-p103">In un web browser, individuare il sito Web principale della raccolta siti e quindi accedere **Alle impostazioni di sito** \> **Caratteristiche raccolta siti**. Quindi, attivare o disattivare la caratteristica **dei flussi di lavoro** :</span><span class="sxs-lookup"><span data-stu-id="5de33-p103">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**. Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="5de33-115">· Se la caratteristica è *attivata* , fare clic su **Disattiva** e quindi fare clic su **Attiva**.</span><span class="sxs-lookup"><span data-stu-id="5de33-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="5de33-116">· Se la caratteristica è *disattivata* , fare clic su **Attiva**.</span><span class="sxs-lookup"><span data-stu-id="5de33-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="5de33-117">Per ulteriori informazioni, consultare l' [articolo](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)seguente.</span><span class="sxs-lookup"><span data-stu-id="5de33-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

