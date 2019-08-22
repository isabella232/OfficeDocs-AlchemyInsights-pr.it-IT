---
title: 1336 cartella RecoverableItems piena
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 8a5859ba29d847606e8b44d169c3cd6a26364744
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36509745"
---
# <a name="the-recoverable-items-folder-is-full"></a>La cartella elementi ripristinabili è piena

Per le cassette postali di Exchange online in Office 365, il limite di archiviazione predefinito per la cartella elementi ripristinabili è 30 GB. Il limite di archiviazione per la cartella elementi ripristinabili viene automaticamente aumentato a 100 GB se la cassetta postale è impostata su blocco per controversia legale, eDiscovery Hold o viene assegnata a un criterio di conservazione di Office 365.

Quando la cartella elementi ripristinabili raggiunge il limite di archiviazione, la funzionalità delle cassette postali viene modificata nei modi seguenti:

- L'utente non può eliminare gli elementi dalla cassetta postale.

- Assistente cartelle gestite non può eliminare elementi basandosi sul tag di conservazione o sulle impostazioni delle cartelle gestite.

- Per le cassette postali a cui è stato abilitato il ripristino di un singolo elemento o che vengono bloccate, il processo di protezione delle pagine copy-on-Write non è in grado di gestire le versioni degli elementi modificati dall'utente

- Per le cassette postali in cui è abilitata la registrazione di controllo delle cassette postali, non è possibile salvare le voci del registro di controllo della cassetta postale nella cartella elementi ripristinabili.

Per le cassette postali che non sono in attesa, gli `Search-Mailbox -SearchDumpsterOnly -DeleteContent` amministratori possono utilizzare il comando in PowerShell di Exchange Online per eliminare gli elementi nella cartella elementi ripristinabili. Per ulteriori informazioni, vedere i seguenti argomenti:

- [Cercare ed eliminare i messaggi](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)

- [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

Per le cassette postali che sono in attesa, gli amministratori devono rimuovere il blocco prima che possano eliminare gli elementi dalla cartella elementi ripristinabili. Per ulteriori informazioni, vedere [eliminare gli elementi nella cartella elementi ripristinabili delle cassette postali basate sul cloud in attesa](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).

Per evitare che la cartella elementi ripristinabili diventi completa, gli amministratori possono aumentare il limite di archiviazione della cartella elementi ripristinabili per le cassette postali in attesa e impostare un criterio di conservazione delle cassette postali che sposta gli elementi dalla cartella elementi ripristinabili all'archivio dell'utente cassetta postale. Vedere [aumentare la quota degli elementi ripristinabili per le cassette postali in blocco](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
