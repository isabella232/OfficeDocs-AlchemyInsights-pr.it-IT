---
title: Problemi di sviluppo di applicazioni con API
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
ms.openlocfilehash: 26d732819b64efa4fb84da44cc2a279368aa28b0
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/25/2021
ms.locfileid: "49951901"
---
# <a name="issues-developing-applications-with-apis"></a>Problemi di sviluppo di applicazioni con API

Per iniziare a utilizzare l'API di Azure Active Directory Graph, vedere la [Guida introduttiva](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) all'API di Azure AD Graph o visualizzare la [documentazione di riferimento relativa all'API di Azure AD Graph interattiva](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).

**Fine del supporto di Azure Active Directory Authentication Library (ADAL) e Azure AD Graph API (AAD Graph)**

A **partire dal 30 giugno 2020**, non verranno più aggiunte nuove funzionalità a adal e Azure AD Graph. Si continuerà a fornire supporto tecnico e aggiornamenti per la sicurezza, ma non verranno più forniti aggiornamenti delle funzionalità.

**A partire dal 30 giugno 2022**, si finirà il supporto per adal e Azure AD Graph e non verranno più forniti supporto tecnico o aggiornamenti per la sicurezza.

Le app che utilizzano ADAL nelle versioni del sistema operativo esistenti continueranno a funzionare dopo questo periodo, ma non riceveranno alcun supporto tecnico o aggiornamenti per la sicurezza.

Le app che utilizzano Azure AD Graph dopo questo intervallo di tempo potrebbero non ricevere più risposte dall'endpoint di Azure AD Graph.

**Migrazione ADAL**

È consigliabile eseguire l'aggiornamento a [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), in cui sono disponibili le funzionalità e gli aggiornamenti della sicurezza più recenti.

Se si utilizzano le app Microsoft, è necessario sapere che Microsoft sta eseguendo la migrazione delle applicazioni a MSAL in base alla scadenza del supporto tecnico, garantendo che possano usufruire dei miglioramenti della sicurezza e delle funzionalità di MSAL in corso.

1. [Leggere le domande frequenti su adal](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. Informazioni su [come eseguire la migrazione delle app per ogni singola piattaforma](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. Se si ha bisogno di assistenza per capire quali app utilizzano ADAL, si consiglia di esaminare tutti i codici sorgente delle app e, se applicabile, di raggiungere tutti gli ISV o i provider di applicazioni. Il supporto tecnico Microsoft può anche fornire un elenco di tutte le app di ADAL non Microsoft nel tenant.

**Migrazione del grafico AAD**

Per le applicazioni che utilizzano Azure AD Graph, seguire le istruzioni riportate di seguito per eseguire la migrazione delle [app di Azure AD Graph a Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).

1. [L'elenco di controllo per la migrazione fornisce un punto introduttivo](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
1. Il portale di registrazione delle app di Azure indica le applicazioni che utilizzano il grafico AAD. È consigliabile esaminare tutti i codici sorgente delle app e, se applicabile, rivolgersi a qualsiasi ISV o provider di applicazioni. Il supporto tecnico Microsoft può anche fornire un elenco di tutti gli utilizzi del grafico AAD nel tenant.
1. Affinché l'app acceda ai dati in Microsoft Graph, l'utente o l'amministratore deve concedergli le autorizzazioni corrette tramite un processo di consenso. La Guida di riferimento per le [autorizzazioni di Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) elenca le autorizzazioni associate a ciascun set principale di API di Microsoft Graph. Vengono inoltre fornite indicazioni su come utilizzare le autorizzazioni.
