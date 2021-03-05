---
title: Verificare la presenza di indirizzi di inoltro nelle cassette postali
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 17/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 1b0a6c8fe368196f2d1f9811aea895c2c024b2e6
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/05/2021
ms.locfileid: "50465089"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a><span data-ttu-id="795b7-102">Verificare la presenza di indirizzi di inoltro nelle cassette postali</span><span class="sxs-lookup"><span data-stu-id="795b7-102">Check for forwarding addresses on mailboxes</span></span>

<span data-ttu-id="795b7-103">A volte gli hacker inoltrano i messaggi di posta elettronica degli utenti a se stessi, quindi prima di tutto verrà verificata la presenza di indirizzi e regole di inoltro nella cassetta postale.</span><span class="sxs-lookup"><span data-stu-id="795b7-103">Sometimes hackers forward users' email messages to themselves, so first we'll check for forwarding addresses and rules on the mailbox.</span></span> <span data-ttu-id="795b7-104">Controlliamo quindi i log di controllo.</span><span class="sxs-lookup"><span data-stu-id="795b7-104">Then we'll check the audit logs.</span></span> <span data-ttu-id="795b7-105">Ecco come controllare gli indirizzi di inoltro:</span><span class="sxs-lookup"><span data-stu-id="795b7-105">Here's how to check for forwarding addresses:</span></span>

1. <span data-ttu-id="795b7-106">Selezionare **Utenti**  >  **attivi**.</span><span class="sxs-lookup"><span data-stu-id="795b7-106">Select **Users** > **Active users**.</span></span>
1. <span data-ttu-id="795b7-107">Selezionare l'utente il cui account è stato compromesso.</span><span class="sxs-lookup"><span data-stu-id="795b7-107">Select the user whose account has been compromised.</span></span>
1. <span data-ttu-id="795b7-108">Nel riquadro a comparsa visualizzato espandere **Impostazioni** posta e quindi fare clic su **Modifica** per **l'inoltro della posta elettronica.**</span><span class="sxs-lookup"><span data-stu-id="795b7-108">In the flyout that appears, expand **Mail Settings**, and then click **Edit** for **Email forwarding**.</span></span>
1. <span data-ttu-id="795b7-109">Rimuovere gli indirizzi di inoltro non riconosciti.</span><span class="sxs-lookup"><span data-stu-id="795b7-109">Remove any forwarding addresses you don't recognize.</span></span>