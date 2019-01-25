---
title: La cartella RecoverableItems 1336 è piena
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: ee96abfa179c36ebaf43dbd327d4608b849395d3
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/24/2019
ms.locfileid: "29475850"
---
# <a name="the-recoverable-items-folder-is-full"></a>La cartella elementi ripristinabili è piena

Per cassette postali di Exchange Online in Office 365, il limite di archiviazione predefinito per la cartella elementi ripristinabili è 30 GB. Il limite di archiviazione per la cartella elementi recuperabili viene aumentato a 100 GB automaticamente se la cassetta postale viene messa in attesa di conservazione per controversia, esenzione di eDiscovery, o viene assegnata a un criterio di conservazione di Office 365.
  
Quando la cartella elementi ripristinabili raggiunge il limite di archiviazione, la funzionalità cassette postali interessata nei modi seguenti:
  
- L'utente non può eliminare gli elementi dalla cassetta postale.
    
- Assistente cartelle gestite non può eliminare elementi basandosi sul tag di conservazione o sulle impostazioni delle cartelle gestite.
    
- Per le cassette postali che dispongono di ripristino di un elemento singolo abilitato o messa in attesa, processo di protezione della pagina copia in scrittura non può mantenere le versioni di elementi modificati dall'utente.
    
- Per le cassette postali con cassetta postale abilitata la registrazione di controllo, nessuna voce di registro di controllo delle cassette postali possono essere salvata nella sottocartella audit nella cartella elementi ripristinabili.
    
Per le cassette postali che non sono in attesa, gli amministratori possono usare il `Search-Mailbox -SearchDumpsterOnly -DeleteContent` comando in Exchange Online PowerShell per eliminare gli elementi nella cartella elementi ripristinabili. Per ulteriori informazioni, vedere gli argomenti seguenti: 
  
- [Cercare ed eliminare i messaggi](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)
    
- [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)
    
Per le cassette postali che sono in attesa, è necessario rimuovere la conservazione prima che è possibile gli elementi eliminati dalla cartella elementi ripristinabili admins. Per ulteriori informazioni, vedere [eliminazione di elementi nella cartella delle cassette postali basate su cloud in attesa agli elementi ripristinabili](https://docs.microsoft.com/en-us/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).
  
Per evitare la cartella elementi recuperabili di diventare completa, gli amministratori possono aumentare il limite di archiviazione degli elementi recuperabili cartella delle cassette postali in attesa e configurare un criterio di conservazione delle cassette postali che sposta gli elementi dalla cartella elementi ripristinabili archivio dell'utente cassetta postale. Vedere [aumentare la quota per le cassette postali in attesa agli elementi ripristinabili](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
  

