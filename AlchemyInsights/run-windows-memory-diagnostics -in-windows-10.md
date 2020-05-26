---
title: Eseguire diagnostica memoria Windows in Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: 3fedc52d02f1f70743429d0313eda0361306c3f3
ms.sourcegitcommit: 18b080c2a5d741af01ec589158effc35ea7cf449
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2020
ms.locfileid: "44289782"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a><span data-ttu-id="d7d7f-102">Eseguire diagnostica memoria Windows in Windows 10</span><span class="sxs-lookup"><span data-stu-id="d7d7f-102">Run Windows Memory Diagnostics in Windows 10</span></span>

<span data-ttu-id="d7d7f-103">Se Windows e le app nel PC si arrestano all'improvviso, si bloccano o si comportano in modo instabile, potrebbe esserci un problema con la memoria del PC.</span><span class="sxs-lookup"><span data-stu-id="d7d7f-103">If Windows and apps on your PC are crashing, freezing, or acting in an unstable manner, you may have a problem with the PC’s memory (RAM).</span></span> <span data-ttu-id="d7d7f-104">È possibile eseguire diagnostica memoria Windows per verificare se sono presenti problemi con la RAM del PC.</span><span class="sxs-lookup"><span data-stu-id="d7d7f-104">You can run the Windows Memory Diagnostic to check for problems with the PC’s RAM.</span></span>

<span data-ttu-id="d7d7f-105">Nella casella di ricerca della barra delle applicazioni digitare **diagnostica memoria**, quindi selezionare **Diagnostica memoria Windows**.</span><span class="sxs-lookup"><span data-stu-id="d7d7f-105">In the search box on your taskbar, type **memory diagnostic**, and then select **Windows Memory Diagnostic**.</span></span> 

<span data-ttu-id="d7d7f-106">Per eseguire la diagnostica, è necessario riavviare il PC.</span><span class="sxs-lookup"><span data-stu-id="d7d7f-106">To run the diagnostic, the PC needs to restart.</span></span> <span data-ttu-id="d7d7f-107">È possibile riavviarlo immediatamente (salvare il lavoro e chiudere i documenti aperti e i messaggi di posta elettronica prima) o pianificare la diagnostica da eseguire automaticamente al successivo riavvio del PC:</span><span class="sxs-lookup"><span data-stu-id="d7d7f-107">You have the option to restart immediately (please save your work and close open documents and e-mails first), or schedule the diagnostic to run automatically the next time the PC restarts:</span></span>

![Diagnostica memoria Windows](media/windows-memory-diagnostic.png)

<span data-ttu-id="d7d7f-109">Quando il PC si riavvia, lo **Strumento di diagnostica memoria Windows** verrà eseguito automaticamente.</span><span class="sxs-lookup"><span data-stu-id="d7d7f-109">When the PC restarts, the **Windows Memory Diagnostics Tool** will run automatically.</span></span> <span data-ttu-id="d7d7f-110">Durante l'esecuzione della diagnostica verranno mostrato lo stato e l'avanzamento e sarà possibile annullare la diagnostica premendo il tasto **ESC** sulla tastiera.</span><span class="sxs-lookup"><span data-stu-id="d7d7f-110">Status and progress will be displayed as the diagnostics run, and you have the option of cancelling the diagnostics by hitting the **ESC** key on your keyboard.</span></span>

<span data-ttu-id="d7d7f-111">Quando la diagnostica è completata, Windows si avvierà normalmente.</span><span class="sxs-lookup"><span data-stu-id="d7d7f-111">When the diagnostics are complete, Windows will start normally.</span></span>
<span data-ttu-id="d7d7f-112">Subito dopo il riavvio, quando viene visualizzato il desktop, sarà visibile una notifica (accanto all'icona del **centro notifiche** nella barra delle applicazioni) che indica se sono stati trovati errori di memoria.</span><span class="sxs-lookup"><span data-stu-id="d7d7f-112">Immediately after restart, when the Desktop appears, a notification will appear (next to the **Action Center** icon on the taskbar), to indicate whether any memory errors were found.</span></span> <span data-ttu-id="d7d7f-113">Ad esempio:</span><span class="sxs-lookup"><span data-stu-id="d7d7f-113">For example:</span></span>

<span data-ttu-id="d7d7f-114">Ecco l'icona del centro notifiche:</span><span class="sxs-lookup"><span data-stu-id="d7d7f-114">Here's the Action Center icon:</span></span> ![Icona del centro notifiche](media/action-center-icon.png) 

<span data-ttu-id="d7d7f-116">Ecco una notifica esemplificativa:</span><span class="sxs-lookup"><span data-stu-id="d7d7f-116">And a sample notification:</span></span> ![Nessun errore di memoria](media/no-memory-errors.png)

<span data-ttu-id="d7d7f-118">Se non è visibile alcuna notifica, è possibile selezionare l'icona del **centro notifiche** nella barra delle applicazioni per visualizzare il **centro notifiche** e vedere un elenco di notifiche scorrevole.</span><span class="sxs-lookup"><span data-stu-id="d7d7f-118">If you missed the notification, you can select the **Action Center** icon  on the taskbar to display the **Action Center** and see a scrollable list of notifications.</span></span>

<span data-ttu-id="d7d7f-119">Per rivedere le informazioni dettagliate, digitare **evento** nella casella di ricerca della barra delle applicazioni, quindi selezionare **Visualizzatore eventi**.</span><span class="sxs-lookup"><span data-stu-id="d7d7f-119">To review detailed information, type **event** into the search box on your taskbar, and then select **Event Viewer**.</span></span> <span data-ttu-id="d7d7f-120">Nel riquadro sinistro di **Visualizzatore eventi** passare a **Log di Windows > Sistema**.</span><span class="sxs-lookup"><span data-stu-id="d7d7f-120">In the **Event Viewer**’s left-hand pane, navigate to **Windows Logs > System**.</span></span> <span data-ttu-id="d7d7f-121">Nel riquadro destro scorrere l'elenco verso il basso esaminando la colonna **Origine** finché non vengono visualizzati gli eventi con il valore di origine **MemoryDiagnostics-Results**.</span><span class="sxs-lookup"><span data-stu-id="d7d7f-121">In the right-hand pane, scan down the list while looking at the **Source** column, until you see events with Source value **MemoryDiagnostics-Results**.</span></span> <span data-ttu-id="d7d7f-122">Evidenziare ogni evento di questo tipo e consultare le informazioni relative ai risultati nella casella nella scheda **Generale** sotto l'elenco.</span><span class="sxs-lookup"><span data-stu-id="d7d7f-122">Highlight each such event and see the result information in the box under the **General** tab below the list.</span></span>
