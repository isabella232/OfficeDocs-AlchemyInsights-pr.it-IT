---
title: 'Errore: le regole del computer non corrispondono'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c46eb856baafbef9bc3b7fa34a0258ef16923fb8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782956"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>Errore: le regole del computer non corrispondono

Per visualizzare lo stato aggiornato di questo problema noto, vedere Le regole in [questo computer non corrispondono alle regole in Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)

Il team di Outlook ha implementato una correzione nella build 12928.10000. La correzione è già disponibile in Insider Fast e verrà passata al Canale mensile alla fine di giugno 2020. Una volta che hai la build fissa, potresti ricevere il prompt "Quali regole vuoi mantenere" un'ultima volta. Scegliere Server quando richiesto, quindi tornare in Outlook e ri abilitare tutte le regole disabilitate.

Fino a quando la correzione non è disponibile, utilizzare la soluzione alternativa seguente:

**Soluzione:** nei report recenti, il problema si è verificato per quelli che hanno creato solo regole client nel desktop di Outlook. Se il problema persiste, è consigliabile eliminare le regole e quindi creare e modificare le regole solo in OWA (Outlook Web App) finché il problema non viene risolto.

Se non è possibile eliminare manualmente le regole, è possibile eseguire un comando di Outlook all'avvio di Outlook eseguendo Outlook.exe /cleanrules. In questo modo verranno eliminate sia le regole client che le regole del server. Verranno eliminate tutte le regole per tutti gli account nel profilo di Outlook. Questo comando è ulteriormente documentato nell'articolo Opzioni della riga di comando.

