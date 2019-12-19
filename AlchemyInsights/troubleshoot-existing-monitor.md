---
title: Risoluzione dei problemi relativi al monitor esistente
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: d90baddd01bdf8508bd6289509c8399b8241887a
ms.sourcegitcommit: 42463e8d8869f36225a27388d83d37629c6b149e
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/18/2019
ms.locfileid: "40738573"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="adfe8-102">Risoluzione dei problemi di un monitor esistente</span><span class="sxs-lookup"><span data-stu-id="adfe8-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="adfe8-103">Provare queste soluzioni per la risoluzione dei problemi relativi a un monitor.</span><span class="sxs-lookup"><span data-stu-id="adfe8-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="adfe8-104">**Aggiornare la visualizzazione del monitor:**</span><span class="sxs-lookup"><span data-stu-id="adfe8-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="adfe8-105">Premere contemporaneamente i tasti seguenti: tasto Windows + CTRL + MAIUSC + B. In questo modo verrà aggiornata la comunicazione con il driver di grafica.</span><span class="sxs-lookup"><span data-stu-id="adfe8-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="adfe8-106">I monitor lampeggeranno momentaneamente e torneranno dopo alcuni secondi.</span><span class="sxs-lookup"><span data-stu-id="adfe8-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="adfe8-107">**Risoluzione dei problemi relativi all'hardware:**</span><span class="sxs-lookup"><span data-stu-id="adfe8-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="adfe8-108">Scollegare il cavo che collega il PC al monitor e ricollegarlo.</span><span class="sxs-lookup"><span data-stu-id="adfe8-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="adfe8-109">Scollegare tutti i dispositivi non essenziali dal PC (ad esempio, adattatori o dock).</span><span class="sxs-lookup"><span data-stu-id="adfe8-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="adfe8-110">**Se è stato installato di recente un aggiornamento sul PC, è possibile eseguire il rollback del driver dello schermo:**</span><span class="sxs-lookup"><span data-stu-id="adfe8-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="adfe8-111">Fare clic su **Start**, digitare **Gestione dispositivi**e selezionare **Gestione dispositivi** dai risultati.</span><span class="sxs-lookup"><span data-stu-id="adfe8-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="adfe8-112">Espandere la sezione **adattatori visualizzazione** , fare clic con il pulsante destro del mouse sulla scheda video, scegliere **Proprietà**.</span><span class="sxs-lookup"><span data-stu-id="adfe8-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="adfe8-113">Passare alla scheda **driver** e selezionare Ripristina **driver**.</span><span class="sxs-lookup"><span data-stu-id="adfe8-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="adfe8-114">Nota: se questa opzione non è disponibile o è disabilitata, selezionare **No** dalle opzioni seguenti per passare al passaggio successivo.</span><span class="sxs-lookup"><span data-stu-id="adfe8-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="adfe8-115">Potrebbe essere necessario riavviare il PC prima che queste modifiche abbiano effetto.</span><span class="sxs-lookup"><span data-stu-id="adfe8-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="adfe8-116">**Disinstallare e reinstallare il driver di visualizzazione:**</span><span class="sxs-lookup"><span data-stu-id="adfe8-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="adfe8-117">Fare clic su **Start**, digitare **Gestione dispositivi**e selezionare **Gestione dispositivi** dai risultati.</span><span class="sxs-lookup"><span data-stu-id="adfe8-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="adfe8-118">Espandere la sezione **adattatori visualizzazione** , fare clic con il pulsante destro del mouse sulla scheda video e scegliere **Disinstalla dispositivo**.</span><span class="sxs-lookup"><span data-stu-id="adfe8-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="adfe8-119">Selezionare la casella accanto a **Elimina il software del driver per il dispositivo** e selezionare **Disinstalla**.</span><span class="sxs-lookup"><span data-stu-id="adfe8-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="adfe8-120">Nota: è possibile che venga richiesto di riavviare il computer in questa fase.</span><span class="sxs-lookup"><span data-stu-id="adfe8-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="adfe8-121">Assicurarsi di annotare le istruzioni rimanenti prima del riavvio.</span><span class="sxs-lookup"><span data-stu-id="adfe8-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="adfe8-122">Aprire di nuovo gestione dispositivi.</span><span class="sxs-lookup"><span data-stu-id="adfe8-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="adfe8-123">Espandere la sezione **adattatori visualizzazione** , fare clic con il pulsante destro del mouse sulla scheda video e selezionare **Aggiorna driver**.</span><span class="sxs-lookup"><span data-stu-id="adfe8-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="adfe8-124">Selezionare **Cerca automaticamente per aggiornare il software del driver** e seguire le istruzioni per l'installazione.</span><span class="sxs-lookup"><span data-stu-id="adfe8-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>