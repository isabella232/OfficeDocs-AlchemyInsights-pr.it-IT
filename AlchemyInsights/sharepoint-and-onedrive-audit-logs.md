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
ms.openlocfilehash: be95034bea3c58a4fde96cfb0f9ba525e810758e
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/05/2019
ms.locfileid: "37992622"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>Registri di controllo di SharePoint e OneDrive

## <a name="sharepoint-classic-audit-logs"></a>Registri di controllo di SharePoint Classic

Il controllo legacy di SPO è stato migrato nel log di controllo unificato (UAL). Tutti i report di controllo legacy di SPO saranno ora alimentati tramite UAL e i segnali di controllo legacy sono stati migrati a UAL.

Modifiche principali:

* Il ritaglio non è disponibile come funzionalità.
* La scelta di eventi specifici da controllare non è disponibile. Fare riferimento a [questo documento](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) per un elenco completo degli eventi controllati disponibili per impostazione predefinita.
* L'opzione **percorso** in **report personalizzati** non è disponibile.
* L'opzione eventi di **apertura o download di documenti** non è disponibile.

[Configurare le impostazioni di controllo per una raccolta siti](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>Registri di controllo unificato di SharePoint e OneDrive moderni dalla conformità

* [Attivazione/disattivazione della registrazione di controllo unificato](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

Non è necessaria alcuna configurazione aggiuntiva all'interno di SharePoint o OneDrive.

Utilizzare la ricerca della registrazione di controllo per controllare l'attività dei file, delle cartelle, degli utenti, delle autorizzazioni:

* [Attività di file e pagine](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
* [Attività cartella](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [Attività di condivisione e accesso alle richieste](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [Attività di sincronizzazione](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [Attività amministrative del sito](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

Per ulteriori informazioni su come recuperare questi eventi, vedere [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).
