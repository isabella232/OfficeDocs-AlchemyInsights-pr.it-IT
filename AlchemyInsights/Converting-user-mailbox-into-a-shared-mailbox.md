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
<span data-ttu-id="c9e00-102">È possibile convertire una cassetta postale utente in una cassetta postale condivisa solo se l'utente dispone di una licenza di Exchange.</span><span class="sxs-lookup"><span data-stu-id="c9e00-102">You can only convert a user mailbox to a shared mailbox if the user has an Exchange license.</span></span> <span data-ttu-id="c9e00-103">Una volta convertita, la cassetta postale continuerà a essere visualizzata nell'elenco utenti attivi, poiché tale elenco include le cassette postali condivise.</span><span class="sxs-lookup"><span data-stu-id="c9e00-103">After the mailbox is converted, it will continue to show up in the active users list because that list includes shared mailboxes.</span></span> <span data-ttu-id="c9e00-104">Tuttavia, la cassetta postale convertita verrà visualizzata anche nell'elenco delle cassette postali condivise.</span><span class="sxs-lookup"><span data-stu-id="c9e00-104">However, the converted mailbox will also show up in the shared mailbox list.</span></span> 
  
<span data-ttu-id="c9e00-105">Se si tenta di convertire una cassetta postale nella console di amministrazione di Exchange e la conversione ha esito negativo, cancellare la cache del browser e i cookie e riprovare.</span><span class="sxs-lookup"><span data-stu-id="c9e00-105">If you try to convert a mailbox in the Exchange Admin Console and the conversion fails, clear your browser cache and cookies and try again.</span></span> <span data-ttu-id="c9e00-106">Se ancora non funziona, provare a convertire la cassetta postale in Exchange Management Shell eseguendo il comando riportato di seguito:</span><span class="sxs-lookup"><span data-stu-id="c9e00-106">If it still isn't working, try converting the mailbox in the Exchange Management Shell by running the following command:</span></span>
  
```
Set-Mailbox -Type Shared
```

<span data-ttu-id="c9e00-107">Ulteriori informazioni sulla conversione delle cassette postali sono disponibili in [convertire una cassetta postale utente in una cassetta postale condivisa](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).</span><span class="sxs-lookup"><span data-stu-id="c9e00-107">More mailbox conversion information is available in [Convert a user mailbox to a shared mailbox](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).</span></span>
  
