---
title: Recuperare elementi eliminati con cmdlet
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800008"
- "5718"
ms.openlocfilehash: d8f2a50f39d7bcd321692ab093e2efa6613e9814
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51835815"
---
# <a name="recover-deleted-items-with-cmdlet"></a><span data-ttu-id="505bb-102">Recuperare elementi eliminati con cmdlet</span><span class="sxs-lookup"><span data-stu-id="505bb-102">Recover deleted items with cmdlet</span></span>

- <span data-ttu-id="505bb-103">Utilizzare il cmdlet [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps)per visualizzare gli elementi eliminati nelle cassette postali.</span><span class="sxs-lookup"><span data-stu-id="505bb-103">Use the [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) cmdlet to view deleted items in mailboxes.</span></span> <span data-ttu-id="505bb-104">Dopo aver individuato gli elementi eliminati, utilizzare il cmdlet [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) per ripristinarli.</span><span class="sxs-lookup"><span data-stu-id="505bb-104">After you find the deleted items, you use the [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) cmdlet to restore them.</span></span>

- <span data-ttu-id="505bb-105">Per informazioni dettagliate, vedere [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="505bb-105">See full details in [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span></span>

- <span data-ttu-id="505bb-106">All'utente deve essere assegnato il ruolo di Importazione/Esportazione cassette postali, prima di eseguire il cmdlet.</span><span class="sxs-lookup"><span data-stu-id="505bb-106">You need to be assigned the Mailbox Import Export role before you can run this cmdlet.</span></span> <span data-ttu-id="505bb-107">Per altre informazioni, vedere [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="505bb-107">Please see [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) for more information.</span></span>
