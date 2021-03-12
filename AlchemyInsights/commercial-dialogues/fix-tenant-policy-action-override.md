---
title: Correggere i criteri tenant (override dell'azione)
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
- "9000760"
- "7391"
ms.openlocfilehash: bc7ad8acd86c9d5b2f99ffdc6fe8a8b53e1fcb8b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50736686"
---
# <a name="fix-tenant-policy-action-override"></a><span data-ttu-id="77822-102">Correggere i criteri tenant (override dell'azione)</span><span class="sxs-lookup"><span data-stu-id="77822-102">Fix Tenant policy (action override)</span></span>

<span data-ttu-id="77822-103">Questo messaggio è stato influenzato da un criterio di protezione da posta indesiderata nel tenant.</span><span class="sxs-lookup"><span data-stu-id="77822-103">An anti-spam policy in your tenant affected this message.</span></span> <span data-ttu-id="77822-104">Per esaminare il criterio, eseguire le operazioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="77822-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="77822-105">Passare al Centro [sicurezza e & conformità di Office 365 e](https://go.microsoft.com/fwlink/p/?linkid=2077143)quindi a Criteri di gestione delle minacce Protezione da posta   >    >  [indesiderata.](https://go.microsoft.com/fwlink/?linkid=2101518)</span><span class="sxs-lookup"><span data-stu-id="77822-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="77822-106">Verificare se **l'origine dei criteri** indica quanto  **segue: Add-Xheader/ModifySubject/Redirect/Delete/No action/BCC message**</span><span class="sxs-lookup"><span data-stu-id="77822-106">Check to see if **Policy source** indicates the following:  **Add-Xheader/ModifySubject/Redirect/Delete/No action/ BCC message**</span></span>

    <span data-ttu-id="77822-107">In tal caso, nella **scheda Personalizzata** controllare le impostazioni del criterio che ha interessato il messaggio.</span><span class="sxs-lookup"><span data-stu-id="77822-107">If so, on the **Custom** tab, check the settings of the policy that affected the message.</span></span> <span data-ttu-id="77822-108">È possibile che il messaggio sia stato influenzato dalle impostazioni **Standard** applicate a tutti i clienti di Exchange Online Protection.</span><span class="sxs-lookup"><span data-stu-id="77822-108">It's possible that the **Standard settings** applied to all Exchange Online Protection customers affected the message.</span></span>

<span data-ttu-id="77822-109">Per ulteriori informazioni sulla configurazione dei criteri di filtro della posta indesiderata, vedere [Configure your spam filter policies](https://go.microsoft.com/fwlink/?linkid=2101431).</span><span class="sxs-lookup"><span data-stu-id="77822-109">For more information on configuring spam filter policies, see [Configure your spam filter policies](https://go.microsoft.com/fwlink/?linkid=2101431).</span></span>
