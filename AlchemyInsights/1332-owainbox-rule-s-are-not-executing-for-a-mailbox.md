---
title: 1332 OWA - regole posta in arrivo non vengono eseguiti per una cassetta postale
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: f090d0a9d84bc6a4d1a1f4c0af55102d4b0ddfbe
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/15/2019
ms.locfileid: "28296703"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>Una regola di posta in arrivo non funziona come previsto

Verificare le impostazioni seguenti:
  
- Un messaggio può essere reindirizzato, inoltrato o di risposta per automaticamente in base alle regole posta in arrivo una sola volta. Una regola di reindirizzare la chiamata (una regola di posta in arrivo o una regola del flusso di posta, noto anche come una regola di trasporto) è possibile aggiungere un massimo di dieci destinatari inoltro a un messaggio. Per ulteriori informazioni, vedere [limiti delle regole del Journal, trasporto e posta in arrivo](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).
    
- Regole posta in arrivo non funzionano con la cassetta del journaling alternativa. Per ulteriori informazioni sulla cassetta del journaling alternativo, vedere [cassetta del journaling alternativa](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).
    
Per risolvere questi problemi, vedere [2829319 KB](https://support.microsoft.com/kb/2829319).
  
Se non si applicano i problemi precedenti, eseguire il rapporto di diagnostica regola posta in arrivo prima trasformare il problema al supporto Microsoft:
  
1. Aprire la cassetta postale di Outlook sul web e fare clic su **Impostazioni** \> **Opzioni** \> **Organizza posta** \> **regole posta in arrivo**.
    
2. Nella parte inferiore della pagina, fare clic su **se le regole non funzionano fare clic qui per generare un rapporto di diagnostica**.
    

