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
# <a name="convert-a-user-mail-box-into-a-shared-mailbox"></a><span data-ttu-id="e326f-102">Convertire una casella di posta utente in una cassetta postale condivisa</span><span class="sxs-lookup"><span data-stu-id="e326f-102">Convert a user mail box into a shared mailbox</span></span>

<span data-ttu-id="e326f-103">È possibile convertire una cassetta postale utente in una cassetta postale condivisa solo se l'utente dispone di una licenza di Exchange.</span><span class="sxs-lookup"><span data-stu-id="e326f-103">You can only convert a user mailbox to a shared mailbox if the user has an Exchange license.</span></span> <span data-ttu-id="e326f-104">Una volta convertita, la cassetta postale continuerà a essere visualizzata nell'elenco utenti attivi, poiché tale elenco include le cassette postali condivise.</span><span class="sxs-lookup"><span data-stu-id="e326f-104">After the mailbox is converted, it will continue to show up in the active users list because that list includes shared mailboxes.</span></span> <span data-ttu-id="e326f-105">Tuttavia, la cassetta postale convertita verrà visualizzata anche nell'elenco delle cassette postali condivise.</span><span class="sxs-lookup"><span data-stu-id="e326f-105">However, the converted mailbox will also show up in the shared mailbox list.</span></span> 
  
<span data-ttu-id="e326f-106">Se si tenta di convertire una cassetta postale nella console di amministrazione di Exchange e la conversione ha esito negativo, cancellare la cache del browser e i cookie e riprovare.</span><span class="sxs-lookup"><span data-stu-id="e326f-106">If you try to convert a mailbox in the Exchange Admin Console and the conversion fails, clear your browser cache and cookies and try again.</span></span> <span data-ttu-id="e326f-107">Se ancora non funziona, provare a convertire la cassetta postale in Exchange Management Shell eseguendo il comando riportato di seguito:</span><span class="sxs-lookup"><span data-stu-id="e326f-107">If it still isn't working, try converting the mailbox in the Exchange Management Shell by running the following command:</span></span>
  
```
Set-Mailbox -Type Shared
```

<span data-ttu-id="e326f-108">Ulteriori informazioni sulla conversione delle cassette postali sono disponibili in [convertire una cassetta postale utente in una cassetta postale condivisa](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox).</span><span class="sxs-lookup"><span data-stu-id="e326f-108">More mailbox conversion information is available in [Convert a user mailbox to a shared mailbox](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox).</span></span>
  
