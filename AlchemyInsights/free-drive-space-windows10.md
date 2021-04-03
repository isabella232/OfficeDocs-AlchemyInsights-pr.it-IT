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
- "9774"
- "9005390"
- "9005403"
ms.openlocfilehash: 2313636307bfddce2810c2d4c4ce9e3b407a7bdf
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505360"
---
# <a name="free-up-drive-space-in-windows-10"></a><span data-ttu-id="3a192-102">Liberare spazio di archiviazione in Windows 10</span><span class="sxs-lookup"><span data-stu-id="3a192-102">Free up drive space in Windows 10</span></span>

<span data-ttu-id="3a192-103">Ci sono due modi per liberare spazio di archiviazione in Windows:</span><span class="sxs-lookup"><span data-stu-id="3a192-103">Here are two options to free up drive space in Windows:</span></span>

- <span data-ttu-id="3a192-104">Liberare spazio di archiviazione in Windows 10.</span><span class="sxs-lookup"><span data-stu-id="3a192-104">Free up drive space in Windows 10.</span></span>
- <span data-ttu-id="3a192-105">Liberare spazio per gli aggiornamenti di Windows 10 con unità di archiviazione esterne. </span><span class="sxs-lookup"><span data-stu-id="3a192-105">Free up space for Windows 10 updates with external storage device.</span></span>

<span data-ttu-id="3a192-106">Se lo spazio di archiviazione è ancora insufficiente dopo la pulizia del disco, è probabile che la cartella Temp sia riempita rapidamente dai file delle applicazioni (.appx) usati da Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="3a192-106">If you still have low disk space after using Disk Cleanup, it’s possible that your Temp folder is quickly filling up with application (.appx) files used by Microsoft Store.</span></span> <span data-ttu-id="3a192-107">Per risolvere il problema, ripristinare Microsoft Store, svuotare la cache dello Store, quindi eseguire lo strumento di risoluzione dei problemi di Windows Update.</span><span class="sxs-lookup"><span data-stu-id="3a192-107">To fix this problem, reset the Store, clear the Store cache, and then run the Windows Update troubleshooter.</span></span> <span data-ttu-id="3a192-108">Assicurare che Microsoft Store sia chiuso prima di procedere con questi passaggi.</span><span class="sxs-lookup"><span data-stu-id="3a192-108">Make sure Microsoft Store is closed before you proceed with these steps.</span></span>

<span data-ttu-id="3a192-109">**Passaggio 1: ripristinare Microsoft Store**</span><span class="sxs-lookup"><span data-stu-id="3a192-109">**Step 1: Reset Microsoft Store**</span></span>

<span data-ttu-id="3a192-110">**Nota:** questa operazione elimina definitivamente i dati delle app sul dispositivo, incluso le preferenze e i dettagli di autenticazione.</span><span class="sxs-lookup"><span data-stu-id="3a192-110">**Note** This permanently deletes the app data on the device, including your preferences and sign-in details.</span></span>

1. <span data-ttu-id="3a192-111">Seleziona **Start** > **Impostazioni** > **App** > **App e funzionalità**.</span><span class="sxs-lookup"><span data-stu-id="3a192-111">Select **Start** > **Settings** > **Apps** > **Apps & features**.</span></span>

1. <span data-ttu-id="3a192-112">Nell'elenco delle app, individua e seleziona Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="3a192-112">In the list of apps, locate and select Microsoft Store.</span></span>

1. <span data-ttu-id="3a192-113">Seleziona **Opzioni avanzate**.</span><span class="sxs-lookup"><span data-stu-id="3a192-113">Select **Advanced options**.</span></span>

1. <span data-ttu-id="3a192-114">Scorri in basso e seleziona **Reimposta**, quindi **Conferma reimpostazione**.</span><span class="sxs-lookup"><span data-stu-id="3a192-114">Scroll down and select **Reset**, and then **Confirm Reset**.</span></span>

<span data-ttu-id="3a192-115">**Passaggio 2: svuotare la cache di Microsoft Store**</span><span class="sxs-lookup"><span data-stu-id="3a192-115">**Step 2: Clear the Microsoft Store cache**</span></span>

1. <span data-ttu-id="3a192-116">Premi il tasto WINDOWS + R per aprire la finestra di dialogo Esegui.</span><span class="sxs-lookup"><span data-stu-id="3a192-116">Press the Windows Logo Key + R to open the Run dialog box.</span></span>

1. <span data-ttu-id="3a192-117">Digita wsreset.exe e seleziona **OK**.</span><span class="sxs-lookup"><span data-stu-id="3a192-117">Type wsreset.exe and select **OK**.</span></span>

1. <span data-ttu-id="3a192-118">Si aprirà una finestra del prompt dei comandi vuota.</span><span class="sxs-lookup"><span data-stu-id="3a192-118">A blank Command Prompt window opens.</span></span> <span data-ttu-id="3a192-119">Dopo circa 10 secondi, la finestra si chiude e lo Store si apre automaticamente.</span><span class="sxs-lookup"><span data-stu-id="3a192-119">After about 10 seconds, the window closes and the Store opens automatically.</span></span>

<span data-ttu-id="3a192-120">**Passaggio 3: ripristinare Windows Update**</span><span class="sxs-lookup"><span data-stu-id="3a192-120">**Step 3: Reset Windows Update**</span></span>

1. <span data-ttu-id="3a192-121">Seleziona **Start** > **Impostazioni** > **Aggiornamento e sicurezza** > **Risoluzione dei problemi**.</span><span class="sxs-lookup"><span data-stu-id="3a192-121">Select **Start** > **Settings** > **Update & Security** > **Troubleshoot**.</span></span>

1. <span data-ttu-id="3a192-122">Scorri in basso e seleziona **Windows Update** dall'elenco, e seleziona **Avvia lo strumento di risoluzione dei problemi**.</span><span class="sxs-lookup"><span data-stu-id="3a192-122">Scroll down and select **Windows Update** from the list, and select **Run the troubleshooter**.</span></span>

1. <span data-ttu-id="3a192-123">Riavvia il computer e verificare se il problema persiste.</span><span class="sxs-lookup"><span data-stu-id="3a192-123">Reboot your computer and check whether you're still experiencing the issue.</span></span>

