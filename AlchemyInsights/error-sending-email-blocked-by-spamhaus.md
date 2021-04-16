---
title: Errore durante l'invio di messaggi di posta elettronica bloccati da SpamHaus
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 8b5ac1df0b6a07a475345235a8b4b555d6881147
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813728"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="d904d-102">Errore durante l'invio della posta elettronica: host client bloccato tramite Spamhaus</span><span class="sxs-lookup"><span data-stu-id="d904d-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="d904d-103">L'indirizzo IP che ha inviato il messaggio si trova in un elenco di blocco di proprietà di [Spamhaus.](https://go.microsoft.com/fwlink/p/?linkid=123245)</span><span class="sxs-lookup"><span data-stu-id="d904d-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="d904d-104">I motivi del blocco da parte di Spamhaus includono account compromessi, computer compromessi che condividono un indirizzo IP pubblico e criteri isp (Internet Service Provider).</span><span class="sxs-lookup"><span data-stu-id="d904d-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="d904d-105">Le possibili correzioni sono:</span><span class="sxs-lookup"><span data-stu-id="d904d-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="d904d-106">Per i messaggi in ingresso bloccati in cui si controlla il server di posta elettronica di origine, è necessario determinare la causa e rimuovere il blocco dal sito Web Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="d904d-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="d904d-107">Per i messaggi in ingresso bloccati in cui l'indirizzo IP di origine appartiene a un altro utente, il proprietario dell'indirizzo deve rimuovere il blocco dal sito Web Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="d904d-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="d904d-108">Se l'indirizzo IP si trova nell'elenco dei criteri di blocco (PBL), il proprietario può assegnare un indirizzo IP statico diverso o rimuovere l'indirizzo dal PBL.</span><span class="sxs-lookup"><span data-stu-id="d904d-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="d904d-109">Per i messaggi in uscita bloccati dal dominio connesso a Microsoft, è possibile ricevere questo errore se i messaggi vengono instradati tramite un servizio di terze parti.</span><span class="sxs-lookup"><span data-stu-id="d904d-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="d904d-110">È possibile utilizzare uno strumento di ricerca WHOIS per trovare il proprietario dell'indirizzo IP bloccato.</span><span class="sxs-lookup"><span data-stu-id="d904d-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
