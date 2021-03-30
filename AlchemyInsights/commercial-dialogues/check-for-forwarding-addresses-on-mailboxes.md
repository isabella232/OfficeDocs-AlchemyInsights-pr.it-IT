---
title: Verificare la presenza di indirizzi di inoltro nelle cassette postali
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 3abd45230360c61ecb62e4b7a39d1b0b547271fc
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403315"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a><span data-ttu-id="0baf2-102">Verificare la presenza di indirizzi di inoltro nelle cassette postali</span><span class="sxs-lookup"><span data-stu-id="0baf2-102">Check for forwarding addresses on mailboxes</span></span>

<span data-ttu-id="0baf2-103">A volte gli hacker inoltrano i messaggi di posta elettronica degli utenti a se stessi, quindi prima di tutto verrà verificata la presenza di indirizzi di inoltro e regole sulla cassetta postale.</span><span class="sxs-lookup"><span data-stu-id="0baf2-103">Sometimes hackers forward users' email messages to themselves, so first we'll check for forwarding addresses and rules on the mailbox.</span></span> <span data-ttu-id="0baf2-104">Verificheremo quindi i log di controllo.</span><span class="sxs-lookup"><span data-stu-id="0baf2-104">Then we'll check the audit logs.</span></span> <span data-ttu-id="0baf2-105">Ecco come verificare la presenza di indirizzi di inoltro:</span><span class="sxs-lookup"><span data-stu-id="0baf2-105">Here's how to check for forwarding addresses:</span></span>

1. <span data-ttu-id="0baf2-106">Selezionare **Utenti**  >  **Utenti attivi**.</span><span class="sxs-lookup"><span data-stu-id="0baf2-106">Select **Users** > **Active users**.</span></span>
1. <span data-ttu-id="0baf2-107">Selezionare l'utente il cui account è stato compromesso.</span><span class="sxs-lookup"><span data-stu-id="0baf2-107">Select the user whose account has been compromised.</span></span>
1. <span data-ttu-id="0baf2-108">Nel riquadro a comparsa visualizzato espandere **Impostazioni** posta e quindi fare clic **su Modifica** per **l'inoltro della posta elettronica.**</span><span class="sxs-lookup"><span data-stu-id="0baf2-108">In the flyout that appears, expand **Mail Settings**, and then click **Edit** for **Email forwarding**.</span></span>
1. <span data-ttu-id="0baf2-109">Rimuovere gli indirizzi di inoltro non riconosciti.</span><span class="sxs-lookup"><span data-stu-id="0baf2-109">Remove any forwarding addresses you don't recognize.</span></span>