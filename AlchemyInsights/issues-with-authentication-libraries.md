---
title: Problemi con le librerie di autenticazione
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004333"
- "7731"
ms.openlocfilehash: 39336fa8840a28befcad449d0afa59c1df5c6bef5988cb197916a03aa2aa66c9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028008"
---
# <a name="issues-with-authentication-libraries"></a>Problemi con le librerie di autenticazione

1. [Microsoft Identity Platform di autenticazione sono](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) elencate le librerie client e middleware supportate da Microsoft e compatibili.
2. Microsoft Authentication Library (MSAL) supporta diversi flussi [di autenticazione](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) da utilizzare in diversi scenari di applicazioni.
3. Per autenticare e acquisire token, inizializza una nuova applicazione client pubblica o riservata nel codice. Puoi impostare diverse opzioni di configurazione quando inizializza l'app client nella Libreria di autenticazione Microsoft (MSAL). Per ulteriori informazioni, vedere [Opzioni di configurazione dell'applicazione](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).

**Fine del supporto per Azure Active Directory Authentication Library (ADAL) e Azure AD Graph API (AAD Graph)**

**A partire dal 30 giugno 2020,** non aggiungeremo più nuove funzionalità ad ADAL e Azure AD Graph. Microsoft continuerà a offrire supporto tecnico e aggiornamenti della sicurezza, ma non fornirà più aggiornamenti delle funzionalità.

**A partire dal 30 giugno 2022,** microsoft terminerà il supporto per ADAL e Azure AD Graph e non fornirà più supporto tecnico o aggiornamenti della sicurezza.

Le app che usano ADAL nelle versioni del sistema operativo esistenti continueranno a funzionare dopo tale data, ma non *riceveranno alcun supporto tecnico o aggiornamento di sicurezza*.

Le app che usano Graph di Azure AD dopo tale data potrebbero non ricevere più risposte dall'endpoint Graph di Azure AD.

**Migrazione ADAL**

È consigliabile eseguire l'aggiornamento a [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), che include le funzionalità e gli aggiornamenti della sicurezza più recenti.

Se si usano le app Microsoft, è necessario sapere che Microsoft sta eseguendo la migrazione delle applicazioni a MSAL entro la scadenza di fine del supporto, assicurandosi che trarranno vantaggio dai continui miglioramenti apportati alla sicurezza e alle funzionalità di MSAL.

Per altre informazioni, vedere:

1. [Consultare le domande frequenti su ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Informazioni su come eseguire la migrazione delle app in base alla piattaforma](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Se hai bisogno di assistenza per capire quale delle tue app usa ADAL, ti consigliamo di esaminare tutto il codice sorgente delle tue app e, se applicabile, contattare qualsiasi PROVIDER di app o ISV. Il supporto Microsoft può fornire un elenco di tutte le app ADAL diverse da Microsoft nel tenant.

**Migrazione Graph di AAD**

Per le applicazioni che usano Azure AD Graph, seguire le indicazioni per eseguire la migrazione delle app [di Azure AD Graph a Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).

1. [L'elenco di controllo per la migrazione costituisce un punto di partenza.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. Il portale di registrazione delle app Azure illustra quali applicazioni usano Graph di AAD. È consigliabile esaminare tutto il codice sorgente delle app e, se applicabile, contattare eventuali fornitori di software indipendenti o provider di app. Il supporto Microsoft può anche fornire un elenco di tutti gli utilizzi Graph AAD nel tenant.
3. Per consentire all'app di accedere ai dati in Microsoft Graph, l'utente o l'amministratore deve concedervi le autorizzazioni corrette tramite un processo di consenso. Il [riferimento alle](https://docs.microsoft.com/graph/permissions-reference) Graph microsoft Graph elenca le autorizzazioni associate a ogni set principale di API microsoft Graph. Vengono inoltre fornite indicazioni su come utilizzare le autorizzazioni.
