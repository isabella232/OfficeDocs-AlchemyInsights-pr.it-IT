---
title: Spostamento automatico dei messaggi di posta elettronica nella cassetta postale di archiviazione
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100008"
- "7217"
ms.openlocfilehash: 14ded561ee2b3c244fadbdab42fd0e833a1c66d5
ms.sourcegitcommit: 7fa9bf6f9fc7438791aa9241a440e5be817d4401
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/08/2021
ms.locfileid: "50522388"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a><span data-ttu-id="16bda-102">Spostamento automatico dei messaggi di posta elettronica nella cassetta postale di archiviazione</span><span class="sxs-lookup"><span data-stu-id="16bda-102">Automatically move email messages to the archive mailbox</span></span>

<span data-ttu-id="16bda-103">Ecco come configurare un criterio per spostare automaticamente la vecchia posta elettronica di un utente nella cassetta postale di archiviazione:</span><span class="sxs-lookup"><span data-stu-id="16bda-103">Here's how to set up a policy to automatically move a user's old email to the archive mailbox:</span></span>

1. <span data-ttu-id="16bda-104">Passare a [**Security & Compliance**](https://go.microsoft.com/fwlink/p/?linkid=2077143)Data Governance Archive per verificare che una cassetta postale di archiviazione sia stata  >    >   abilitata per l'utente.</span><span class="sxs-lookup"><span data-stu-id="16bda-104">Go to [**Security & Compliance**](https://go.microsoft.com/fwlink/p/?linkid=2077143) > **Data governance** > **Archive** to verify an archive mailbox has been enabled for the user.</span></span> <span data-ttu-id="16bda-105">In caso contrario, fare clic su **Abilita** e quindi su **Sì** nella casella di avviso.</span><span class="sxs-lookup"><span data-stu-id="16bda-105">If it hasn't, click **Enable** then **Yes** in the warning box.</span></span>
2. <span data-ttu-id="16bda-106">Passare [**all'interfaccia di amministrazione di Exchange > gestione della conformità > tag di conservazione.**](https://go.microsoft.com/fwlink/?linkid=2059104)</span><span class="sxs-lookup"><span data-stu-id="16bda-106">Go to [**Exchange admin center > compliance management > retention tags**](https://go.microsoft.com/fwlink/?linkid=2059104).</span></span>
3. <span data-ttu-id="16bda-107">Scegliere l'icona + e quindi applicare **automaticamente all'intera cassetta postale.**</span><span class="sxs-lookup"><span data-stu-id="16bda-107">Choose the + icon then choose **automatically apply to entire mailbox**.</span></span>
4. <span data-ttu-id="16bda-108">Assegnare un nome al tag di conservazione e scegliere **Sposta nell'archivio.**</span><span class="sxs-lookup"><span data-stu-id="16bda-108">Assign a name to the retention tag, and choose **Move to Archive**.</span></span> <span data-ttu-id="16bda-109">Per il periodo di conservazione, immettere il tempo desiderato, ad esempio 90 giorni.</span><span class="sxs-lookup"><span data-stu-id="16bda-109">For the retention period, enter the time you want, such as 90 days.</span></span> <span data-ttu-id="16bda-110">Fare clic su **Salva**.</span><span class="sxs-lookup"><span data-stu-id="16bda-110">Click **Save**.</span></span>
5. <span data-ttu-id="16bda-111">A questo punto, creare un criterio di conservazione: scegliere i **criteri di conservazione,** scegliere l'icona per aggiungere un nuovo criterio.</span><span class="sxs-lookup"><span data-stu-id="16bda-111">Now create a retention policy: choose **retention policies**, choose the icon to add a new policy.</span></span>
6. <span data-ttu-id="16bda-112">Assegnare un nome al criterio di conservazione, quindi fare clic e scorrere per trovare e aggiungere il tag di conservazione appena creato.</span><span class="sxs-lookup"><span data-stu-id="16bda-112">Assign a name to the retention policy, then click and scroll to find and add the retention tag you just created.</span></span> <span data-ttu-id="16bda-113">Fare clic su **Salva**.</span><span class="sxs-lookup"><span data-stu-id="16bda-113">Click **Save**.</span></span>
7. <span data-ttu-id="16bda-114">Infine, applicare il criterio di conservazione alla cassetta postale dell'utente: ancora nell'interfaccia di amministrazione di Exchange, passare alle cassette **postali dei**  >  **destinatari.**</span><span class="sxs-lookup"><span data-stu-id="16bda-114">Finally, apply the retention policy to the user's mailbox: still in the Exchange admin center, go to **recipients** > **mailboxes**.</span></span> <span data-ttu-id="16bda-115">Scegliere tutti gli utenti a cui si desidera applicare il criterio, quindi **scegliere Modifica** (icona della matita).</span><span class="sxs-lookup"><span data-stu-id="16bda-115">Choose all the users who you want to apply the policy to, then choose **Edit** (the pencil icon).</span></span>
8. <span data-ttu-id="16bda-116">Nella finestra di dialogo, fare clic su **Funzionalità cassetta postale.**</span><span class="sxs-lookup"><span data-stu-id="16bda-116">In the dialog box, click **mailbox features**.</span></span> <span data-ttu-id="16bda-117">In **Criteri di conservazione,** applicare il criterio appena creato > **Salva.**</span><span class="sxs-lookup"><span data-stu-id="16bda-117">Under **Retention policy**, apply the policy you just created > **Save**.</span></span>
9. <span data-ttu-id="16bda-118">Per istruzioni sull'applicazione del criterio a tutti gli utenti, vedere [Applicare un criterio di conservazione alle cassette postali.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)</span><span class="sxs-lookup"><span data-stu-id="16bda-118">For instructions for applying the policy to all users, see [Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).</span></span>
