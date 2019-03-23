---
title: Errore durante l'invio di messaggi di posta elettronica bloccati da SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 7d6ad2667613ae948a4abcefafe8d91cf89d2418
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/22/2019
ms.locfileid: "30761637"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="86558-102">Errore durante l'invio di posta elettronica: host client bloccato tramite Spamhaus</span><span class="sxs-lookup"><span data-stu-id="86558-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="86558-103">L'indirizzo IP che ha inviato il messaggio si trova in un elenco di blocco di proprietà di [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span><span class="sxs-lookup"><span data-stu-id="86558-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="86558-104">Per motivi di blocco da parte di Spamhaus sono inclusi gli account compromessi, le macchine compromesse che condividono un indirizzo IP pubblico e i criteri provider di servizi Internet (ISP).</span><span class="sxs-lookup"><span data-stu-id="86558-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="86558-105">Le possibili correzioni sono:</span><span class="sxs-lookup"><span data-stu-id="86558-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="86558-106">Per i messaggi in ingresso bloccati in Office 365 in cui è possibile controllare il server di posta elettronica di origine, è necessario determinare la causa e rimuovere il blocco dal sito Web Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="86558-106">For blocked inbound messages to Office 365 where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>
    
- <span data-ttu-id="86558-107">Per i messaggi in ingresso bloccati in Office 365 in cui l'indirizzo IP di origine appartiene a un altro utente, il proprietario dell'indirizzo deve rimuovere il blocco dal sito Web Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="86558-107">For blocked inbound messages to Office 365 where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="86558-108">Se l'indirizzo IP è presente nell'elenco dei criteri di blocco (PBL), il proprietario può assegnare un indirizzo IP statico diverso o rimuovere l'indirizzo dall'PBL.</span><span class="sxs-lookup"><span data-stu-id="86558-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>
    
- <span data-ttu-id="86558-109">Per i messaggi in uscita bloccati dal dominio di Office 365, è possibile che venga visualizzato questo errore se i messaggi vengono instradati tramite un servizio di terze parti.</span><span class="sxs-lookup"><span data-stu-id="86558-109">For blocked outbound messages from your Office 365 domain, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="86558-110">È possibile utilizzare uno strumento di ricerca WHOIS per trovare il proprietario dell'indirizzo IP bloccato.</span><span class="sxs-lookup"><span data-stu-id="86558-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
    

