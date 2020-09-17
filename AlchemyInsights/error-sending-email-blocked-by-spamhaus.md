---
title: Errore durante l'invio di messaggi di posta elettronica bloccati da SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: a0c2f4be0b2d8ba6fd3dadbdf306e6ce623ad380
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783807"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="2cc5e-102">Errore durante l'invio di posta elettronica: host client bloccato tramite Spamhaus</span><span class="sxs-lookup"><span data-stu-id="2cc5e-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="2cc5e-103">L'indirizzo IP che ha inviato il messaggio si trova in un elenco di blocco di proprietà di [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span><span class="sxs-lookup"><span data-stu-id="2cc5e-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="2cc5e-104">Per motivi di blocco da parte di Spamhaus sono inclusi gli account compromessi, le macchine compromesse che condividono un indirizzo IP pubblico e i criteri provider di servizi Internet (ISP).</span><span class="sxs-lookup"><span data-stu-id="2cc5e-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="2cc5e-105">Le possibili correzioni sono:</span><span class="sxs-lookup"><span data-stu-id="2cc5e-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="2cc5e-106">Per i messaggi in ingresso bloccati in cui è possibile controllare il server di posta elettronica di origine, è necessario determinare la causa e rimuovere il blocco dal sito Web Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="2cc5e-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="2cc5e-107">Per i messaggi in ingresso bloccati in cui l'indirizzo IP di origine appartiene a un altro utente, il proprietario dell'indirizzo deve rimuovere il blocco dal sito Web Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="2cc5e-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="2cc5e-108">Se l'indirizzo IP è presente nell'elenco dei criteri di blocco (PBL), il proprietario può assegnare un indirizzo IP statico diverso o rimuovere l'indirizzo dall'PBL.</span><span class="sxs-lookup"><span data-stu-id="2cc5e-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="2cc5e-109">Per i messaggi in uscita bloccati dal dominio connesso a Microsoft, è possibile che venga visualizzato questo errore se i messaggi vengono instradati tramite un servizio di terze parti.</span><span class="sxs-lookup"><span data-stu-id="2cc5e-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="2cc5e-110">È possibile utilizzare uno strumento di ricerca WHOIS per trovare il proprietario dell'indirizzo IP bloccato.</span><span class="sxs-lookup"><span data-stu-id="2cc5e-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
