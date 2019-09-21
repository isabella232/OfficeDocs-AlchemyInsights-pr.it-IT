---
title: Report del registro di controllo di SharePoint classico
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: af5b3c76b82db13bc89c917247e41fa1d8779b68
ms.sourcegitcommit: d5bf97a0bf0547f36b6da9684ce9f16a13a7749e
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/20/2019
ms.locfileid: "37068027"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>Registri di controllo di SharePoint e OneDrive

**Registri di controllo unificato di SharePoint e OneDrive moderni dalla conformità**

- [Attivazione/disattivazione della registrazione di controllo unificato](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

Non è necessaria alcuna configurazione aggiuntiva all'interno di SharePoint o OneDrive.

- Utilizzare la ricerca della registrazione di controllo per controllare l'attività dei file, delle cartelle, degli utenti, delle autorizzazioni:

    - [Attività di file e pagine](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
    - [Attività cartella](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    - [Attività di condivisione e accesso alle richieste](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
    - [Attività di sincronizzazione](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
    - [Attività amministrative del sito](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)
- Per ulteriori informazioni su come recuperare questi eventi, vedere [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).

**Registri di controllo di SharePoint Classic**

È stata eseguita la migrazione del controllo legacy di SPO al log di controllo unificato (UAL). Questo significa in sostanza che tutti i report di controllo legacy di SPO saranno ora alimentati tramite UAL e i segnali di controllo legacy sono stati migrati a UAL.

Modifiche principali:

- Il taglio come funzionalità non è disponibile.
- La sezione in cui si scelgono gli eventi specifici da controllare non è disponibile. Fare riferimento a [questo documento](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) per un elenco completo degli eventi controllati disponibili per impostazione predefinita.
- L'opzione "location" in **report personalizzati** non è disponibile. 
- Gli eventi "apertura o download di documenti" non sono disponibili. 

