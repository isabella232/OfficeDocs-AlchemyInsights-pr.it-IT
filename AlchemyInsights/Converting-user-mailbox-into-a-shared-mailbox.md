---
title: Conversione delle cassette postali utente in una cassetta postale condivisa?
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
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 02/12/2019
ms.locfileid: "29906736"
---
È possibile convertire una cassetta postale utente a una cassetta postale condivisa solo se l'utente dispone di una licenza di Exchange. Una volta convertita la cassetta postale, continuerà possa essere visualizzata nell'elenco utenti attivi in quanto tale elenco include le cassette postali condivise. Tuttavia, la cassetta postale convertita verrà inoltre visualizzati nell'elenco cassetta postale condivisa. 
  
Se si tenta di convertire una cassetta postale nella Console di amministrazione di Exchange e la conversione non riesce, cancellare la cache del browser e i cookie e riprovare. Se ancora non funziona, provare a eseguire la conversione delle cassette postali in Exchange Management Shell eseguendo il comando seguente:
  
```
Set-Mailbox -Type Shared
```

Ulteriori informazioni sulla conversione di cassetta postale è disponibile in [convertire una cassetta postale utente a una cassetta postale condivisa](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).
  
