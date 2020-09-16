---
title: Risoluzione dei problemi relativi all'audio in Windows 10
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
- "3476"
- "9001463"
ms.openlocfilehash: 88157f9c82bc970e989d47f5cf376b7ce485cb2a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750311"
---
# <a name="troubleshooting-audio-issues-in-windows-10"></a><span data-ttu-id="7025f-102">Risoluzione dei problemi relativi all'audio in Windows 10</span><span class="sxs-lookup"><span data-stu-id="7025f-102">Troubleshooting audio issues in Windows 10</span></span>

<span data-ttu-id="7025f-103">**Eseguire lo strumento per la risoluzione dei problemi audio**</span><span class="sxs-lookup"><span data-stu-id="7025f-103">**Run the audio troubleshooter**</span></span>

1.  <span data-ttu-id="7025f-104">Aprire le [impostazioni per la risoluzione dei problemi](ms-settings:troubleshoot).</span><span class="sxs-lookup"><span data-stu-id="7025f-104">Open the [Troubleshoot settings](ms-settings:troubleshoot).</span></span>

2.  <span data-ttu-id="7025f-105">Selezionare **riproduzione audio**  >  **eseguire la risoluzione dei problemi**.</span><span class="sxs-lookup"><span data-stu-id="7025f-105">Select **Playing Audio** > **Run the troubleshooter**.</span></span>

<span data-ttu-id="7025f-106">**Impostare il dispositivo predefinito**</span><span class="sxs-lookup"><span data-stu-id="7025f-106">**Set the default device**</span></span>

<span data-ttu-id="7025f-107">Se si sta effettuando la connessione a un dispositivo audio tramite USB o HDMI, potrebbe essere necessario impostare il dispositivo come predefinito:</span><span class="sxs-lookup"><span data-stu-id="7025f-107">If you're connecting to an audio device using USB or HDMI, you might need to set that device as the default:</span></span>

1. <span data-ttu-id="7025f-108">Aprire **Start**  >  **Sound**Start, quindi selezionare **Sound** o **Cambia suoni di sistema** dall'elenco dei risultati.</span><span class="sxs-lookup"><span data-stu-id="7025f-108">Open **Start** > **Sound**, and then select **Sound** or **Change system sounds** from the list of results.</span></span>

2.  <span data-ttu-id="7025f-109">Nella scheda **riproduzione** selezionare un dispositivo, selezionare **Imposta predefinito**, quindi fare clic su **OK**.</span><span class="sxs-lookup"><span data-stu-id="7025f-109">On the **Playback** tab, select a device, select **Set Default**, and then select **OK**.</span></span>

<span data-ttu-id="7025f-110">**Controllare cavi, volume, altoparlanti e cuffie**</span><span class="sxs-lookup"><span data-stu-id="7025f-110">**Check cables, volume, speakers, and headphones**</span></span>

1. <span data-ttu-id="7025f-111">Controllare le connessioni di altoparlanti e cuffie per i cavi sciolti e assicurarsi che siano connessi alla presa corretta.</span><span class="sxs-lookup"><span data-stu-id="7025f-111">Check your speaker and headphone connections for loose cables, and make sure they're connected to the correct jack.</span></span>

2. <span data-ttu-id="7025f-112">Controllare i livelli di alimentazione e volume e provare a attivare tutti i controlli volume.</span><span class="sxs-lookup"><span data-stu-id="7025f-112">Check your power and volume levels and try turning all the volume controls up.</span></span>

3. <span data-ttu-id="7025f-113">Alcuni oratori e app hanno i propri controlli volume; potrebbe essere necessario controllare tutti per assicurarsi che siano ai livelli giusti.</span><span class="sxs-lookup"><span data-stu-id="7025f-113">Some speakers and apps have their own volume controls; you might have to check them all to make sure they're at the right levels.</span></span>

4. <span data-ttu-id="7025f-114">Provare a connettersi utilizzando una porta USB diversa.</span><span class="sxs-lookup"><span data-stu-id="7025f-114">Try connecting using a different USB port.</span></span>

<span data-ttu-id="7025f-115">**Nota**: tenere presente che gli altoparlanti potrebbero non funzionare quando si collegano le cuffie.</span><span class="sxs-lookup"><span data-stu-id="7025f-115">**Note**: Remember that your speakers may not work when headphones are plugged in.</span></span>

<span data-ttu-id="7025f-116">**Controllare Gestione dispositivi**</span><span class="sxs-lookup"><span data-stu-id="7025f-116">**Check Device Manager**</span></span>

<span data-ttu-id="7025f-117">Per assicurarsi che i driver siano aggiornati:</span><span class="sxs-lookup"><span data-stu-id="7025f-117">To make sure the drivers are up to date:</span></span>

1. <span data-ttu-id="7025f-118">Selezionare **Start**, digitare **Gestione dispositivi**, quindi selezionare **Gestione dispositivi** dall'elenco dei risultati.</span><span class="sxs-lookup"><span data-stu-id="7025f-118">Select **Start**, type **Device Manager**, and then select **Device Manager** from the list of results.</span></span>

2. <span data-ttu-id="7025f-119">In **Controller audio, video e giochi**selezionare la scheda audio, aprirla, selezionare la scheda **driver** e quindi fare clic su **Aggiorna driver**.</span><span class="sxs-lookup"><span data-stu-id="7025f-119">Under **Sound, video, and game controllers**, select your sound card, open it, select the **Driver** tab, and select **Update Driver**.</span></span>

<span data-ttu-id="7025f-120">**Nota**: se Windows non trova un nuovo driver, cercane uno nel sito Web del produttore del dispositivo e segui le istruzioni.</span><span class="sxs-lookup"><span data-stu-id="7025f-120">**Note**: If Windows doesn't find a new driver, look for one on the device manufacturer's website and follow their instructions.</span></span>

<span data-ttu-id="7025f-121">**Reinstallare il driver**</span><span class="sxs-lookup"><span data-stu-id="7025f-121">**Reinstall the driver**</span></span>

<span data-ttu-id="7025f-122">Se non è possibile eseguire l'aggiornamento tramite Gestione dispositivi o trovare un nuovo driver nel sito Web del produttore, provare a eseguire la procedura seguente:</span><span class="sxs-lookup"><span data-stu-id="7025f-122">If you can't update via Device Manager or find a new driver on the manufacturer's website, try these steps:</span></span>

1. <span data-ttu-id="7025f-123">In gestione dispositivi fare clic con il pulsante destro del mouse (o tieni premuto) sul driver audio e scegliere **Disinstalla**.</span><span class="sxs-lookup"><span data-stu-id="7025f-123">In Device Manager, right-click (or press and hold) the audio driver, and select **Uninstall**.</span></span> <span data-ttu-id="7025f-124">Riavviare il dispositivo e Windows tenterà di reinstallare il driver.</span><span class="sxs-lookup"><span data-stu-id="7025f-124">Restart your device and Windows will attempt to reinstall the driver.</span></span>

2. <span data-ttu-id="7025f-125">Se la reinstallazione del driver non funziona, provare a utilizzare il driver audio generico fornito con Windows.</span><span class="sxs-lookup"><span data-stu-id="7025f-125">If reinstalling the driver doesn't work, try using the generic audio driver that comes with Windows.</span></span> <span data-ttu-id="7025f-126">In gestione dispositivi, fare clic con il pulsante destro del mouse (o tenere premuto) il driver audio > **aggiornare il software del driver**  >  **Sfoglia risorse del computer per il software driver**  >  **let me scegliere da un elenco di driver di dispositivo nel computer in**uso, selezionare **dispositivo audio ad alta definizione**, selezionare **Avanti**e seguire le istruzioni per installarlo.</span><span class="sxs-lookup"><span data-stu-id="7025f-126">In Device Manager, right-click (or press and hold) your audio driver > **Update driver software** > **Browse my computer for driver software** > **Let me pick from a list of device drivers on my computer**, select **High Definition Audio Device**, select **Next**, and follow the instructions to install it.</span></span>
