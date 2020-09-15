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
ms.openlocfilehash: 604dc770c5c14ded6a8de1cec9e311b03b69f094
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667090"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="bbb5b-102">Impossibile attivare il flusso di lavoro mancante</span><span class="sxs-lookup"><span data-stu-id="bbb5b-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="bbb5b-103">In una raccolta siti di Microsoft SharePoint non è possibile aggiungere un flusso di lavoro riutilizzabile a livello globale, ad esempio "approvazione-SharePoint 2010", a un elenco o una raccolta.</span><span class="sxs-lookup"><span data-stu-id="bbb5b-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="bbb5b-104">Per risolvere il problema, attenersi alla seguente procedura:</span><span class="sxs-lookup"><span data-stu-id="bbb5b-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="bbb5b-105">Aprire il sito Web radice della raccolta siti in SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="bbb5b-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="bbb5b-106">In **oggetti sito**selezionare **flussi di lavoro**.</span><span class="sxs-lookup"><span data-stu-id="bbb5b-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="bbb5b-107">Nella **nuova** sezione della barra multifunzione **flussi di lavoro** , selezionare **flusso di lavoro riutilizzabile**.</span><span class="sxs-lookup"><span data-stu-id="bbb5b-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="bbb5b-108">Nel modulo **Crea flusso di lavoro riutilizzabile** , immettere il nome \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="bbb5b-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="bbb5b-109">Per il **tipo di piattaforma**, fare clic su flusso di lavoro di **SharePoint 2010**e quindi fare clic su **OK**.</span><span class="sxs-lookup"><span data-stu-id="bbb5b-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="bbb5b-110">Nella sezione **Salva** della barra multifunzione del **flusso di lavoro** Selezionare **pubblica**.</span><span class="sxs-lookup"><span data-stu-id="bbb5b-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="bbb5b-111">Nella sezione **Gestisci** della barra multifunzione del **flusso di lavoro** Selezionare **pubblica globalmente**.</span><span class="sxs-lookup"><span data-stu-id="bbb5b-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="bbb5b-112">Nella finestra di dialogo di conferma che viene visualizzata, selezionare **OK**.</span><span class="sxs-lookup"><span data-stu-id="bbb5b-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="bbb5b-113">In un Web browser individuare il sito Web radice della raccolta siti e quindi accedere alle **Site Settings** \> **funzionalità di raccolta siti**delle impostazioni del sito.</span><span class="sxs-lookup"><span data-stu-id="bbb5b-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="bbb5b-114">Passare quindi alla funzionalità **flussi di lavoro** :</span><span class="sxs-lookup"><span data-stu-id="bbb5b-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="bbb5b-115">· Se la funzionalità è  *attivata*  , fare clic su Disattiva **e quindi** su **attiva**.</span><span class="sxs-lookup"><span data-stu-id="bbb5b-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="bbb5b-116">· Se la funzionalità è  *disattivata*  , fare clic su **attiva**.</span><span class="sxs-lookup"><span data-stu-id="bbb5b-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="bbb5b-117">Per ulteriori informazioni, vedere l' [articolo](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)seguente.</span><span class="sxs-lookup"><span data-stu-id="bbb5b-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

