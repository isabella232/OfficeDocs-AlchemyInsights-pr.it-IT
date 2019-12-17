---
title: Impossibile attivare il flusso di lavoro mancante
ms.author: pebaum
author: pebaum
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 3df1ddc1059c4cd6cc3f9f42dc157d20be79a63a
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052617"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="d5f8e-102">Impossibile attivare il flusso di lavoro mancante</span><span class="sxs-lookup"><span data-stu-id="d5f8e-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="d5f8e-103">In una raccolta siti di Microsoft SharePoint non è possibile aggiungere un flusso di lavoro riutilizzabile a livello globale, ad esempio "approvazione-SharePoint 2010", a un elenco o una raccolta.</span><span class="sxs-lookup"><span data-stu-id="d5f8e-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="d5f8e-104">Per risolvere il problema, attenersi alla seguente procedura:</span><span class="sxs-lookup"><span data-stu-id="d5f8e-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="d5f8e-105">Aprire il sito Web radice della raccolta siti in SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="d5f8e-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="d5f8e-106">In **oggetti sito**selezionare **flussi di lavoro**.</span><span class="sxs-lookup"><span data-stu-id="d5f8e-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="d5f8e-107">Nella **nuova** sezione della barra multifunzione **flussi di lavoro** , selezionare **flusso di lavoro riutilizzabile**.</span><span class="sxs-lookup"><span data-stu-id="d5f8e-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="d5f8e-108">Nel modulo **Crea flusso di lavoro riutilizzabile** , immettere il nome \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="d5f8e-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="d5f8e-109">Per il **tipo di piattaforma**, fare clic su flusso di lavoro di **SharePoint 2010**e quindi fare clic su **OK**.</span><span class="sxs-lookup"><span data-stu-id="d5f8e-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="d5f8e-110">Nella sezione **Salva** della barra multifunzione del **flusso di lavoro** Selezionare **pubblica**.</span><span class="sxs-lookup"><span data-stu-id="d5f8e-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="d5f8e-111">Nella sezione **Gestisci** della barra multifunzione del **flusso di lavoro** Selezionare **pubblica globalmente**.</span><span class="sxs-lookup"><span data-stu-id="d5f8e-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="d5f8e-112">Nella finestra di dialogo di conferma che viene visualizzata, selezionare **OK**.</span><span class="sxs-lookup"><span data-stu-id="d5f8e-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="d5f8e-113">In un Web browser individuare il sito Web radice della raccolta siti e quindi accedere alle **funzionalità di raccolta siti** **delle impostazioni** \> del sito.</span><span class="sxs-lookup"><span data-stu-id="d5f8e-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="d5f8e-114">Passare quindi alla funzionalità **flussi di lavoro** :</span><span class="sxs-lookup"><span data-stu-id="d5f8e-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="d5f8e-115">· Se la funzionalità è *attivata* , fare clic su Disattiva **e quindi** su **attiva**.</span><span class="sxs-lookup"><span data-stu-id="d5f8e-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="d5f8e-116">· Se la funzionalità è *disattivata* , fare clic su **attiva**.</span><span class="sxs-lookup"><span data-stu-id="d5f8e-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="d5f8e-117">Per ulteriori informazioni, vedere l' [articolo](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)seguente.</span><span class="sxs-lookup"><span data-stu-id="d5f8e-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

