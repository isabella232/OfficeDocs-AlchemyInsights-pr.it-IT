---
title: Conversione della cassetta postale utente in una cassetta postale condivisa?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Normal
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: ab34b8939b95b29bedb797f640dd744bc783adef
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36496439"
---
# <a name="convert-a-user-mail-box-into-a-shared-mailbox"></a>Convertire una casella di posta utente in una cassetta postale condivisa

È possibile convertire una cassetta postale utente in una cassetta postale condivisa solo se l'utente dispone di una licenza di Exchange. Una volta convertita, la cassetta postale continuerà a essere visualizzata nell'elenco utenti attivi, poiché tale elenco include le cassette postali condivise. Tuttavia, la cassetta postale convertita verrà visualizzata anche nell'elenco delle cassette postali condivise. 
  
Se si tenta di convertire una cassetta postale nella console di amministrazione di Exchange e la conversione ha esito negativo, cancellare la cache del browser e i cookie e riprovare. Se ancora non funziona, provare a convertire la cassetta postale in Exchange Management Shell eseguendo il comando riportato di seguito:
  
```
Set-Mailbox -Type Shared
```

Ulteriori informazioni sulla conversione delle cassette postali sono disponibili in [convertire una cassetta postale utente in una cassetta postale condivisa](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox).
  
