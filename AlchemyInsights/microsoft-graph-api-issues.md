---
title: Problemi dell'API di Microsoft Graph
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
- "9004345"
- "7759"
ms.openlocfilehash: 9df021211c8a65997889d9303dbf28a27104cfa95841d4cb810427c652ba0784
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53975897"
---
# <a name="microsoft-graph-api-issues"></a>Problemi dell'API di Microsoft Graph

Questo argomento può essere applicabile anche agli sviluppatori che usano ancora l'API Graph Azure AD. È tuttavia consigliabile **utilizzare** Microsoft Graph per tutti gli scenari di gestione di directory, identità e accessi.

**Problemi di autenticazione o autorizzazione**

- Se la tua app non è in grado di acquisire **token** per chiamare Microsoft Graph, seleziona Problema con il recupero di un token di accesso **(autenticazione)** categoria Microsoft Graph per ottenere assistenza e supporto più specifici su questo argomento.
- Se l'app riceve errori di autorizzazione **401 o 403** durante la chiamata a Microsoft Graph, seleziona la categoria Ottenere un errore di accesso negato **(autorizzazione)** API di Microsoft Graph per ottenere assistenza e supporto più specifici su questo argomento.

**Voglio usare Microsoft Graph, ma non so da dove iniziare**

- [Panoramica di Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Panoramica della gestione delle identità e degli accessi in Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Introduzione alla creazione di app Graph Microsoft](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** - Testare le API di Microsoft Graph nel tenant o in un tenant demo

**Voglio usare Microsoft Graph, ma supporta le API della directory v1.0 necessarie?**

Microsoft Graph è l'API consigliata per la gestione di directory, identità e accessi. Tuttavia, esistono ancora alcune lacune tra ciò che è possibile in Azure AD Graph e Microsoft Graph. Leggere gli articoli seguenti, che evidenziano le differenze più aggiornate per agevolare la scelta:

- [Differenze tra i tipi di risorse tra Azure AD Graph e Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Differenze di proprietà tra Azure AD Graph e Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Differenze di metodo tra Azure AD e Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**L'API che chiamo non funziona: dove posso eseguire altri test?**

**Microsoft Graph Explorer** - Testare le API di Microsoft Graph nel tenant o in un tenant demo e consultare anche le query di esempio **in** Microsoft Graph Explorer.

**L'app è troppo lenta e viene anche limitato. Quali miglioramenti è possibile apportare?**

A seconda dello scenario, sono disponibili diverse opzioni per rendere l'applicazione più performante e, in alcuni casi, meno inclini a essere limitate dal servizio (quando si effettuano troppe chiamate).

- [Procedure consigliate Graph Microsoft](https://docs.microsoft.com/graph/best-practices-concept)
- [Invio in batch delle richieste](https://docs.microsoft.com/graph/json-batching)
- [Tenere traccia delle modifiche tramite query delta](https://docs.microsoft.com/graph/delta-query-overview)
- [Ricevere notifiche delle modifiche tramite webhook](https://docs.microsoft.com/graph/webhooks)
- [Linee guida sulla limitazione](https://docs.microsoft.com/graph/throttling)

**Dove è possibile trovare ulteriori informazioni su errori e problemi noti?**

- [Informazioni sulla risposta Graph errore di Microsoft](https://docs.microsoft.com/graph/errors)
- [Problemi noti con Microsoft Graph](https://docs.microsoft.com/graph/known-issues)

**Dove è possibile verificare lo stato della disponibilità e della connettività del servizio?**

La disponibilità e la connettività dei servizi sottostanti accessibili tramite Microsoft Graph possono influire sulla disponibilità e sulle prestazioni complessive di Microsoft Graph.

- Per Azure Active Directory integrità del servizio, controllare lo stato dei servizi di sicurezza **e** identità elencati nella pagina [stato di Azure.](https://azure.microsoft.com/status/)
- Per Office servizi che contribuiscono a Microsoft Graph, controllare lo stato dei servizi elencati nel dashboard Office [Service Health Dashboard](https://portal.office.com/adminportal/home#/servicehealth).

Gli Graph di autorizzazione di Microsoft Graph possono essere il risultato di diversi problemi, la maggior parte dei quali genera un errore 401 o 403. Ad esempio, quanto segue può causare errori di autorizzazione:

- [Flussi di acquisizione di token di accesso](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios) non corretti
- [Ambiti di autorizzazione](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) non configurati correttamente
- Mancanza di [consenso](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

***Fine del supporto per Azure Active Directory Authentication Library (ADAL) e Azure AD Graph API (AAD Graph)***

**A partire dal 30 giugno 2020,** non aggiungeremo più nuove funzionalità ad ADAL e Azure AD Graph. Microsoft continuerà a offrire supporto tecnico e aggiornamenti della sicurezza, ma non fornirà più aggiornamenti delle funzionalità.

**A partire dal 30 giugno 2022,** microsoft terminerà il supporto per ADAL e Azure AD Graph e non fornirà più supporto tecnico o aggiornamenti della sicurezza.

Le app che usano ADAL nelle versioni del sistema operativo esistenti continueranno a funzionare dopo tale data, ma non *riceveranno alcun supporto tecnico o aggiornamento di sicurezza*.

Le app che usano Graph di Azure AD dopo tale data potrebbero non ricevere più risposte dall'endpoint Graph di Azure AD.

**Migrazione ADAL**

È consigliabile eseguire l'aggiornamento a [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), che include le funzionalità e gli aggiornamenti della sicurezza più recenti.

Se si usano le app Microsoft, è necessario sapere che Microsoft sta per eseguire la migrazione delle applicazioni a MSAL entro la scadenza di fine del supporto, assicurandosi che trarranno vantaggio dai continui miglioramenti apportati alla sicurezza e alle funzionalità di MSAL.

1. [Consultare le domande frequenti su ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Informazioni su come eseguire la migrazione delle app in base alla piattaforma](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Se hai bisogno di assistenza per capire quale delle tue app usa ADAL, ti consigliamo di esaminare tutto il codice sorgente delle tue app e, se applicabile, contattare qualsiasi PROVIDER di app o ISV. Il supporto Microsoft può fornire un elenco di tutte le app ADAL diverse da Microsoft nel tenant.

**Migrazione Graph di AAD**

Per le applicazioni che usano Azure AD Graph, seguire le indicazioni per eseguire la migrazione delle app [di Azure AD Graph a Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).

1. [L'elenco di controllo per la migrazione fornisce un punto di partenza](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).
2. Il portale di registrazione delle app Azure illustra quali applicazioni usano Graph di AAD. È consigliabile esaminare tutto il codice sorgente delle app e, se applicabile, contattare eventuali fornitori di software indipendenti o provider di app. Il supporto Microsoft può anche fornire un elenco di tutti gli utilizzi Graph AAD nel tenant.
3. Per consentire all'app di accedere ai dati in Microsoft Graph, l'utente o l'amministratore deve concedervi le autorizzazioni corrette tramite un processo di consenso. Il [riferimento alle](https://docs.microsoft.com/graph/permissions-reference) Graph microsoft Graph elenca le autorizzazioni associate a ogni set principale di API microsoft Graph. Vengono inoltre fornite indicazioni su come utilizzare le autorizzazioni.
