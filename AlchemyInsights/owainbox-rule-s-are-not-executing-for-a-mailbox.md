---
title: 1332 OWA-la regola di posta in arrivo non è in esecuzione per una cassetta postale
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 9abdcdcb33d39b8b9fe2df80f0c15a8b55e465fd
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/05/2020
ms.locfileid: "44576564"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>Una regola di posta in arrivo non funziona come previsto

Verificare le impostazioni seguenti in Outlook sul Web:

- Un messaggio può essere reindirizzato, inoltrato o risposto automaticamente in base alle regole della posta in arrivo solo una volta. Una regola di reindirizzamento (una regola di posta in arrivo o una regola del flusso di posta, nota anche come regola di trasporto) può aggiungere un massimo di dieci destinatari di inoltro a un messaggio. Per ulteriori informazioni, vedere [Journal, Transport, and Inbox Rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).

- Le regole di posta in arrivo non funzionano nella cassetta postale di inserimento nel journal alternativa. Per ulteriori informazioni sulla cassetta postale di inserimento nel journal alternativa, vedere [cassetta del journaling alternativa](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).

Per risolvere questi problemi, vedere [KB 2829319](https://support.microsoft.com/kb/2829319).

Se non si applicano i problemi precedenti, eseguire il rapporto di diagnostica della regola di posta in arrivo prima di inoltrare il problema al supporto tecnico Microsoft:

1. Aprire la cassetta postale in Outlook sul Web e fare clic su <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 **Impostazioni**  >  di **Visualizzazione di tutte le impostazioni**  >  di Outlook **Posta elettronica**  >  **Regole**.

2. Nella parte inferiore della pagina fare clic su **se le regole non funzionano, fare clic qui per generare un rapporto di diagnostica**.
