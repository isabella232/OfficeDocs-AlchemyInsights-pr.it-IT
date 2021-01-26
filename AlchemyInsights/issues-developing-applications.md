---
title: Problemi relativi allo sviluppo di applicazioni
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7754"
- "9004342"
ms.openlocfilehash: 652fd6431201380e8e96619f63ecac15a6704d4f
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 01/25/2021
ms.locfileid: "49950801"
---
# <a name="issues-developing-applications"></a>Problemi relativi allo sviluppo di applicazioni

Per la risoluzione dei problemi più comuni durante la creazione di app Azure Active Directory (AD), vedere gli articoli seguenti:

- [Problemi di accesso alle applicazioni solo usando il browser Chrome](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [Come modificare le impostazioni predefinite di durata del token per l'applicazione](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [Come funziona il consenso dell'applicazione](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [Come concedere le autorizzazioni all'applicazione](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [Differenze tra le autorizzazioni delegate e le autorizzazioni dell'applicazione](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

***Fine del supporto per Active Directory Authentication Library (ADAL) e l'API Graph di Azure AD (AAD Graph)** _

- A partire dal 30 giugno 2020, non verranno più aggiunte nuove funzionalità ad Active Directory Authentication Library (ADAL) e all'API Graph di Azure AD (A AD Graph). Microsoft continuerà a offrire supporto tecnico e aggiornamenti della sicurezza, ma non fornirà più aggiornamenti delle funzionalità.

- A partire dal 30 giugno 2022, Microsoft terminerà il supporto per ADAL e Graph di AAD e non fornirà più supporto tecnico o aggiornamenti della sicurezza. In considerazione di quanto illustrato in precedenza, le implicazioni sono le seguenti:

    - Le app che usano ADAL nelle versioni del sistema operativo esistenti continueranno a funzionare dopo tale data, ma non riceveranno alcun supporto tecnico o aggiornamento della sicurezza.

    - Le app che usano Graph di AAD dopo tale data potrebbero non ricevere più risposte dall'endpoint Graph di AAD

_ *Migrazione ADAL**

Se si usano app Microsoft, è consigliabile eseguire l'aggiornamento a Microsoft Authentication Library (MSAL), che include le funzionalità e gli aggiornamenti della sicurezza più recenti. Questo suggerimento è valido nel caso in cui Microsoft avvii il processo di migrazione delle app a MSAL prima della scadenza del supporto. 

Tramite la migrazione a MSAL da parte di Microsoft, le app beneficeranno dei vantaggi derivanti dai continui miglioramenti della sicurezza e delle funzionalità di MSAL.

1. [Consultare le domande frequenti su ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [Informazioni su come eseguire la migrazione delle app in base alla piattaforma](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. Se serve assistenza per capire quale app usa ADAL, è consigliabile esaminare tutto il codice sorgente delle app e, se applicabile, contattare eventuali fornitori di software indipendenti (ISV) o provider di app. Il supporto Microsoft può fornire un elenco di tutte le app ADAL diverse da Microsoft nel tenant.

**Migrazione Graph di AAD**

Per le applicazioni che usano Graph di AAD, seguire le indicazioni per la migrazione delle app Graph di AAD a Microsoft Graph:

1. [L'elenco di controllo per la migrazione fornisce un punto di partenza](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
2. Il portale di registrazione delle app Azure illustra quali applicazioni usano Graph di AAD. È consigliabile esaminare tutto il codice sorgente delle app e, se applicabile, contattare eventuali fornitori di software indipendenti o provider di app. Il supporto Microsoft può fornire informazioni sull'utilizzo di Graph di AAD nel tenant.







