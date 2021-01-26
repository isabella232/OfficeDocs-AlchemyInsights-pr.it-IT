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
# <a name="your-archive-mailbox-is-almost-full"></a>La cassetta postale di archiviazione è quasi completa

Se l'utente riceve l'avviso; **La cassetta postale di archiviazione è quasi piena** oppure è necessario aumentare le dimensioni della cassetta postale di archiviazione, ecco alcuni suggerimenti:

1. Se all'utente viene assegnato un Exchange Online piano 1, eseguire l'aggiornamento a **Exchange Online piano 2** per aumentare la dimensione da 50 GB a $100.
1. Se all'utente è già stata assegnata una delle operazioni seguenti: **Exchange Online piano 2** o Exchange Online, piano 1 con un componente aggiuntivo di archiviazione Exchange Online, utilizzare i passaggi riportati di seguito per abilitare l'archiviazione in espansione automatica:.
 
    1. [Connettersi a PowerShell di Exchange Online](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).
    2. Eseguire le seguenti cmdlet sharepointsync per l'utente:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    1. Eseguire il seguente cmdlet sharepointsync per confermare che sia abilitato per l'utente:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

Per ulteriori informazioni, vedere:

- [ Abilitare l'archiviazione illimitata-guida per gli amministratori-Microsoft 365 Compliance | Documenti Microsoft](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [Limiti di Exchange Online-descrizioni dei servizi | Documenti Microsoft](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [Eseguire l'aggiornamento a un piano aziendale diverso | Documenti Microsoft](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

