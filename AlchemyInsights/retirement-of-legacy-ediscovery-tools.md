---
title: Ritiro degli strumenti legacy di eDiscovery
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 986c78f20e7b8c303c302913d63d817a56ce2896
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51798553"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Ritiro degli strumenti legacy di eDiscovery

Come risultato della nuova e migliorata funzionalità di eDiscovery nel Centro conformità Microsoft 365, i seguenti strumenti e commandlet legacy di eDiscovery verranno ritirati nei prossimi mesi:

- [EDiscovery sul posto](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) e [blocchi sul posto](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) nell'interfaccia di amministrazione di Exchange.

- I cmdlet di PowerShell di Exchange Online che supportano In-Place eDiscovery e In-Place blocchi. Questi cmdlet sono identificati collettivamente come cmdlet *-MailboxSearch. Sono inclusi i cmdlet seguenti:

    - [New-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Il cmdlet [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) in PowerShell di Exchange Online.
- Nell'API dei servizi Web Exchange vengono eseguite le operazioni seguenti:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Advanced eDiscovery v1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Sequenza temporale per il ritiro**:
- **1 luglio 2020** Non è più possibile creare nuove ricerche e blocchi, ma è possibile eseguire, modificare ed eliminare le ricerche esistenti a proprio rischio. Il supporto Microsoft non supporta più In-Place eDiscovery & blocchi nell'interfaccia di amministrazione di Exchange.
    
- **1 ottobre 2020** In-Place funzionalità di eDiscovery & I blocchi nell'interfaccia di amministrazione di Exchange verranno posizionati in modalità di sola lettura, pertanto è possibile rimuovere solo le ricerche e i blocchi esistenti.

**Per ulteriori informazioni, vedere**:

 - [Eseguire la migrazione delle ricerche e dei blocchi legacy di eDiscovery nel Centro conformità Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Ritiro degli strumenti legacy di eDiscovery](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Domande frequenti su In-Place eDiscovery e In-Place blocchi](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



