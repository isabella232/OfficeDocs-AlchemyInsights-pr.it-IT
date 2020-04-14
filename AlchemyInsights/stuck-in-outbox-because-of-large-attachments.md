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
- "9002385"
- "4645"
ms.openlocfilehash: 4f69de167dc51961fa7cf71b4d73ca7ee3ed4d55
ms.sourcegitcommit: 57fb994ddd3854d06faa67680c971b003b06bf83
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/13/2020
ms.locfileid: "43241256"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="ab2e7-102">Risoluzione dei messaggi bloccati nella posta in uscita</span><span class="sxs-lookup"><span data-stu-id="ab2e7-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="ab2e7-103">Si consiglia di iniziare eseguendo lo scenario ["sono presenti problemi di invio, ricezione o individuazione dei messaggi di posta elettronica"](https://aka.ms/SaRA-OutlookSendReceive) dallo strumento [Assistente supporto e ripristino di Microsoft](https://diagnostics.office.com/#/) .</span><span class="sxs-lookup"><span data-stu-id="ab2e7-103">We recommend that you start by running the scenario ["I'm having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool.</span></span>

<span data-ttu-id="ab2e7-104">Quando un messaggio viene bloccato nella posta in uscita, la causa più probabile è un allegato di grandi dimensioni o l'opzione "Invia immediatamente quando connesso" non è abilitata.</span><span class="sxs-lookup"><span data-stu-id="ab2e7-104">When a message gets stuck in your Outbox, the most likely cause is a large attachment or the option "Send immediately when connected" is not enabled.</span></span>

<span data-ttu-id="ab2e7-105">**Rimuovere l'allegato di grandi dimensioni**</span><span class="sxs-lookup"><span data-stu-id="ab2e7-105">**Remove the large attachment**</span></span>

1. <span data-ttu-id="ab2e7-106">In Outlook selezionare **Invia/Ricevi** > **lavoro offline**.</span><span class="sxs-lookup"><span data-stu-id="ab2e7-106">In Outlook, select **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="ab2e7-107">Nel riquadro di spostamento, selezionare **posta in uscita**.</span><span class="sxs-lookup"><span data-stu-id="ab2e7-107">In the navigation pane, select **Outbox**.</span></span> <span data-ttu-id="ab2e7-108">Da qui, è possibile:</span><span class="sxs-lookup"><span data-stu-id="ab2e7-108">From here, you can:</span></span> 
    - <span data-ttu-id="ab2e7-109">Eliminare il messaggio (selezionarlo e quindi fare clic su **Elimina**).</span><span class="sxs-lookup"><span data-stu-id="ab2e7-109">Delete the message (select it and then select **Delete**).</span></span>
    - <span data-ttu-id="ab2e7-110">Trascinare il messaggio nella cartella bozze, fare doppio clic per aprirlo e rimuovere l'allegato selezionarlo e quindi scegliere **Elimina**.</span><span class="sxs-lookup"><span data-stu-id="ab2e7-110">Drag the message to your Drafts folder, double-click to open it, and remove the attachment select it and then select **Delete**).</span></span>
3. <span data-ttu-id="ab2e7-111">Se viene visualizzato un messaggio di errore che indica che Outlook sta tentando di trasmetterlo, chiudere Outlook.</span><span class="sxs-lookup"><span data-stu-id="ab2e7-111">If you receive an error that says Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="ab2e7-112">Potrebbe essere necessario qualche minuto per uscire.</span><span class="sxs-lookup"><span data-stu-id="ab2e7-112">It may take a few moments to exit.</span></span> <span data-ttu-id="ab2e7-113">Se Outlook non si chiude, premere CTRL + ALT + CANC e selezionare **Avvia Gestione attività**.</span><span class="sxs-lookup"><span data-stu-id="ab2e7-113">If Outlook doesn't close, press Ctrl+Alt+Delete and select **Start Task Manager**.</span></span> <span data-ttu-id="ab2e7-114">In Task Manager selezionare la scheda **processi** , scorrere verso il basso fino a Outlook. exe e selezionare **Termina processo**.</span><span class="sxs-lookup"><span data-stu-id="ab2e7-114">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and select **End Process**.</span></span>
4. <span data-ttu-id="ab2e7-115">Dopo la chiusura di Outlook, riavviarlo e ripetere i passaggi 2 e 3.</span><span class="sxs-lookup"><span data-stu-id="ab2e7-115">After Outlook closes, restart it and repeat steps 2 and 3.</span></span> 
5. <span data-ttu-id="ab2e7-116">Dopo aver rimosso l'allegato, fare clic su **Invia/Ricevi** > **lavoro offline** per riprendere a lavorare online.</span><span class="sxs-lookup"><span data-stu-id="ab2e7-116">After you remove the attachment, click **Send / Receive** > **Work Offline** to resume working online.</span></span> 

<span data-ttu-id="ab2e7-117">I messaggi vengono bloccati anche nella cartella posta in uscita quando si fa clic su **Invia**, ma non si è connessi.</span><span class="sxs-lookup"><span data-stu-id="ab2e7-117">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="ab2e7-118">Fare clic su **Invia/Ricevi** e guardare il pulsante **lavora in modalità** non in linea.</span><span class="sxs-lookup"><span data-stu-id="ab2e7-118">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="ab2e7-119">Se è blu, si è scollegati.</span><span class="sxs-lookup"><span data-stu-id="ab2e7-119">If it's blue, you're disconnected.</span></span> <span data-ttu-id="ab2e7-120">Fare clic su di esso per connettersi (il pulsante diventa bianco) e fare clic su **Invia tutto**.</span><span class="sxs-lookup"><span data-stu-id="ab2e7-120">Click it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="ab2e7-121">**Abilita invio immediato quando si è connessi**</span><span class="sxs-lookup"><span data-stu-id="ab2e7-121">**Enable Send immediately when connected**</span></span>
 
1. <span data-ttu-id="ab2e7-122">Nella scheda File fare clic su **Opzioni**.</span><span class="sxs-lookup"><span data-stu-id="ab2e7-122">On the File tab, click **Options**.</span></span>

2. <span data-ttu-id="ab2e7-123">Nella finestra di dialogo Opzioni di Outlook fare clic su **Avanzate**.</span><span class="sxs-lookup"><span data-stu-id="ab2e7-123">In the Outlook Options dialog box, click **Advanced**.</span></span>

3. <span data-ttu-id="ab2e7-124">Nella sezione invio e ricezione fare clic per abilitare l' **invio immediato quando**si è connessi.</span><span class="sxs-lookup"><span data-stu-id="ab2e7-124">In the Send and receive section, click to enable **Send immediately when connected**.</span></span> <span data-ttu-id="ab2e7-125">Fare clic su **OK**.</span><span class="sxs-lookup"><span data-stu-id="ab2e7-125">Click **OK**.</span></span>
 
<span data-ttu-id="ab2e7-126">Per informazioni complete, vedere:</span><span class="sxs-lookup"><span data-stu-id="ab2e7-126">For full details, see:</span></span>
- [<span data-ttu-id="ab2e7-127">Video: invio o eliminazione di un messaggio di posta elettronica bloccato</span><span class="sxs-lookup"><span data-stu-id="ab2e7-127">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="ab2e7-128">La posta elettronica rimane nella cartella posta in uscita fino a quando non viene avviata manualmente un'operazione di invio/ricezione in Outlook</span><span class="sxs-lookup"><span data-stu-id="ab2e7-128">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
