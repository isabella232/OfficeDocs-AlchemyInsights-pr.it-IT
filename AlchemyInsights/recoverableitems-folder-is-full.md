---
title: 1336 La cartella RecoverableItems è piena
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 5c8d53ceabf2428f3d6d765040f1b789b6bbeda04a22dd7fde0d2d728fd17d93
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54061760"
---
# <a name="the-recoverable-items-folder-is-full"></a>La cartella Elementi ripristinabili è piena

Per Exchange Online cassette postali, il limite di archiviazione predefinito per la cartella Elementi ripristinabili è 30 GB. Il limite di archiviazione per la cartella Elementi ripristinabili viene automaticamente aumentato a 100 GB se la cassetta postale viene messa in conservazione per controversia legale, eDiscovery o è assegnata a un criterio di conservazione.

Quando la cartella Elementi ripristinabili raggiunge il limite di archiviazione, la funzionalità delle cassette postali è influenzata nei modi seguenti:

- L'utente non può eliminare elementi dalla cassetta postale.

- Assistente cartelle gestite non può eliminare elementi basandosi sul tag di conservazione o sulle impostazioni delle cartelle gestite.

- Per le cassette postali in cui il ripristino di un singolo elemento è abilitato o viene messo in attesa, il processo di protezione delle pagine copy-on-write non è in grado di gestire le versioni degli elementi modificati dall'utente.

- Per le cassette postali in cui è abilitata la registrazione di controllo delle cassette postali, non è possibile salvare alcuna voce del registro di controllo delle cassette postali nella sottocartella Controlli nella cartella Elementi ripristinabili.

Per le cassette postali che non sono in attesa, gli amministratori possono utilizzare il comando in Exchange Online PowerShell per eliminare gli elementi `Search-Mailbox -SearchDumpsterOnly -DeleteContent` nella cartella Elementi ripristinabili. Per ulteriori informazioni, vedere i seguenti argomenti:

- [Cercare ed eliminare i messaggi](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

Per le cassette postali in attesa, gli amministratori devono rimuovere il blocco prima di poter eliminare gli elementi dalla cartella Elementi ripristinabili. Per ulteriori informazioni, vedere [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).

Per evitare che la cartella Elementi ripristinabili diventi piena, gli amministratori possono aumentare il limite di archiviazione della cartella Elementi ripristinabili per le cassette postali in attesa e impostare un criterio di conservazione delle cassette postali che sposta gli elementi dalla cartella Elementi ripristinabili alla cassetta postale di archiviazione dell'utente. Vedere [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
