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
ms.openlocfilehash: ab4ffbc78a7cadd8acee3c98eaa5f3323da9c7e3
ms.sourcegitcommit: 7e6d89f47eca1babf5aeba4995bceccd990c3963
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/28/2021
ms.locfileid: "50037216"
---
# <a name="issues-with-authentication-libraries"></a>Problemi con le librerie di autenticazione

1. [Le raccolte di autenticazione della piattaforma di](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) identità Microsoft elencano le librerie client e middleware supportate e compatibili da Microsoft.
2. Microsoft Authentication Library (MSAL) supporta diversi flussi [di autenticazione](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) da utilizzare in diversi scenari di applicazioni.
3. Per autenticare e acquisire token, inizializza una nuova applicazione client pubblica o riservata nel codice. Puoi impostare diverse opzioni di configurazione quando inizializza l'app client in Microsoft Authentication Library (MSAL). Per ulteriori informazioni, vedere [Opzioni di configurazione dell'applicazione.](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration)

**Fine del supporto per Azure Active Directory Authentication Library (ADAL) e Azure AD Graph API (AAD Graph)**

**A partire dal 30 giugno 2020,** non aggiungeremo più nuove funzionalità ad ADAL e Azure AD Graph. Microsoft continuerà a offrire supporto tecnico e aggiornamenti della sicurezza, ma non fornirà più aggiornamenti delle funzionalità.

**A partire dal 30 giugno 2022,** microsoft terminerà il supporto per ADAL e Azure AD Graph e non fornirà più supporto tecnico o aggiornamenti della sicurezza.

Le app che usano ADAL nelle versioni esistenti del sistema operativo continueranno a funzionare dopo questo periodo, ma non riceveranno alcun supporto tecnico o aggiornamenti *della sicurezza.*

Le app che usano Azure AD Graph dopo questo periodo potrebbero non ricevere più risposte dall'endpoint di Azure AD Graph.

**Migrazione ADAL**

È consigliabile eseguire l'aggiornamento a [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), che include le funzionalità e gli aggiornamenti della sicurezza più recenti.

Se si usano le app Microsoft, è importante sapere che Microsoft sta eseguendo la migrazione delle applicazioni a MSAL entro la scadenza del supporto, assicurandosi che trarranno vantaggio dai continui miglioramenti delle funzionalità e della sicurezza di MSAL.

Per altre informazioni, vedere:

1. [Consultare le domande frequenti su ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Informazioni su come eseguire la migrazione delle app in base alla piattaforma](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Se ti serve aiuto per capire quale delle tue app usa ADAL, ti consigliamo di esaminare tutto il codice sorgente delle tue app e, se applicabile, contattare qualsiasi ISV o provider di app. Il supporto Microsoft può fornire un elenco di tutte le app ADAL diverse da Microsoft nel tenant.

**Migrazione Graph di AAD**

Per le applicazioni che usano Azure AD Graph, seguire le indicazioni per eseguire la [migrazione delle app Di Azure AD Graph a Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)

1. [L'elenco di controllo per la migrazione fornisce un punto di partenza.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. Il portale di registrazione delle app Azure illustra quali applicazioni usano Graph di AAD. È consigliabile esaminare tutto il codice sorgente delle app e, se applicabile, contattare eventuali fornitori di software indipendenti o provider di app. Il supporto Tecnico Microsoft può anche fornire un elenco di tutti gli utilizzi di AAD Graph nel tenant.
3. Per consentire all'app di accedere ai dati in Microsoft Graph, l'utente o l'amministratore deve concedervi le autorizzazioni corrette tramite un processo di consenso. Nella [guida di riferimento alle autorizzazioni di Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) sono elencate le autorizzazioni associate a ogni set principale di API di Microsoft Graph. Vengono inoltre fornite indicazioni su come utilizzare le autorizzazioni.
