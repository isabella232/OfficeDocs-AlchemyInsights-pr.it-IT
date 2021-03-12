---
title: Correggere i criteri di connessione
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
ms.openlocfilehash: 0b6286350e706e493f6d30b7978aacedc02daff5
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50737140"
---
# <a name="fix-connection-policy"></a><span data-ttu-id="362a3-102">Correggere i criteri di connessione</span><span class="sxs-lookup"><span data-stu-id="362a3-102">Fix connection policy</span></span>

<span data-ttu-id="362a3-103">Il messaggio di posta elettronica è stato contrassegnato come sicuro e recapitato nella posta in arrivo dell'utente perché l'indirizzo IP di invio è stato contrassegnato come sicuro nel criterio Filtro connessioni.</span><span class="sxs-lookup"><span data-stu-id="362a3-103">The email was marked safe and delivered to the user's inbox because the sending IP address was marked safe in the Connection Filter policy.</span></span> <span data-ttu-id="362a3-104">Per esaminare il criterio, eseguire le operazioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="362a3-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="362a3-105">Passare al Centro [sicurezza e & conformità di Office 365 e](https://go.microsoft.com/fwlink/p/?linkid=2077143)quindi a Criteri di gestione delle minacce Protezione da posta   >    >  [indesiderata.](https://go.microsoft.com/fwlink/?linkid=2101518)</span><span class="sxs-lookup"><span data-stu-id="362a3-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="362a3-106">Nella scheda **Personalizzata** selezionare il criterio Filtro **connessioni** e quindi **selezionare Modifica criterio.**</span><span class="sxs-lookup"><span data-stu-id="362a3-106">On the **Custom** tab, select the **Connection filter policy**, and then select **Edit policy**.</span></span>
3. <span data-ttu-id="362a3-107">Esaminare **l'elenco indirizzi IP** consentiti.</span><span class="sxs-lookup"><span data-stu-id="362a3-107">Review the **IP Allow** list.</span></span> <span data-ttu-id="362a3-108">Verificare se **l'elenco indirizzi attendibili** è abilitato.</span><span class="sxs-lookup"><span data-stu-id="362a3-108">See if **Safe list** is enabled.</span></span>

    > [!NOTE]
    > <span data-ttu-id="362a3-109">Microsoft sottoscrive origini di terze parti di mittenti attendibili.</span><span class="sxs-lookup"><span data-stu-id="362a3-109">Microsoft subscribes to third-party sources of trusted senders.</span></span> <span data-ttu-id="362a3-110">Se **l'elenco** indirizzi attendibili è abilitato, questi mittenti attendibili non vengono erroneamente contrassegnati come posta indesiderata.</span><span class="sxs-lookup"><span data-stu-id="362a3-110">If **Safe list** is enabled, these trusted senders aren't mistakenly marked as spam.</span></span> <span data-ttu-id="362a3-111">È consigliabile selezionare questa opzione perché ridurrà il numero di falsi positivi (buona posta classificata come posta indesiderata) ricevuti.</span><span class="sxs-lookup"><span data-stu-id="362a3-111">I recommend selecting this option, because it will reduce the number of false positives (good mail that's classified as spam) that you receive.</span></span>
