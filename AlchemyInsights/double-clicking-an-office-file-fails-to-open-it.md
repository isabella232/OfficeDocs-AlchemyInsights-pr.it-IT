---
title: Se si fa doppio clic su un file di Office, non è possibile aprirlo
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2200002"
- "161"
ms.openlocfilehash: b9c563f7dd099bf3bad9018f69e2096816dd7290
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814809"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a><span data-ttu-id="a2283-102">Se si fa doppio clic su un file di Office, non è possibile aprirlo</span><span class="sxs-lookup"><span data-stu-id="a2283-102">Double-clicking an Office file fails to open it</span></span>

<span data-ttu-id="a2283-103">Dopo aver fatto doppio clic su un file di Office, è possibile che il programma venga aperto, ma il file stesso non si apre.</span><span class="sxs-lookup"><span data-stu-id="a2283-103">After double-clicking an Office file, you may see the program open but the file itself doesn't open.</span></span> <span data-ttu-id="a2283-104">In caso di errore: "Si è verificato un problema durante l'invio del comando al programma".</span><span class="sxs-lookup"><span data-stu-id="a2283-104">Or you may get the error: "There was a problem sending the command to the program."</span></span> <span data-ttu-id="a2283-105">Esistono molte cause, ma le due soluzioni più comuni sono:</span><span class="sxs-lookup"><span data-stu-id="a2283-105">There are many causes for this, but the two most common solutions are:</span></span>

- <span data-ttu-id="a2283-106">Dall'interno di Excel, verificare che l'opzione DDE sia deselezionata.</span><span class="sxs-lookup"><span data-stu-id="a2283-106">From within Excel, ensure that the DDE option is unchecked.</span></span> <span data-ttu-id="a2283-107">L'opzione è disponibile creando una nuova cartella di lavoro e scegliendo File **> Opzioni > Avanzate**.</span><span class="sxs-lookup"><span data-stu-id="a2283-107">The option can be found by creating a new workbook and then choosing **File > Options > Advanced**.</span></span> <span data-ttu-id="a2283-108">Nella sezione **Generale** deselezionare la casella di controllo Ignora altre applicazioni che **utilizzano DDE (Dynamic Data Exchange).**</span><span class="sxs-lookup"><span data-stu-id="a2283-108">In the **General** section, uncheck the **Ignore other applications that use Dynamic Data Exchange (DDE)**.</span></span>

- <span data-ttu-id="a2283-109">Eseguire un ripristino online per ripristinare le impostazioni predefinite.</span><span class="sxs-lookup"><span data-stu-id="a2283-109">Run an Online Repair to restore default settings.</span></span> <span data-ttu-id="a2283-110">Fai clic sul pulsante Start di Windows e cerca "Pannello di controllo".</span><span class="sxs-lookup"><span data-stu-id="a2283-110">Click the Windows Start button and search for "Control Panel."</span></span> <span data-ttu-id="a2283-111">Aprire il **Pannello di** controllo e passare a Programmi > Programmi **e funzionalità**.</span><span class="sxs-lookup"><span data-stu-id="a2283-111">Open the **Control Panel**, and go to **Programs > Programs and Features**.</span></span> <span data-ttu-id="a2283-112">Fare quindi clic con il **Microsoft Office destro del mouse su [Versione]** e scegliere Cambia > Ripristino **online**.</span><span class="sxs-lookup"><span data-stu-id="a2283-112">Then right-click **Microsoft Office [Version]** and choose **Change > Online Repair**.</span></span>

<span data-ttu-id="a2283-113">Se nessuna di queste soluzioni funziona, nell'articolo del supporto è disponibile un elenco più completo delle soluzioni, facendo doppio clic su un file di Office non è possibile [aprirlo.](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6)</span><span class="sxs-lookup"><span data-stu-id="a2283-113">If neither of these solutions work, a more complete list of solutions can be found in the support article, [Double-clicking an Office file fails to open it](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).</span></span>
