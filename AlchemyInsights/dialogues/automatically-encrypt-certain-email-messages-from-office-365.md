---
title: Crittografare automaticamente determinati messaggi di posta elettronica da Office 365
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
ms.openlocfilehash: 5ddaaed361f6ec934cfffb00cc62a9df2d1a04e8
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/05/2021
ms.locfileid: "50510224"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a><span data-ttu-id="39c10-102">Crittografare automaticamente determinati messaggi di posta elettronica da Office 365</span><span class="sxs-lookup"><span data-stu-id="39c10-102">Automatically encrypt certain email messages from office 365</span></span>

1. <span data-ttu-id="39c10-103">[Nell'interfaccia di amministrazione di Exchange](https://outlook.office365.com/ecp/)scegliere le regole del flusso > **posta.**</span><span class="sxs-lookup"><span data-stu-id="39c10-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="39c10-104">Fare clic **sull'icona Nuovo (+)** e quindi su Applica crittografia dei messaggi di **Office 365 e** protezione dei diritti ai messaggi.</span><span class="sxs-lookup"><span data-stu-id="39c10-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="39c10-105">In **Nome** immettere un nome per la regola, ad esempio *Crittografa tutti i messaggi.*</span><span class="sxs-lookup"><span data-stu-id="39c10-105">In **Name**, enter a name for the rule, such as *Encrypt all messages*.</span></span>
4. <span data-ttu-id="39c10-106">In **Applica questa regola se**, scegliere **[Applica a tutti i messaggi]**.</span><span class="sxs-lookup"><span data-stu-id="39c10-106">In **Apply this rule if**, choose **[Apply to all messages]**.</span></span> 
5. <span data-ttu-id="39c10-107">Accanto al campo **Fare clic** su **Seleziona.**</span><span class="sxs-lookup"><span data-stu-id="39c10-107">Next to the **Do the following** field, click **Select one**.</span></span> 
6. <span data-ttu-id="39c10-108">Nel menu **a discesa del** modello RMS selezionare **Crittografa** e quindi fare clic su **OK.**</span><span class="sxs-lookup"><span data-stu-id="39c10-108">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="39c10-109">Se questa opzione non è visualizzata, significa che il piano non include la crittografia automatica.</span><span class="sxs-lookup"><span data-stu-id="39c10-109">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="39c10-110">Ma puoi aggiungerlo!)</span><span class="sxs-lookup"><span data-stu-id="39c10-110">But you can add it!)</span></span>
7. <span data-ttu-id="39c10-111">Selezionare la **casella di controllo Controlla questa regola con livello di gravità** e quindi selezionare il livello desiderato.</span><span class="sxs-lookup"><span data-stu-id="39c10-111">Check the **Audit this rule with severity level** check box, and then select the desired level.</span></span> <span data-ttu-id="39c10-112">Se l'azienda ha obblighi contrattuali per inviare tutti i messaggi di posta elettronica crittografati, ti consigliamo di impostare il livello su **Alto.**</span><span class="sxs-lookup"><span data-stu-id="39c10-112">If your company has contractual obligations to send all emails encrypted, I recommend setting the level to **High**.</span></span>
8. <span data-ttu-id="39c10-113">In **Scegliere un modello per la regola fare** clic su **Applica.**</span><span class="sxs-lookup"><span data-stu-id="39c10-113">Under **Choose a model for this rule**, click **Enforce**.</span></span> 
9. <span data-ttu-id="39c10-114">Scegli una selezione facoltativa (da un elenco di selezioni facoltative che puoi effettuare a questo punto, molte delle quali possono essere lasciata con l'impostazione predefinita per semplicità).</span><span class="sxs-lookup"><span data-stu-id="39c10-114">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="39c10-115">Fare clic su **Salva**.</span><span class="sxs-lookup"><span data-stu-id="39c10-115">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="39c10-116">È sempre possibile tornare indietro e modificare questa regola in un secondo momento.</span><span class="sxs-lookup"><span data-stu-id="39c10-116">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="39c10-117">Per ulteriori informazioni sulla creazione di regole per la crittografia, vedere Definire le regole del flusso di posta per crittografare i messaggi di posta [elettronica in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="39c10-117">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>

