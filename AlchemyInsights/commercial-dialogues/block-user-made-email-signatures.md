---
title: Bloccare le firme di posta elettronica effettuate dall'utente
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200009"
- "7310"
ms.openlocfilehash: dab7eacb617c8f3a8bd63634e974166b6e448d75
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/05/2021
ms.locfileid: "50464617"
---
# <a name="block-user-made-email-signatures"></a><span data-ttu-id="66f21-102">Bloccare le firme di posta elettronica effettuate dall'utente</span><span class="sxs-lookup"><span data-stu-id="66f21-102">Block user-made email signatures</span></span>

<span data-ttu-id="66f21-103">La soluzione seguente si applica solo alle firme di posta elettronica create in Outlook sul Web.</span><span class="sxs-lookup"><span data-stu-id="66f21-103">The following solution only applies to email signatures created in Outlook on the web.</span></span> <span data-ttu-id="66f21-104">È possibile bloccare le firme nell'app Outlook solo se si dispone di un Exchange Server locale.</span><span class="sxs-lookup"><span data-stu-id="66f21-104">You can only block signatures in the Outlook app if you have an on-premises Exchange Server.</span></span>

1. <span data-ttu-id="66f21-105">Nell'interfaccia di amministrazione scegliere **Interfaccia di amministrazione di**  >  **Exchange.**</span><span class="sxs-lookup"><span data-stu-id="66f21-105">In the admin center, choose **Admin centers** > **Exchange**.</span></span>
2. <span data-ttu-id="66f21-106">Fare clic **su Autorizzazioni** criteri di Outlook  >  **Web App.**</span><span class="sxs-lookup"><span data-stu-id="66f21-106">Click **permissions** > **Outlook Web App policies**.</span></span>
3. <span data-ttu-id="66f21-107">Selezionare il criterio e quindi fare clic sull'icona della matita per modificarlo.</span><span class="sxs-lookup"><span data-stu-id="66f21-107">Select the policy, and then click the pencil icon to edit it.</span></span>
4. <span data-ttu-id="66f21-108">Fare clic **su funzionalità**  >  **Altre opzioni.**</span><span class="sxs-lookup"><span data-stu-id="66f21-108">Click **features** > **More options**.</span></span>
5. <span data-ttu-id="66f21-109">In **Esperienza utente** deselezionare la casella di controllo Firma **di** posta elettronica e quindi fare clic su **Salva.**</span><span class="sxs-lookup"><span data-stu-id="66f21-109">Under **User experience**, clear the **Email signature** check box, and then click **Save**.</span></span>

<span data-ttu-id="66f21-110">**Importante:** Se una firma è stata aggiunta prima di deselezionare questa casella di controllo, l'utente potrà comunque utilizzarla.</span><span class="sxs-lookup"><span data-stu-id="66f21-110">**Important:** If a signature was added before clearing this check box, the user will still be able to use it.</span></span> <span data-ttu-id="66f21-111">Chiedere loro di rimuoverlo.</span><span class="sxs-lookup"><span data-stu-id="66f21-111">Ask them to remove it.</span></span>
