---
title: Informazioni su come aggiungere o rimuovere un delegato in Outlook per Windows
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800004"
- "7334"
ms.openlocfilehash: fcbd6082c104f0e1bca022a23cbbeb6e3363a6c5
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/04/2020
ms.locfileid: "49571913"
---
# <a name="how-to-add-or-remove-a-delegate-in-outlook-for-windows"></a><span data-ttu-id="aec0f-102">Informazioni su come aggiungere o rimuovere un delegato in Outlook per Windows</span><span class="sxs-lookup"><span data-stu-id="aec0f-102">How to add or remove a Delegate in Outlook for Windows</span></span>

<span data-ttu-id="aec0f-103">Per aggiungere un delegato in Outlook per Windows:</span><span class="sxs-lookup"><span data-stu-id="aec0f-103">To add a Delegate in Outlook for Windows:</span></span> 

1. <span data-ttu-id="aec0f-104">Fare clic sulla scheda **file** seguita dalle **impostazioni dell'account**, quindi selezionare **Delega accesso**.</span><span class="sxs-lookup"><span data-stu-id="aec0f-104">Click on the **File** tab followed by **Account Settings**, and then choose **Delegate Access**.</span></span>
2. <span data-ttu-id="aec0f-105">Fare clic su **Aggiungi**.</span><span class="sxs-lookup"><span data-stu-id="aec0f-105">Click on **Add**.</span></span> <span data-ttu-id="aec0f-106">Se **Add** non viene visualizzato, una connessione attiva potrebbe non esistere tra Outlook ed Exchange.</span><span class="sxs-lookup"><span data-stu-id="aec0f-106">If **Add** doesn’t appear, an active connection might not exist between Outlook and Exchange.</span></span> <span data-ttu-id="aec0f-107">La barra di stato di Outlook Visualizza lo stato della connessione.</span><span class="sxs-lookup"><span data-stu-id="aec0f-107">The Outlook status bar displays the connection status.</span></span>
3. <span data-ttu-id="aec0f-108">Digitare il nome della persona che si desidera designare come delegato oppure cercare e scegliere il nome nell'elenco dei risultati della ricerca.</span><span class="sxs-lookup"><span data-stu-id="aec0f-108">Type the name of the person you want to designate as your delegate, or search and choose the name in the search results list.</span></span>

    > [!NOTE]
    > <span data-ttu-id="aec0f-109">Il delegato deve essere una persona nell'elenco indirizzi globale (GAL, Global Address List) dell'organizzazione.</span><span class="sxs-lookup"><span data-stu-id="aec0f-109">The delegate must be a person in your organization's Exchange Global Address List (GAL).</span></span>
4. <span data-ttu-id="aec0f-110">Fare clic su **Aggiungi** seguito da **OK**.</span><span class="sxs-lookup"><span data-stu-id="aec0f-110">Click on **Add** followed by **OK**.</span></span>
5. <span data-ttu-id="aec0f-111">Nella finestra di dialogo **autorizzazioni delegati** accettare le impostazioni predefinite per le autorizzazioni o selezionare livelli di accesso personalizzati per le cartelle di Exchange.</span><span class="sxs-lookup"><span data-stu-id="aec0f-111">In the **Delegate Permissions** dialog box, accept the default permission settings or select custom access levels for Exchange folders.</span></span>

    - <span data-ttu-id="aec0f-112">Se un delegato deve disporre dell'autorizzazione necessaria per funzionare solo con le richieste di riunione e le risposte, le impostazioni di autorizzazione predefinite come **delegate ricevono le copie dei messaggi relativi a riunioni inviate a me** sono sufficienti.</span><span class="sxs-lookup"><span data-stu-id="aec0f-112">If a delegate needs permission to work only with meeting requests and responses, the default permission settings such as **Delegate receives copies of meeting-related messages sent to me** are sufficient.</span></span> <span data-ttu-id="aec0f-113">È possibile lasciare l'impostazione di autorizzazione **posta in arrivo** in **Nessuna**.</span><span class="sxs-lookup"><span data-stu-id="aec0f-113">You can leave the **Inbox** permission setting at **None**.</span></span> <span data-ttu-id="aec0f-114">Le convocazioni di riunione e le risposte andranno direttamente alla posta in arrivo del delegato.</span><span class="sxs-lookup"><span data-stu-id="aec0f-114">Meeting requests and responses will go directly to the delegate's inbox.</span></span>

    > [!NOTE]
    > <span data-ttu-id="aec0f-115">Per impostazione predefinita, al delegato viene concessa l'autorizzazione **Editor (in grado di leggere, creare e modificare elementi)** per la cartella **Calendario** .</span><span class="sxs-lookup"><span data-stu-id="aec0f-115">By default, the delegate is granted **Editor (can read, create, and modify items)** permission to your **Calendar** folder.</span></span> <span data-ttu-id="aec0f-116">Quando il delegato risponde a una riunione per conto dell'utente, viene aggiunta automaticamente alla cartella **Calendario** .</span><span class="sxs-lookup"><span data-stu-id="aec0f-116">When the delegate responds to a meeting on your behalf, it is automatically added to your **Calendar** folder.</span></span>

5. <span data-ttu-id="aec0f-117">Per inviare un messaggio per notificare al delegato le autorizzazioni modificate, selezionare la casella di controllo **Invia automaticamente un messaggio per delegare il riepilogo di queste autorizzazioni** .</span><span class="sxs-lookup"><span data-stu-id="aec0f-117">To send a message to notify the delegate of the changed permissions, select the **Automatically send a message to delegate summarizing these permissions** check box.</span></span>
6. <span data-ttu-id="aec0f-118">Se lo si desidera, selezionare la casella di controllo il **delegato può visualizzare gli elementi** personali.</span><span class="sxs-lookup"><span data-stu-id="aec0f-118">If you want, select the **Delegate can see my private items** check box.</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="aec0f-119">Questa impostazione ha effetto su tutte le cartelle di Exchange.</span><span class="sxs-lookup"><span data-stu-id="aec0f-119">This setting affects all Exchange folders.</span></span> <span data-ttu-id="aec0f-120">Sono inclusi tutti i messaggi, i contatti, il calendario, le attività, le note e le cartelle del journal.</span><span class="sxs-lookup"><span data-stu-id="aec0f-120">This includes all Mail, Contacts, Calendar, Tasks, Notes, and Journal folders.</span></span> <span data-ttu-id="aec0f-121">Non esiste alcun modo per concedere l'accesso agli elementi privati solo nelle cartelle specificate.</span><span class="sxs-lookup"><span data-stu-id="aec0f-121">There is no way to grant access to private items in only specified folders.</span></span>

7. <span data-ttu-id="aec0f-122">Scegliere **OK**.</span><span class="sxs-lookup"><span data-stu-id="aec0f-122">Choose **OK**.</span></span>

    > [!NOTE]
    >
    > - <span data-ttu-id="aec0f-123">I messaggi inviati con le autorizzazioni Invia per conto di sono sia i delegati sia i nomi accanto a **from**.</span><span class="sxs-lookup"><span data-stu-id="aec0f-123">Messages sent with Send on Behalf permissions include both the delegate's and your names next to **From**.</span></span> <span data-ttu-id="aec0f-124">Quando un messaggio viene inviato con l'autorizzazione Invia come, viene visualizzato solo il nome.</span><span class="sxs-lookup"><span data-stu-id="aec0f-124">When a message is sent with Send As permissions, only your name appears.</span></span>
    > - <span data-ttu-id="aec0f-125">Dopo aver aggiunto un utente come delegato, è possibile aggiungere la cassetta postale di Exchange al proprio profilo di Outlook.</span><span class="sxs-lookup"><span data-stu-id="aec0f-125">Once you add someone as a delegate, they can add your Exchange mailbox to their Outlook profile.</span></span> <span data-ttu-id="aec0f-126">Per istruzioni, vedere [gestire i messaggi di posta elettronica e gli elementi del calendario di un'altra persona](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5).</span><span class="sxs-lookup"><span data-stu-id="aec0f-126">For instructions, see [Manage another person's mail and calendar items](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5).</span></span>

<span data-ttu-id="aec0f-127">Per rimuovere un delegato in Outlook per Windows:</span><span class="sxs-lookup"><span data-stu-id="aec0f-127">To remove a Delegate in Outlook for Windows:</span></span>

1. <span data-ttu-id="aec0f-128">Fare clic sulla scheda **file** .</span><span class="sxs-lookup"><span data-stu-id="aec0f-128">Click on the **File** tab.</span></span>
2. <span data-ttu-id="aec0f-129">Fare clic su **Impostazioni account** seguite da **accesso delegato**.</span><span class="sxs-lookup"><span data-stu-id="aec0f-129">Click on **Account Settings** followed by **Delegate Access**.</span></span>
3. <span data-ttu-id="aec0f-130">Scegliere il nome del delegato per il quale si desidera modificare le autorizzazioni e quindi fare clic su **Rimuovi** seguito da **OK**.</span><span class="sxs-lookup"><span data-stu-id="aec0f-130">Choose the name of the delegate for whom you want to change permissions, and then click on **Remove** followed by **OK**.</span></span>
