---
title: Liberare spazio di archiviazione in Windows 10
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 03/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9771"
- "9005403"
ms.openlocfilehash: 3838f3db3bc5f54bcb1a2558484056f3194b76e1
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 03/19/2021
ms.locfileid: "50898349"
---
# <a name="free-up-drive-space-in-windows-10"></a><span data-ttu-id="a0dae-102">Liberare spazio di archiviazione in Windows 10</span><span class="sxs-lookup"><span data-stu-id="a0dae-102">Free up drive space in Windows 10</span></span>

<span data-ttu-id="a0dae-103">Ci sono due modi per liberare spazio di archiviazione in Windows:</span><span class="sxs-lookup"><span data-stu-id="a0dae-103">Here are two options to free up drive space in Windows:</span></span>

- <span data-ttu-id="a0dae-104">Liberare spazio di archiviazione in Windows 10.</span><span class="sxs-lookup"><span data-stu-id="a0dae-104">Free up drive space in Windows 10.</span></span>
- <span data-ttu-id="a0dae-105">Liberare spazio per gli aggiornamenti di Windows 10 con unità di archiviazione esterne. </span><span class="sxs-lookup"><span data-stu-id="a0dae-105">Free up space for Windows 10 updates with external storage device.</span></span>

<span data-ttu-id="a0dae-106">Se lo spazio di archiviazione è ancora insufficiente dopo la pulizia del disco, è probabile che la cartella Temp sia riempita rapidamente dai file delle applicazioni (.appx) usati da Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="a0dae-106">If you still have low disk space after using Disk Cleanup, it’s possible that your Temp folder is quickly filling up with application (.appx) files used by Microsoft Store.</span></span> <span data-ttu-id="a0dae-107">Per risolvere il problema, ripristinare Microsoft Store, svuotare la cache dello Store, quindi eseguire lo strumento di risoluzione dei problemi di Windows Update.</span><span class="sxs-lookup"><span data-stu-id="a0dae-107">To fix this problem, reset the Store, clear the Store cache, and then run the Windows Update troubleshooter.</span></span> <span data-ttu-id="a0dae-108">Assicurare che Microsoft Store sia chiuso prima di procedere con questi passaggi.</span><span class="sxs-lookup"><span data-stu-id="a0dae-108">Make sure Microsoft Store is closed before you proceed with these steps.</span></span>

<span data-ttu-id="a0dae-109">**Passaggio 1: ripristinare Microsoft Store**</span><span class="sxs-lookup"><span data-stu-id="a0dae-109">**Step 1: Reset Microsoft Store**</span></span>

<span data-ttu-id="a0dae-110">**Nota:** questa operazione elimina definitivamente i dati delle app sul dispositivo, incluso le preferenze e i dettagli di autenticazione.</span><span class="sxs-lookup"><span data-stu-id="a0dae-110">**Note** This permanently deletes the app data on the device, including your preferences and sign-in details.</span></span>

1. <span data-ttu-id="a0dae-111">Seleziona **Start** > **Impostazioni** > **App** > **App e funzionalità**.</span><span class="sxs-lookup"><span data-stu-id="a0dae-111">Select **Start** > **Settings** > **Apps** > **Apps & features**.</span></span>

1. <span data-ttu-id="a0dae-112">Nell'elenco delle app, individua e seleziona Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="a0dae-112">In the list of apps, locate and select Microsoft Store.</span></span>

1. <span data-ttu-id="a0dae-113">Seleziona **Opzioni avanzate**.</span><span class="sxs-lookup"><span data-stu-id="a0dae-113">Select **Advanced options**.</span></span>

1. <span data-ttu-id="a0dae-114">Scorri in basso e seleziona **Reimposta**, quindi **Conferma reimpostazione**.</span><span class="sxs-lookup"><span data-stu-id="a0dae-114">Scroll down and select **Reset**, and then **Confirm Reset**.</span></span>

<span data-ttu-id="a0dae-115">**Passaggio 2: svuotare la cache di Microsoft Store**</span><span class="sxs-lookup"><span data-stu-id="a0dae-115">**Step 2: Clear the Microsoft Store cache**</span></span>

1. <span data-ttu-id="a0dae-116">Premi il tasto WINDOWS + R per aprire la finestra di dialogo Esegui.</span><span class="sxs-lookup"><span data-stu-id="a0dae-116">Press the Windows Logo Key + R to open the Run dialog box.</span></span>

1. <span data-ttu-id="a0dae-117">Digita wsreset.exe e seleziona **OK**.</span><span class="sxs-lookup"><span data-stu-id="a0dae-117">Type wsreset.exe and select **OK**.</span></span>

1. <span data-ttu-id="a0dae-118">Si aprirà una finestra del prompt dei comandi vuota.</span><span class="sxs-lookup"><span data-stu-id="a0dae-118">A blank Command Prompt window opens.</span></span> <span data-ttu-id="a0dae-119">Dopo circa 10 secondi, la finestra si chiude e lo Store si apre automaticamente.</span><span class="sxs-lookup"><span data-stu-id="a0dae-119">After about 10 seconds, the window closes and the Store opens automatically.</span></span>

<span data-ttu-id="a0dae-120">**Passaggio 3: ripristinare Windows Update**</span><span class="sxs-lookup"><span data-stu-id="a0dae-120">**Step 3: Reset Windows Update**</span></span>

1. <span data-ttu-id="a0dae-121">Seleziona **Start** > **Impostazioni** > **Aggiornamento e sicurezza** > **Risoluzione dei problemi**.</span><span class="sxs-lookup"><span data-stu-id="a0dae-121">Select **Start** > **Settings** > **Update & Security** > **Troubleshoot**.</span></span>

1. <span data-ttu-id="a0dae-122">Scorri in basso e seleziona **Windows Update** dall'elenco, e seleziona **Avvia lo strumento di risoluzione dei problemi**.</span><span class="sxs-lookup"><span data-stu-id="a0dae-122">Scroll down and select **Windows Update** from the list, and select **Run the troubleshooter**.</span></span>

1. <span data-ttu-id="a0dae-123">Riavvia il computer e verificare se il problema persiste.</span><span class="sxs-lookup"><span data-stu-id="a0dae-123">Reboot your computer and check whether you're still experiencing the issue.</span></span>

