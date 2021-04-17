---
title: Impostazioni di avvio in Windows 10
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
- "9001691"
- "3768"
ms.openlocfilehash: 6dfae58a398db088ba00d9c2ea9788bab929ccc1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51828156"
---
# <a name="startup-settings-in-windows-10"></a><span data-ttu-id="d0300-102">Impostazioni di avvio in Windows 10</span><span class="sxs-lookup"><span data-stu-id="d0300-102">Startup settings in Windows 10</span></span>

<span data-ttu-id="d0300-103">**Modificare le app eseguite automaticamente all'avvio**</span><span class="sxs-lookup"><span data-stu-id="d0300-103">**Change which apps run automatically at startup**</span></span>

1. <span data-ttu-id="d0300-104">Vai a [Impostazioni > App > Avvio](ms-settings:startupapps?activationSource=GetHelp).</span><span class="sxs-lookup"><span data-stu-id="d0300-104">Go to [Settings > Apps > Startup](ms-settings:startupapps?activationSource=GetHelp).</span></span>

2. <span data-ttu-id="d0300-105">Assicurati che tutte le app che vuoi eseguire all'avvio siano **attivate.**</span><span class="sxs-lookup"><span data-stu-id="d0300-105">Make sure any app you want to run at startup is turned **On**.</span></span>

<span data-ttu-id="d0300-106">**Aggiungere un'app da eseguire automaticamente all'avvio**</span><span class="sxs-lookup"><span data-stu-id="d0300-106">**Add an app to run automatically at startup**</span></span>

1. <span data-ttu-id="d0300-107">Tocca o fai **clic sul pulsante Start** e trova l'app che vuoi eseguire all'avvio.</span><span class="sxs-lookup"><span data-stu-id="d0300-107">Click or tap **Start** and find the app you want to run at startup.</span></span>

2. <span data-ttu-id="d0300-108">Fai clic con il pulsante destro del mouse sull'app, fai clic **su Altro** e quindi su Apri **percorso file.**</span><span class="sxs-lookup"><span data-stu-id="d0300-108">Right-click the app, click **More**, and then click **Open file location**.</span></span> <span data-ttu-id="d0300-109">Verrà aperto il percorso in cui viene salvato il collegamento all'app.</span><span class="sxs-lookup"><span data-stu-id="d0300-109">This opens the location where the shortcut to the app is saved.</span></span> <span data-ttu-id="d0300-110">Se non è disponibile alcuna opzione per Apri percorso file, significa che l'app non può essere eseguita all'avvio.</span><span class="sxs-lookup"><span data-stu-id="d0300-110">If there is no option for Open file location, it means the app can't run at startup.</span></span>

3. <span data-ttu-id="d0300-111">Con il percorso del file aperto, premi il **tasto WINDOWS + R,** digita **shell:startup,** quindi fai clic su **OK.**</span><span class="sxs-lookup"><span data-stu-id="d0300-111">With the file location open, press the **Windows logo key  + R**, type **shell:startup**, then click **OK**.</span></span> <span data-ttu-id="d0300-112">Verrà aperta la cartella Esecuzione automatica.</span><span class="sxs-lookup"><span data-stu-id="d0300-112">This opens the Startup folder.</span></span>

4. <span data-ttu-id="d0300-113">Copia e incolla il collegamento all'app dal percorso del file alla cartella Startup.</span><span class="sxs-lookup"><span data-stu-id="d0300-113">Copy and paste the shortcut to the app from the file location to the Startup folder.</span></span>

<span data-ttu-id="d0300-114">**Opzioni di avvio avanzate (incluse la modalità provvisoria, le impostazioni UEFI e l'avvio da un altro dispositivo)**</span><span class="sxs-lookup"><span data-stu-id="d0300-114">**Advanced startup options (including Safe Mode, UEFI settings, and booting from another device)**</span></span>

1. <span data-ttu-id="d0300-115">Salva il lavoro e chiudi tutti i documenti aperti, poiché questi passaggi riavvieranno il PC.</span><span class="sxs-lookup"><span data-stu-id="d0300-115">Save your work and close any open documents, since these steps will restart your PC.</span></span>

2. <span data-ttu-id="d0300-116">Passare a [Impostazioni > aggiornamento & sicurezza > ripristino](ms-settings:recovery?activationSource=GetHelp).</span><span class="sxs-lookup"><span data-stu-id="d0300-116">Go to [Settings > Update & Security > Recovery](ms-settings:recovery?activationSource=GetHelp).</span></span>

3. <span data-ttu-id="d0300-117">In **Avvio avanzato** fare clic su **Riavvia ora.**</span><span class="sxs-lookup"><span data-stu-id="d0300-117">Under **Advanced startup**, click **Restart now**.</span></span> 

4. <span data-ttu-id="d0300-118">Dopo il riavvio del PC nella schermata Scegliere un'opzione:</span><span class="sxs-lookup"><span data-stu-id="d0300-118">After your PC restarts to the Choose an option screen:</span></span>

    - <span data-ttu-id="d0300-119">Per eseguire l'avvio da un dispositivo come un'unità USB, fai clic **su Usa un dispositivo.**</span><span class="sxs-lookup"><span data-stu-id="d0300-119">To boot from a device like a USB drive, click **Use a device**.</span></span>

    - <span data-ttu-id="d0300-120">Per immettere le impostazioni UEFI (a volte denominate configurazione del BIOS), fare clic su Risoluzione dei > opzioni avanzate **> impostazioni firmware UEFI**.</span><span class="sxs-lookup"><span data-stu-id="d0300-120">To enter the UEFI settings (sometimes called BIOS setup), click **Troubleshoot > Advanced options > UEFI Firmware Settings**.</span></span> 

    - <span data-ttu-id="d0300-121">Per accedere alla modalità provvisoria o modificare le impostazioni di avvio avanzate, fare clic su Risoluzione dei problemi > **opzioni avanzate >** impostazioni di avvio, quindi fare clic su **Riavvia**.</span><span class="sxs-lookup"><span data-stu-id="d0300-121">To enter Safe Mode or change advanced startup settings, click **Troubleshoot > Advanced options > Startup Settings**, then click **Restart**.</span></span> <span data-ttu-id="d0300-122">Potrebbe essere richiesto di immettere la chiave di [ripristino di BitLocker.](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key)</span><span class="sxs-lookup"><span data-stu-id="d0300-122">You may be asked to enter your [BitLocker recovery key](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span></span> <span data-ttu-id="d0300-123">Dopo il riavvio del PC, fai clic sull'impostazione di avvio che vuoi usare.</span><span class="sxs-lookup"><span data-stu-id="d0300-123">After your PC restarts again, click the startup setting you want to use.</span></span>