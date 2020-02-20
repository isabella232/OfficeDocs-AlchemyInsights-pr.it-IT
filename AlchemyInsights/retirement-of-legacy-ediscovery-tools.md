---
title: Pensionamento degli strumenti di eDiscovery legacy
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: c4632b52dde579b7d5b2e6e15f1583300a0bd136
ms.sourcegitcommit: a7c17217c170ead24571421baaf5a14f1525b1a6
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 02/20/2020
ms.locfileid: "42157628"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Pensionamento degli strumenti di eDiscovery legacy

Come risultato della nuova e migliorata funzionalità di eDiscovery nel centro conformità di Microsoft 365, nei prossimi mesi verranno ritirati i seguenti strumenti di eDiscovery e commandlets legacy:

- [EDiscovery sul posto](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) e [archiviazioni sul posto](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) nell'interfaccia di amministrazione di Exchange.

- Cmdlet di Exchange Online PowerShell che supportano le archiviazioni sul posto di eDiscovery e sul posto. Questi cmdlet sono identificati in modo collettivo come cmdlet *-MailboxSearch. Sono inclusi i cmdlet seguenti:

    - [New-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Il cmdlet [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) in Exchange Online PowerShell.
- Le operazioni seguenti nell'API dei servizi Web di Exchange:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Office 365 Advanced eDiscovery v 1.0](https://docs.microsoft.com/en-us/microsoft-365/compliance/office-365-advanced-ediscovery)

**Sequenza temporale per la pensione**:
- 2020 aprile 1: non sarà possibile creare nuove ricerche e conservazioni, ma è comunque possibile eseguire, modificare ed eliminare le ricerche esistenti a proprio rischio. Il supporto tecnico Microsoft non supporterà più il eDiscovery sul posto & conserva nell'interfaccia di amministrazione di Exchange.

- 2020 luglio 1: la eDiscovery sul posto & contiene la funzionalità nell'interfaccia di amministrazione di Exchange verrà messa in modalità di sola lettura. Questo significa che sarà possibile rimuovere solo le ricerche e le esenzioni esistenti.

**Per ulteriori informazioni, vedere**:

 - [Eseguire la migrazione delle ricerche e delle esenzioni eDiscovery legacy al centro conformità di Microsoft 365](https://docs.microsoft.com/en-us/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Pensionamento degli strumenti di eDiscovery legacy](https://docs.microsoft.com/en-us/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Domande frequenti su eDiscovery sul posto e sulle archiviazioni sul posto](https://docs.microsoft.com/en-us/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



