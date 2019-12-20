---
title: Risoluzione dei problemi relativi all'audio in Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3476"
- "9001463"
ms.openlocfilehash: 46b23f97c2e682258224dc95e7a76b1201991828
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/19/2019
ms.locfileid: "40796203"
---
# <a name="troubleshooting-audio-problems-in-windows-10"></a><span data-ttu-id="acbb5-102">Risoluzione dei problemi relativi all'audio in Windows 10</span><span class="sxs-lookup"><span data-stu-id="acbb5-102">Troubleshooting audio problems in Windows 10</span></span>

<span data-ttu-id="acbb5-103">**Eseguire lo strumento per la risoluzione dei problemi audio**</span><span class="sxs-lookup"><span data-stu-id="acbb5-103">**Run the audio troubleshooter**</span></span>

<span data-ttu-id="acbb5-104">Lo strumento per la risoluzione dei problemi audio potrebbe essere in grado di risolvere automaticamente gli errori audio:</span><span class="sxs-lookup"><span data-stu-id="acbb5-104">The audio troubleshooter might be able to fix the audio problems automatically:</span></span> 

1. <span data-ttu-id="acbb5-105">Fare clic su **Start**, digitare **risoluzione dei problemi**e quindi selezionare **risoluzione dei problemi** nell'elenco di risultati.</span><span class="sxs-lookup"><span data-stu-id="acbb5-105">Select **Start**, type **troubleshoot**, and then select **Troubleshoot** from the list of results.</span></span> 
2. <span data-ttu-id="acbb5-106">Selezionare **riproduzione audio** > **eseguire la risoluzione dei problemi**.</span><span class="sxs-lookup"><span data-stu-id="acbb5-106">Select **Playing Audio** > **Run the troubleshooter**.</span></span>

<span data-ttu-id="acbb5-107">**Controllare cavi, volume, altoparlanti e cuffie**</span><span class="sxs-lookup"><span data-stu-id="acbb5-107">**Check cables, volume, speakers, and headphones**</span></span>

- <span data-ttu-id="acbb5-108">Controllare le connessioni di altoparlanti e cuffie per i cavi sciolti e assicurarsi che siano connessi alla presa corretta.</span><span class="sxs-lookup"><span data-stu-id="acbb5-108">Check your speaker and headphone connections for loose cables, and make sure they're connected to the correct jack.</span></span>
- <span data-ttu-id="acbb5-109">Controllare i livelli di alimentazione e volume e provare a attivare tutti i controlli volume.</span><span class="sxs-lookup"><span data-stu-id="acbb5-109">Check your power and volume levels, and try turning all the volume controls up.</span></span>
- <span data-ttu-id="acbb5-110">Alcuni oratori e app hanno i propri controlli del volume e potrebbe essere necessario controllarli tutti per assicurarsi che siano ai livelli giusti.</span><span class="sxs-lookup"><span data-stu-id="acbb5-110">Some speakers and apps have their own volume controls, and you might have to check them all to make sure they're at the right levels.</span></span>
- <span data-ttu-id="acbb5-111">Provare a connettersi utilizzando una porta USB diversa.</span><span class="sxs-lookup"><span data-stu-id="acbb5-111">Try connecting using a different USB port.</span></span>
- <span data-ttu-id="acbb5-112">**Nota:** Tenere presente che gli altoparlanti potrebbero non funzionare quando si collegano le cuffie.</span><span class="sxs-lookup"><span data-stu-id="acbb5-112">**Note:** Remember that your speakers may not work when headphones are plugged in.</span></span>

<span data-ttu-id="acbb5-113">**Controllare Gestione dispositivi**</span><span class="sxs-lookup"><span data-stu-id="acbb5-113">**Check Device Manager**</span></span>

<span data-ttu-id="acbb5-114">Per assicurarsi che i driver siano aggiornati:</span><span class="sxs-lookup"><span data-stu-id="acbb5-114">To make sure the drivers are up to date:</span></span>

- <span data-ttu-id="acbb5-115">Selezionare **Start**, digitare **Gestione dispositivi**, quindi selezionare **Gestione dispositivi** dall'elenco dei risultati.</span><span class="sxs-lookup"><span data-stu-id="acbb5-115">Select **Start**, type **Device Manager**, and then select **Device Manager** from the list of results.</span></span>

2. <span data-ttu-id="acbb5-116">In **Controller audio, video e giochi**selezionare la scheda audio, aprirla, selezionare la scheda **driver** e quindi fare clic su **Aggiorna driver**.</span><span class="sxs-lookup"><span data-stu-id="acbb5-116">Under **Sound, video, and game controllers**, select your sound card, open it, select the **Driver** tab, and select **Update Driver**.</span></span> 

<span data-ttu-id="acbb5-117">**Nota:** Se Windows non trova un nuovo driver, cercane uno nel sito Web del produttore del dispositivo e segui le istruzioni.</span><span class="sxs-lookup"><span data-stu-id="acbb5-117">**Note:** If Windows doesn't find a new driver, look for one on the device manufacturer's website and follow their instructions.</span></span>

<span data-ttu-id="acbb5-118">**Reinstallare il driver**</span><span class="sxs-lookup"><span data-stu-id="acbb5-118">**Reinstall the driver**</span></span>

<span data-ttu-id="acbb5-119">Se non è possibile eseguire l'aggiornamento tramite Gestione dispositivi o trovare un nuovo driver nel sito Web del produttore, provare a eseguire la procedura seguente:</span><span class="sxs-lookup"><span data-stu-id="acbb5-119">If you can't update via Device Manager or find a new driver on the manufacturer's website, try these steps:</span></span> 

1. <span data-ttu-id="acbb5-120">In gestione dispositivi fare clic con il pulsante destro del mouse (o tieni premuto) sul driver audio e scegliere **Disinstalla**.</span><span class="sxs-lookup"><span data-stu-id="acbb5-120">In Device Manager, right-click (or press and hold) the audio driver, and select **Uninstall**.</span></span> <span data-ttu-id="acbb5-121">Riavviare il dispositivo e Windows tenterà di reinstallare il driver.</span><span class="sxs-lookup"><span data-stu-id="acbb5-121">Restart your device and Windows will attempt to reinstall the driver.</span></span>

2. <span data-ttu-id="acbb5-122">Se la reinstallazione del driver non funziona, provare a utilizzare il driver audio generico fornito con Windows.</span><span class="sxs-lookup"><span data-stu-id="acbb5-122">If reinstalling the driver doesn't work, try using the generic audio driver that comes with Windows.</span></span> <span data-ttu-id="acbb5-123">In gestione dispositivi, fare clic con il pulsante destro del mouse (o tenere premuto) il driver audio > **aggiornare il software** > del driver**Sfoglia risorse del computer per il software** > driver**let me scegliere da un elenco di driver di dispositivo nel computer in**uso, selezionare **dispositivo audio ad alta definizione**, selezionare **Avanti**e seguire le istruzioni per installarlo.</span><span class="sxs-lookup"><span data-stu-id="acbb5-123">In Device Manager, right-click (or press and hold) your audio driver > **Update driver software** > **Browse my computer for driver software** > **Let me pick from a list of device drivers on my computer**, select **High Definition Audio Device**, select **Next**, and follow the instructions to install it.</span></span>

<span data-ttu-id="acbb5-124">**Impostare il dispositivo predefinito**</span><span class="sxs-lookup"><span data-stu-id="acbb5-124">**Set the default device**</span></span>

<span data-ttu-id="acbb5-125">Se si sta effettuando la connessione a un dispositivo audio tramite USB o HDMI, potrebbe essere necessario impostare il dispositivo come predefinito:</span><span class="sxs-lookup"><span data-stu-id="acbb5-125">If you're connecting to an audio device using USB or HDMI, you might need to set that device as the default:</span></span> 

1. <span data-ttu-id="acbb5-126">Fare clic su **Start**, digitare **Sound**e quindi selezionare **Sound** o **Cambia suoni di sistema** dall'elenco dei risultati.</span><span class="sxs-lookup"><span data-stu-id="acbb5-126">Select **Start**, type **Sound**, and then select **Sound** or **Change system sounds** from the list of results.</span></span>

2. <span data-ttu-id="acbb5-127">Nella scheda **riproduzione** selezionare un dispositivo, selezionare **Imposta predefinito**, quindi fare clic su **OK**.</span><span class="sxs-lookup"><span data-stu-id="acbb5-127">On the **Playback** tab, select a device, select **Set Default**, and then select **OK**.</span></span>

