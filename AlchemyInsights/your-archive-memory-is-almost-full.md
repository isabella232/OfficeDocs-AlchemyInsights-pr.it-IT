---
title: La cassetta postale di archiviazione è quasi piena
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
ms.openlocfilehash: 085d9b211d5a8e9a0e1eb12af14d87a4e59c844a3afa012095dfd60db316ad14
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046756"
---
# <a name="your-archive-mailbox-is-almost-full"></a>La cassetta postale di archiviazione è quasi piena

Se l'utente riceve l'avviso; **La cassetta postale di archiviazione è quasi piena** o è necessario aumentare le dimensioni della cassetta postale di archiviazione, ecco alcuni suggerimenti:

1. Se all'utente viene assegnata una licenza Exchange Online Piano 1, eseguire l'aggiornamento alla licenza **Exchange Online Piano 2** per aumentare le dimensioni da 50 GB a 100 GB.
1. Se all'utente è già assegnato uno dei seguenti elementi: **Exchange Online Piano 2** o piano 1 di Exchange Online con un componente aggiuntivo Archiviazione Exchange Online, eseguire la procedura seguente per abilitare l'archiviazione con espansione automatica:.
 
    1. [Connessione per Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).
    2. Eseguire il seguente commandlet per l'utente:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    1. Eseguire il seguente commandlet per verificare che sia abilitato per l'utente:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

Per ulteriori informazioni consulta:

- [Abilitare l'archiviazione illimitata - Guida per gli amministratori - Microsoft 365 conformità | Documenti Microsoft](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [Exchange Online - Descrizioni dei servizi | Documenti Microsoft](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [Eseguire l'aggiornamento a un piano aziendale diverso | Documenti Microsoft](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

