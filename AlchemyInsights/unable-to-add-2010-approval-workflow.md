---
title: Impossibile aggiungere flusso di lavoro approvazione 2010
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: a83a9621ca0f7764d3f2c0a698dbffd80d55e80c
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/15/2019
ms.locfileid: "28297011"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="f71a2-102">Impossibile aggiungere flusso di lavoro approvazione 2010</span><span class="sxs-lookup"><span data-stu-id="f71a2-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="f71a2-103">In una raccolta siti di Microsoft SharePoint, è possibile aggiungere un flusso di lavoro riutilizzabile globalmente (ad esempio "approvazione - SharePoint 2010") per un elenco o raccolta.</span><span class="sxs-lookup"><span data-stu-id="f71a2-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="f71a2-104">Per risolvere questo problema, eseguire la procedura seguente:</span><span class="sxs-lookup"><span data-stu-id="f71a2-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="f71a2-105">Aprire il sito Web principale della raccolta siti in SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="f71a2-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="f71a2-106">In **Oggetti dei siti**, selezionare **i flussi di lavoro**.</span><span class="sxs-lookup"><span data-stu-id="f71a2-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="f71a2-107">Nella sezione **Nuovo** della barra multifunzione di **flussi di lavoro** , selezionare **Flusso di lavoro riutilizzabile**.</span><span class="sxs-lookup"><span data-stu-id="f71a2-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="f71a2-p101">Nella maschera **Crea flusso di lavoro riutilizzabile** , immettere il nome \* \* *Repair2010* \* \*. Per **Tipo di piattaforma**, fare clic su **Flusso di lavoro di SharePoint 2010**e quindi fare clic su **OK**.</span><span class="sxs-lookup"><span data-stu-id="f71a2-p101">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*. For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="f71a2-110">Nella sezione **Salva** della barra multifunzione di **flusso di lavoro** , selezionare **pubblica**.</span><span class="sxs-lookup"><span data-stu-id="f71a2-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="f71a2-p102">Nella sezione **Gestisci** della barra multifunzione di **flusso di lavoro** , selezionare **La pubblicazione a livello globale**. Nella finestra di conferma visualizzata scegliere **OK**.</span><span class="sxs-lookup"><span data-stu-id="f71a2-p102">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**. In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="f71a2-p103">In un web browser, individuare il sito Web principale della raccolta siti e quindi accedere **Alle impostazioni di sito** \> **Caratteristiche raccolta siti**. Attivare o disattivare la caratteristica **dei flussi di lavoro** :</span><span class="sxs-lookup"><span data-stu-id="f71a2-p103">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**. Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="f71a2-115">· Se la caratteristica è *attivata* , fare clic su **Disattiva** e quindi fare clic su **Attiva**.</span><span class="sxs-lookup"><span data-stu-id="f71a2-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="f71a2-116">· Se la caratteristica è *disattivata* , fare clic su **Attiva**.</span><span class="sxs-lookup"><span data-stu-id="f71a2-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="f71a2-117">Per ulteriori informazioni, consultare l' [articolo](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)seguente.</span><span class="sxs-lookup"><span data-stu-id="f71a2-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

