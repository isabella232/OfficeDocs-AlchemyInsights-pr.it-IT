---
title: Crittografare automaticamente i messaggi di posta elettronica di Office 365 inviati a determinati domini
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
ms.openlocfilehash: 7fb96a30cd1922bd39a4b99a7ecd869622f3a466
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/05/2021
ms.locfileid: "50510200"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a><span data-ttu-id="36183-102">Crittografare automaticamente i messaggi di posta elettronica di Office 365 inviati a determinati domini</span><span class="sxs-lookup"><span data-stu-id="36183-102">Automatically encrypt Office 365 email messages sent to certain domains</span></span>

1. <span data-ttu-id="36183-103">[Dall'interfaccia di amministrazione di Exchange,](https://outlook.office365.com/ecp/)scegliere le regole del flusso > **posta.**</span><span class="sxs-lookup"><span data-stu-id="36183-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="36183-104">Fare clic **sull'icona Nuovo (+)** e quindi su Applica crittografia dei messaggi di **Office 365 e** protezione dei diritti ai messaggi.</span><span class="sxs-lookup"><span data-stu-id="36183-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="36183-105">In **Nome** immettere un nome per la regola, ad esempio *Crittografa* i messaggi inviati a contoso.com .</span><span class="sxs-lookup"><span data-stu-id="36183-105">In **Name**, enter a name for the rule, such as *Encrypt messages sent to contoso.com*.</span></span>
4. <span data-ttu-id="36183-106">In **Applica questa regola se**, scegliere Il **destinatario > dominio è**.</span><span class="sxs-lookup"><span data-stu-id="36183-106">In **Apply this rule if**, choose **The recipient > domain is**.</span></span> 
5. <span data-ttu-id="36183-107">Immettere il nome del dominio, ad esempio **contoso.com.**</span><span class="sxs-lookup"><span data-stu-id="36183-107">Enter the name of the domain, such as **contoso.com**.</span></span>
6. <span data-ttu-id="36183-108">Fare clic **sull'icona Aggiungi (+)** e quindi su **OK.**</span><span class="sxs-lookup"><span data-stu-id="36183-108">Click the **Add (+)** icon, and then click **OK**.</span></span>
7. <span data-ttu-id="36183-109">Accanto al campo **Fare clic** su **Seleziona.**</span><span class="sxs-lookup"><span data-stu-id="36183-109">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="36183-110">Nel menu **a discesa del** modello RMS selezionare **Crittografa** e quindi fare clic su **OK.**</span><span class="sxs-lookup"><span data-stu-id="36183-110">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="36183-111">Se questa opzione non è visualizzata, significa che il piano non include la crittografia automatica.</span><span class="sxs-lookup"><span data-stu-id="36183-111">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="36183-112">Ma è possibile aggiungerlo.)</span><span class="sxs-lookup"><span data-stu-id="36183-112">But you can add it!)</span></span>
9. <span data-ttu-id="36183-113">Scegliere qualsiasi selezione facoltativa (da un elenco di selezioni facoltative che è possibile effettuare a questo punto, molte delle quali possono essere lasciata con l'impostazione predefinita per semplicità).</span><span class="sxs-lookup"><span data-stu-id="36183-113">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="36183-114">Fare clic su **Salva**.</span><span class="sxs-lookup"><span data-stu-id="36183-114">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="36183-115">È sempre possibile tornare indietro e modificare questa regola in un secondo momento.</span><span class="sxs-lookup"><span data-stu-id="36183-115">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="36183-116">Per ulteriori informazioni sulla creazione di regole per la crittografia, vedere Definire le regole del flusso di posta per crittografare i messaggi di posta [elettronica in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="36183-116">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>