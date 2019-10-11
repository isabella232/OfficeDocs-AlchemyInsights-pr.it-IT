---
title: Bloccato in posta in uscita a causa di allegati di grandi dimensioni
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2713"
- "9000768"
ms.openlocfilehash: d5fb20fcc146be67c5a04de0640ed4efd625311a
ms.sourcegitcommit: 8004ee243b5c68ff9532224a2e6c69dda0abbd0b
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 10/10/2019
ms.locfileid: "37441310"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="ab56c-102">Risoluzione dei messaggi bloccati nella posta in uscita</span><span class="sxs-lookup"><span data-stu-id="ab56c-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="ab56c-103">Si consiglia di iniziare eseguendo lo scenario ["sono presenti problemi di invio, ricezione o individuazione dei messaggi di posta elettronica"](https://aka.ms/SaRA-OutlookSendReceive) dallo strumento [Assistente supporto e ripristino di Microsoft](https://diagnostics.office.com/#/) .</span><span class="sxs-lookup"><span data-stu-id="ab56c-103">We recommend that you start by running the scenario ["I’m having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool.</span></span>

<span data-ttu-id="ab56c-104">Quando un messaggio viene bloccato nella posta in uscita, le cause più probabili sono le seguenti:</span><span class="sxs-lookup"><span data-stu-id="ab56c-104">When a message gets stuck in your Outbox, the most likely causes are:</span></span>
- <span data-ttu-id="ab56c-105">Allegati di grandi dimensioni.</span><span class="sxs-lookup"><span data-stu-id="ab56c-105">Large attachments.</span></span>
- <span data-ttu-id="ab56c-106">L'opzione **Invia immediatamente quando connesso** non è abilitata.</span><span class="sxs-lookup"><span data-stu-id="ab56c-106">The **Send immediately when connected** option is not enabled.</span></span>

<span data-ttu-id="ab56c-107">Per rimuovere allegati di grandi dimensioni:</span><span class="sxs-lookup"><span data-stu-id="ab56c-107">To remove large attachments:</span></span> 

1. <span data-ttu-id="ab56c-108">In Outlook selezionare **Invia/Ricevi** > **lavoro offline**.</span><span class="sxs-lookup"><span data-stu-id="ab56c-108">In Outlook, select **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="ab56c-109">Nel riquadro di spostamento, selezionare **posta in uscita**.</span><span class="sxs-lookup"><span data-stu-id="ab56c-109">In the navigation pane, select **Outbox**.</span></span> <span data-ttu-id="ab56c-110">Da qui, è possibile:</span><span class="sxs-lookup"><span data-stu-id="ab56c-110">From here, you can:</span></span> 
    - <span data-ttu-id="ab56c-111">Eliminare il messaggio (selezionarlo e quindi fare clic su **Elimina**).</span><span class="sxs-lookup"><span data-stu-id="ab56c-111">Delete the message (select it and then select **Delete**).</span></span>
    - <span data-ttu-id="ab56c-112">Trascinare il messaggio nella cartella bozze, fare doppio clic per aprirlo e rimuovere l'allegato selezionarlo e quindi scegliere **Elimina**.</span><span class="sxs-lookup"><span data-stu-id="ab56c-112">Drag the message to your Drafts folder, double-click to open it, and remove the attachment select it and then select **Delete**).</span></span>
3. <span data-ttu-id="ab56c-113">Se viene visualizzato un messaggio di errore che indica che Outlook sta tentando di trasmetterlo, chiudere Outlook.</span><span class="sxs-lookup"><span data-stu-id="ab56c-113">If you receive an error that says Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="ab56c-114">Potrebbe essere necessario qualche minuto per uscire.</span><span class="sxs-lookup"><span data-stu-id="ab56c-114">It may take a few moments to exit.</span></span> <span data-ttu-id="ab56c-115">Se Outlook non si chiude, premere CTRL + ALT + CANC e selezionare **Avvia Gestione attività**.</span><span class="sxs-lookup"><span data-stu-id="ab56c-115">If Outlook doesn’t close, press Ctrl+Alt+Delete and select **Start Task Manager**.</span></span> <span data-ttu-id="ab56c-116">In Task Manager selezionare la scheda **processi** , scorrere verso il basso fino a Outlook. exe e selezionare **Termina processo**.</span><span class="sxs-lookup"><span data-stu-id="ab56c-116">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and select **End Process**.</span></span>
4. <span data-ttu-id="ab56c-117">Dopo la chiusura di Outlook, riavviarlo e ripetere i passaggi 2 e 3.</span><span class="sxs-lookup"><span data-stu-id="ab56c-117">After Outlook closes, restart it and repeat steps 2 and 3.</span></span> 
5. <span data-ttu-id="ab56c-118">Dopo aver rimosso l'allegato, fare clic su **Invia/Ricevi** > **lavoro offline** per riprendere a lavorare online.</span><span class="sxs-lookup"><span data-stu-id="ab56c-118">After you remove the attachment, click **Send / Receive** > **Work Offline** to resume working online.</span></span> 

<span data-ttu-id="ab56c-119">I messaggi vengono bloccati anche nella cartella posta in uscita quando si fa clic su **Invia**, ma non si è connessi.</span><span class="sxs-lookup"><span data-stu-id="ab56c-119">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="ab56c-120">Fare clic su **Invia/Ricevi** e guardare il pulsante **lavora in modalità** non in linea.</span><span class="sxs-lookup"><span data-stu-id="ab56c-120">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="ab56c-121">Se è blu, si è scollegati.</span><span class="sxs-lookup"><span data-stu-id="ab56c-121">If it's blue, you're disconnected.</span></span> <span data-ttu-id="ab56c-122">Selezionarlo per la connessione (il pulsante diventa bianco) e fare clic su **Invia tutto**.</span><span class="sxs-lookup"><span data-stu-id="ab56c-122">Select it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="ab56c-123">Per abilitare l' **invio immediato quando**si è connessi:</span><span class="sxs-lookup"><span data-stu-id="ab56c-123">To enable **Send immediately when connected**:</span></span>
 
- <span data-ttu-id="ab56c-124">Selezionare \*\*\*\* > \*\*\*\* opzioni >  file**Avanzate**.</span><span class="sxs-lookup"><span data-stu-id="ab56c-124">Select **File** > **Options** >  **Advanced**.</span></span>
<span data-ttu-id="ab56c-125">Nella sezione **invio e ricezione** selezionare **Invia immediatamente quando**si è connessi e quindi fare clic su **OK**.</span><span class="sxs-lookup"><span data-stu-id="ab56c-125">In the **Send and receive** section, select **Send immediately when connected**, and then choose **OK**.</span></span>
 
<span data-ttu-id="ab56c-126">Per i dettagli completi, vedere:</span><span class="sxs-lookup"><span data-stu-id="ab56c-126">For full details see:</span></span>
- [<span data-ttu-id="ab56c-127">Video: invio o eliminazione di un messaggio di posta elettronica bloccato</span><span class="sxs-lookup"><span data-stu-id="ab56c-127">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="ab56c-128">La posta elettronica rimane nella cartella posta in uscita fino a quando non viene avviata manualmente un'operazione di invio/ricezione in Outlook</span><span class="sxs-lookup"><span data-stu-id="ab56c-128">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
