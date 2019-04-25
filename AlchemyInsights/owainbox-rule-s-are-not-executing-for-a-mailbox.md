---
title: 1332 OWA-la regola di posta in arrivo non è in esecuzione per una cassetta postale
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1332
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: c0b221b5335254bd0f1eb4b258efa6946376ca12
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32372564"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>Una regola di posta in arrivo non funziona come previsto

Verificare le impostazioni seguenti:

- Un messaggio può essere reindirizzato, inoltrato o risposto automaticamente in base alle regole della posta in arrivo solo una volta. Una regola di reindirizzamento (una regola di posta in arrivo o una regola del flusso di posta, nota anche come regola di trasporto) può aggiungere un massimo di dieci destinatari di inoltro a un messaggio. Per ulteriori informazioni, vedere [Journal, Transport, and Inbox Rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).

- Le regole di posta in arrivo non funzionano nella cassetta postale di inserimento nel journal alternativa. Per ulteriori informazioni sulla cassetta postale di inserimento nel journal alternativa, vedere [cassetta del journalIng alternativa](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).

Per risolvere questi problemi, vedere [KB 2829319](https://support.microsoft.com/kb/2829319).

Se non si applicano i problemi precedenti, eseguire il rapporto di diagnostica della regola di posta in arrivo prima di inoltrare il problema al supporto tecnico Microsoft:

1. Aprire la cassetta postale in Outlook sul Web e fare clic su **Opzioni** \> **Impostazioni** \> per **organizzare** \> **le regole**della posta in arrivo.

2. Nella parte inferiore della pagina fare clic su **se le regole non funzionano, fare clic qui per generare un rapporto di diagnostica**.
