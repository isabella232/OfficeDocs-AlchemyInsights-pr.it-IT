---
title: Usare TeamViewer per gestire da remoto i dispositivi Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1284"
- "6700008"
ms.openlocfilehash: 63e7f068f3c53240ad13d1679df460c97a1a94f4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 07/28/2020
ms.locfileid: "46505211"
---
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a><span data-ttu-id="d214d-102">Usare TeamViewer per gestire da remoto i dispositivi Intune</span><span class="sxs-lookup"><span data-stu-id="d214d-102">Use TeamViewer to remotely administer Intune devices</span></span>

<span data-ttu-id="d214d-103">I dispositivi gestiti da Intune possono essere amministrati da remoto con [TeamViewer](https://www.teamviewer.com/).</span><span class="sxs-lookup"><span data-stu-id="d214d-103">Devices managed by Intune can be administered remotely by using [TeamViewer](https://www.teamviewer.com/).</span></span>

<span data-ttu-id="d214d-104">Per gestire Intune con TeamViewer, eseguire le operazioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="d214d-104">To administer Intune by using TeamViewer, use these steps:</span></span> 

<span data-ttu-id="d214d-105">Per iniziare, occorre ottenere le credenziali da TeamViewer per configurare TeamViewer Connector in Intune.</span><span class="sxs-lookup"><span data-stu-id="d214d-105">Begin by obtaining credentials from TeamViewer to set up the TeamViewer Connector on Intune.</span></span> <span data-ttu-id="d214d-106">Questo consente all'amministratore di immettere le credenziali nell'interfaccia utente di TeamViewer Connector sotto Dispositivi, un'operazione una tantum per stabilire il collegamento tra Intune e il servizio TeamViewer.</span><span class="sxs-lookup"><span data-stu-id="d214d-106">This allows the admin to enter credentials in the TeamViewer Connector UI under Devices, a one-time operation to establish the link between Intune and the TeamViewer service.</span></span>

<span data-ttu-id="d214d-107">**Parte 1: avviare una sessione con un dispositivo remoto**</span><span class="sxs-lookup"><span data-stu-id="d214d-107">**Part 1: Start a session with a remote device**</span></span>

1. <span data-ttu-id="d214d-108">In **Tutti i dispositivi** selezionare il dispositivo con cui si vuole iniziare una sessione remota.</span><span class="sxs-lookup"><span data-stu-id="d214d-108">Under **All devices**, select the device you want to start a remote session with.</span></span>
2. <span data-ttu-id="d214d-109">Da **... Altro**, selezionare **Nuova sessione di assistenza remota**.</span><span class="sxs-lookup"><span data-stu-id="d214d-109">From  **…More**, select **New remote assistance session**.</span></span>
3. <span data-ttu-id="d214d-110">Selezionare **Sì** per confermare che si vuole stabilire una sessione remota.</span><span class="sxs-lookup"><span data-stu-id="d214d-110">Select **Yes** to acknowledge you want to establish a remote session.</span></span>
    <span data-ttu-id="d214d-111">Dopo la conferma della richiesta di "Avvio di una nuova sessione remota" da parte del servizio TeamViewer, viene visualizzata un'opzione che consente di **Avviare assistenza remota** sotto i dettagli del riquadro Panoramica o Informazioni di base per il dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d214d-111">After the "Initiating a new remote session" request is acknowledged by the TeamViewer service, you'll see an option to **Start remote assistance** under the details of the Overview (or, Essentials) pane for the device.</span></span> <span data-ttu-id="d214d-112">Selezionare **Vedere altro** per espandere il riquadro e visualizzare lo stato dell'assistenza remota.</span><span class="sxs-lookup"><span data-stu-id="d214d-112">Select **See More** to expand the pane and show the Remote Assistance status.</span></span>
4. <span data-ttu-id="d214d-113">Selezionare **Avvia sessione remota** per avviare la sessione a favore dell’amministratore.</span><span class="sxs-lookup"><span data-stu-id="d214d-113">Select **Start remote session** to initiate the session on the admin side.</span></span>
5. <span data-ttu-id="d214d-114">Scegliere di scaricare il file binario di TeamViewer (Windows) e selezionare **Eseguire**.</span><span class="sxs-lookup"><span data-stu-id="d214d-114">Choose to download the TeamViewer binary (Windows), and select **Run**.</span></span><br/>
    <span data-ttu-id="d214d-115">**Nota** È possibile ignorare qualsiasi pagina del Web browser aperta sul sito Web di TeamViewer.</span><span class="sxs-lookup"><span data-stu-id="d214d-115">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

6. <span data-ttu-id="d214d-116">Confermare la richiesta dell'app TeamViewer di apportare modifiche al dispositivo (solo per Windows).</span><span class="sxs-lookup"><span data-stu-id="d214d-116">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
7. <span data-ttu-id="d214d-117">L'app TeamViewer è avviata e include il codice di sessione per autenticare la connessione con il dispositivo remoto.</span><span class="sxs-lookup"><span data-stu-id="d214d-117">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>

<span data-ttu-id="d214d-118">**Parte 2: nel dispositivo di destinazione di una sessione remota**</span><span class="sxs-lookup"><span data-stu-id="d214d-118">**Part 2: On the device being targeted for a remote session**</span></span>

1. <span data-ttu-id="d214d-119">Aprire il portale aziendale Intune.</span><span class="sxs-lookup"><span data-stu-id="d214d-119">Open the Intune company portal.</span></span>
2. <span data-ttu-id="d214d-120">Cercare un contrassegno di notifica: "L’amministratore IT richiede un controllo del dispositivo per una sessione di assistenza remota" e selezionare la notifica.</span><span class="sxs-lookup"><span data-stu-id="d214d-120">Look for a notification flag: "Your IT administrator is requesting control of this device for a remote assistance session," and select the notification.</span></span>
3. <span data-ttu-id="d214d-121">Scegliere di scaricare l'applicazione TeamViewer o confermare il download dell'app TeamViewer dall'App Store e selezionare **Eseguire**.</span><span class="sxs-lookup"><span data-stu-id="d214d-121">Choose to download the TeamViewer application, or acknowledge download of the TeamViewer app from the app store, and select **Run**.</span></span>
    <span data-ttu-id="d214d-122">**Nota** È possibile ignorare qualsiasi pagina del Web browser aperta sul sito Web di TeamViewer.</span><span class="sxs-lookup"><span data-stu-id="d214d-122">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

4. <span data-ttu-id="d214d-123">Confermare la richiesta dell'app TeamViewer di apportare modifiche al dispositivo (solo per Windows).</span><span class="sxs-lookup"><span data-stu-id="d214d-123">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
5. <span data-ttu-id="d214d-124">L'app TeamViewer è avviata e include il codice di sessione per autenticare la connessione con il dispositivo remoto.</span><span class="sxs-lookup"><span data-stu-id="d214d-124">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>
6. <span data-ttu-id="d214d-125">Un popup richiede se si vuole consentire l'avvio della sessione.</span><span class="sxs-lookup"><span data-stu-id="d214d-125">A popup asks if you want to allow the session to start.</span></span>

<span data-ttu-id="d214d-126">**Nota** I codici di sessione generati dal servizio TeamViewer sono utilizzabili una sola volta.</span><span class="sxs-lookup"><span data-stu-id="d214d-126">**Note** The session codes generated by the TeamViewer service are one-time use only.</span></span> <span data-ttu-id="d214d-127">Se si perde la connessione, è necessario:</span><span class="sxs-lookup"><span data-stu-id="d214d-127">If you lose the connection, you must:</span></span>

1. <span data-ttu-id="d214d-128">Chiudere l'istanza dell'app TeamViewer nel dispositivo remoto e nella postazione di lavoro dell’amministratore.</span><span class="sxs-lookup"><span data-stu-id="d214d-128">Close the instance of the TeamViewer app on the remote device and on the admin workstation.</span></span>
2. <span data-ttu-id="d214d-129">Chiudere il portale aziendale nel dispositivo remoto.</span><span class="sxs-lookup"><span data-stu-id="d214d-129">Close the company portal on the remote device.</span></span>
3. <span data-ttu-id="d214d-130">Avviare una "Nuova sessione di assistenza remota" nel portale di amministrazione.</span><span class="sxs-lookup"><span data-stu-id="d214d-130">Initiate a new "New remote Assistance session" from the admin portal.</span></span>
4. <span data-ttu-id="d214d-131">Riaprire il portale aziendale nel dispositivo remoto per ricevere la nuova notifica.</span><span class="sxs-lookup"><span data-stu-id="d214d-131">Re-open the company portal on the remote device to receive the new notification.</span></span>
5. <span data-ttu-id="d214d-132">Scaricare e aprire l'app TeamViewer sia nel dispositivo remoto sia nella postazione di lavoro dell’amministratore, come in precedenza.</span><span class="sxs-lookup"><span data-stu-id="d214d-132">Download and open the TeamViewer app on both the remote device and the admin workstation, as before.</span></span>