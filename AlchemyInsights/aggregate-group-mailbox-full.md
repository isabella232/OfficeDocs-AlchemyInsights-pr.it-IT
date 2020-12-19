---
title: AggregateGroupMailbox di mancato recapito completo ricevuto per la posta elettronica inviata al gruppo Microsoft 365
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
ms.openlocfilehash: 9de09ab4cbd2f09648305b11da6273ed990907cf
ms.sourcegitcommit: 2ffdf6096de5608b117c6677d3cd7dd4c23ea024
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/18/2020
ms.locfileid: "49715697"
---
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a>AggregateGroupMailbox di mancato recapito completo ricevuto per la posta elettronica inviata al gruppo Microsoft 365

Utilizzare il seguente comando EXO Shell per creare una regola di trasporto di Exchange per eliminare automaticamente i messaggi di posta elettronica inviati alla cassetta postale di aggregazione del gruppo:

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

> [!NOTE]
> Sostituire l'indirizzo SMTP in **-SentTo** con l'indirizzo SMTP della cassetta postale del gruppo di aggregazione nel tenant. È possibile ottenere l'indirizzo SMTP della cassetta postale del gruppo di aggregazione dal rapporto di mancato recapito ricevuto.



