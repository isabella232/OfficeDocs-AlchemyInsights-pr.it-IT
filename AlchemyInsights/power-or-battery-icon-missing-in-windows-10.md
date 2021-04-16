---
title: Icona della batteria o dell'alimentazione non presente in Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002953"
- "5655"
ms.openlocfilehash: 95b68cee58f88d04f02e29477b139f7f583dc0b1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51790552"
---
# <a name="power-or-battery-icon-missing-in-windows-10"></a><span data-ttu-id="04fea-102">Icona della batteria o dell'alimentazione non presente in Windows 10</span><span class="sxs-lookup"><span data-stu-id="04fea-102">Power or battery icon missing in Windows 10</span></span>

<span data-ttu-id="04fea-103">Se il dispositivo Windows 10 è dotato di una batteria (ad es. portatile o tablet o PC connesso a un USP tramite USB), in genere l'icona della batteria/alimentazione è visibile nella barra delle applicazioni accanto all'orologio, ad esempio:</span><span class="sxs-lookup"><span data-stu-id="04fea-103">If your Windows 10 device has a battery (e.g., laptop or tablet, or a PC connected via USB to a UPS), normally a power/battery icon is shown in the taskbar near the clock, for example:</span></span>

![Icona della batteria](media/battery-icon.png)

<span data-ttu-id="04fea-105">Se tale icona non è visibile, è possibile che sia nascosta:</span><span class="sxs-lookup"><span data-stu-id="04fea-105">If you don't see this icon, it may be hidden:</span></span>

1. <span data-ttu-id="04fea-106">Passare a **[Impostazioni > Personalizzazione > Barra delle applicazioni](ms-settings:taskbar?activationSource=GetHelp)**.</span><span class="sxs-lookup"><span data-stu-id="04fea-106">Go to **[Settings > Personalization > Taskbar](ms-settings:taskbar?activationSource=GetHelp)**.</span></span>

2. <span data-ttu-id="04fea-107">Nell'area Notifica fare clic su **Seleziona le icone da visualizzare sulla barra delle applicazioni**.</span><span class="sxs-lookup"><span data-stu-id="04fea-107">In the Notification area, click **Select which icons appear on the taskbar**.</span></span>

3. <span data-ttu-id="04fea-108">Trovare quindi l'elemento **Alimentazione** nell'elenco e spostare l'impostazione su **Attivato**.</span><span class="sxs-lookup"><span data-stu-id="04fea-108">Then find the **Power** item in the list and toggle its setting to **On**.</span></span>

    ![Mostrare l'icona dell'alimentazione nella barra delle applicazioni](media/power-icon-on.png)

<span data-ttu-id="04fea-110">**Risoluzione dei problemi**</span><span class="sxs-lookup"><span data-stu-id="04fea-110">**Troubleshooting**</span></span>

<span data-ttu-id="04fea-111">Se sono state seguite le istruzioni riportate sopra e l'interruttore **Alimentazione** è disattivato o non è visibile, nella casella di ricerca della barra delle applicazioni digitare **gestione dispositivi**, quindi selezionare **Gestione dispositivi** nell'elenco dei risultati.</span><span class="sxs-lookup"><span data-stu-id="04fea-111">If you followed the above instructions and the **Power** toggle is greyed out or not visible, in the search box on the taskbar, type **device manager**, and then select **Device Manager** in the list of results.</span></span> <span data-ttu-id="04fea-112">In **Batterie** fare clic con il pulsante destro sulla batteria del dispositivo, fare clic su **Disabilita**, quindi su **Sì**.</span><span class="sxs-lookup"><span data-stu-id="04fea-112">Under **Batteries**, right-click the battery for your device, click **Disable**, and click **Yes**.</span></span> <span data-ttu-id="04fea-113">Attendere qualche secondo, quindi fare clic con il pulsante destro sulla batteria e fare clic su **Abilita**.</span><span class="sxs-lookup"><span data-stu-id="04fea-113">Wait a few seconds, and then right-click the battery and click **Enable**.</span></span> <span data-ttu-id="04fea-114">Riavviare il dispositivo.</span><span class="sxs-lookup"><span data-stu-id="04fea-114">Then restart your device.</span></span>

<span data-ttu-id="04fea-115">Se sono state seguite le istruzioni riportate sopra, ma l'icona della batteria non viene visualizzata nella barra delle applicazioni, nella casella di ricerca della barra delle applicazioni digitare **gestione attività**, quindi fare clic su **Gestione attività** nell'elenco dei risultati.</span><span class="sxs-lookup"><span data-stu-id="04fea-115">If you followed the above instructions, but the battery icon does not appear on the taskbar, in the search box on the taskbar, type **task manager**, and then click **Task Manager** in the list of results.</span></span> <span data-ttu-id="04fea-116">Nella scheda **Processi** sotto **Nome** fare clic con il pulsante destro su **Explorer**, quindi fare clic su **Riavvia**.</span><span class="sxs-lookup"><span data-stu-id="04fea-116">On the **Processes** tab, under **Name**, right-click **Explorer**, and then click **Restart**.</span></span>
