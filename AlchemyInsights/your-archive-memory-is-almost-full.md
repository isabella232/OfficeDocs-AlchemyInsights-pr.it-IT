---
title: La cassetta postale di archiviazione è quasi completa
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100006"
- "7960"
ms.openlocfilehash: 5c7081f8991716a8ac72f462c6c7ef88e800ab9c
ms.sourcegitcommit: 6f1af4aed507d4c074c36d77666cf00100efe168
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/25/2021
ms.locfileid: "49950509"
---
# <a name="your-archive-mailbox-is-almost-full"></a><span data-ttu-id="5d397-102">La cassetta postale di archiviazione è quasi completa</span><span class="sxs-lookup"><span data-stu-id="5d397-102">Your archive mailbox is almost full</span></span>

<span data-ttu-id="5d397-103">Se l'utente riceve l'avviso; **La cassetta postale di archiviazione è quasi piena** oppure è necessario aumentare le dimensioni della cassetta postale di archiviazione, ecco alcuni suggerimenti:</span><span class="sxs-lookup"><span data-stu-id="5d397-103">If the user receives the warning; **Your archive mailbox is almost full**, or you need to increase the size of their archive mailbox, here are some tips:</span></span>

1. <span data-ttu-id="5d397-104">Se all'utente viene assegnato un Exchange Online piano 1, eseguire l'aggiornamento a **Exchange Online piano 2** per aumentare la dimensione da 50 GB a $100.</span><span class="sxs-lookup"><span data-stu-id="5d397-104">If the user is assigned an Exchange Online Plan 1, upgrade to **Exchange Online Plan 2** license to increase the size from 50 GB to 100GB.</span></span>
1. <span data-ttu-id="5d397-105">Se all'utente è già stata assegnata una delle operazioni seguenti: **Exchange Online piano 2** o Exchange Online, piano 1 con un componente aggiuntivo di archiviazione Exchange Online, utilizzare i passaggi riportati di seguito per abilitare l'archiviazione in espansione automatica:.</span><span class="sxs-lookup"><span data-stu-id="5d397-105">If the user is already assigned either of the following: **Exchange Online Plan 2** or an Exchange Online Plan 1 with an Exchange Online Archiving add-on, use the steps below to enable Auto-Expanding archiving:.</span></span>
 
    1. <span data-ttu-id="5d397-106">[Connettersi a PowerShell di Exchange Online](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="5d397-106">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).</span></span>
    2. <span data-ttu-id="5d397-107">Eseguire le seguenti cmdlet sharepointsync per l'utente:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span><span class="sxs-lookup"><span data-stu-id="5d397-107">Run the following commandlet for the user:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span></span>
    1. <span data-ttu-id="5d397-108">Eseguire il seguente cmdlet sharepointsync per confermare che sia abilitato per l'utente:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span><span class="sxs-lookup"><span data-stu-id="5d397-108">Run the following commandlet to confirm it is enabled for the user:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span></span>

<span data-ttu-id="5d397-109">Per ulteriori informazioni, vedere:</span><span class="sxs-lookup"><span data-stu-id="5d397-109">For more information see:</span></span>

- [<span data-ttu-id="5d397-110"> Abilitare l'archiviazione illimitata-guida per gli amministratori-Microsoft 365 Compliance | Documenti Microsoft</span><span class="sxs-lookup"><span data-stu-id="5d397-110"> Enable unlimited archiving - Admin Help - Microsoft 365 Compliance | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [<span data-ttu-id="5d397-111">Limiti di Exchange Online-descrizioni dei servizi | Documenti Microsoft</span><span class="sxs-lookup"><span data-stu-id="5d397-111">Exchange Online limits - Service Descriptions | Microsoft Docs</span></span>](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [<span data-ttu-id="5d397-112">Eseguire l'aggiornamento a un piano aziendale diverso | Documenti Microsoft</span><span class="sxs-lookup"><span data-stu-id="5d397-112">Upgrade to a different business plan | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

