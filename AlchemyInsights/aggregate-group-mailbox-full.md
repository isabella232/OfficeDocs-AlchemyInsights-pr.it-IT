---
title: AggregateGroupMailbox rapporto di mancato recapito completo ricevuto per la posta elettronica inviata Microsoft 365 gruppo
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004286"
- "7656"
ms.openlocfilehash: 6655bbe9482400eeb3cfdf0b91bdc595e3d98fbff0f6d9244db8bb4dd958305e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951857"
---
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a>AggregateGroupMailbox rapporto di mancato recapito completo ricevuto per la posta elettronica inviata Microsoft 365 gruppo

Utilizzare il seguente comando exO Shell per creare una regola di Exchange di trasporto per eliminare automaticamente i messaggi di posta elettronica inviati alla cassetta postale di gruppo aggregata:

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

> [!NOTE]
> Sostituire l'indirizzo SMTP in **-SentTo** con l'indirizzo SMTP della cassetta postale del gruppo aggregato nel tenant. È possibile ottenere l'indirizzo SMTP della cassetta postale del gruppo aggregato dal rapporto di mancato recapito ricevuto.



