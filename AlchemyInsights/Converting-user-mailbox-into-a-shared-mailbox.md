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
ms.openlocfilehash: 4da54121763fd33aa111f3bb3c26963cd271dc51
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32374327"
---
È possibile convertire una cassetta postale utente in una cassetta postale condivisa solo se l'utente dispone di una licenza di Exchange. Una volta convertita, la cassetta postale continuerà a essere visualizzata nell'elenco utenti attivi, poiché tale elenco include le cassette postali condivise. Tuttavia, la cassetta postale convertita verrà visualizzata anche nell'elenco delle cassette postali condivise. 
  
Se si tenta di convertire una cassetta postale nella console di amministrazione di Exchange e la conversione ha esito negativo, cancellare la cache del browser e i cookie e riprovare. Se ancora non funziona, provare a convertire la cassetta postale in Exchange Management Shell eseguendo il comando riportato di seguito:
  
```
Set-Mailbox -Type Shared
```

Ulteriori informazioni sulla conversione delle cassette postali sono disponibili in [convertire una cassetta postale utente in una cassetta postale condivisa](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).
  
