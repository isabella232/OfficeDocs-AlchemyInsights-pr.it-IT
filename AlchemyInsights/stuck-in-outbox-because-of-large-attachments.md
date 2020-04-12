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
ms.openlocfilehash: 35fe9ae76ca77faa43796b288af09be8525cb6df
ms.sourcegitcommit: 929f8accdca2b8e5be170e0fc8edd527581453d4
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/12/2020
ms.locfileid: "43232634"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="793c3-102">Risoluzione dei messaggi bloccati nella posta in uscita</span><span class="sxs-lookup"><span data-stu-id="793c3-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="793c3-103">Si consiglia di iniziare eseguendo lo scenario ["sono presenti problemi di invio, ricezione o individuazione dei messaggi di posta elettronica"](https://aka.ms/SaRA-OutlookSendReceive) dallo strumento [Assistente supporto e ripristino di Microsoft](https://diagnostics.office.com/#/) nel computer in questione.</span><span class="sxs-lookup"><span data-stu-id="793c3-103">We recommend that you start by running the scenario ["I'm having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool on the affected machine.</span></span>

<span data-ttu-id="793c3-104">Quando un messaggio viene bloccato nella posta in uscita, la causa più probabile è un allegato di grandi dimensioni o l'opzione "Invia immediatamente quando connesso" non è abilitata.</span><span class="sxs-lookup"><span data-stu-id="793c3-104">When a message gets stuck in your Outbox, the most likely cause is a large attachment or the option "Send immediately when connected" is not enabled.</span></span>

<span data-ttu-id="793c3-105">**Rimuovere l'allegato di grandi dimensioni**</span><span class="sxs-lookup"><span data-stu-id="793c3-105">**Remove the large attachment**</span></span>

1. <span data-ttu-id="793c3-106">Fare clic su **Invia/Ricevi** > **lavoro offline**.</span><span class="sxs-lookup"><span data-stu-id="793c3-106">Click **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="793c3-107">Nel riquadro di spostamento, fare clic su **posta in uscita**.</span><span class="sxs-lookup"><span data-stu-id="793c3-107">In the navigation pane, click **Outbox**.</span></span> <span data-ttu-id="793c3-108">Da qui, è possibile:</span><span class="sxs-lookup"><span data-stu-id="793c3-108">From here, you can:</span></span> 
    - <span data-ttu-id="793c3-109">Eliminare il messaggio.</span><span class="sxs-lookup"><span data-stu-id="793c3-109">Delete the message.</span></span> <span data-ttu-id="793c3-110">Basta selezionarlo e fare clic su **Elimina**.</span><span class="sxs-lookup"><span data-stu-id="793c3-110">Just select it and click **Delete**.</span></span>
    - <span data-ttu-id="793c3-111">Trascinare il messaggio nella **cartella bozze**, fare doppio clic per aprire il messaggio ed eliminare l'allegato (fare clic su di esso e fare clic su **Elimina**).</span><span class="sxs-lookup"><span data-stu-id="793c3-111">Drag the message to your **drafts folder**, double-click to open the message, and delete the attachment (click it and click **Delete**).</span></span>
3. <span data-ttu-id="793c3-112">Se un errore indica che Outlook sta tentando di trasmettere il messaggio, chiudere Outlook.</span><span class="sxs-lookup"><span data-stu-id="793c3-112">If an error tells you Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="793c3-113">Potrebbe essere necessario qualche minuto per uscire.</span><span class="sxs-lookup"><span data-stu-id="793c3-113">It may take a few moments to exit.</span></span> <span data-ttu-id="793c3-114">Se Outlook non si chiude, premere **CTRL + ALT + CANC** e fare clic su **Avvia Gestione attività**.</span><span class="sxs-lookup"><span data-stu-id="793c3-114">If Outlook doesn't close, press **Ctrl+Alt+Delete** and click **Start Task Manager**.</span></span> <span data-ttu-id="793c3-115">In Task Manager selezionare la scheda **processi** , scorrere verso il basso fino a Outlook. exe e fare clic su **Termina processo**.</span><span class="sxs-lookup"><span data-stu-id="793c3-115">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and click **End Process**.</span></span>
4. <span data-ttu-id="793c3-116">Dopo la chiusura di Outlook, riavviare Outlook e ripetere i passaggi 2-3.</span><span class="sxs-lookup"><span data-stu-id="793c3-116">After Outlook closes, restart Outlook and repeat steps 2-3.</span></span> 
5. <span data-ttu-id="793c3-117">Dopo aver rimosso l'allegato, fare clic su **Invia/Ricevi** > **lavoro offline** per deselezionare il pulsante e riprendere a lavorare online.</span><span class="sxs-lookup"><span data-stu-id="793c3-117">After you remove the attachment, click **Send / Receive** > **Work Offline** to deselect the button and to resume working online.</span></span> 

<span data-ttu-id="793c3-118">I messaggi vengono bloccati anche nella cartella posta in uscita quando si fa clic su **Invia**, ma non si è connessi.</span><span class="sxs-lookup"><span data-stu-id="793c3-118">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="793c3-119">Fare clic su **Invia/Ricevi** e guardare il pulsante **lavora in modalità** non in linea.</span><span class="sxs-lookup"><span data-stu-id="793c3-119">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="793c3-120">Se è blu, si è scollegati.</span><span class="sxs-lookup"><span data-stu-id="793c3-120">If it's blue, you're disconnected.</span></span> <span data-ttu-id="793c3-121">Fare clic su di esso per connettersi (il pulsante diventa bianco) e fare clic su **Invia tutto**.</span><span class="sxs-lookup"><span data-stu-id="793c3-121">Click it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="793c3-122">**Abilita invio immediato quando si è connessi**</span><span class="sxs-lookup"><span data-stu-id="793c3-122">**Enable Send immediately when connected**</span></span>
 
1. <span data-ttu-id="793c3-123">Nella scheda File fare clic su **Opzioni**.</span><span class="sxs-lookup"><span data-stu-id="793c3-123">On the File tab, click **Options**.</span></span>

2. <span data-ttu-id="793c3-124">Nella finestra di dialogo Opzioni di Outlook fare clic su **Avanzate**.</span><span class="sxs-lookup"><span data-stu-id="793c3-124">In the Outlook Options dialog box, click **Advanced**.</span></span>

3. <span data-ttu-id="793c3-125">Nella sezione invio e ricezione fare clic per abilitare l' **invio immediato quando**si è connessi.</span><span class="sxs-lookup"><span data-stu-id="793c3-125">In the Send and receive section, click to enable **Send immediately when connected**.</span></span> <span data-ttu-id="793c3-126">Fare clic su **OK**.</span><span class="sxs-lookup"><span data-stu-id="793c3-126">Click **OK**.</span></span>
 
<span data-ttu-id="793c3-127">Per informazioni complete, vedere:</span><span class="sxs-lookup"><span data-stu-id="793c3-127">For full details, see:</span></span>
- [<span data-ttu-id="793c3-128">Video: invio o eliminazione di un messaggio di posta elettronica bloccato</span><span class="sxs-lookup"><span data-stu-id="793c3-128">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="793c3-129">La posta elettronica rimane nella cartella posta in uscita fino a quando non viene avviata manualmente un'operazione di invio/ricezione in Outlook</span><span class="sxs-lookup"><span data-stu-id="793c3-129">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
