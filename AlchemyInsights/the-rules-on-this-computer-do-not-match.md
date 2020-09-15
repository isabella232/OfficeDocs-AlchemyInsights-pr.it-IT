---
title: 'Errore: le regole del computer non corrispondono'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c2feb6da651d8b3eb7af6a057335b28d26f9e7f6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690967"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>Errore: le regole del computer non corrispondono

Per visualizzare lo stato aggiornato di questo problema noto, vedere [le regole in questo computer non corrispondono alle regole di Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)

Il team di Outlook ha implementato una correzione nella build 12928,10000. La correzione è già in Insider Fast e passerà a Monthly Channel alla fine di giugno 2020. Dopo aver creato la build fissa, è possibile che venga visualizzato il messaggio "quali regole si desidera mantenere" un'ultima volta. Quando viene richiesto, scegliere Server e quindi tornare indietro in Outlook e riattivare le regole disabilitate.

Fino a quando non è disponibile la correzione, utilizzare la soluzione seguente:

**Soluzione**: nei rapporti recenti, si è verificato il problema per gli utenti che hanno creato solo le regole client in Outlook desktop. Se si continua a eseguire il problema, prendere in considerazione l'eliminazione delle regole e quindi creare e modificare le regole solo in OWA (Outlook Web App) fino a quando il problema non viene risolto.

Se non è possibile eliminare le regole manualmente, è possibile eseguire un comando di Outlook quando si avvia Outlook eseguendo Outlook.exe/cleanrules. Questo eliminerà sia le regole client che quelle del server. Eliminerà tutte le regole per tutti gli account nel profilo di Outlook. Questo comando è ulteriormente documentato nell'articolo delle opzioni della riga di comando.

