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
ms.openlocfilehash: 8372032e19bd2ebaf3ba8cc8e87f19ef3e2edf1e607b1739a919f6dcc443cd97
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946750"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Errore durante l'invio della posta elettronica: host client bloccato tramite Spamhaus

L'indirizzo IP che ha inviato il messaggio si trova in un elenco di blocco di proprietà di [Spamhaus.](https://go.microsoft.com/fwlink/p/?linkid=123245) I motivi del blocco da parte di Spamhaus includono account compromessi, computer compromessi che condividono un indirizzo IP pubblico e criteri isp (Internet Service Provider). Le possibili correzioni sono:
  
- Per i messaggi in ingresso bloccati in cui si controlla il server di posta elettronica di origine, è necessario determinare la causa e rimuovere il blocco dal sito Web Spamhaus.

- Per i messaggi in ingresso bloccati in cui l'indirizzo IP di origine appartiene a un altro utente, il proprietario dell'indirizzo deve rimuovere il blocco dal sito Web Spamhaus. Se l'indirizzo IP si trova nell'elenco dei criteri di blocco (PBL), il proprietario può assegnare un indirizzo IP statico diverso o rimuovere l'indirizzo dal PBL.

- Per i messaggi in uscita bloccati dal dominio connesso a Microsoft, è possibile ricevere questo errore se i messaggi vengono instradati tramite un servizio di terze parti. È possibile utilizzare uno strumento di ricerca WHOIS per trovare il proprietario dell'indirizzo IP bloccato.
