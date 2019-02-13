---
title: Mancanti del flusso di lavoro non riuscito per l'attivazione
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: ce088227a3206fa05b99331fdb022fbe4886203f
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 02/12/2019
ms.locfileid: "29917572"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="6f6ad-102">Mancanti del flusso di lavoro non riuscito per l'attivazione</span><span class="sxs-lookup"><span data-stu-id="6f6ad-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="6f6ad-103">In una raccolta siti di Microsoft SharePoint, è possibile aggiungere un flusso di lavoro riutilizzabile globalmente (ad esempio "approvazione - SharePoint 2010") per un elenco o raccolta.</span><span class="sxs-lookup"><span data-stu-id="6f6ad-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="6f6ad-104">Per risolvere questo problema, eseguire la procedura seguente:</span><span class="sxs-lookup"><span data-stu-id="6f6ad-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="6f6ad-105">Aprire il sito Web principale della raccolta siti in SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="6f6ad-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="6f6ad-106">In **Oggetti dei siti**, selezionare **i flussi di lavoro**.</span><span class="sxs-lookup"><span data-stu-id="6f6ad-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="6f6ad-107">Nella sezione **Nuovo** della barra multifunzione di **flussi di lavoro** , selezionare **Flusso di lavoro riutilizzabile**.</span><span class="sxs-lookup"><span data-stu-id="6f6ad-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="6f6ad-p101">Nella maschera **Crea flusso di lavoro riutilizzabile** , immettere il nome \* \* *Repair2010* \* \*. Per **Tipo di piattaforma**, fare clic su **Flusso di lavoro di SharePoint 2010**e quindi fare clic su **OK**.</span><span class="sxs-lookup"><span data-stu-id="6f6ad-p101">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*. For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="6f6ad-110">Nella sezione **Salva** della barra multifunzione di **flusso di lavoro** , selezionare **pubblica**.</span><span class="sxs-lookup"><span data-stu-id="6f6ad-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="6f6ad-p102">Nella sezione **Gestisci** della barra multifunzione di **flusso di lavoro** , selezionare **La pubblicazione a livello globale**. Nella finestra di conferma visualizzata scegliere **OK**.</span><span class="sxs-lookup"><span data-stu-id="6f6ad-p102">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**. In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="6f6ad-p103">In un web browser, individuare il sito Web principale della raccolta siti e quindi accedere **Alle impostazioni di sito** \> **Caratteristiche raccolta siti**. Quindi, attivare o disattivare la caratteristica **dei flussi di lavoro** :</span><span class="sxs-lookup"><span data-stu-id="6f6ad-p103">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**. Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="6f6ad-115">· Se la caratteristica è *attivata* , fare clic su **Disattiva** e quindi fare clic su **Attiva**.</span><span class="sxs-lookup"><span data-stu-id="6f6ad-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="6f6ad-116">· Se la caratteristica è *disattivata* , fare clic su **Attiva**.</span><span class="sxs-lookup"><span data-stu-id="6f6ad-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="6f6ad-117">Per ulteriori informazioni, consultare l' [articolo](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)seguente.</span><span class="sxs-lookup"><span data-stu-id="6f6ad-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

