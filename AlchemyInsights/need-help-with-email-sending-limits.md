---
title: Assistenza con i limiti di invio dei messaggi di posta elettronica
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002938"
- "5630"
ms.openlocfilehash: 7f563df313c869d18c3e4240d271c649a74914af
ms.sourcegitcommit: 88d2918aa51f4ba10771527380c3e0db0f5a9147
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 05/20/2020
ms.locfileid: "44328792"
---
# <a name="need-help-with-email-sending-limits"></a><span data-ttu-id="79ce2-102">Assistenza con i limiti di invio dei messaggi di posta elettronica</span><span class="sxs-lookup"><span data-stu-id="79ce2-102">Need help with email sending limits?</span></span>

<span data-ttu-id="79ce2-103">Di seguito sono riportati i **limiti di invio da progettazione** applicati al servizio.</span><span class="sxs-lookup"><span data-stu-id="79ce2-103">Below is the **by-design sending limits** enforced in the service.</span></span> <span data-ttu-id="79ce2-104">Altre informazioni si questi limiti sono disponibili [qui](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span><span class="sxs-lookup"><span data-stu-id="79ce2-104">More information on these limits is documented [here](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span></span>

- <span data-ttu-id="79ce2-105">Per scoraggiare l'invio di messaggi in blocco indesiderati, vengono applicati **limiti al numero di destinatari per ogni utente in relazione a tutti i messaggi esterni e interni**.</span><span class="sxs-lookup"><span data-stu-id="79ce2-105">To discourage the delivery of unsolicited bulk messages, we apply per-user **recipient rate limits to all outbound and internal messages**.</span></span> <span data-ttu-id="79ce2-106">Per tutte le SKU, il limite è di **10.000 destinatari al giorno**.</span><span class="sxs-lookup"><span data-stu-id="79ce2-106">Across all SKUs, this limit is **10,000 recipients per day**.</span></span>  <span data-ttu-id="79ce2-107">Per gli utenti che hanno l'esigenza di inviare messaggi di posta commerciale in blocco legittima (ad esempio, le newsletter ai clienti), è consigliabile continuare a utilizzare provider di terze parti specializzati in tali servizi.</span><span class="sxs-lookup"><span data-stu-id="79ce2-107">Customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.</span></span>
    - <span data-ttu-id="79ce2-108">**Nota**: al raggiungimento del limite massimo, non è possibile inviare ulteriori messaggi dalla cassetta postale fino a quando il numero di destinatari a cui sono stati inviati messaggi nelle ultime 24 ore non scende al di sotto del limite.</span><span class="sxs-lookup"><span data-stu-id="79ce2-108">**Note**: Once the recipient rate limit is reached, messages can't be sent from the mailbox until the number of recipients that were sent messages in the past 24 hours drops below the limit.</span></span> <span data-ttu-id="79ce2-109">L'utente non potrà inviare messaggi fino a quel momento.</span><span class="sxs-lookup"><span data-stu-id="79ce2-109">The user will not be able to send messages until that point.</span></span>
- <span data-ttu-id="79ce2-110">Il limite di frequenza dei messaggi di **30 messaggi al minuto** è applicato in tutte le SKU.</span><span class="sxs-lookup"><span data-stu-id="79ce2-110">Message rate limit of **30 messages per minute** is applied across all SKUs.</span></span> <span data-ttu-id="79ce2-111">Questo consente di determinare il numero massimo di messaggi che un utente può inviare dal proprio account Exchange Online in un determinato periodo di tempo.</span><span class="sxs-lookup"><span data-stu-id="79ce2-111">This determines how many messages a user can send from their Exchange Online account within a specified period.</span></span>
- <span data-ttu-id="79ce2-112">Il **numero massimo di destinatari che possono essere inseriti nei campi A:, Cc: e Bcc:** di ciascun messaggio è **1.000** in tutte le SKU.</span><span class="sxs-lookup"><span data-stu-id="79ce2-112">The **maximum number of recipients allowed in the To, Cc, and Bcc** fields for a single email message, across all SKUs, is **1000 recipients**.</span></span> <span data-ttu-id="79ce2-113">Per personalizzare tale limite, fare clic [qui](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span><span class="sxs-lookup"><span data-stu-id="79ce2-113">To customize this limit, go [here](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span></span>
