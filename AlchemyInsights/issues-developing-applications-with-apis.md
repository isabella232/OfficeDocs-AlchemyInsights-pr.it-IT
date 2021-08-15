---
title: Problemi di sviluppo di applicazioni con LE API
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
- "9004343"
- "7755"
ms.openlocfilehash: 1de4e9aa5078507eecdbe53366e446e733029ecb1342f20ca701fa7f95a06fa9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013464"
---
# <a name="issues-developing-applications-with-apis"></a>Problemi di sviluppo di applicazioni con LE API

Per iniziare a usare l'API di Azure Active Directory Graph, vedere la guida introduttiva all'API di [azure AD Graph](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) o visualizzare la documentazione di riferimento interattiva sull'API di azure AD [Graph](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).

**Fine del supporto per Azure Active Directory Authentication Library (ADAL) e Azure AD Graph API (AAD Graph)**

**A partire dal 30 giugno 2020,** non aggiungeremo più nuove funzionalità ad ADAL e Azure AD Graph. Microsoft continuerà a offrire supporto tecnico e aggiornamenti della sicurezza, ma non fornirà più aggiornamenti delle funzionalità.

**A partire dal 30 giugno 2022,** microsoft terminerà il supporto per ADAL e Azure AD Graph e non fornirà più supporto tecnico o aggiornamenti della sicurezza.

Le app che usano ADAL nelle versioni del sistema operativo esistenti continueranno a funzionare dopo tale data, ma non riceveranno alcun supporto tecnico o aggiornamento della sicurezza.

Le app che usano Graph di Azure AD dopo tale data potrebbero non ricevere più risposte dall'endpoint Graph di Azure AD.

**Migrazione ADAL**

È consigliabile eseguire l'aggiornamento a [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), che include le funzionalità e gli aggiornamenti della sicurezza più recenti.

Se si usano app Microsoft, è necessario sapere che Microsoft sta per eseguire la migrazione delle applicazioni a MSAL entro la scadenza di fine del supporto, assicurandosi che trarranno vantaggio dai continui miglioramenti apportati alla sicurezza e alle funzionalità di MSAL.

1. [Leggi le domande frequenti su ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. [Informazioni su come eseguire la migrazione delle app in base alla piattaforma](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. Se hai bisogno di assistenza per capire quale delle tue app usa ADAL, ti consigliamo di esaminare tutto il codice sorgente delle tue app e, se applicabile, contattare qualsiasi PROVIDER di app o ISV. Il supporto Microsoft può fornire un elenco di tutte le app ADAL diverse da Microsoft nel tenant.

**Migrazione Graph di AAD**

Per le applicazioni che usano Azure AD Graph, seguire le indicazioni per eseguire la migrazione delle app [di Azure AD Graph a Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).

1. [L'elenco di controllo per la migrazione fornisce un punto di partenza](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
1. Il portale di registrazione delle app Azure illustra quali applicazioni usano Graph di AAD. È consigliabile esaminare tutto il codice sorgente delle app e, se applicabile, contattare eventuali fornitori di software indipendenti o provider di app. Il supporto Microsoft può anche fornire un elenco di tutti gli utilizzi Graph AAD nel tenant.
1. Per consentire all'app di accedere ai dati in Microsoft Graph, l'utente o l'amministratore deve concedervi le autorizzazioni corrette tramite un processo di consenso. Il [riferimento alle](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) Graph microsoft Graph elenca le autorizzazioni associate a ogni set principale di API microsoft Graph. Vengono inoltre fornite indicazioni su come utilizzare le autorizzazioni.
