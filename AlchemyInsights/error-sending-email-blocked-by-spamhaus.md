---
title: Errore durante l'invio di posta elettronica bloccato da SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: a16c998d2f289ea2da52454819f6677c405381a1
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/24/2019
ms.locfileid: "29475643"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="3808e-102">Errore durante l'invio di posta elettronica: Client host bloccato utilizzando Spamhaus</span><span class="sxs-lookup"><span data-stu-id="3808e-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="3808e-p101">L'indirizzo IP che ha inviato il messaggio è in un elenco di blocco e di proprietà di [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Motivi per cui viene bloccato da Spamhaus includono gli account compromessi, esposto a possibili violazioni macchine la condivisione di un indirizzo IP pubblico e criteri di Provider di servizi Internet (ISP). Correzioni possibili sono:</span><span class="sxs-lookup"><span data-stu-id="3808e-p101">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies. Possible fixes are:</span></span>
  
- <span data-ttu-id="3808e-106">Per i messaggi in ingresso bloccati a cui è possibile controllare il server di posta elettronica di origine di Office 365, è necessario determinare la causa e rimuovere il blocco dal sito Web Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="3808e-106">For blocked inbound messages to Office 365 where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>
    
- <span data-ttu-id="3808e-p102">Per i messaggi in ingresso bloccati a cui appartiene l'indirizzo IP di origine a un utente di Office 365, è necessario rimuovere il blocco dal sito Web Spamhaus il proprietario dell'indirizzo. Se l'indirizzo IP nel criterio di blocco di elenco (PBL), il proprietario può si assegna un indirizzo IP statico diverso o rimuovere l'indirizzo dal PBL.</span><span class="sxs-lookup"><span data-stu-id="3808e-p102">For blocked inbound messages to Office 365 where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website. If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>
    
- <span data-ttu-id="3808e-p103">Per i messaggi in uscita bloccati dal dominio Office 365, è possibile ricevere questo errore se i messaggi vengono instradati attraverso un servizio di terze parti 3. È possibile utilizzare uno strumento di ricerca WHOIS per trovare il proprietario di indirizzi IP bloccato.</span><span class="sxs-lookup"><span data-stu-id="3808e-p103">For blocked outbound messages from your Office 365 domain, you can receive this error if the messages are routed through a 3rd party service. You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
    

