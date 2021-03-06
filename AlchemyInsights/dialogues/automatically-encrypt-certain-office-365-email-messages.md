---
title: Crittografare automaticamente determinati messaggi di posta elettronica di Office 365
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: e4b2f4ffcacf03e145b4c6d5ff6e73a75cb7c184
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/05/2021
ms.locfileid: "50510216"
---
# <a name="automatically-encrypt-certain-office-365-email-messages"></a><span data-ttu-id="2d677-102">Crittografare automaticamente determinati messaggi di posta elettronica di Office 365</span><span class="sxs-lookup"><span data-stu-id="2d677-102">Automatically encrypt certain Office 365 email messages</span></span>

<span data-ttu-id="2d677-103">È possibile crittografare automaticamente i messaggi inviati dagli utenti a determinate persone o organizzazioni esterne.</span><span class="sxs-lookup"><span data-stu-id="2d677-103">You can automatically encrypt messages that users send to certain external people or organizations.</span></span> <span data-ttu-id="2d677-104">A tale scopo, eseguire la procedura seguente:</span><span class="sxs-lookup"><span data-stu-id="2d677-104">To do this, perform the following steps:</span></span>

1. <span data-ttu-id="2d677-105">[Dall'interfaccia di amministrazione di Exchange,](https://outlook.office365.com/ecp/)scegliere le regole del flusso > **posta.**</span><span class="sxs-lookup"><span data-stu-id="2d677-105">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="2d677-106">Fare clic **sull'icona Nuovo (+)** e quindi su Applica crittografia dei messaggi di **Office 365 e** protezione dei diritti ai messaggi.</span><span class="sxs-lookup"><span data-stu-id="2d677-106">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="2d677-107">In **Nome** immettere un nome per la regola, ad esempio Crittografa i *messaggi inviati a DrToniRamos@gmail.com.*</span><span class="sxs-lookup"><span data-stu-id="2d677-107">In **Name**, enter a name for the rule, such as *Encrypt messages sent to DrToniRamos@gmail.com*.</span></span>
4. <span data-ttu-id="2d677-108">In **Applica questa regola se**, scegliere Il **destinatario > è questa persona.**</span><span class="sxs-lookup"><span data-stu-id="2d677-108">In **Apply this rule if**, choose **The recipient > is this person**.</span></span> 
5. <span data-ttu-id="2d677-109">Nella finestra **Seleziona membri** selezionare il nome della persona a cui si desidera applicare la regola di crittografia e quindi fare clic su **Aggiungi.**</span><span class="sxs-lookup"><span data-stu-id="2d677-109">In the **Select Members** window, select the name of the person you want the encryption rule to apply to, and then click **add**.</span></span> 
6. <span data-ttu-id="2d677-110">Al termine dell'aggiunta degli utenti, fare clic su **OK.**</span><span class="sxs-lookup"><span data-stu-id="2d677-110">When you're done adding users, click **OK**.</span></span>
7. <span data-ttu-id="2d677-111">Accanto al campo **Fare clic** su **Seleziona.**</span><span class="sxs-lookup"><span data-stu-id="2d677-111">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="2d677-112">Nel menu **a discesa del** modello RMS selezionare **Crittografa** e quindi fare clic su **OK.**</span><span class="sxs-lookup"><span data-stu-id="2d677-112">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="2d677-113">Se questa opzione non è visualizzata, significa che il piano non include la crittografia automatica.</span><span class="sxs-lookup"><span data-stu-id="2d677-113">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="2d677-114">Ma puoi aggiungerlo!)</span><span class="sxs-lookup"><span data-stu-id="2d677-114">But you can add it!)</span></span>
9. <span data-ttu-id="2d677-115">Scegli una selezione facoltativa (da un elenco di selezioni facoltative che puoi effettuare a questo punto, molte delle quali possono essere lasciata con l'impostazione predefinita per semplicità).</span><span class="sxs-lookup"><span data-stu-id="2d677-115">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="2d677-116">Fare clic su **Salva**.</span><span class="sxs-lookup"><span data-stu-id="2d677-116">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="2d677-117">È sempre possibile tornare indietro e modificare questa regola in un secondo momento.</span><span class="sxs-lookup"><span data-stu-id="2d677-117">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="2d677-118">Per ulteriori informazioni sulla creazione di regole per la crittografia, vedere Definire le regole del flusso di posta per crittografare i messaggi di posta [elettronica in Office 365.](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="2d677-118">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span></span>

