---
title: 1332 OWA - Le regole di Posta in arrivo non sono in esecuzione per una cassetta postale
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: b05ed9f0ee8c18b49b5338c53e67a79f1bf65464385dfa0ebd0639172a1b18f2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54040906"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>Una regola di Posta in arrivo non funziona come previsto

Verificare le impostazioni seguenti in Outlook sul web:

- Un messaggio può essere reindirizzato, inoltrato o risposto automaticamente in base alle regole di Posta in arrivo una sola volta. Una regola di reindirizzamento (una regola di posta in arrivo o una regola del flusso di posta, nota anche come regola di trasporto) può aggiungere un massimo di dieci destinatari di inoltro a un messaggio. Per ulteriori informazioni, vedere Limiti delle regole di [Journal, Transport e Inbox](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).

- Le regole di Posta in arrivo non funzionano nella cassetta del journaling alternativa. Per ulteriori informazioni sulla cassetta del journaling alternativa, vedere [Cassetta del journaling alternativa.](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox)

Per risolvere questi problemi, vedere [KB 2829319](https://support.microsoft.com/kb/2829319).

Se i problemi precedenti non si applicano, eseguire il rapporto di diagnostica delle regole di Posta in arrivo prima di inoltrare il problema al supporto tecnico Microsoft:

1. Aprire la cassetta postale in Outlook sul web e fare clic su <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 **Impostazioni**  >  **Visualizza tutte le Outlook Impostazioni**  >  **Posta**  >  **Regole**.

2. Nella parte inferiore della pagina fare clic su Se le regole **non funzionano fare clic qui per generare un report di diagnostica.**
