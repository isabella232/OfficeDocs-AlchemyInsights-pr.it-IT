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
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/15/2019
ms.locfileid: "28296601"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Errore durante l'invio di posta elettronica: Client host bloccato utilizzando Spamhaus

L'indirizzo IP che ha inviato il messaggio è in un elenco di blocco e di proprietà di [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Motivi per cui viene bloccato da Spamhaus includono gli account compromessi, esposto a possibili violazioni macchine la condivisione di un indirizzo IP pubblico e criteri di Provider di servizi Internet (ISP). Correzioni possibili sono:
  
- Per i messaggi in ingresso bloccati a cui è possibile controllare il server di posta elettronica di origine di Office 365, è necessario determinare la causa e rimuovere il blocco dal sito Web Spamhaus.
    
- Per i messaggi in ingresso bloccati a cui appartiene l'indirizzo IP di origine a un utente di Office 365, è necessario rimuovere il blocco dal sito Web Spamhaus il proprietario dell'indirizzo. Se l'indirizzo IP nel criterio di blocco di elenco (PBL), il proprietario può si assegna un indirizzo IP statico diverso o rimuovere l'indirizzo dal PBL.
    
- Per i messaggi in uscita bloccati dal dominio Office 365, è possibile ricevere questo errore se i messaggi vengono instradati attraverso un servizio di terze parti 3. È possibile utilizzare uno strumento di ricerca WHOIS per trovare il proprietario di indirizzi IP bloccato.
    

