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
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Errore durante l'invio di posta elettronica: host client bloccato tramite Spamhaus

L'indirizzo IP che ha inviato il messaggio si trova in un elenco di blocco di proprietà di [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Per motivi di blocco da parte di Spamhaus sono inclusi gli account compromessi, le macchine compromesse che condividono un indirizzo IP pubblico e i criteri provider di servizi Internet (ISP). Le possibili correzioni sono:
  
- Per i messaggi in ingresso bloccati in cui è possibile controllare il server di posta elettronica di origine, è necessario determinare la causa e rimuovere il blocco dal sito Web Spamhaus.

- Per i messaggi in ingresso bloccati in cui l'indirizzo IP di origine appartiene a un altro utente, il proprietario dell'indirizzo deve rimuovere il blocco dal sito Web Spamhaus. Se l'indirizzo IP è presente nell'elenco dei criteri di blocco (PBL), il proprietario può assegnare un indirizzo IP statico diverso o rimuovere l'indirizzo dall'PBL.

- Per i messaggi in uscita bloccati dal dominio connesso a Microsoft, è possibile che venga visualizzato questo errore se i messaggi vengono instradati tramite un servizio di terze parti. È possibile utilizzare uno strumento di ricerca WHOIS per trovare il proprietario dell'indirizzo IP bloccato.
