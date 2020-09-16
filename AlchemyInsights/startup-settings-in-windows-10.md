---
title: Impostazioni di avvio in Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001691"
- "3768"
ms.openlocfilehash: e49faca66785c6611dda702a381c39cdb10884f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751139"
---
# <a name="startup-settings-in-windows-10"></a><span data-ttu-id="349c5-102">Impostazioni di avvio in Windows 10</span><span class="sxs-lookup"><span data-stu-id="349c5-102">Startup settings in Windows 10</span></span>

<span data-ttu-id="349c5-103">**Modificare le app eseguite automaticamente all'avvio**</span><span class="sxs-lookup"><span data-stu-id="349c5-103">**Change which apps run automatically at startup**</span></span>

1. <span data-ttu-id="349c5-104">Andare a [impostazioni > > di avvio delle app](ms-settings:startupapps?activationSource=GetHelp).</span><span class="sxs-lookup"><span data-stu-id="349c5-104">Go to [Settings > Apps > Startup](ms-settings:startupapps?activationSource=GetHelp).</span></span>

2. <span data-ttu-id="349c5-105">Verificare che l'applicazione che si desidera eseguire all'avvio sia attivata **.**</span><span class="sxs-lookup"><span data-stu-id="349c5-105">Make sure any app you want to run at startup is turned **On**.</span></span>

<span data-ttu-id="349c5-106">**Aggiungere un'app per l'esecuzione automatica all'avvio**</span><span class="sxs-lookup"><span data-stu-id="349c5-106">**Add an app to run automatically at startup**</span></span>

1. <span data-ttu-id="349c5-107">Fare clic o toccare **Avvia** e trovare l'app che si desidera eseguire all'avvio.</span><span class="sxs-lookup"><span data-stu-id="349c5-107">Click or tap **Start** and find the app you want to run at startup.</span></span>

2. <span data-ttu-id="349c5-108">Fare clic con il pulsante destro del mouse sull'app, scegliere **altro**e quindi fare clic su **Apri percorso file**.</span><span class="sxs-lookup"><span data-stu-id="349c5-108">Right-click the app, click **More**, and then click **Open file location**.</span></span> <span data-ttu-id="349c5-109">Verrà aperta la posizione in cui viene salvato il collegamento all'app.</span><span class="sxs-lookup"><span data-stu-id="349c5-109">This opens the location where the shortcut to the app is saved.</span></span> <span data-ttu-id="349c5-110">Se non è disponibile alcuna opzione per il percorso del file aperto, significa che l'app non può essere eseguita all'avvio.</span><span class="sxs-lookup"><span data-stu-id="349c5-110">If there is no option for Open file location, it means the app can't run at startup.</span></span>

3. <span data-ttu-id="349c5-111">Con il percorso del file aperto, premere il **tasto logo Windows + R**, digitare **Shell: Startup**e quindi fare clic su **OK**.</span><span class="sxs-lookup"><span data-stu-id="349c5-111">With the file location open, press the **Windows logo key  + R**, type **shell:startup**, then click **OK**.</span></span> <span data-ttu-id="349c5-112">Verrà aperta la cartella di avvio.</span><span class="sxs-lookup"><span data-stu-id="349c5-112">This opens the Startup folder.</span></span>

4. <span data-ttu-id="349c5-113">Copiare e incollare il collegamento all'app dal percorso del file alla cartella di avvio.</span><span class="sxs-lookup"><span data-stu-id="349c5-113">Copy and paste the shortcut to the app from the file location to the Startup folder.</span></span>

<span data-ttu-id="349c5-114">**Opzioni di avvio avanzate (tra cui modalità provvisoria, impostazioni UEFI e avvio da un altro dispositivo)**</span><span class="sxs-lookup"><span data-stu-id="349c5-114">**Advanced startup options (including Safe Mode, UEFI settings, and booting from another device)**</span></span>

1. <span data-ttu-id="349c5-115">Salvare il lavoro e chiudere tutti i documenti aperti, poiché questi passaggi ricominceranno il PC.</span><span class="sxs-lookup"><span data-stu-id="349c5-115">Save your work and close any open documents, since these steps will restart your PC.</span></span>

2. <span data-ttu-id="349c5-116">Passare a [impostazioni > aggiornamento & sicurezza > ripristino](ms-settings:recovery?activationSource=GetHelp).</span><span class="sxs-lookup"><span data-stu-id="349c5-116">Go to [Settings > Update & Security > Recovery](ms-settings:recovery?activationSource=GetHelp).</span></span>

3. <span data-ttu-id="349c5-117">In **avvio avanzato**fare clic su **Riavvia**.</span><span class="sxs-lookup"><span data-stu-id="349c5-117">Under **Advanced startup**, click **Restart now**.</span></span> 

4. <span data-ttu-id="349c5-118">Dopo aver riavviato il PC nella schermata Scegli un'opzione:</span><span class="sxs-lookup"><span data-stu-id="349c5-118">After your PC restarts to the Choose an option screen:</span></span>

    - <span data-ttu-id="349c5-119">Per eseguire l'avvio da un dispositivo come un'unità USB, fare clic su **USA dispositivo**.</span><span class="sxs-lookup"><span data-stu-id="349c5-119">To boot from a device like a USB drive, click **Use a device**.</span></span>

    - <span data-ttu-id="349c5-120">Per immettere le impostazioni UEFI (a volte chiamata configurazione del BIOS), fare clic su **risoluzione dei problemi > opzioni avanzate > impostazioni del firmware UEFI**.</span><span class="sxs-lookup"><span data-stu-id="349c5-120">To enter the UEFI settings (sometimes called BIOS setup), click **Troubleshoot > Advanced options > UEFI Firmware Settings**.</span></span> 

    - <span data-ttu-id="349c5-121">Per attivare la modalità provvisoria o modificare le impostazioni di avvio avanzato, fare clic su **risoluzione dei problemi > opzioni avanzate > impostazioni di avvio**, quindi fare clic su **Riavvia**</span><span class="sxs-lookup"><span data-stu-id="349c5-121">To enter Safe Mode or change advanced startup settings, click **Troubleshoot > Advanced options > Startup Settings**, then click **Restart**.</span></span> <span data-ttu-id="349c5-122">Potrebbe essere richiesto di immettere la [chiave di ripristino di BitLocker](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span><span class="sxs-lookup"><span data-stu-id="349c5-122">You may be asked to enter your [BitLocker recovery key](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span></span> <span data-ttu-id="349c5-123">Dopo aver riavviato il PC, fare clic sull'impostazione di avvio che si desidera utilizzare.</span><span class="sxs-lookup"><span data-stu-id="349c5-123">After your PC restarts again, click the startup setting you want to use.</span></span>