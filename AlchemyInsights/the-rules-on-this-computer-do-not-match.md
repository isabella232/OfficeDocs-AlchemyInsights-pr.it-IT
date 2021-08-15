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
ms.openlocfilehash: b77573e9d94195e1f0ef4a1566c45a30d53b7e68e502aeb834e2ca5b9e6c5c76
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53981117"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>Errore: le regole del computer non corrispondono

Per visualizzare lo stato aggiornato di questo problema noto, vedere Le regole in [questo computer non corrispondono alle regole in Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)

Il Outlook Team ha implementato una correzione nella build 12928.10000. La correzione è già disponibile in Insider Fast e verrà passata al Canale mensile alla fine di giugno 2020. Una volta che hai la build fissa, potresti ricevere il prompt "Quali regole vuoi mantenere" un'ultima volta. Scegliere Server quando richiesto, quindi tornare a Outlook e abilitare di nuovo tutte le regole disabilitate.

Fino a quando la correzione non è disponibile, utilizzare la soluzione alternativa seguente:

**Soluzione:** nei report recenti, il problema si è verificato per quelli che hanno creato solo regole client in Outlook desktop. Se il problema persiste, è consigliabile eliminare le regole e quindi creare e modificare le regole solo in OWA (Outlook Web App) finché il problema non viene risolto.

Se non è possibile eliminare manualmente le regole, è possibile eseguire un comando Outlook all'avvio Outlook eseguendo Outlook.exe /cleanrules. In questo modo verranno eliminate sia le regole client che le regole del server. Verranno eliminate tutte le regole per tutti gli account nel Outlook profilo. Questo comando è ulteriormente documentato nell'articolo Opzioni della riga di comando.

