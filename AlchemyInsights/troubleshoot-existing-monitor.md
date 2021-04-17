---
title: Risoluzione dei problemi del monitor esistente
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
- "3454"
- "9001450"
ms.openlocfilehash: c4d2bb64b6b5ea79d4cd585e2be85c3c17e0f76f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824583"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="ccaaf-102">Risolvere i problemi di un monitor esistente</span><span class="sxs-lookup"><span data-stu-id="ccaaf-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="ccaaf-103">Provare queste soluzioni per risolvere i problemi relativi a un monitor.</span><span class="sxs-lookup"><span data-stu-id="ccaaf-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="ccaaf-104">**Aggiornare lo schermo del monitor:**</span><span class="sxs-lookup"><span data-stu-id="ccaaf-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="ccaaf-105">Premere contemporaneamente i tasti seguenti: Tasto Windows + CTRL + MAIUSC + B. In questo modo verrà aggiornata la comunicazione con il driver di grafica.</span><span class="sxs-lookup"><span data-stu-id="ccaaf-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="ccaaf-106">I monitor lampeggiano momentaneamente e tornano dopo alcuni secondi.</span><span class="sxs-lookup"><span data-stu-id="ccaaf-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="ccaaf-107">**Risolvere i problemi relativi all'hardware di monitoraggio:**</span><span class="sxs-lookup"><span data-stu-id="ccaaf-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="ccaaf-108">Scollegare e ricollegare il cavo che collega il PC al monitor.</span><span class="sxs-lookup"><span data-stu-id="ccaaf-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="ccaaf-109">Disconnettere i dispositivi non essenziali dal PC (ad esempio adattatori o dock).</span><span class="sxs-lookup"><span data-stu-id="ccaaf-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="ccaaf-110">**Se hai installato di recente un aggiornamento nel PC, puoi eseguire il rollback del driver video:**</span><span class="sxs-lookup"><span data-stu-id="ccaaf-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="ccaaf-111">Seleziona **Start,** digita **Gestione dispositivi** e seleziona Gestione **dispositivi** dai risultati.</span><span class="sxs-lookup"><span data-stu-id="ccaaf-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="ccaaf-112">Espandere la **sezione Schede di visualizzazione,** fare clic con il pulsante destro del mouse sulla scheda di visualizzazione e scegliere **Proprietà.**</span><span class="sxs-lookup"><span data-stu-id="ccaaf-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="ccaaf-113">Passare alla scheda **Driver** e selezionare **Roll Back Driver**.</span><span class="sxs-lookup"><span data-stu-id="ccaaf-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="ccaaf-114">Nota: se questa opzione non è disponibile o è disattivata, selezionare **No** nelle opzioni seguenti per passare al passaggio successivo.</span><span class="sxs-lookup"><span data-stu-id="ccaaf-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="ccaaf-115">Potrebbe essere necessario riavviare il PC prima che queste modifiche si apportare.</span><span class="sxs-lookup"><span data-stu-id="ccaaf-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="ccaaf-116">**Disinstallare e reinstallare il driver video:**</span><span class="sxs-lookup"><span data-stu-id="ccaaf-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="ccaaf-117">Seleziona **Start,** digita **Gestione dispositivi** e seleziona Gestione **dispositivi** dai risultati.</span><span class="sxs-lookup"><span data-stu-id="ccaaf-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="ccaaf-118">Espandi la **sezione Schede di visualizzazione,** fai clic con il pulsante destro del mouse sulla scheda video e scegli **Disinstalla dispositivo.**</span><span class="sxs-lookup"><span data-stu-id="ccaaf-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="ccaaf-119">Seleziona la casella accanto a **Elimina il software driver per questo dispositivo** e seleziona **Disinstalla.**</span><span class="sxs-lookup"><span data-stu-id="ccaaf-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="ccaaf-120">Nota: potrebbe essere richiesto di riavviare il computer in questa fase.</span><span class="sxs-lookup"><span data-stu-id="ccaaf-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="ccaaf-121">Prima di riavviare, assicurati di scrivere le istruzioni rimanenti.</span><span class="sxs-lookup"><span data-stu-id="ccaaf-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="ccaaf-122">Aprire di nuovo Gestione dispositivi.</span><span class="sxs-lookup"><span data-stu-id="ccaaf-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="ccaaf-123">Espandi la **sezione Schede video,** fai clic con il pulsante destro del mouse sulla scheda video e scegli **Aggiorna driver.**</span><span class="sxs-lookup"><span data-stu-id="ccaaf-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="ccaaf-124">Selezionare **Cerca automaticamente il software del driver di** aggiornamento e seguire le istruzioni di installazione.</span><span class="sxs-lookup"><span data-stu-id="ccaaf-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>