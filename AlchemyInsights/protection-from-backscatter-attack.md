---
title: Protezione contro gli attacchi backscatter
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9779"
- "9005743"
ms.openlocfilehash: 8d9214fe2f5d55a21c72296421dd837d7f1d7e7d
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 03/19/2021
ms.locfileid: "50898021"
---
# <a name="protection-from-backscatter-attack"></a><span data-ttu-id="70e3d-102">Protezione contro gli attacchi backscatter</span><span class="sxs-lookup"><span data-stu-id="70e3d-102">Protection from Backscatter attack</span></span>

<span data-ttu-id="70e3d-103">Il backscatter sono notifiche di mancato recapito (note come NDR o notifiche di mancato recapito) che ricevi per messaggi che non hai inviato.</span><span class="sxs-lookup"><span data-stu-id="70e3d-103">Backscatter is non-delivery reports (also known as NDRs or bounce messages) you receive for messages that you did not send.</span></span> <span data-ttu-id="70e3d-104">Gli spammer falsificano l'indirizzo **Da:** dei messaggi, e spesso usano indirizzi di posta elettronica reali per rendere credibili i propri messaggi.</span><span class="sxs-lookup"><span data-stu-id="70e3d-104">Spammers forge (spoof) the **From:** address of their messages, and they often use real email addresses to lend credibility to their messages.</span></span> <span data-ttu-id="70e3d-105">Quando gli spammer inviano i messaggi a destinatari inesistenti, il server di posta elettronica di destinazione viene spinto a inviare il messaggio non recapitabile in una notifica di mancato recapito al mittente contraffatto nell'indirizzo **Da:**.</span><span class="sxs-lookup"><span data-stu-id="70e3d-105">So, when spammers inevitably send messages to non-existent recipients, the destination email server is essentially tricked into returning the undeliverable message in an NDR to the forged sender in the **From:** address.</span></span>

<span data-ttu-id="70e3d-106">Altre informazioni sono disponibili in [Backscatter in EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop).</span><span class="sxs-lookup"><span data-stu-id="70e3d-106">Additional Information can be found in [Backscatter in EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop).</span></span>

<span data-ttu-id="70e3d-107">**Abilitare la protezione contro il backscatter**</span><span class="sxs-lookup"><span data-stu-id="70e3d-107">**Enabling Backscatter protection**</span></span>

<span data-ttu-id="70e3d-108">Per abilitare la protezione contro il backscatter, segui il passaggio sottostante.</span><span class="sxs-lookup"><span data-stu-id="70e3d-108">To enable Backscatter protection, follow the path below.</span></span>

<span data-ttu-id="70e3d-109">**protection.office.com > Gestione delle minacce > Criterio > Antispam > Seleziona il criterio del filtro antispam e modifica il criterio > Proprietà posta indesiderata > Segna come posta indesiderata > Backscatter > Imposta su “Attivo”**</span><span class="sxs-lookup"><span data-stu-id="70e3d-109">**protection.office.com > Threat Management > Policy > Antispam > Select the Spam Filter Policy and Edit policy > Spam properties > Mark as spam > NDR backscatter > Set it to “On”**</span></span>

<span data-ttu-id="70e3d-110">Se ritieni che il tuo account sia compromesso, vedi quanto segue:</span><span class="sxs-lookup"><span data-stu-id="70e3d-110">If you believe an account has been compromised, see the following:</span></span>

- [<span data-ttu-id="70e3d-111">Rispondere a un account di posta elettronica compromesso</span><span class="sxs-lookup"><span data-stu-id="70e3d-111">Responding to a Compromised Email Account</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)
- [<span data-ttu-id="70e3d-112">Rimuovere utenti bloccati dal portale Utenti con restrizioni in Office 365</span><span class="sxs-lookup"><span data-stu-id="70e3d-112">Removing blocked users from the Restricted Users portal in Office 365</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam)



