---
title: Il grafico mostra un numero diverso di record nella griglia
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5611"
- "9002930"
ms.openlocfilehash: e499a439e7cf7e9ecbb6566f9f089f3b7b82f48e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47793762"
---
# <a name="chart-shows-different-number-of-records-in-grid"></a><span data-ttu-id="840b2-102">Il grafico mostra un numero diverso di record nella griglia</span><span class="sxs-lookup"><span data-stu-id="840b2-102">Chart shows different number of records in grid</span></span>

<span data-ttu-id="840b2-103">**Sintomo**</span><span class="sxs-lookup"><span data-stu-id="840b2-103">**Symptom**</span></span>

<span data-ttu-id="840b2-104">Per il grafico nella pagina del dashboard, quando si fa clic sul grafico "..." e su "Visualizza record", si passa alla pagina della griglia per visualizzare tutti i record. A volte il numero di record cambia.</span><span class="sxs-lookup"><span data-stu-id="840b2-104">For chart on dashboard page, when you click on chart "…" and click "View records", you navigate to grid page to see all the records.Sometimes, the number of records changes.</span></span>

<span data-ttu-id="840b2-105">**Causa**</span><span class="sxs-lookup"><span data-stu-id="840b2-105">**Cause**</span></span>

<span data-ttu-id="840b2-106">Ciò è dovuto alle diverse visualizzazioni tra il grafico nella pagina del dashboard originale e il grafico nella griglia della home page.</span><span class="sxs-lookup"><span data-stu-id="840b2-106">This is due to the difference of views between the chart on the original dashboard page and the chart on the grid home page.</span></span>  

<span data-ttu-id="840b2-107">**Soluzione**</span><span class="sxs-lookup"><span data-stu-id="840b2-107">**Solution**</span></span>

1. <span data-ttu-id="840b2-108">Controllare la visualizzazione dalla pagina originale e quella nella griglia per vedere se sono diverse.</span><span class="sxs-lookup"><span data-stu-id="840b2-108">Check the view from the original page and the view in the grid to see if they are different.</span></span>
2. <span data-ttu-id="840b2-109">Cambiare la visualizzazione nella griglia in modo che corrisponda alla visualizzazione nella pagina originale.</span><span class="sxs-lookup"><span data-stu-id="840b2-109">Change the view in grid to match the view in the original page.</span></span>
3. <span data-ttu-id="840b2-110">Se non è possibile trovare la visualizzazione corretta, in genere significa che la visualizzazione non è abilitata nella progettazione app.</span><span class="sxs-lookup"><span data-stu-id="840b2-110">If the correct view cannot be found, usually it means the view is not enabled in app designer.</span></span>
4. <span data-ttu-id="840b2-111">Passare alla progettazione app dell'app specifica, scegliere l'entità e le relative visualizzazioni, selezionare la visualizzazione che si desidera abilitare, salvare, pubblicare e chiudere.</span><span class="sxs-lookup"><span data-stu-id="840b2-111">Go to app designer of the specific app, choose the entity and its views, check the view you want to enable, save, publish and close.</span></span>
5. <span data-ttu-id="840b2-112">Aggiornare la pagina.</span><span class="sxs-lookup"><span data-stu-id="840b2-112">Refresh the page.</span></span>